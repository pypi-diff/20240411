# Comparing `tmp/indico-client-6.1.0a1.tar.gz` & `tmp/indico-client-6.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indico-client-6.1.0a1.tar", last modified: Wed Feb 28 20:58:49 2024, max compression
+gzip compressed data, was "indico-client-6.7.0a0.tar", last modified: Thu Apr 11 14:26:42 2024, max compression
```

## Comparing `indico-client-6.1.0a1.tar` & `indico-client-6.7.0a0.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/
--rw-r--r--   0 root         (0) root         (0)       57 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1086 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      697 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      370 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/indico/
--rw-r--r--   0 root         (0) root         (0)      308 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/__init__.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/indico/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.402001 indico-client-6.1.0a1/indico/client/
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6321 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/client/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.406001 indico-client-6.1.0a1/indico/config/
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2299 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/config/config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.406001 indico-client-6.1.0a1/indico/filters/
--rw-r--r--   0 root         (0) root         (0)     6230 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.406001 indico-client-6.1.0a1/indico/http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12859 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/client.py
--rw-r--r--   0 root         (0) root         (0)     2396 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/retry.py
--rw-r--r--   0 root         (0) root         (0)     4846 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.410001 indico-client-6.1.0a1/indico/queries/
--rw-r--r--   0 root         (0) root         (0)      326 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4449 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/custom_blueprint.py
--rw-r--r--   0 root         (0) root         (0)    18007 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/datasets.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/document_report.py
--rw-r--r--   0 root         (0) root         (0)     3354 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/documents.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/example.py
--rw-r--r--   0 root         (0) root         (0)     6747 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/export.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/forms.py
--rw-r--r--   0 root         (0) root         (0)     3549 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/integration.py
--rw-r--r--   0 root         (0) root         (0)     2882 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/jobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.410001 indico-client-6.1.0a1/indico/queries/model_groups/
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/model_groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4179 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/model_groups/metrics.py
--rw-r--r--   0 root         (0) root         (0)    10268 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/model_groups/model_groups.py
--rw-r--r--   0 root         (0) root         (0)    10455 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     4517 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/storage.py
--rw-r--r--   0 root         (0) root         (0)    15108 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/submission.py
--rw-r--r--   0 root         (0) root         (0)     5722 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/usermetrics.py
--rw-r--r--   0 root         (0) root         (0)    18024 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/workflow.py
--rw-r--r--   0 root         (0) root         (0)    15781 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/workflow_components.py
--rw-r--r--   0 root         (0) root         (0)     5939 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/workflow_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.410001 indico-client-6.1.0a1/indico/types/
--rw-r--r--   0 root         (0) root         (0)      257 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1853 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/base.py
--rw-r--r--   0 root         (0) root         (0)      248 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/custom_blueprint.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/datafile.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/dataset.py
--rw-r--r--   0 root         (0) root         (0)      457 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/document_report.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/export.py
--rw-r--r--   0 root         (0) root         (0)     1298 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/integration.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/jobs.py
--rw-r--r--   0 root         (0) root         (0)      732 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/model.py
--rw-r--r--   0 root         (0) root         (0)     2187 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/model_group.py
--rw-r--r--   0 root         (0) root         (0)     2168 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/model_metrics.py
--rw-r--r--   0 root         (0) root         (0)      590 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     3396 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/submission.py
--rw-r--r--   0 root         (0) root         (0)      824 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/submission_file.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/user_metrics.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/utils.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/workflow.py
--rw-r--r--   0 root         (0) root         (0)     9437 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/workflow_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.414002 indico-client-6.1.0a1/indico_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      697 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2624 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      210 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      170 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1035 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.402001 indico-client-6.1.0a1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.414002 indico-client-6.1.0a1/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1252 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.414002 indico-client-6.1.0a1/tests/integration/data/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/data/async_datasets.py
--rw-r--r--   0 root         (0) root         (0)     9776 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/data/datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/tests/integration/queries/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_custom_blueprint.py
--rw-r--r--   0 root         (0) root         (0)    13980 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5479 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_document.py
--rw-r--r--   0 root         (0) root         (0)     2385 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_document_report.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_export.py
--rw-r--r--   0 root         (0) root         (0)     2167 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_job.py
--rw-r--r--   0 root         (0) root         (0)     9063 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_model_group.py
--rw-r--r--   0 root         (0) root         (0)     5104 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     2641 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_user_metrics.py
--rw-r--r--   0 root         (0) root         (0)    19409 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_workflow.py
--rw-r--r--   0 root         (0) root         (0)     7281 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_workflow_component.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_workflow_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1545 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/test_base_aioclient.py
--rw-r--r--   0 root         (0) root         (0)     2214 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/test_base_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/unit/test_filters.py
--rw-r--r--   0 root         (0) root         (0)    70238 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.337951 indico-client-6.7.0a0/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      698 2024-04-11 14:26:42.337951 indico-client-6.7.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.341951 indico-client-6.7.0a0/indico/
+-rw-r--r--   0 root         (0) root         (0)      341 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-11 14:26:42.341951 indico-client-6.7.0a0/indico/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.325951 indico-client-6.7.0a0/indico/client/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7816 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     3925 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/client/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.325951 indico-client-6.7.0a0/indico/config/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/config/config.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.325951 indico-client-6.7.0a0/indico/filters/
+-rw-r--r--   0 root         (0) root         (0)     8926 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.325951 indico-client-6.7.0a0/indico/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14093 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/http/client.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/http/retry.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/http/serialization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.329951 indico-client-6.7.0a0/indico/queries/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/custom_blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    16712 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/document_report.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/documents.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/example.py
+-rw-r--r--   0 root         (0) root         (0)     8601 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/export.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/forms.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/integration.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.329951 indico-client-6.7.0a0/indico/queries/model_groups/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/model_groups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/model_groups/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10618 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/model_groups/model_groups.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/storage.py
+-rw-r--r--   0 root         (0) root         (0)    19015 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/submission.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/usermetrics.py
+-rw-r--r--   0 root         (0) root         (0)    19010 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    16685 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/workflow_components.py
+-rw-r--r--   0 root         (0) root         (0)     6174 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/queries/workflow_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.333951 indico-client-6.7.0a0/indico/types/
+-rw-r--r--   0 root         (0) root         (0)      498 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/base.py
+-rw-r--r--   0 root         (0) root         (0)      296 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/custom_blueprint.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/datafile.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      439 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/document_report.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/export.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/integration.py
+-rw-r--r--   0 root         (0) root         (0)      906 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/jobs.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/model.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/model_group.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/model_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/output_file.py
+-rw-r--r--   0 root         (0) root         (0)      591 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/submission.py
+-rw-r--r--   0 root         (0) root         (0)      824 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/submission_file.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/user_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     9453 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/types/workflow_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/indico/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.333951 indico-client-6.7.0a0/indico_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      698 2024-04-11 14:26:42.000000 indico-client-6.7.0a0/indico_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2745 2024-04-11 14:26:42.000000 indico-client-6.7.0a0/indico_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 14:26:42.000000 indico-client-6.7.0a0/indico_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2024-04-11 14:26:42.000000 indico-client-6.7.0a0/indico_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 14:26:42.000000 indico-client-6.7.0a0/indico_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-11 14:26:42.341951 indico-client-6.7.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.321951 indico-client-6.7.0a0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.333951 indico-client-6.7.0a0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.337951 indico-client-6.7.0a0/tests/integration/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/data/async_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     9652 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/data/datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.337951 indico-client-6.7.0a0/tests/integration/queries/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_custom_blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    12935 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_document.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_document_report.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_export.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_job.py
+-rw-r--r--   0 root         (0) root         (0)     6882 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_model_group.py
+-rw-r--r--   0 root         (0) root         (0)     6045 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_submission.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_user_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    20212 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_workflow_component.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/queries/test_workflow_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/test_base_aioclient.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/integration/test_base_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:26:42.337951 indico-client-6.7.0a0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/tests/unit/test_filters.py
+-rw-r--r--   0 root         (0) root         (0)    70238 2024-04-11 14:22:55.000000 indico-client-6.7.0a0/versioneer.py
```

### Comparing `indico-client-6.1.0a1/LICENSE` & `indico-client-6.7.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a1/PKG-INFO` & `indico-client-6.7.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indico-client
-Version: 6.1.0a1
+Version: 6.7.0a0
 Summary: A Python Wrapper for indico app API.
 Home-page: https://github.com/IndicoDataSolutions/indico-client-python
 Author: indico
 Author-email: engineering@indico.io
 License: MIT License (See LICENSE)
 Platform: UNKNOWN
 License-File: LICENSE
@@ -29,7 +29,8 @@
 From source:
 
 .. code:: bash
 
     git clone https://github.com/IndicoDataSolutions/indico-client-python.git
     python setup.py install
 
+
```

### Comparing `indico-client-6.1.0a1/indico/config/config.py` & `indico-client-6.7.0a0/indico/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # -*- coding: utf-8 -*-
 
 import os
-
 from pathlib import Path
+from typing import TYPE_CHECKING
+
 from indico.errors import IndicoInvalidConfigSetting
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Optional, Tuple, Union
+
+    from indico.typing import AnyDict
+
 
 class IndicoConfig:
     """
     Configuration for the IndicoClient.
 
     Args:
         host= (str, optional): Indico Platform hostname (eg mycluster.indico.io )
@@ -20,50 +26,46 @@
     Returns:
         IndicoConfig object
 
     Raises:
         RuntimeError: If api_token_path does not exist.
     """
 
-    host: str
-    protocol: str
-    serializer: str
-    api_token_path: str
-    api_token: str = None
-    verify_ssl: bool = True
-    requests_params: dict = None
-    _disable_cookie_domain: bool = False
-
-    def __init__(self, **kwargs):
-
-        self.host: str = os.getenv("INDICO_HOST")
+    def __init__(self, **kwargs: "Any"):
+        self.host: str = os.getenv("INDICO_HOST", "")
         self.protocol: str = os.getenv("INDICO_PROTOCOL", "https")
         self.serializer: str = os.getenv("INDICO_SERIALIZER", "msgpack")
-        self.api_token_path: str = os.getenv("INDICO_API_TOKEN_PATH", Path.home())
-        self.api_token: str = os.getenv("INDICO_API_TOKEN")
+        self.api_token_path: "Union[str, Path]" = os.getenv(
+            "INDICO_API_TOKEN_PATH", Path.home()
+        )
+        self.api_token: "Optional[str]" = os.getenv("INDICO_API_TOKEN")
+        self.verify_ssl: bool = True
+        self.requests_params: "Optional[AnyDict]" = None
+        self._disable_cookie_domain: bool = False
 
         for key, value in kwargs.items():
             if hasattr(self, key):
                 setattr(self, key, value)
             else:
                 raise IndicoInvalidConfigSetting(key)
 
         if not self.api_token:
             self.api_token_path, self.api_token = self._resolve_api_token()
 
-    def _resolve_api_token(self):
+    def _resolve_api_token(self) -> "Tuple[Path, str]":
         path = self.api_token_path
+
         if not isinstance(path, Path):
             path = Path(path)
+
         if not path.exists():
             path = Path.home()
         if not path.is_file():
             path = path / "indico_api_token.txt"
 
         if not path.exists():
             raise RuntimeError(
                 "Expected indico_api_token.txt in home directory, "
                 "or provided as indicoio.config.api_token_path"
             )
 
-        with path.open("r") as f:
-            return path, f.read().strip()
+        return path, path.read_text().strip()
```

### Comparing `indico-client-6.1.0a1/indico/errors.py` & `indico-client-6.7.0a0/indico/errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,59 @@
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Union
+
+
 class IndicoError(Exception):
-    pass
+    """Base exception for known error modes"""
 
 
 class IndicoRequestError(IndicoError):
-    def __init__(self, error, code, extras=None):
+    def __init__(
+        self,
+        error: str,
+        code: "Union[int, str]",
+        extras: "Any" = None,
+    ):
         super().__init__(f"Status: {code}, Error: {error}\n\tExtras: {extras}")
 
 
 class IndicoTimeoutError(IndicoError):
-    def __init__(self, duration):
+    def __init__(self, duration: "Union[int, float]"):
         super().__init__(f"Request timed out after {duration:0.3f} seconds.")
 
 
 class IndicoDecodingError(IndicoError):
-    def __init__(self, mime, charset, content):
+    def __init__(self, mime: str, charset: str, content: str):
         super().__init__(f"Failed to decode with {mime}:{charset}. Content {content}")
 
 
 class IndicoInputError(IndicoError):
-    def __init__(self, msg):
+    def __init__(self, msg: str):
         super().__init__(msg)
 
 
 class IndicoInvalidConfigSetting(IndicoError):
     def __init__(
         self,
-        setting_name,
+        setting_name: str,
     ):
         super().__init__(f"{setting_name} is not a valid configuration setting")
 
 
 class IndicoNotFound(IndicoError):
-    def __init__(self, cls):
+    def __init__(self, cls: str):
         super().__init__(f"Could not find {cls}")
 
 
 class IndicoAuthenticationFailed(IndicoError):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("Failed to authenticate")
 
 
 class IndicoHibernationError(IndicoError):
-    def __init__(self, after):
-        self.after = after
-        super().__init__(f"Platform is currently hibernating. Wait {after} seconds and retry this request.")
-
+    def __init__(self, after: int):
+        self.after: int = after
+        super().__init__(
+            f"Platform is currently hibernating. Wait {after} seconds and retry this request."
+        )
```

### Comparing `indico-client-6.1.0a1/indico/filters/__init__.py` & `indico-client-6.7.0a0/indico/filters/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import datetime
-from typing import Any, Iterable, Mapping
+from typing import TYPE_CHECKING, Dict
 
 from indico.errors import IndicoInputError
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, ClassVar, List, Optional, Tuple, Union
 
-def or_(*args: Iterable[Mapping[str, Any]]):
+    from indico.typing import AnyDict
+
+
+def or_(*args: "Any") -> "Dict[str, List[Any]]":
     return {"OR": list(args)}
 
 
-def and_(*args: Iterable[Mapping[str, Any]]):
+def and_(*args: "Any") -> "Dict[str, List[Any]]":
     return {"AND": list(args)}
 
 
-class Filter(dict):
+class Filter(Dict[str, "Any"]):
     """
     Base filter class that allows users to construct filter statements for
     GraphQL queries. Search keys are constrained by the implementing subclasses
     If multiple arguments are supplied, they are treated as arg1 AND arg2 AND ...
     """
 
-    __options__ = None
+    __options__: "ClassVar[Tuple[Any, ...]]" = tuple()
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: "Any"):
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         if not kwargs:
             raise IndicoInputError(f"One of {self.__options__} must be specified")
         self.update(and_(kwargs) if len(kwargs) > 1 else kwargs)
 
 
 class DatasetFilter(Filter):
@@ -44,52 +49,97 @@
         super().__init__(name=name)
 
 
 class SubmissionReviewFilter(Filter):
     __options__ = ("rejected", "created_by", "review_type")
 
     def __init__(
-        self, rejected: bool = None, created_by: int = None, review_type: str = None
+        self,
+        rejected: "Optional[bool]" = None,
+        created_by: "Optional[int]" = None,
+        review_type: "Optional[str]" = None,
     ):
         kwargs = {
             "rejected": rejected,
             "createdBy": created_by,
             "reviewType": review_type.upper() if review_type else review_type,
         }
 
         super().__init__(**kwargs)
 
 
+class DateRangeFilter(Dict[str, "Optional[str]"]):
+    """
+    Create a Filter when querying for Submissions within a certain date range
+    Args:
+        filter_from (str): A valid string representation of a datetime for start date to filter
+        filter_to (str): A valid string representation of a datetime for end date to filter
+    """
+
+    def __init__(
+        self, filter_from: "Optional[str]" = None, filter_to: "Optional[str]" = None
+    ):
+        kwargs: "Dict[str, Optional[str]]" = {"from": filter_from, "to": filter_to}
+        self.update(kwargs)
+
+
 class SubmissionFilter(Filter):
     """
     Create a Filter when querying for WorkflowSubmissions.
 
     Args:
+        file_type (list): submissions with a file type in this list. Options:
+            [CSV, PDF, EXCEL, DOC, DOCX, PPT, PPTX, PNG, JPG, TIFF, TXT, RTF, XLS, XLSX, UNKNOWN, MSG, EML]
         input_filename (str): submissions with input file names containing this string
         status (str): submissions in this status. Options:
             [PROCESSING, PENDING_REVIEW, PENDING_ADMIN_REVIEW, COMPLETE, FAILED]
-        retrieved(bool): Filter submissions on the retrieved flag
+        retrieved (bool): submissions that have been retrieved (True) or not (False)
+        reviews (SubmissionReviewFilter): submissions whose completed reviews match this review filter
+        review_in_progress (bool): submissions where a review is in progress (True) or not (False)
+        files_deleted (bool): submissions that have had their internal files removed (True) or not (False)
+        created_at (DateRangeFilter): submissions created during given time range
+        updated_at (DateRangeFilter): submissions updated during given time range
     Returns:
         dict containing query filter parameters
     """
 
-    __options__ = ("input_filename", "status", "retrieved")
+    __options__ = (
+        "file_type",
+        "input_filename",
+        "status",
+        "retrieved",
+        "reviews",
+        "review_in_progress",
+        "files_deleted",
+        "created_at",
+        "updated_at",
+    )
 
     def __init__(
         self,
-        input_filename: str = None,
-        status: str = None,
-        retrieved: bool = None,
-        reviews: SubmissionReviewFilter = None,
+        file_type: "Optional[List[str]]" = None,
+        input_filename: "Optional[str]" = None,
+        status: "Optional[str]" = None,
+        retrieved: "Optional[bool]" = None,
+        reviews: "Optional[SubmissionReviewFilter]" = None,
+        review_in_progress: "Optional[bool]" = None,
+        files_deleted: "Optional[bool]" = None,
+        created_at: "Optional[DateRangeFilter]" = None,
+        updated_at: "Optional[DateRangeFilter]" = None,
     ):
-        kwargs = {
+        kwargs: "AnyDict" = {
+            "filetype": file_type,
             "inputFilename": input_filename,
             "status": status.upper() if status else status,
             "retrieved": retrieved,
             "reviews": reviews,
+            "reviewInProgress": review_in_progress,
+            "filesDeleted": files_deleted,
+            "createdAt": created_at,
+            "updatedAt": updated_at,
         }
 
         super().__init__(**kwargs)
 
 
 class ModelGroupExampleFilter(Filter):
     """
@@ -106,20 +156,20 @@
     """
 
     # TODO: extend to support full filter list
     __options__ = ("file_name", "partial", "status", "text_search")
 
     def __init__(
         self,
-        file_name: str = None,
-        partial: bool = None,
-        status: str = None,
-        text_search: str = None,
+        file_name: "Optional[str]" = None,
+        partial: "Optional[bool]" = None,
+        status: "Optional[str]" = None,
+        text_search: "Optional[str]" = None,
     ):
-        kwargs = {
+        kwargs: "Dict[str, Optional[Union[bool, str]]]" = {
             "fileName": file_name,
             "partial": partial,
             "textSearch": text_search,
         }
         kwargs["status"] = status.upper() if status else None
 
         super().__init__(**kwargs)
@@ -134,16 +184,23 @@
         user_email (str): email to filter for
     Returns:
         dict containing query filter parameters
     """
 
     __options__ = ("user_id", "user_email")
 
-    def __init__(self, user_id: int = None, user_email: str = None):
-        kwargs = {"userId": user_id, "userEmail": user_email}
+    def __init__(
+        self,
+        user_id: "Optional[int]" = None,
+        user_email: "Optional[str]" = None,
+    ):
+        kwargs: "Dict[str, Optional[Union[int, str]]]" = {
+            "userId": user_id,
+            "userEmail": user_email,
+        }
 
         super().__init__(**kwargs)
 
 
 class DocumentReportFilter(Filter):
     """
     Create a filter for the DocumentReport query.
@@ -168,36 +225,44 @@
         "created_at_end_date",
         "updated_at_start_date",
         "updated_at_end_date",
     )
 
     def __init__(
         self,
-        submission_id: int = None,
-        workflow_id: int = None,
-        status: str = None,
-        created_at_start_date: datetime = None,
-        created_at_end_date: datetime = None,
-        updated_at_start_date: datetime = None,
-        updated_at_end_date: datetime = None,
+        submission_id: "Optional[int]" = None,
+        workflow_id: "Optional[int]" = None,
+        status: "Optional[str]" = None,
+        created_at_start_date: "Optional[datetime.datetime]" = None,
+        created_at_end_date: "Optional[datetime.datetime]" = None,
+        updated_at_start_date: "Optional[datetime.datetime]" = None,
+        updated_at_end_date: "Optional[datetime.datetime]" = None,
     ):
-        kwargs = {"workflowId": workflow_id, "id": submission_id, "status": status}
+        kwargs: "AnyDict" = {
+            "workflowId": workflow_id,
+            "id": submission_id,
+            "status": status,
+        }
         if created_at_end_date and not created_at_start_date:
             raise IndicoInputError("Must specify created_at_start_date")
         if created_at_start_date:
             kwargs["createdAt"] = {
                 "from": created_at_start_date.strftime("%Y-%m-%d"),
-                "to": created_at_end_date.strftime("%Y-%m-%d")
-                if created_at_end_date is not None
-                else datetime.datetime.now().strftime("%Y-%m-%d"),
+                "to": (
+                    created_at_end_date.strftime("%Y-%m-%d")
+                    if created_at_end_date is not None
+                    else datetime.datetime.now().strftime("%Y-%m-%d")
+                ),
             }
 
         if updated_at_end_date and not updated_at_start_date:
             raise IndicoInputError("Must specify updated_at_start_date")
         if updated_at_start_date is not None:
             kwargs["updatedAt"] = {
                 "from": updated_at_start_date.strftime("%Y-%m-%d"),
-                "to": updated_at_end_date.strftime("%Y-%m-%d")
-                if updated_at_end_date is not None
-                else datetime.datetime.now().strftime("%Y-%m-%d"),
+                "to": (
+                    updated_at_end_date.strftime("%Y-%m-%d")
+                    if updated_at_end_date is not None
+                    else datetime.datetime.now().strftime("%Y-%m-%d")
+                ),
             }
         super().__init__(**kwargs)
```

### Comparing `indico-client-6.1.0a1/indico/http/client.py` & `indico-client-6.7.0a0/indico/http/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,85 @@
 import asyncio
-import aiohttp
-import http.cookiejar
 import logging
 from contextlib import contextmanager
 from copy import deepcopy
+from http.cookiejar import DefaultCookiePolicy
 from pathlib import Path
-from typing import Union, Optional
+from typing import TYPE_CHECKING, cast
 
+import aiohttp
 import requests
-from indico.client.request import HTTPRequest
+
 from indico.config import IndicoConfig
 from indico.errors import (
     IndicoAuthenticationFailed,
-    IndicoRequestError,
     IndicoHibernationError,
+    IndicoRequestError,
 )
-from indico.http.serialization import deserialize, aio_deserialize
+from indico.http.serialization import aio_deserialize, deserialize
+
 from .retry import aioretry
 
+if TYPE_CHECKING:  # pragma: no cover
+    from http.cookiejar import Cookie
+    from io import IOBase
+    from typing import Any, Dict, Iterator, List, Optional, Union
+    from urllib.request import Request
+
+    from indico.client.request import HTTPRequest, ResponseType
+    from indico.typing import AnyDict
+
+
 logger = logging.getLogger(__file__)
 
 
-class CookiePolicyOverride(http.cookiejar.DefaultCookiePolicy):
-    def set_ok(self, cookie, request):
+class CookiePolicyOverride(DefaultCookiePolicy):
+    def set_ok(self, cookie: "Cookie", request: "Request") -> bool:
         return True
 
-    def return_ok(self, cookie, request):
+    def return_ok(self, cookie: "Cookie", request: "Request") -> bool:
         return True
 
-    def path_return_ok(self, path, request):
+    def path_return_ok(self, path: str, request: "Request") -> bool:
         return True
 
-    def domain_return_ok(self, domain, request):
+    def domain_return_ok(self, domain: str, request: "Request") -> bool:
         return True
 
 
 class HTTPClient:
-    def __init__(self, config: IndicoConfig = None):
-        self.config = config
+    def __init__(self, config: "Optional[IndicoConfig]" = None):
+        self.config = config or IndicoConfig()
         self.base_url = f"{self.config.protocol}://{self.config.host}"
 
         self.request_session = requests.Session()
-        if config and isinstance(config.requests_params, dict):
-            for param in config.requests_params.keys():
-                setattr(self.request_session, param, config.requests_params[param])
+        if isinstance(self.config.requests_params, dict):
+            for param in self.config.requests_params.keys():
+                setattr(self.request_session, param, self.config.requests_params[param])
         self.request_session.cookies.set_policy(CookiePolicyOverride())
+
         self.get_short_lived_access_token()
 
-    def post(self, *args, json: Union[dict, list] = None, **kwargs):
+    def post(
+        self,
+        *args: "Any",
+        json: "Optional[Union[AnyDict, List[Any]]]" = None,
+        **kwargs: "Any",
+    ) -> "Any":
         return self._make_request("post", *args, json=json, **kwargs)
 
-    def get(self, *args, params: dict = None, **kwargs):
+    def get(
+        self, *args: "Any", params: "Optional[AnyDict]" = None, **kwargs: "Any"
+    ) -> "Any":
         return self._make_request("post", *args, params=params, **kwargs)
 
-    def get_short_lived_access_token(self):
-        # If the cookie here is already due to _disable_cookie_domain set and we try to pop it later
-        # it will error out because we have two cookies with the same name. We just remove the old one
-        # here as we are about to refresh it.
+    def get_short_lived_access_token(self) -> "AnyDict":
+        # If the cookie here is already due to _disable_cookie_domain set and we try to
+        # pop it later it will error out because we have two cookies with the same
+        # name. We just remove the old one here as we are about to refresh it.
         if "auth_token" in self.request_session.cookies:
             self.request_session.cookies.pop("auth_token")
 
         r = self.post(
             "/auth/users/refresh_token",
             headers={"Authorization": f"Bearer {self.config.api_token}"},
             _refreshed=True,
@@ -69,42 +88,42 @@
         # Disable cookie domain in cases where the domain won't match due to using short name domains
         if self.config._disable_cookie_domain:
             value = self.request_session.cookies.get("auth_token", None)
             if not value:
                 raise IndicoAuthenticationFailed()
             self.request_session.cookies.pop("auth_token")
             self.request_session.cookies.set_cookie(
-                requests.cookies.create_cookie(name="auth_token", value=value)
+                # must ignore because untyped in typeshed
+                requests.cookies.create_cookie(name="auth_token", value=value)  # type: ignore
             )
 
-        return r
+        return cast("AnyDict", r)
 
-    def execute_request(self, request: HTTPRequest):
+    def execute_request(self, request: "HTTPRequest[ResponseType]") -> "ResponseType":
         return request.process_response(
             self._make_request(
                 method=request.method.value.lower(), path=request.path, **request.kwargs
             )
         )
 
     @contextmanager
-    def _handle_files(self, req_kwargs):
-
+    def _handle_files(self, req_kwargs: "AnyDict") -> "Iterator[AnyDict]":
         streams = None
         # deepcopying buffers is not supported
         # so, remove "streams" before the deepcopy.
         if "streams" in req_kwargs:
             if req_kwargs["streams"] is not None:
                 streams = req_kwargs["streams"].copy()
             del req_kwargs["streams"]
 
-        new_kwargs = deepcopy(req_kwargs)
+        new_kwargs: "AnyDict" = deepcopy(req_kwargs)
 
-        files = []
+        files: "List[IOBase]" = []
         file_arg = {}
-        dup_counts = {}
+        dup_counts: "Dict[str, int]" = {}
         if "files" in new_kwargs and new_kwargs["files"] is not None:
             for filepath in new_kwargs["files"]:
                 path = Path(filepath)
                 fd = path.open("rb")
                 files.append(fd)
                 # follow the convention of adding (n) after a duplicate filename
                 if path.stem in dup_counts:
@@ -124,27 +143,28 @@
                     dup_counts[filename] += 1
                 else:
                     file_arg[filename] = stream
                     dup_counts[filename] = 1
 
         new_kwargs["files"] = file_arg
 
-        yield new_kwargs
-
-        if files:
-            [f.close() for f in files]
+        try:
+            yield new_kwargs
+        finally:
+            for f in files:
+                f.close()
 
     def _make_request(
         self,
         method: str,
         path: str,
-        headers: dict = None,
-        _refreshed=False,
-        **request_kwargs,
-    ):
+        headers: "Optional[Dict[str, str]]" = None,
+        _refreshed: bool = False,
+        **request_kwargs: "Any",
+    ) -> "Any":
         logger.debug(
             f"[{method}] {path}\n\t Headers: {headers}\n\tRequest Args:{request_kwargs}"
         )
         with self._handle_files(request_kwargs) as new_kwargs:
             response = getattr(self.request_session, method)(
                 f"{self.base_url}{path}",
                 headers=headers,
@@ -173,15 +193,17 @@
         if response.status_code >= 500:
             raise IndicoRequestError(
                 code=response.status_code,
                 error=response.reason,
                 extras=repr(response.content),
             )
 
-        content = deserialize(response, force_json=json, force_decompress=decompress)
+        content: "Any" = deserialize(
+            response, force_json=json, force_decompress=decompress
+        )
 
         if response.status_code >= 400:
             if isinstance(content, dict):
                 error = (
                     f"{content.pop('error_type', 'Unknown Error')}, "
                     f"{content.pop('message', '')}"
                 )
@@ -189,62 +211,74 @@
             else:
                 error = content
                 extras = None
 
             raise IndicoRequestError(
                 error=error, code=response.status_code, extras=extras
             )
+
         return content
 
 
-class AIOHTTPClient(HTTPClient):
+class AIOHTTPClient:
     """
     Beta client with a minimal set of features that can execute
     requests using the aiohttp library
     """
 
-    def __init__(self, config: Optional[IndicoConfig] = None):
+    def __init__(self, config: "Optional[IndicoConfig]" = None):
         """
         Config options specific to aiohttp
         unsafe - allows interacting with IP urls
         """
         self.config = config or IndicoConfig()
         self.base_url = f"{self.config.protocol}://{self.config.host}"
 
         self.request_session = aiohttp.ClientSession()
-        if config and isinstance(config.requests_params, dict):
-            for param in config.requests_params.keys():
-                setattr(self.request_session, param, config.requests_params[param])
+        if isinstance(self.config.requests_params, dict):
+            for param in self.config.requests_params.keys():
+                setattr(self.request_session, param, self.config.requests_params[param])
 
-    async def post(self, *args, json: Union[dict, list] = None, **kwargs):
+    async def post(
+        self,
+        *args: "Any",
+        json: "Optional[Union[AnyDict, List[Any]]]" = None,
+        **kwargs: "Any",
+    ) -> "Any":
         return await self._make_request("post", *args, json=json, **kwargs)
 
-    async def get(self, *args, params: dict = None, **kwargs):
+    async def get(
+        self, *args: "Any", params: "Optional[AnyDict]" = None, **kwargs: "Any"
+    ) -> "Any":
         return await self._make_request("post", *args, params=params, **kwargs)
 
-    async def get_short_lived_access_token(self):
+    async def get_short_lived_access_token(self) -> "AnyDict":
         r = await self.post(
             "/auth/users/refresh_token",
             headers={"Authorization": f"Bearer {self.config.api_token}"},
             _refreshed=True,
         )
-        return r
+        return cast("AnyDict", r)
 
-    async def execute_request(self, request: HTTPRequest):
+    async def execute_request(
+        self, request: "HTTPRequest[ResponseType]"
+    ) -> "ResponseType":
         return request.process_response(
             await self._make_request(
                 method=request.method.value.lower(), path=request.path, **request.kwargs
             )
         )
 
     @contextmanager
-    def _handle_files(self, req_kwargs):
+    def _handle_files(
+        self, req_kwargs: "AnyDict"
+    ) -> "Iterator[List[aiohttp.FormData]]":
         files = []
         file_args = []
-        dup_counts = {}
+        dup_counts: "Dict[str, int]" = {}
         for filepath in req_kwargs.pop("files", []) or []:
             data = aiohttp.FormData()
             path = Path(filepath)
             fd = path.open("rb")
             files.append(fd)
             # follow the convention of adding (n) after a duplicate filename
             _add_suffix = f".{path.suffix}" if path.suffix else ""
@@ -264,36 +298,37 @@
             # similar operation as above.
             files.append(stream)
             data = aiohttp.FormData()
             if filename in dup_counts:
                 data.add_field(
                     "file",
                     stream,
-                    filename=filename + f"({dup_counts[filename]})" + _add_suffix,
+                    filename=filename + f"({dup_counts[filename]})",
                 )
                 dup_counts[filename] += 1
             else:
                 data.add_field("file", stream, filename=filename)
                 dup_counts[filename] = 1
             file_args.append(data)
 
-        yield file_args
-
-        if files:
-            [f.close() for f in files]
+        try:
+            yield file_args
+        finally:
+            for f in files:
+                f.close()
 
-    @aioretry((aiohttp.ClientConnectionError, aiohttp.ServerDisconnectedError))
+    @aioretry(aiohttp.ClientConnectionError, aiohttp.ServerDisconnectedError)
     async def _make_request(
         self,
         method: str,
         path: str,
-        headers: dict = None,
-        _refreshed=False,
-        **request_kwargs,
-    ):
+        headers: "Optional[Dict[str, str]]" = None,
+        _refreshed: bool = False,
+        **request_kwargs: "Any",
+    ) -> "Any":
         logger.debug(
             f"[{method}] {path}\n\t Headers: {headers}\n\tRequest Args:{request_kwargs}"
         )
         json: bool = ".json" in Path(path).suffixes
         decompress: bool = Path(path).suffix == ".gz"
 
         with self._handle_files(request_kwargs) as file_args:
@@ -303,21 +338,21 @@
                         self._make_request(
                             method, path, headers, **request_kwargs, data=data
                         )
                         for data in file_args
                     )
                 )
                 return [resp for resp_set in resps for resp in resp_set]
+
             async with getattr(self.request_session, method)(
                 f"{self.base_url}{path}",
                 headers=headers,
                 verify_ssl=self.config.verify_ssl,
                 **request_kwargs,
             ) as response:
-
                 # If auth expired refresh
                 if response.status == 401 and not _refreshed:
                     await self.get_short_lived_access_token()
                     return await self._make_request(
                         method, path, headers, _refreshed=True, **request_kwargs
                     )
                 elif response.status == 401 and _refreshed:
@@ -331,15 +366,15 @@
                 if response.status >= 500:
                     raise IndicoRequestError(
                         code=response.status_code,
                         error=response.reason,
                         extras=repr(response.content),
                     )
 
-                content = await aio_deserialize(
+                content: "Any" = await aio_deserialize(
                     response, force_json=json, force_decompress=decompress
                 )
 
                 if response.status >= 400:
                     if isinstance(content, dict):
                         error = (
                             f"{content.pop('error_type', 'Unknown Error')}, "
@@ -349,8 +384,9 @@
                     else:
                         error = content
                         extras = None
 
                     raise IndicoRequestError(
                         error=error, code=response.status_code, extras=extras
                     )
+
                 return content
```

### Comparing `indico-client-6.1.0a1/indico/http/retry.py` & `indico-client-6.7.0a0/indico/http/retry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 import asyncio
-from random import randint
 import time
-import typing as t
 from functools import wraps
+from random import randint
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Awaitable, Callable, Optional, Tuple, Type, TypeVar, Union
 
+    from typing_extensions import ParamSpec
+
+    P = ParamSpec("P")
+    T = TypeVar("T")
 
 
 def retry(
-    ExceptionTypes: t.Type[Exception], tries: int = 3, delay: int = 1, backoff: int = 2
-) -> t.Callable:
+    *ExceptionTypes: "Type[Exception]", tries: int = 3, delay: int = 1, backoff: int = 2
+) -> "Callable[[Callable[P, T]], Callable[P, T]]":
     """
     Retry with exponential backoff
 
     Original from: http://wiki.python.org/moin/PythonDecoratorLibrary#Retry
     """
 
-    def retry_decorator(f: t.Callable) -> t.Any:
+    def retry_decorator(f: "Callable[P, T]") -> "Callable[P, T]":
         @wraps(f)
-        def retry_fn(*args: t.Any, **kwargs: t.Any) -> t.Any:
+        def retry_fn(*args: "P.args", **kwargs: "P.kwargs") -> "T":
             n_tries, n_delay = tries, delay
             while n_tries > 1:
                 try:
                     return f(*args, **kwargs)
                 except ExceptionTypes:
                     time.sleep(n_delay)
                     n_tries -= 1
                     n_delay *= backoff
             return f(*args, **kwargs)
 
         return retry_fn
 
     return retry_decorator
 
+
 def aioretry(
-    ExceptionTypes: t.Type[Exception],
+    *ExceptionTypes: "Type[Exception]",
     tries: int = 3,
-    delay: t.Union[int, t.Tuple[int, int]] = 1,
+    delay: "Union[int, Tuple[int, int]]" = 1,
     backoff: int = 2,
-    condition: t.Optional[t.Callable[[Exception], bool]] = None,
-) -> t.Callable:
+    condition: "Optional[Callable[[Exception], bool]]" = None,
+) -> "Callable[[Callable[P, Awaitable[T]]], Callable[P, Awaitable[T]]]":
     """
     Retry with exponential backoff
 
     Original from: http://wiki.python.org/moin/PythonDecoratorLibrary#Retry
     Options:
         condition: Callable to evaluate if an exception of a given type
             is retryable for additional handling
         delay: an initial time to wait (seconds). If a tuple, choose a random number
             in that range to start. This can helps prevent retries at the exact
             same time across multiple concurrent function calls
     """
 
-    def retry_decorator(f: t.Callable) -> t.Callable:
+    def retry_decorator(f: "Callable[P, Awaitable[T]]") -> "Callable[P, Awaitable[T]]":
         @wraps(f)
-        async def retry_fn(*args: t.Any, **kwargs: t.Any) -> t.Any:
+        async def retry_fn(*args: "P.args", **kwargs: "P.kwargs") -> "T":
             n_tries = tries
             if isinstance(delay, tuple):
                 # pick a random number to sleep
                 n_delay = randint(*delay)
             else:
                 n_delay = delay
             while True:
```

### Comparing `indico-client-6.1.0a1/indico/http/serialization.py` & `indico-client-6.7.0a0/indico/http/serialization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 """
 Handles deserialization / decoding of responses
 """
+
 import cgi
 import gzip
 import io
 import json
 import logging
 import traceback
 from collections import defaultdict
+from typing import TYPE_CHECKING
 
 import msgpack
 
 from indico.errors import IndicoDecodingError
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Callable, Mapping, Optional
+
+    from aiohttp import ClientResponse
+    from requests import Response
+
 logger = logging.getLogger(__name__)
 
 
-def decompress(response):
+def decompress(response: "Response") -> bytes:
     response.raw.decode_content = True
-    value = io.BytesIO(response.raw.data).getvalue()
+    value: bytes = io.BytesIO(response.raw.data).getvalue()
     return gzip.decompress(value)
 
 
-def deserialize(response, force_json=False, force_decompress=False):
-    content_type, params = cgi.parse_header(response.headers.get("Content-Type"))
+def deserialize(
+    response: "Response", force_json: bool = False, force_decompress: bool = False
+) -> "Any":
+    content_type, params = cgi.parse_header(response.headers["Content-Type"])
+    content: bytes
 
     if force_decompress or content_type in ["application/x-gzip", "application/gzip"]:
         content = decompress(response)
     else:
         content = response.content
 
     charset = params.get("charset", "utf-8")
@@ -40,87 +51,91 @@
         return _SERIALIZATION_FNS[content_type](content, charset)
     except Exception:
         logger.debug(traceback.format_exc())
         raise IndicoDecodingError(
             content_type, charset, content.decode("ascii", "ignore")
         )
 
-async def aio_deserialize(response, force_json=False, force_decompress=False):
-    content_type, params = cgi.parse_header(response.headers.get("Content-Type"))
-    content = await response.read()
+
+async def aio_deserialize(
+    response: "ClientResponse", force_json: bool = False, force_decompress: bool = False
+) -> "Any":
+    content_type, params = cgi.parse_header(response.headers["Content-Type"])
+    content: bytes = await response.read()
 
     if force_decompress or content_type in ["application/x-gzip", "application/gzip"]:
-        content = gzip.decompress(io.BytesIO(content).get_value())
+        content = gzip.decompress(io.BytesIO(content).getvalue())
 
-    charset = params.get("charset", "utf-8")
+    charset: str = params.get("charset", "utf-8")
 
     # For storage object for example where the content is json based on url ending
     if force_json:
         content_type = "application/json"
 
     try:
         return _SERIALIZATION_FNS[content_type](content, charset)
     except Exception:
         logger.debug(traceback.format_exc())
         raise IndicoDecodingError(
             content_type, charset, content.decode("ascii", "ignore")
         )
 
-def raw_bytes(content, *args, **kwargs):
+
+def raw_bytes(
+    content: bytes, charset: "Optional[str]", *args: "Any", **kwargs: "Any"
+) -> bytes:
     return content
 
 
-def msgpack_deserialization(content, charset):
+def msgpack_deserialization(content: bytes, charset: "Optional[str]" = None) -> "Any":
     return msgpack.unpackb(content)
 
 
-def json_deserialization(content, charset="utf-8"):
+def json_deserialization(content: bytes, charset: str = "utf-8") -> "Any":
     return json.loads(content.decode(charset))
 
 
-def text_deserialization(content, charset="utf-8"):
+def text_deserialization(content: bytes, charset: str = "utf-8") -> str:
     return content.decode(charset)
 
 
-def image_serialization(content, charset=None):
+def image_serialization(content: bytes, charset: "Optional[str]" = None) -> bytes:
     return content
 
 
-def zip_serialization(content, charset=None):
+def zip_serialization(content: bytes, charset: "Optional[str]" = None) -> bytes:
     return content
 
 
-_SERIALIZATION_FNS = defaultdict(
+_SERIALIZATION_FNS: "Mapping[str, Callable[[bytes, str], Any]]" = defaultdict(
     lambda: text_deserialization,
     {
         "application/pdf": raw_bytes,
         "application/octet-stream": raw_bytes,
         "application/doc": raw_bytes,
         "application/ms-doc": raw_bytes,
         "application/msword": raw_bytes,
         "application/vnd.openxmlformats-officedocument.wordprocessingml.document": raw_bytes,
         "application/vnd.oasis.opendocument.text": raw_bytes,
         "application/zip": zip_serialization,
         "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet": raw_bytes,
         "application/vnd.ms-excel": raw_bytes,
         "application/msexcel": raw_bytes,
         "application/excel": raw_bytes,
-        "application/msexcel": raw_bytes,
         "application/x-dos_ms_excel": raw_bytes,
         "application/x-excel": raw_bytes,
         "application/x-ms-excel": raw_bytes,
         "application/x-xls": raw_bytes,
         "application/xlc": raw_bytes,
         "application/xls": raw_bytes,
         "application/xlt": raw_bytes,
         "application/vnd.ms-powerpoint": raw_bytes,
         "application/vnd.openxmlformats-officedocument.presentationml.presentation": raw_bytes,
         "application/mspowerpoint": raw_bytes,
         "application/powerpoint": raw_bytes,
-        "application/vnd.ms-powerpoint": raw_bytes,
         "application/x-mspowerpoint": raw_bytes,
         "image/png": image_serialization,
         "image/jpeg": image_serialization,
         "image/jpg": image_serialization,
         "image/tiff": image_serialization,
         "text/html": text_deserialization,
         "text/plain": text_deserialization,
```

### Comparing `indico-client-6.1.0a1/indico/queries/custom_blueprint.py` & `indico-client-6.7.0a0/indico/queries/custom_blueprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-import typing as t
+from typing import TYPE_CHECKING
 
 from indico import GraphQLRequest
 from indico.errors import IndicoInputError
-from indico.types.workflow import ComponentFamily
 from indico.types.custom_blueprint import TaskBlueprint
+from indico.types.workflow import ComponentFamily
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import List, Optional
+
+    from indico.typing import AnyDict, Payload
+
 
-SUPPORTED_CUSTOM_COMPONENT_FAMILIES = [
+SUPPORTED_CUSTOM_COMPONENT_FAMILIES: "List[ComponentFamily]" = [
     ComponentFamily.OUTPUT,
     ComponentFamily.FILTER,
     ComponentFamily.MODEL,
 ]
 
 
-class RegisterCustomBlueprint(GraphQLRequest):
+class RegisterCustomBlueprint(GraphQLRequest["TaskBlueprint"]):
     """
     Mutation to register a custom blueprint, making it available in the gallery to add to workflows
 
     Args:
         component_family (ComponentFamily): family this blueprint belongs to; supported families are Output, Filter, and Model
         name (str): Name of the blueprint
         description (str): Description of this blueprint
@@ -66,23 +72,23 @@
     config
   }}
 }}
 """
 
     def __init__(
         self,
-        component_family: ComponentFamily,
+        component_family: "ComponentFamily",
         name: str,
         description: str,
-        config: t.Dict,
-        tags: t.List[str],
+        config: "AnyDict",
+        tags: "List[str]",
         footer: str = "",
-        icon: str = None,
-        all_access: bool = None,
-        dataset_ids: t.List[int] = None,
+        icon: "Optional[str]" = None,
+        all_access: "Optional[bool]" = None,
+        dataset_ids: "Optional[List[int]]" = None,
     ):
         if (
             not component_family
             or not name
             or not description
             or not config
             or not tags
@@ -129,9 +135,9 @@
                 "tags": tags,
                 "icon": icon,
                 "allAccess": all_access,
                 "datasetIds": dataset_ids,
             },
         )
 
-    def process_response(self, response) -> TaskBlueprint:
-        return TaskBlueprint(**super().process_response(response)[self.mutation_name])
+    def process_response(self, response: "Payload") -> "TaskBlueprint":
+        return TaskBlueprint(**super().parse_payload(response)[self.mutation_name])
```

### Comparing `indico-client-6.1.0a1/indico/queries/datasets.py` & `indico-client-6.7.0a0/indico/queries/datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # -*- coding: utf-8 -*-
 
 import json
-import jsons
 import tempfile
 from pathlib import Path
-from typing import List, Union, Dict, Optional
+from typing import TYPE_CHECKING
 
+import jsons
 import pandas as pd
-import deprecation
 
 from indico.client.request import (
-    Debouncer,
+    Delay,
     GraphQLRequest,
     HTTPMethod,
     HTTPRequest,
     PagedRequest,
     RequestChain,
 )
-from indico.errors import IndicoNotFound, IndicoInputError
-from indico.queries.storage import UploadBatched, UploadImages
-from indico.types.dataset import (
-    Dataset,
-    OcrEngine,
-    OmnipageOcrOptionsInput,
-    ReadApiOcrOptionsInput,
-    OcrInputLanguage,
-)
+from indico.errors import IndicoInputError, IndicoNotFound
 from indico.filters import DatasetFilter
+from indico.queries.storage import UploadBatched, UploadImages
+from indico.types.dataset import Dataset, OcrEngine, OcrInputLanguage
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Iterator, List, Optional, Union
 
+    from indico.types.dataset import OmnipageOcrOptionsInput, ReadApiOcrOptionsInput
+    from indico.typing import AnyDict, Payload
 
-class ListDatasets(PagedRequest):
+
+class ListDatasets(PagedRequest["List[Dataset]"]):
     """
     List all of your datasets
 
     Options:
         limit (int, default=100): Max number of datasets to retrieve
 
     Returns:
@@ -67,35 +66,35 @@
             }
         }
     """
 
     def __init__(
         self,
         *,
-        filters: Optional[Union[Dict, DatasetFilter]] = None,
+        filters: "Optional[Union[AnyDict, DatasetFilter]]" = None,
         limit: int = 100,
         order_by: str = "ID",
         desc: bool = False,
     ):
         super().__init__(
             self.query,
             variables={
                 "filters": filters,
                 "limit": limit,
                 "orderBy": order_by,
                 "desc": desc,
             },
         )
 
-    def process_response(self, response) -> List[Dataset]:
-        response = super().process_response(response)
+    def process_response(self, response: "Payload") -> "List[Dataset]":
+        response = super().parse_payload(response)
         return [Dataset(**dataset) for dataset in response["datasetsPage"]["datasets"]]
 
 
-class GetDataset(GraphQLRequest):
+class GetDataset(GraphQLRequest["Dataset"]):
     """
     Retrieve a dataset description object
 
     Args:
         id (int): id of the dataset to query
 
     Returns:
@@ -121,16 +120,16 @@
             }
         }
     """
 
     def __init__(self, id: int):
         super().__init__(self.query, variables={"id": id})
 
-    def process_response(self, response) -> Dataset:
-        response = super().process_response(response)
+    def process_response(self, response: "Payload") -> "Dataset":
+        response = super().parse_payload(response)
         if "dataset" not in response or not isinstance(response["dataset"], dict):
             raise IndicoNotFound("Failed to find dataset")
         return Dataset(**response["dataset"])
 
 
 class GetDatasetFileStatus(GetDataset):
     """
@@ -161,15 +160,15 @@
                     failureType
                 }
             }
         }
     """
 
 
-class GetDatasetStatus(GraphQLRequest):
+class GetDatasetStatus(GraphQLRequest[str]):
     """
     Get the status of a dataset
 
     Args:
         id (int): id of the dataset to query
 
     Returns:
@@ -183,68 +182,81 @@
             }
         }
     """
 
     def __init__(self, id: int):
         super().__init__(self.query, variables={"id": id})
 
-    def process_response(self, response) -> str:
-        return response["data"]["dataset"]["status"]
+    def process_response(self, response: "Payload") -> str:
+        status: str = super().parse_payload(response)["dataset"]["status"]
+        return status
 
 
-class CreateDataset(RequestChain):
+class CreateDataset(RequestChain["Dataset"]):
     """
     Create a dataset and upload the associated files.
 
     Args:
-        name (str): Name of the dataset
-        files (List[str]): List of pathnames to the dataset files
-
-    Options:
-        dataset_type (str): Type of dataset to create [TEXT, DOCUMENT, IMAGE]
-        wait (bool, default=True): Wait for the dataset to upload and finish
+        name (str): Name of the dataset.
+        files (List[str]): List of path names to the dataset files.
+        wait (bool, optional): Wait for the dataset to upload and finish. Defaults to True.
+        dataset_type (str, optional): Type of dataset to create [TEXT, DOCUMENT, IMAGE]. Defaults to TEXT.
+        from_local_images (bool, optional): Flag whether files are local images or not. Defaults to False.
+        image_filename_col (str, optional): Image filename column. Defaults to 'filename'.
+        batch_size (int, optional): Size of file batch to upload at a time. Defaults to 20.
+        ocr_engine (OcrEngine, optional): Specify an OCR engine [OMNIPAGE, READAPI, READAPI_V2, READAPI_TABLES_V1]. Defaults to None.
+        omnipage_ocr_options (OmnipageOcrOptionsInput, optional): If using Omnipage, specify Omnipage OCR options. Defaults to None.
+        read_api_ocr_options: (ReadApiOcrOptionsInput, optional): If using ReadAPI, specify ReadAPI OCR options. Defaults to None.
+        request_interval (int or float, optional): The maximum time in between retry calls when waiting. Defaults to 5 seconds.
 
     Returns:
         Dataset object
 
     """
 
-    previous = None
-
     def __init__(
         self,
         name: str,
-        files: List[str],
+        files: "Union[str, List[str]]",
         wait: bool = True,
         dataset_type: str = "TEXT",
         from_local_images: bool = False,
         image_filename_col: str = "filename",
         batch_size: int = 20,
-        ocr_engine: OcrEngine = None,
-        omnipage_ocr_options: OmnipageOcrOptionsInput = None,
-        read_api_ocr_options: ReadApiOcrOptionsInput = None,
+        ocr_engine: "Optional[OcrEngine]" = None,
+        omnipage_ocr_options: "Optional[OmnipageOcrOptionsInput]" = None,
+        read_api_ocr_options: "Optional[ReadApiOcrOptionsInput]" = None,
+        request_interval: "Union[int, float]" = 5,
     ):
         self.files = files
         self.name = name
         self.wait = wait
         self.dataset_type = dataset_type
         self.from_local_images = from_local_images
         self.image_filename_col = image_filename_col
         self.batch_size = batch_size
         self.ocr_engine = ocr_engine
         self.omnipage_ocr_options = omnipage_ocr_options
         self.read_api_ocr_options = read_api_ocr_options
+        self.request_interval = request_interval
         if omnipage_ocr_options is not None and read_api_ocr_options is not None:
             raise IndicoInputError(
                 "Must supply either omnipage or readapi options but not both."
             )
         super().__init__()
 
-    def requests(self):
+    def requests(
+        self,
+    ) -> "Iterator[Union[UploadBatched, _UploadDatasetFiles, CreateEmptyDataset, _AddFiles, GetDatasetFileStatus, Delay, GetDataset]]":
         if self.from_local_images:
+            if not isinstance(self.files, str):
+                raise ValueError(
+                    "'files' should be a string path when using `from_local_images`."
+                )
+
             self.dataset_type = "IMAGE"
             # Assume image filenames are in the same directory as the csv with
             # image labels and that there is a column representing their name
             df = pd.read_csv(self.files)
             img_filenames = df[self.image_filename_col].tolist()
             img_filepaths = [
                 str(Path(self.files).parent / imgfn) for imgfn in img_filenames
@@ -256,43 +268,46 @@
             )
             df["urls"] = self.previous
             with tempfile.TemporaryDirectory() as tmpdir:
                 image_csv_path = str(Path(tmpdir) / "image_urls.csv")
                 df.to_csv(image_csv_path)
                 yield _UploadDatasetFiles(files=[image_csv_path])
         else:
+            if not isinstance(self.files, list):
+                raise ValueError("'files' should be a list of paths.")
+
             yield UploadBatched(
                 files=self.files,
                 batch_size=self.batch_size,
                 request_cls=_UploadDatasetFiles,
             )
+
         file_metadata = self.previous
         yield CreateEmptyDataset(
             name=self.name,
             dataset_type=self.dataset_type,
             readapi_ocr_options=self.read_api_ocr_options,
             omnipage_ocr_options=self.omnipage_ocr_options,
             ocr_engine=self.ocr_engine,
         )
         yield _AddFiles(
             dataset_id=self.previous.id, metadata=file_metadata, autoprocess=True
         )
         dataset_id = self.previous.id
         yield GetDatasetFileStatus(id=dataset_id)
-        debouncer = Debouncer()
         if self.wait is True:
             while not all(
                 [f.status in ["PROCESSED", "FAILED"] for f in self.previous.files]
             ):
                 yield GetDatasetFileStatus(id=dataset_id)
-                debouncer.backoff()
+                yield Delay(seconds=self.request_interval)
         yield GetDataset(id=dataset_id)
 
 
-class RemoveDatasetFile(GraphQLRequest):
+class RemoveDatasetFile(GraphQLRequest["Dataset"]):
     """
     Remove a file from a dataset by ID.  To retrieve a list of files in a dataset,
     see `GetDatasetFileStatus`.
 
     Args:
         dataset_id (int): Dataset ID
         file_id (int): Datafile ID (returned by GetDatasetFileStatus)
@@ -312,26 +327,26 @@
 
     def __init__(self, dataset_id: int, file_id: int):
         super().__init__(
             self.query,
             variables={"datasetId": dataset_id, "fileId": file_id},
         )
 
-    def process_response(self, response):
-        return Dataset(**super().process_response(response)["deleteDatasetFile"])
+    def process_response(self, response: "Payload") -> "Dataset":
+        return Dataset(**super().parse_payload(response)["deleteDatasetFile"])
 
 
-class _UploadDatasetFiles(HTTPRequest):
-    def __init__(self, files: List[str]):
+class _UploadDatasetFiles(HTTPRequest["List[AnyDict]"]):
+    def __init__(self, files: "List[str]"):
         super().__init__(
             method=HTTPMethod.POST, path="/storage/files/upload", files=files
         )
 
 
-class DeleteDataset(GraphQLRequest):
+class DeleteDataset(GraphQLRequest[bool]):
     """
     Delete a dataset
 
     Args:
         id (int): ID of the dataset
 
     Returns:
@@ -342,38 +357,39 @@
     mutation deleteDataset($id: Int!) {
         deleteDataset(id: $id) {
             success
         }
     }
     """
 
-    def __init__(self, id):
+    def __init__(self, id: int):
         super().__init__(self.query, variables={"id": id})
 
-    def process_response(self, response):
-        return super().process_response(response)["deleteDataset"]["success"]
+    def process_response(self, response: "Payload") -> bool:
+        status: bool = super().parse_payload(response)["deleteDataset"]["success"]
+        return status
 
 
-class CreateEmptyDataset(GraphQLRequest):
+class CreateEmptyDataset(GraphQLRequest["Dataset"]):
     query = """
     mutation($name: String!, $datasetType: DatasetType, $config: DataConfigInput) {
         createDataset(name: $name, datasetType: $datasetType, config: $config ) {
             id
             name
         }
     }
     """
 
     def __init__(
         self,
         name: str,
-        dataset_type: str = None,
-        ocr_engine: OcrEngine = None,
-        omnipage_ocr_options: OmnipageOcrOptionsInput = None,
-        readapi_ocr_options: ReadApiOcrOptionsInput = None,
+        dataset_type: "Optional[str]" = None,
+        ocr_engine: "Optional[OcrEngine]" = None,
+        omnipage_ocr_options: "Optional[OmnipageOcrOptionsInput]" = None,
+        readapi_ocr_options: "Optional[ReadApiOcrOptionsInput]" = None,
     ):
         if not dataset_type:
             dataset_type = "TEXT"
         config = None
         if ocr_engine is not None:
             config = {
                 "ocrOptions": {
@@ -391,43 +407,43 @@
                     config,
                     key_transformer=jsons.KEY_TRANSFORMER_CAMELCASE,
                     strip_nulls=True,
                 ),
             },
         )
 
-    def process_response(self, response):
-        return Dataset(**super().process_response(response)["createDataset"])
+    def process_response(self, response: "Payload") -> "Dataset":
+        return Dataset(**super().parse_payload(response)["createDataset"])
 
 
-class _AddFiles(GraphQLRequest):
+class _AddFiles(GraphQLRequest["Dataset"]):
     query = """
     mutation AddFiles($datasetId: Int!, $metadata: JSONString!, $autoprocess: Boolean){
         addDatasetFiles(datasetId: $datasetId, metadataList: $metadata, autoprocess: $autoprocess) {
             id
             status
         }
     }
     """
 
-    def __init__(self, dataset_id: int, metadata: List[str], autoprocess: bool):
+    def __init__(self, dataset_id: int, metadata: "List[str]", autoprocess: bool):
         super().__init__(
             self.query,
             variables={
                 "datasetId": dataset_id,
                 "metadata": json.dumps(metadata),
                 "autoprocess": autoprocess,
             },
         )
 
-    def process_response(self, response):
-        return Dataset(**super().process_response(response)["addDatasetFiles"])
+    def process_response(self, response: "Payload") -> "Dataset":
+        return Dataset(**super().parse_payload(response)["addDatasetFiles"])
 
 
-class AddDatasetFiles(RequestChain):
+class AddDatasetFiles(RequestChain["Dataset"]):
     """
     Add files to a dataset.
 
     Args:
         dataset_id (int): ID of the dataset
         files (List[str]): List of pathnames to the dataset files
 
@@ -436,20 +452,18 @@
         wait (bool, default=True): Block while polling for status of files
         batch_size (int, default=20): Batch size for uploading files
 
     Returns:
         Dataset
     """
 
-    previous = None
-
     def __init__(
         self,
         dataset_id: int,
-        files: List[str],
+        files: "List[str]",
         autoprocess: bool = False,
         wait: bool = True,
         batch_size: int = 20,
     ):
         self.dataset_id = dataset_id
         self.files = files
         self.wait = wait
@@ -458,177 +472,62 @@
         self.expected_statuses = (
             {"FAILED", "PROCESSED"}
             if autoprocess
             else {"DOWNLOADED", "FAILED", "PROCESSED"}
         )
         super().__init__()
 
-    def requests(self):
+    def requests(
+        self,
+    ) -> "Iterator[Union[UploadBatched, _AddFiles, GetDatasetFileStatus, Delay]]":
         yield UploadBatched(
             files=self.files,
             batch_size=self.batch_size,
             request_cls=_UploadDatasetFiles,
         )
         yield _AddFiles(
             dataset_id=self.dataset_id,
             metadata=self.previous,
             autoprocess=self.autoprocess,
         )
         yield GetDatasetFileStatus(id=self.dataset_id)
         if self.wait:
-            debouncer = Debouncer()
             while not all(
                 f.status in self.expected_statuses for f in self.previous.files
             ):
+                yield Delay()
                 yield GetDatasetFileStatus(id=self.previous.id)
-                debouncer.backoff()
 
 
 # Alias for backwards compatibility
 AddFiles = AddDatasetFiles
 
 
-class _ProcessFiles(GraphQLRequest):
-    query = """
-    mutation (
-        $datasetId: Int!,
-        $datafileIds: [Int]) {
-        addDataFiles(
-          datasetId: $datasetId,
-          datafileIds: $datafileIds) {
-            id
-            name
-        }
-    }
-    """
-
-    def __init__(self, dataset_id: int, datafile_ids: List[int]):
-        super().__init__(
-            self.query,
-            variables={"datasetId": dataset_id, "datafileIds": datafile_ids},
-        )
-
-    def process_response(self, response):
-        return Dataset(**super().process_response(response)["addDataFiles"])
-
-
-class _ProcessCSV(GraphQLRequest):
-    query = """
-    mutation ($datasetId: Int!, $datafileIds: [Int]) {
-        addDataCsv(datasetId: $datasetId, datafileIds: $datafileIds) {
-            id
-            name
-        }
-    }
-    """
-
-    def __init__(self, dataset_id: int, datafile_ids: List[int]):
-        super().__init__(
-            self.query, variables={"datasetId": dataset_id, "datafileIds": datafile_ids}
-        )
-
-    def process_response(self, response):
-        return Dataset(**super().process_response(response)["addDataCsv"])
-
-
-@deprecation.deprecated(
-    deprecated_in="5.3", details="Use AddFiles wtih autoprocess=True instead"
-)
-class ProcessFiles(RequestChain):
-    """
-    Process files associated with a dataset and add corresponding data to the dataset
-
-    Args:
-        dataset_id (int): ID of the dataset
-        datafile_ids (List[str]): IDs of the datafiles to process
-        wait (bool): Block while polling for status of files
-
-
-    Returns:
-        Dataset
-    """
-
-    def __init__(
-        self,
-        dataset_id: int,
-        datafile_ids: List[int],
-        wait: bool = True,
-    ):
-        self.dataset_id = dataset_id
-        self.datafile_ids = datafile_ids
-        self.wait = wait
-
-    def requests(self):
-        yield _ProcessFiles(self.dataset_id, self.datafile_ids)
-        debouncer = Debouncer()
-        yield GetDatasetFileStatus(id=self.dataset_id)
-        if self.wait:
-            while not all(
-                f.status in ["PROCESSED", "FAILED"] for f in self.previous.files
-            ):
-                yield GetDatasetFileStatus(id=self.dataset_id)
-                debouncer.backoff()
-
-
-@deprecation.deprecated(
-    deprecated_in="5.3", details="Use AddFiles wtih autoprocess=True instead"
-)
-class ProcessCSV(RequestChain):
-    """
-    Process CSV associated with a dataset and add corresponding data to the dataset
-
-    Args:
-        dataset_id (int): ID of the dataset
-        datafile_ids (List[str]): IDs of the CSV datafiles to process
-    Options:
-        wait (bool, default=True): Block while polling for status of files
-
-    Returns:
-        Dataset
-    """
-
-    def __init__(self, dataset_id: int, datafile_ids: List[int], wait: bool = True):
-        self.dataset_id = dataset_id
-        self.datafile_ids = datafile_ids
-        self.wait = wait
-
-    def requests(self):
-        yield _ProcessCSV(self.dataset_id, self.datafile_ids)
-        debouncer = Debouncer()
-        yield GetDatasetFileStatus(id=self.dataset_id)
-        if self.wait:
-            while not all(
-                f.status in ["PROCESSED", "FAILED"] for f in self.previous.files
-            ):
-                yield GetDatasetFileStatus(id=self.dataset_id)
-                debouncer.backoff()
-
-
-class GetAvailableOcrEngines(GraphQLRequest):
+class GetAvailableOcrEngines(GraphQLRequest["List[OcrEngine]"]):
     """
     Fetches and lists the available OCR engines
     """
 
     query = """query{
         ocrOptions {
             engines{
                 name
             }
         }
     }"""
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(self.query)
 
-    def process_response(self, response):
-        engines = super().process_response(response)["ocrOptions"]["engines"]
+    def process_response(self, response: "Payload") -> "List[OcrEngine]":
+        engines = super().parse_payload(response)["ocrOptions"]["engines"]
         return [OcrEngine[e["name"]] for e in engines]
 
 
-class GetOcrEngineLanguageCodes(GraphQLRequest):
+class GetOcrEngineLanguageCodes(GraphQLRequest["List[OcrInputLanguage]"]):
     """
     Fetches and lists the available languages by name and code for the given OCR Engine
 
     Args:
         ocr_engine(OcrEngine): The engine to fetch for.
     """
 
@@ -640,17 +539,17 @@
                 name
                 code
                 }
             }
         }
     }"""
 
-    def __init__(self, engine: OcrEngine):
+    def __init__(self, engine: "OcrEngine"):
         self.engine = engine
         super().__init__(self.query)
 
-    def process_response(self, response):
-        data = super().process_response(response)["ocrOptions"]["engines"]
+    def process_response(self, response: "Payload") -> "List[OcrInputLanguage]":
+        data = super().parse_payload(response)["ocrOptions"]["engines"]
         engine_laguages = next(
             x["languages"] for x in data if x["name"] == self.engine.name
         )
         return [OcrInputLanguage(**option) for option in engine_laguages]
```

### Comparing `indico-client-6.1.0a1/indico/queries/document_report.py` & `indico-client-6.7.0a0/indico/queries/document_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """"""
-from typing import List, Union
+
+from typing import TYPE_CHECKING, List
 
 from indico import PagedRequest
 from indico.filters import DocumentReportFilter
 from indico.types import BaseType
 from indico.types.document_report import DocumentReport
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Optional, Union
+
+    from indico.typing import AnyDict, Payload
+
 
 class _DocumentReportList(BaseType):
     submissions: List[DocumentReport]
-    pass
 
 
-class GetDocumentReport(PagedRequest):
+class GetDocumentReport(PagedRequest["List[DocumentReport]"]):
     """
     Query to generate a Document Report, otherwise known as a log of past submissions.
     """
 
     query = """
        query SubmissionsLog($filters: SubmissionLogFilter, $limit: Int, $after: Int, $allSubmissions: Boolean){
           submissionsLog(filters: $filters, limit: $limit, after: $after, allSubmissions: $allSubmissions){
@@ -28,15 +33,15 @@
               createdBy
               updatedAt
               updatedBy
               completedAt
               errors
               retrieved
               submissionId
-              deleted
+              filesDeleted
               inputFiles{
                 id
                 filename
                 filepath
                 submissionId
                 fileSize
                 numPages
@@ -49,16 +54,23 @@
               aggregateCount
             }
           }
         }
         """
 
     def __init__(
-        self, filters: Union[dict, DocumentReportFilter] = None, limit: int = None, all_submissions = False
+        self,
+        filters: "Optional[Union[AnyDict, DocumentReportFilter]]" = None,
+        limit: "Optional[int]" = None,
+        all_submissions: bool = False,
     ):
-        variables = {"filters": filters, "limit": limit, "allSubmissions": all_submissions}
+        variables = {
+            "filters": filters,
+            "limit": limit,
+            "allSubmissions": all_submissions,
+        }
         super().__init__(self.query, variables=variables)
 
-    def process_response(self, response):
+    def process_response(self, response: "Payload") -> "List[DocumentReport]":
         return _DocumentReportList(
-            **super().process_response(response)["submissionsLog"]
+            **super().parse_payload(response)["submissionsLog"]
         ).submissions
```

### Comparing `indico-client-6.1.0a1/indico/queries/documents.py` & `indico-client-6.7.0a0/indico/queries/documents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 # -*- coding: utf-8 -*-
 
 import json
-from typing import List
+from typing import TYPE_CHECKING
 
-from indico.client.request import RequestChain, GraphQLRequest, HTTPMethod, HTTPRequest
+from indico.client.request import GraphQLRequest, RequestChain
+from indico.queries.storage import UploadBatched, UploadDocument
 from indico.types.jobs import Job
-from indico.queries.storage import UploadDocument, UploadBatched
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Iterator, List, Optional, Union
 
-class _DocumentExtraction(GraphQLRequest):
+    from indico.typing import AnyDict, Payload
 
+
+class _DocumentExtraction(GraphQLRequest["List[Job]"]):
     query = """
         mutation($files: [FileInput], $jsonConfig: JSONString, $ocrEngine: OCREngine) {
             documentExtraction(files: $files, jsonConfig: $jsonConfig, ocrEngine: $ocrEngine) {
                 jobIds
             }
         }
     """
 
-    def __init__(self, files, json_config={"preset_config": "legacy"}, ocr_engine=None):
-        if json_config and type(json_config) == dict:
-            json_config = json.dumps(json_config)
+    def __init__(
+        self,
+        files: "List[AnyDict]",
+        json_config: "Optional[Union[AnyDict, str]]" = {"preset_config": "legacy"},
+        ocr_engine: "Optional[str]" = None,
+    ):
+        json_config_json: "Optional[str]" = None
+        if json_config:
+            if isinstance(json_config, dict):
+                json_config_json = json.dumps(json_config)
+            else:
+                json_config_json = json_config
+
         super().__init__(
-            query=self.query, variables={"files": files, "jsonConfig": json_config, "ocrEngine": ocr_engine}
+            query=self.query,
+            variables={
+                "files": files,
+                "jsonConfig": json_config_json,
+                "ocrEngine": ocr_engine,
+            },
         )
 
-    def process_response(self, response):
-        jobs = super().process_response(response)["documentExtraction"]["jobIds"]
-        if jobs:
-            return [Job(id=j) for j in jobs]
-        else:
-            return []
+    def process_response(self, response: "Payload") -> "List[Job]":
+        jobs = super().parse_payload(response)["documentExtraction"]["jobIds"] or set()
+        return [Job(id=j) for j in jobs]
 
 
-class DocumentExtraction(RequestChain):
+class DocumentExtraction(RequestChain["Job"]):
     """
     Extract raw text from PDF or TIF files.
 
     DocumentExtraction performs Optical Character Recognition (OCR) on PDF or TIF files to
     extract raw text for model training and prediction.
 
     Args:
@@ -63,24 +79,35 @@
         standard - Provides page text and block text/position in a nested format.
 
         For more information, please reference the Indico knowledgebase article on OCR:
         https://docs.indicodata.ai/articles/documentation-publication/ocr
     """
 
     def __init__(
-        self, files: List[str], json_config: dict = None, upload_batch_size: int = None, ocr_engine: str = "OMNIPAGE"
+        self,
+        files: "List[str]",
+        json_config: "Optional[AnyDict]" = None,
+        upload_batch_size: "Optional[int]" = None,
+        ocr_engine: str = "OMNIPAGE",
     ):
         self.files = files
         self.json_config = json_config
         self.upload_batch_size = upload_batch_size
         self.ocr_engine = ocr_engine
 
-    def requests(self):
+    def requests(
+        self,
+    ) -> "Iterator[Union[UploadBatched, UploadDocument, _DocumentExtraction]]":
         if self.upload_batch_size:
             yield UploadBatched(
                 files=self.files,
                 batch_size=self.upload_batch_size,
                 request_cls=UploadDocument,
             )
         else:
             yield UploadDocument(files=self.files)
-        yield _DocumentExtraction(files=self.previous, json_config=self.json_config, ocr_engine=self.ocr_engine)
+
+        yield _DocumentExtraction(
+            files=self.previous,
+            json_config=self.json_config,
+            ocr_engine=self.ocr_engine,
+        )
```

### Comparing `indico-client-6.1.0a1/indico/queries/example.py` & `indico-client-6.7.0a0/indico/queries/example.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Dict, List, Union
+from typing import TYPE_CHECKING
 
-from indico.client.request import GraphQLRequest, RequestChain, PagedRequest
+from indico.client.request import PagedRequest
 from indico.filters import ModelGroupExampleFilter
-from indico.types import Example, model_group
+from indico.types.questionnaire import Example
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import List, Optional, Union
 
-class ListModelGroupExamples(PagedRequest):
+    from indico.typing import AnyDict, Payload
+
+
+class ListModelGroupExamples(PagedRequest["List[Example]"]):
     """
     List all examples associated with a given model group ID.
     Supports pagination (limit becomes page_size)
 
     Options:
         model_group_ids (List[int]): Model group ids to filter by
         filters (ModelGroupExampleFilter or Dict): Example attributes to filter by
@@ -33,30 +38,30 @@
                             datafileId
                         }
                         pageInfo {
                             startCursor
                             endCursor
                             hasNextPage
                         }
-                    }  
+                    }
                 }
-            }                
+            }
         }
     """
 
     def __init__(
         self,
         *,
-        model_group_id: int = None,
-        filters: Union[Dict, ModelGroupExampleFilter] = None,
+        model_group_id: "Optional[int]" = None,
+        filters: "Optional[Union[AnyDict, ModelGroupExampleFilter]]" = None,
         limit: int = 1000,
         order_by: str = "ID",
         desc: bool = True,
-        after: int = None,
-        before: int = None,
+        after: "Optional[int]" = None,
+        before: "Optional[int]" = None,
     ):
         variables = {
             "modelGroupId": model_group_id,
             "filters": filters,
             "limit": limit,
             "orderBy": order_by,
             "desc": desc,
@@ -64,13 +69,10 @@
             "before": before,
         }
         super().__init__(
             self.query,
             variables=variables,
         )
 
-    def process_response(self, response) -> List[Example]:
-        response = response["data"]["modelGroups"]["modelGroups"][0]
-        _pg = next(iter(response.values()))["pageInfo"]
-        self.has_next_page = _pg["hasNextPage"]
-        self.variables["after"] = _pg["endCursor"] if self.has_next_page else None
-        return [Example(**s) for s in response["pagedExamples"]["examples"]]
+    def process_response(self, response: "Payload") -> "List[Example]":
+        example_page = super().parse_payload(response)["modelGroups"]["modelGroups"][0]
+        return [Example(**s) for s in example_page["pagedExamples"]["examples"]]
```

### Comparing `indico-client-6.1.0a1/indico/queries/forms.py` & `indico-client-6.7.0a0/indico/queries/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-from typing import List
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from indico.client.request import RequestChain, GraphQLRequest
+from indico.client.request import GraphQLRequest, RequestChain
 from indico.queries.storage import UploadBatched, UploadDocument
-from indico.queries.jobs import Job
+from indico.types import Job
 
+if TYPE_CHECKING:
+    from typing import Iterator, List, Optional, Union
 
-class _FormPreprocessing(GraphQLRequest):
+    from indico.typing import AnyDict, Payload
 
+
+class _FormPreprocessing(GraphQLRequest["List[Job]"]):
     query = """
         mutation($files: [FileInput]) {
             activeFormFields(
                 files: $files
             ) {
                 jobIds
             }
         }
     """
 
-    def __init__(self, files):
+    def __init__(self, files: "List[AnyDict]"):
         super().__init__(query=self.query, variables={"files": files})
 
-    def process_response(self, response):
-        jobs = super().process_response(response)["activeFormFields"]["jobIds"]
-        if jobs:
-            return [Job(id=j) for j in jobs]
-        else:
-            return []
+    def process_response(self, response: "Payload") -> "List[Job]":
+        jobs = super().parse_payload(response)["activeFormFields"]["jobIds"] or set()
+        return [Job(id=j) for j in jobs]
 
 
 # TODO: move into indico-client
-class FormPreprocessing(RequestChain):
+class FormPreprocessing(RequestChain["List[Job]"]):
     """
     Attempt to auto-detect form fields and labels
 
     Args:
         files (str): list of filepaths to upload
 
     Returns:
         suggested_fields: list of dictionarys (1 per PDF) containing structured field data
     """
 
     def __init__(
-        self, files: List[str], json_config: dict = None, upload_batch_size: int = None
+        self,
+        files: "List[str]",
+        json_config: "Optional[AnyDict]" = None,
+        upload_batch_size: "Optional[int]" = None,
     ):
         self.files = files
         self.upload_batch_size = upload_batch_size
 
-    def requests(self):
+    def requests(
+        self,
+    ) -> "Iterator[Union[UploadBatched, UploadDocument, _FormPreprocessing]]":
         if self.upload_batch_size:
             yield UploadBatched(
                 files=self.files,
                 batch_size=self.upload_batch_size,
                 request_cls=UploadDocument,
             )
         else:
             yield UploadDocument(files=self.files)
+
         yield _FormPreprocessing(files=self.previous)
```

### Comparing `indico-client-6.1.0a1/indico/queries/integration.py` & `indico-client-6.7.0a0/indico/queries/integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import jsons
-from typing import List
+from typing import TYPE_CHECKING
 
-from indico import GraphQLRequest, RequestChain
-from indico.errors import IndicoInputError
-from indico.types.integration import (
-    ExchangeIntegration,
-    ExchangeIntegrationConfiguration,
-    ExchangeIntegrationCredentials,
-)
+from indico import GraphQLRequest
+from indico.types.integration import ExchangeIntegration
 
+if TYPE_CHECKING:  # pragma: no cover
+    from indico.types.integration import (
+        ExchangeIntegrationConfiguration,
+        ExchangeIntegrationCredentials,
+    )
+    from indico.typing import AnyDict, Payload  # noqa: F401
 
-class AddExchangeIntegration(GraphQLRequest):
+
+class AddExchangeIntegration(GraphQLRequest["ExchangeIntegration"]):
     """
     Mutation to add a Microsoft Exchange integration to a workflow
 
     Args:
         workflow_id(int): workflow to add integration to
         config(ExchangeIntegrationConfiguration): settings for which mailbox to point to and which emails to process
         credentials(ExchangeIntegrationCredentials): client id, client secret, and tenant id for authenticating with Exchange
@@ -38,36 +39,36 @@
     }
   }
 }
     """
 
     def __init__(
         self,
-        config: ExchangeIntegrationConfiguration,
-        credentials: ExchangeIntegrationCredentials,
+        config: "ExchangeIntegrationConfiguration",
+        credentials: "ExchangeIntegrationCredentials",
         workflow_id: int,
     ):
         super().__init__(
             self.query,
             variables={
                 "config": config,
                 "credentials": credentials,
                 "workflow_id": workflow_id,
             },
         )
 
-    def process_response(self, response) -> ExchangeIntegration:
+    def process_response(self, response: "Payload") -> "ExchangeIntegration":
         return ExchangeIntegration(
-            **super().process_response(response)["addExchangeIntegrationToWorkflow"][
+            **super().parse_payload(response)["addExchangeIntegrationToWorkflow"][
                 "integration"
             ]
         )
 
 
-class StartIntegration(GraphQLRequest):
+class StartIntegration(GraphQLRequest["AnyDict"]):
     """
     Mutation to start an existing integration. Once an integration is started, documents will be submitted to the associated workflow.
 
     Args:
         integration_id(int): id of the integration to start
 
     """
@@ -86,15 +87,15 @@
     ):
         super().__init__(
             self.query,
             variables={"integration_id": integration_id},
         )
 
 
-class DeleteIntegration(GraphQLRequest):
+class DeleteIntegration(GraphQLRequest["AnyDict"]):
     """
     Mutation to delete an existing Integration.
 
     Args:
         integration_id(int): id of the integration to delete
 
     """
@@ -110,28 +111,28 @@
     def __init__(self, integration_id: int):
         super().__init__(
             self.query,
             variables={"integrationId": integration_id},
         )
 
 
-class PauseIntegration(GraphQLRequest):
+class PauseIntegration(GraphQLRequest["AnyDict"]):
     """
     Mutation to pause an existing Integration.
 
     Args:
         integration_id(int): id of the integration to pause
     """
-    
+
     query = """
         mutation PauseIntegration($integrationId: Int!){
             pauseWorkflowIntegration(integrationId: $integrationId){
              success # bool
         }
     }
     """
-    
+
     def __init__(self, integration_id: int):
         super().__init__(
             self.query,
             variables={"integrationId": integration_id},
         )
```

### Comparing `indico-client-6.1.0a1/indico/queries/model_groups/metrics.py` & `indico-client-6.7.0a0/indico/queries/model_groups/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+import json
+from typing import TYPE_CHECKING
+
 from indico.client.request import GraphQLRequest, RequestChain
-from indico.types.model_metrics import SequenceMetrics
+from indico.errors import IndicoInputError
 from indico.queries.model_groups import GetModelGroup
-from indico.errors import IndicoRequestError
-import json
+from indico.types.model_metrics import SequenceMetrics
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Dict, Iterator, Type, Union
+
+    from indico.typing import AnyDict, Payload
 
 
-class AnnotationModelGroupMetrics(GraphQLRequest):
+class AnnotationModelGroupMetrics(GraphQLRequest["SequenceMetrics"]):
     """
     Get metrics for annotation or "sequence" models. Metrics for the
     most recently succesfully trained model of the model group are returned.
 
     Args:
         id (int): model group id to query
 
@@ -54,23 +61,23 @@
         }
     }
     """
 
     def __init__(self, model_group_id: int):
         super().__init__(self.query, variables={"modelGroupId": model_group_id})
 
-    def process_response(self, response):
+    def process_response(self, response: "Payload") -> "SequenceMetrics":
         return SequenceMetrics(
-            **super().process_response(response)["modelGroups"]["modelGroups"][0][
+            **super().parse_payload(response)["modelGroups"]["modelGroups"][0][
                 "selectedModel"
             ]["evaluation"]["metrics"]
         )
 
 
-class ObjectDetectionMetrics(GraphQLRequest):
+class ObjectDetectionMetrics(GraphQLRequest["AnyDict"]):
     """
     Get metrics for a trained object detection model. Metrics for the
     most recently succesfully trained model of the model group are returned.
 
     Args:
         id (int): model group id to query
 
@@ -93,43 +100,46 @@
       }
     }
     """
 
     def __init__(self, model_group_id: int):
         super().__init__(self.query, variables={"modelGroupId": model_group_id})
 
-    def process_response(self, response):
-        return json.loads(
+    def process_response(self, response: "Payload") -> "AnyDict":
+        raw_response: "AnyDict" = json.loads(
             super().process_response(response)["modelGroups"]["modelGroups"][0][
                 "selectedModel"
             ]["evaluation"]["metrics"]
         )
+        return raw_response
 
 
-task_type_query_mapping = {
+task_type_query_mapping: "Dict[str, Type[Union[AnnotationModelGroupMetrics, ObjectDetectionMetrics]]]" = {
     "ANNOTATION": AnnotationModelGroupMetrics,
     "OBJECT_DETECTION": ObjectDetectionMetrics,
 }
 
 
-class GetModelGroupMetrics(RequestChain):
+class GetModelGroupMetrics(RequestChain["Union[SequenceMetrics, AnyDict]"]):
     """
     Args:
         model_group_id (int): ModelGroup id
 
     Returns
         Metrics object depending on task type the model solves
     """
 
     def __init__(self, model_group_id: int):
         self.model_group_id = model_group_id
         super().__init__()
 
-    def requests(self):
+    def requests(
+        self,
+    ) -> "Iterator[Union[GetModelGroup, AnnotationModelGroupMetrics, ObjectDetectionMetrics]]":
         yield GetModelGroup(id=self.model_group_id)
         if self.previous.task_type not in task_type_query_mapping:
-            raise IndicoRequestError(
+            raise IndicoInputError(
                 "Metrics queries are only supported for annotation and object detection at this time."
             )
-        metrics_query_fn = task_type_query_mapping.get(self.previous.task_type)
+        metrics_query_fn = task_type_query_mapping[self.previous.task_type]
         yield metrics_query_fn(self.model_group_id)
         return self.previous
```

### Comparing `indico-client-6.1.0a1/indico/queries/storage.py` & `indico-client-6.7.0a0/indico/queries/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,113 +1,128 @@
 import io
 import json
-from typing import List, Dict
+from typing import TYPE_CHECKING
+
 from indico.client.request import HTTPMethod, HTTPRequest, RequestChain
-from indico.errors import IndicoRequestError, IndicoInputError
+from indico.errors import IndicoInputError, IndicoRequestError
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Dict, Iterator, List, Optional, Type, Union
 
+    from indico.typing import AnyDict
 
 URL_PREFIX = "indico-file:///storage"
 
 
-class RetrieveStorageObject(HTTPRequest):
+class RetrieveStorageObject(HTTPRequest["Any"]):
     """
     Retrieve an object stored on the Indico Platform
 
     Results of some operations, notably DocumentExtraction can be quite large
     and are stored on disk in the Indico Platform. You need to retrieve them
     using RetrieveStorageObject.
 
     Args:
         storage_object (str or dict): either a string or dict with a url of the storage object to be retrieved. If a dict then "url" should be used as the key for the storage object url.
 
     Returns:
         contents (dict): Contents of the storage object, most often JSON
     """
 
-    def __init__(self, storage_object):
-        if type(storage_object) == dict:
+    def __init__(self, storage_object: "Union[AnyDict, str]"):
+        if isinstance(storage_object, dict):
             try:
                 url = storage_object["url"]
             except KeyError:
                 raise IndicoRequestError(
                     code="FAILURE",
-                    error="Unable to retrieve result. Please check the status of the job object. If the status is \
-                    'FAILURE', check the job object result for more detailed information.",
+                    error=(
+                        "Unable to retrieve result. Please check the status of the job"
+                        " object. If the status is 'FAILURE', check the job object"
+                        " result for more detailed information."
+                    ),
                 )
         else:
             url = storage_object
 
         url = url.replace("indico-file://", "")
         super().__init__(method=HTTPMethod.GET, path=url)
 
 
-class UploadDocument(HTTPRequest):
+class UploadDocument(HTTPRequest["List[AnyDict]"]):
     """
     Upload an object stored on the Indico Platform
 
     Used internally for uploading documents to indico platform for later processing
 
     Args:
         files (str): A list of local filepaths to upload.
         streams (Dict[str, io.BufferedIOBase]): A dict of filenames to BufferedIOBase streams
             (any class that inherits BufferedIOBase is acceptable).
 
     Returns:
         files: Storage object to be used for further processing requests (e.g., document extraction).
     """
 
-    def __init__(self, files: List[str] = None, streams: Dict[str, io.BufferedIOBase] = None):
-
-        if (files is None and streams is None) or (files is not None and streams is not None):
+    def __init__(
+        self,
+        files: "Optional[List[str]]" = None,
+        streams: "Optional[Dict[str, io.BufferedIOBase]]" = None,
+    ):
+        if (files is None and streams is None) or (
+            files is not None and streams is not None
+        ):
             raise IndicoInputError("Must define one of files or streams, but not both.")
 
-        super().__init__(HTTPMethod.POST, "/storage/files/store", files=files, streams=streams)
+        super().__init__(
+            HTTPMethod.POST, "/storage/files/store", files=files, streams=streams
+        )
 
-    def process_response(self, uploaded_files: List[dict]):
+    def process_response(self, response: "List[AnyDict]") -> "List[AnyDict]":
         files = [
             {
                 "filename": f["name"],
                 "filemeta": json.dumps(
                     {
                         "path": f["path"],
                         "name": f["name"],
                         "uploadType": f["upload_type"],
                     }
                 ),
             }
-            for f in uploaded_files
+            for f in response
         ]
         return files
 
 
-class UploadBatched(RequestChain):
+class UploadBatched(RequestChain["List[AnyDict]"]):
     """
     Batch uploading of files to the Indico Platform
 
     Args:
         filepaths (str): list of filepaths to upload
         batch_size (int): number of files to load per batch
         request_cls (HTTPRequest): Type of upload request: UploadDocument or UploadImage
 
     Returns:
         files: storage objects for further processing (e.g., document extraction or dataset creation)
     """
 
     def __init__(
         self,
-        files: List[str],
+        files: "List[str]",
         batch_size: int = 20,
-        request_cls: HTTPRequest = UploadDocument,
+        request_cls: "Type[Any]" = UploadDocument,
     ):
-        self.result = None
+        self.result: "Optional[List[Any]]" = None
         self.files = files
         self.batch_size = batch_size
         self.request_cls = request_cls
 
-    def requests(self):
+    def requests(self) -> "Iterator[Any]":
         self.result = []
         for i in range(0, len(self.files), self.batch_size):
             yield self.request_cls(self.files[i : i + self.batch_size])
             self.result.extend(self.previous)
 
 
 class CreateStorageURLs(UploadDocument):
@@ -117,19 +132,19 @@
     Args:
         files (str): list of filepaths to upload
 
     Returns:
         urls: list of storage urls to be use for further processing requests (e.g., form extraction)
     """
 
-    def process_response(self, uploaded_files: List[dict]) -> List[str]:
-        errors = [f["error"] for f in uploaded_files if f.get("error")]
+    def process_response(self, response: "Any") -> "Any":
+        errors = [f["error"] for f in response if f.get("error")]
         if errors:
             raise IndicoInputError(
                 "\n".join(error for error in errors),
             )
-        urls = [URL_PREFIX + f["path"] for f in uploaded_files]
+        urls = [URL_PREFIX + f["path"] for f in response]
         return urls
 
 
 # Alias to ensure backwards compatibility
 UploadImages = CreateStorageURLs
```

### Comparing `indico-client-6.1.0a1/indico/queries/submission.py` & `indico-client-6.7.0a0/indico/queries/submission.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import json
-import time
 from functools import partial
 from operator import eq, ne
-from typing import Dict, List, Union
+from typing import TYPE_CHECKING
 
-from indico.client.request import GraphQLRequest, PagedRequest, RequestChain
+from indico.client.request import Delay, GraphQLRequest, PagedRequest, RequestChain
 from indico.errors import IndicoInputError, IndicoTimeoutError
 from indico.filters import SubmissionFilter
 from indico.queries import JobStatus
-from indico.types import Job, Submission
+from indico.types import Job, Submission, SubmissionReviewFull
 from indico.types.submission import VALID_SUBMISSION_STATUSES
 from indico.types.utils import Timer
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Iterator, List, Optional, Union
 
-class ListSubmissions(PagedRequest):
+    from indico.typing import AnyDict, Payload
+
+
+class ListSubmissions(PagedRequest["List[Submission]"]):
     """
     List all Submissions visible to the authenticated user by most recent.
     Supports pagination (limit becomes page_size)
 
     Options:
         submission_ids (List[int]): Submission ids to filter by
         workflow_ids (List[int]): Workflow ids to filter by
@@ -29,77 +33,111 @@
     Returns:
         List[Submission]: All the found Submission objects
         If paginated, yields results one at a time
     """
 
     query = """
         query ListSubmissions(
-            $submissionIds: [Int],
-            $workflowIds: [Int],
-            $filters: SubmissionFilter,
-            $limit: Int,
-            $orderBy: SUBMISSION_COLUMN_ENUM,
-            $desc: Boolean,
+            $submissionIds: [Int]
+            $workflowIds: [Int]
+            $filters: SubmissionFilter
+            $limit: Int
+            $orderBy: SUBMISSION_COLUMN_ENUM
+            $desc: Boolean
             $after: Int
-
-        ){
+            ) {
             submissions(
-                submissionIds: $submissionIds,
-                workflowIds: $workflowIds,
-                filters: $filters,
+                submissionIds: $submissionIds
+                workflowIds: $workflowIds
+                filters: $filters
                 limit: $limit
-                orderBy: $orderBy,
-                desc: $desc,
+                orderBy: $orderBy
+                desc: $desc
                 after: $after
-
-            ){
+            ) {
                 submissions {
+                id
+                datasetId
+                workflowId
+                status
+                createdAt
+                updatedAt
+                createdBy
+                updatedBy
+                completedAt
+                errors
+                filesDeleted
+                inputFiles {
                     id
-                    datasetId
-                    workflowId
-                    status
-                    inputFiles {
-                        id
-                        filename
-                        filepath
-                        filetype
-                        fileSize
-                        numPages
-                    }
-                    inputFile
-                    inputFilename
-                    resultFile
-                    deleted
-                    retrieved
-                    errors
-                    reviews {
-                        id
-                        createdAt
-                        createdBy
-                        completedAt
-                        rejected
-                        reviewType
-                        notes
-                    }
+                    filepath
+                    filename
+                    filetype
+                    submissionId
+                    fileSize
+                    numPages
+                }
+                inputFile
+                inputFilename
+                resultFile
+                outputFiles {
+                    id
+                    filepath
+                    submissionId
+                    componentId
+                    createdAt
+                }
+                retrieved
+                autoReview {
+                    id
+                    submissionId
+                    createdAt
+                    createdBy
+                    startedAt
+                    completedAt
+                    rejected
+                    reviewType
+                    notes
+                }
+                retries {
+                    id
+                    submissionId
+                    previousErrors
+                    previousStatus
+                    retryErrors
+                }
+                reviews {
+                    id
+                    submissionId
+                    createdAt
+                    createdBy
+                    startedAt
+                    completedAt
+                    rejected
+                    reviewType
+                    notes
+                }
+                reviewInProgress
                 }
                 pageInfo {
-                    endCursor
-                    hasNextPage
+                startCursor
+                endCursor
+                hasNextPage
+                aggregateCount
                 }
             }
         }
     """
 
     def __init__(
         self,
         *,
-        submission_ids: List[int] = None,
-        workflow_ids: List[int] = None,
-        filters: Union[Dict, SubmissionFilter] = None,
-        limit: int = 1000,
+        submission_ids: "Optional[List[int]]" = None,
+        workflow_ids: "Optional[List[int]]" = None,
+        filters: "Optional[Union[AnyDict, SubmissionFilter]]" = None,
+        limit: "Optional[int]" = 1000,
         order_by: str = "ID",
         desc: bool = True,
     ):
         super().__init__(
             self.query,
             variables={
                 "submissionIds": submission_ids,
@@ -107,22 +145,22 @@
                 "filters": filters,
                 "limit": limit,
                 "orderBy": order_by,
                 "desc": desc,
             },
         )
 
-    def process_response(self, response) -> List[Submission]:
+    def process_response(self, response: "Payload") -> "List[Submission]":
         return [
             Submission(**s)
-            for s in super().process_response(response)["submissions"]["submissions"]
+            for s in super().parse_payload(response)["submissions"]["submissions"]
         ]
 
 
-class GetSubmission(GraphQLRequest):
+class GetSubmission(GraphQLRequest["Submission"]):
     """
     Retrieve a Submission by id
 
     Args:
         submission_id (int): Submission id
 
     Returns:
@@ -132,49 +170,83 @@
     query = """
         query GetSubmission($submissionId: Int!){
             submission(id: $submissionId){
                 id
                 datasetId
                 workflowId
                 status
+                createdAt
+                updatedAt
+                createdBy
+                updatedBy
+                completedAt
+                errors
+                filesDeleted
                 inputFiles {
                     id
-                    filename
                     filepath
+                    filename
                     filetype
+                    submissionId
                     fileSize
                     numPages
                 }
                 inputFile
                 inputFilename
                 resultFile
+                outputFiles {
+                    id
+                    filepath
+                    submissionId
+                    componentId
+                    createdAt
+                }
                 retrieved
-                deleted
-                errors
+                autoReview {
+                    id
+                    submissionId
+                    createdAt
+                    createdBy
+                    startedAt
+                    completedAt
+                    rejected
+                    reviewType
+                    notes
+                }
+                retries {
+                    id
+                    submissionId
+                    previousErrors
+                    previousStatus
+                    retryErrors
+                }
                 reviews {
                     id
+                    submissionId
                     createdAt
                     createdBy
+                    startedAt
                     completedAt
                     rejected
                     reviewType
                     notes
                 }
+                reviewInProgress
             }
         }
     """
 
     def __init__(self, submission_id: int):
         super().__init__(self.query, variables={"submissionId": submission_id})
 
-    def process_response(self, response) -> Submission:
-        return Submission(**(super().process_response(response)["submission"]))
+    def process_response(self, response: "Payload") -> "Submission":
+        return Submission(**(super().parse_payload(response)["submission"]))
 
 
-class WaitForSubmissions(RequestChain):
+class WaitForSubmissions(RequestChain["List[Submission]"]):
     """
     Given submission_ids, wait for all to finish processing
     """
 
     query = """
         query ListSubmissions(
             $submissionIds: [Int],
@@ -195,15 +267,15 @@
                         fileSize
                         numPages
                     }
                     inputFile
                     inputFilename
                     resultFile
                     retrieved
-                    deleted
+                    filesDeleted
                     errors
                     reviews {
                         id
                         createdAt
                         createdBy
                         completedAt
                         rejected
@@ -211,36 +283,36 @@
                         notes
                     }
                 }
             }
         }
     """
 
-    def __init__(self, submission_ids: List[int], timeout: Union[int, float] = 60):
+    def __init__(self, submission_ids: "List[int]", timeout: "Union[int, float]" = 60):
         if not submission_ids:
             raise IndicoInputError("Please provide submission ids")
 
         self.submission_ids = submission_ids
         self.timeout = timeout
         self.status_check = partial(ne, "PROCESSING")
         self.status_getter = partial(
             ListSubmissions, submission_ids=self.submission_ids, limit=None
         )
 
-    def requests(self) -> List[Submission]:
+    def requests(self) -> "Iterator[ListSubmissions]":
         timer = Timer(self.timeout)
 
         while True:
             timer.check()
             yield self.status_getter()
             if all(self.status_check(s.status) for s in self.previous):
                 break
 
 
-class UpdateSubmission(GraphQLRequest):
+class UpdateSubmission(GraphQLRequest["Submission"]):
     """
     Update the retrieval status of a Submission by id
 
     Args:
         submission_id (int): Submission id
         retrieved (bool): Bool to indicate if you have retrieved prediction results
 
@@ -263,15 +335,15 @@
                     fileSize
                     numPages
                 }
                 inputFile
                 inputFilename
                 resultFile
                 retrieved
-                deleted
+                filesDeleted
                 errors
             }
         }
     """
 
     def __init__(self, submission_id: int, retrieved: bool):
         """
@@ -285,108 +357,111 @@
             Submission: The updated Submission object
         """
         super().__init__(
             self.query,
             variables={"submissionId": submission_id, "retrieved": retrieved},
         )
 
-    def process_response(self, response) -> Submission:
-        return Submission(**(super().process_response(response)["updateSubmission"]))
+    def process_response(self, response: "Payload") -> "Submission":
+        return Submission(**(super().parse_payload(response)["updateSubmission"]))
 
 
-class GenerateSubmissionResult(GraphQLRequest):
+class GenerateSubmissionResult(GraphQLRequest["Job"]):
     query = """
         mutation CreateSubmissionResults($submissionId: Int!) {
             submissionResults(submissionId: $submissionId) {
                 jobId
             }
         }
 
     """
 
-    def __init__(self, submission: Union[int, Submission]):
+    def __init__(self, submission: "Union[int, Submission]"):
         submission_id = submission if isinstance(submission, int) else submission.id
         super().__init__(self.query, variables={"submissionId": submission_id})
 
-    def process_response(self, response) -> Job:
-        response = super().process_response(response)["submissionResults"]
+    def process_response(self, response: "Payload") -> "Job":
+        response = super().parse_payload(response)["submissionResults"]
         return Job(id=response["jobId"])
 
 
-class SubmissionResult(RequestChain):
+class SubmissionResult(RequestChain["Job"]):
     """
     Generate a result file for a Submission
 
     Args:
         submission (int or Submission): Id of the submission or Submission object
         check_status (str, optional): Submission status to check for.
             Defaults to any status other than `PROCESSING`
         wait (bool, optional): Wait until the submission is `check_status`
             and wait for the result file to be generated. Defaults to False
         timeout (int or float, optional): Maximum number of seconds to wait before
             timing out. Ignored if not `wait`. Defaults to 30
+        request_interval (int or float, optional): The maximum time in between retry calls when waiting. Defaults to 5 seconds.
 
     Returns:
         Job: A Job that can be watched for results
 
     Raises:
         if `wait`:
             IndicoTimeoutError: Submission was not `check_status`
                `or result file Job did not complete within `timeout` seconds.
         If not `wait`:
             IndicoInputError: The requested Submission is not `check_status`
     """
 
-    previous: Submission = None
-
     def __init__(
         self,
-        submission: Union[int, Submission],
-        check_status: str = None,
+        submission: "Union[int, Submission]",
+        check_status: "Optional[str]" = None,
         wait: bool = False,
-        timeout: Union[int, float] = 30,
+        timeout: "Union[int, float]" = 30,
+        request_interval: "Union[int, float]" = 5,
     ):
         self.submission_id = (
             submission if isinstance(submission, int) else submission.id
         )
         self.wait = wait
         self.timeout = timeout
+        self.request_interval = request_interval
         if check_status and check_status.upper() not in VALID_SUBMISSION_STATUSES:
             raise IndicoInputError(
                 f"{check_status} is not one of valid submission statuses: "
                 f"{VALID_SUBMISSION_STATUSES}"
             )
         self.status_check = (
             partial(eq, check_status.upper())
             if check_status
             else partial(ne, "PROCESSING")
         )
 
-    def requests(self) -> Union[Job, str]:
+    def requests(
+        self,
+    ) -> "Iterator[Union[GetSubmission, Delay, GenerateSubmissionResult, JobStatus]]":
         timer = Timer(self.timeout)
         timer.check()
         yield GetSubmission(self.submission_id)
         if self.wait:
             while not self.status_check(self.previous.status):
                 timer.check()
                 yield GetSubmission(self.submission_id)
-                time.sleep(1)
+                yield Delay(seconds=self.request_interval)
             if not self.status_check(self.previous.status):
                 raise IndicoTimeoutError(timer.elapsed)
         elif not self.status_check(self.previous.status):
             raise IndicoInputError(
                 f"Submission {self.submission_id} does not meet status requirements"
             )
 
         yield GenerateSubmissionResult(self.submission_id)
         if self.wait:
             yield JobStatus(id=self.previous.id, wait=True, timeout=self.timeout)
 
 
-class SubmitReview(GraphQLRequest):
+class SubmitReview(GraphQLRequest["Job"]):
     """
     Submit an "Auto" Review for a submission. Requires that the submission be in PENDING_AUTO_REVIEW status.
 
     Args:
         submission_id (int): Id of submission to submit reviewEnabled for
 
     Options:
@@ -415,27 +490,32 @@
         "submissionId": "Int!",
         "changes": "JSONString",
         "rejected": "Boolean",
     }
 
     def __init__(
         self,
-        submission: Union[int, Submission],
-        changes: Dict | List = None,
+        submission: "Union[int, Submission]",
+        changes: "Optional[Union[str, AnyDict, List[AnyDict]]]" = None,
         rejected: bool = False,
-        force_complete: bool = None,
+        force_complete: "Optional[bool]" = None,
     ):
+        changes_json: "Optional[str]" = None
         submission_id = submission if isinstance(submission, int) else submission.id
         if not changes and not rejected:
             raise IndicoInputError("Must provide changes or reject=True")
-        elif changes and isinstance(changes, (dict, list)):
-            changes = json.dumps(changes)
+        elif changes:
+            if isinstance(changes, (dict, list)):
+                changes_json = json.dumps(changes)
+            else:
+                changes_json = changes
+
         _vars = {
             "submissionId": submission_id,
-            "changes": changes,
+            "changes": changes_json,
             "rejected": rejected,
         }
 
         # Add backwards-incompatible args now
         if force_complete is not None:
             _vars["forceComplete"] = force_complete
             self.query_args["forceComplete"] = "Boolean"
@@ -445,20 +525,63 @@
         )
         query = query.replace(
             "<AUTO REVIEW ARGS>", ",".join(f"{k}: ${k}" for k in self.query_args)
         )
 
         super().__init__(query, variables=_vars)
 
-    def process_response(self, response) -> Job:
-        response = super().process_response(response)["submitAutoReview"]
+    def process_response(self, response: "Payload") -> "Job":
+        response = super().parse_payload(response)["submitAutoReview"]
         return Job(id=response["jobId"])
 
 
-class RetrySubmission(GraphQLRequest):
+class GetReviews(GraphQLRequest["List[SubmissionReviewFull]"]):
+    """
+    Given a submission Id, return all the full Review objects back with changes
+
+    Args:
+        submission_id (int): Id of submission to submit reviewEnabled for
+    Options:
+
+    Returns:
+        A list of Review objects with changes
+    """
+
+    query = """
+    query GetReview($submissionId: Int!)
+    {
+        submission(id: $submissionId) {
+            id
+            reviews(includeChanges: true) {
+                id
+                submissionId
+                createdAt
+                createdBy
+                startedAt
+                completedAt
+                rejected
+                reviewType
+                notes
+                changes
+            }
+        }
+    }
+    """
+
+    def __init__(self, submission_id: int):
+        super().__init__(self.query, variables={"submissionId": submission_id})
+
+    def process_response(self, response: "Payload") -> "List[SubmissionReviewFull]":
+        return [
+            SubmissionReviewFull(**review)
+            for review in super().parse_payload(response)["submission"]["reviews"]
+        ]
+
+
+class RetrySubmission(GraphQLRequest["List[Submission]"]):
     """
     Given a list of submission ids, retry those failed submissions.
     Submissions must be in a failed state and cannot be requested before
     the cool-off period (typically 180ms).
 
     Args:
         submission_ids (List[int]): the given submission ids to retry.
@@ -482,18 +605,17 @@
       retryErrors
       submissionId
     }
   }
 }
     """
 
-    def __init__(self, submission_ids: List[int]):
+    def __init__(self, submission_ids: "List[int]"):
         if submission_ids is None or len(submission_ids) < 1:
             raise IndicoInputError("You must specify submission ids")
 
         super().__init__(self.query, variables={"submissionIds": submission_ids})
 
-    def process_response(self, response) -> List[Submission]:
+    def process_response(self, response: "Payload") -> "List[Submission]":
         return [
-            Submission(**s)
-            for s in super().process_response(response)["retrySubmissions"]
+            Submission(**s) for s in super().parse_payload(response)["retrySubmissions"]
         ]
```

### Comparing `indico-client-6.1.0a1/indico/queries/usermetrics.py` & `indico-client-6.7.0a0/indico/queries/usermetrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-import datetime
-from typing import List, Union, Dict
+from typing import TYPE_CHECKING, List
 
-from indico.client.request import (
-    GraphQLRequest,
-    PagedRequest,
-)
+from indico.client.request import GraphQLRequest, PagedRequest
 from indico.filters import UserMetricsFilter
 from indico.types import BaseType
-from indico.types.user_metrics import UserSummary, UserSnapshot, UserChangelog, UserChangelogReport
+from indico.types.user_metrics import (
+    UserChangelog,
+    UserChangelogReport,
+    UserSnapshot,
+    UserSummary,
+)
+
+if TYPE_CHECKING:  # pragma: no cover
+    from datetime import datetime
+    from typing import Optional, Union
+
+    from indico.typing import AnyDict, Payload
 
 
 class _PagedUserSnapshots(BaseType):
     """
     Class to hold paged snapshot data to make parsing easier.
     """
+
     results: List[UserSnapshot]
 
 
 class _PagedUserChangelog(BaseType):
     """
     Class to hold paged snapshot data to make parsing easier.
     """
+
     results: List[UserChangelog]
 
 
-class GetUserSummary(GraphQLRequest):
+class GetUserSummary(GraphQLRequest["UserSummary"]):
     """
     Requests summary-level information of users in the app on a specific date.
 
     Args:
         date (datetime): specific day to summarize.
 
     """
+
     query = """
 query GetUserSummary($date: Date){
   userSummary(date: $date){
     users{
       enabled
       disabled
     }
@@ -43,83 +53,93 @@
       role
       count
     }
   }
 }
     """
 
-    def __init__(self, date=None):
+    def __init__(self, date: "Optional[datetime]" = None):
         if date is not None:
-            super().__init__(self.query, variables={"date": date.strftime('%Y-%m-%d')})
+            super().__init__(self.query, variables={"date": date.strftime("%Y-%m-%d")})
         else:
             super().__init__(self.query)
 
-    def process_response(self, response) -> UserSummary:
-        return UserSummary(**super().process_response(response)["userSummary"])
+    def process_response(self, response: "Payload") -> "UserSummary":
+        return UserSummary(**super().parse_payload(response)["userSummary"])
 
 
-class GetUserSnapshots(PagedRequest):
+class GetUserSnapshots(PagedRequest["List[UserSnapshot]"]):
     """
 
     Requests paged detailed information about app users on a specific date.
 
     Args:
         filters (UserMetricsFilter): filter the query based on UserMetricsFilter criteria.
         date (datetime): specific day to query.
         limit (int): limit how many come back per query or per page.
     """
+
     query = """
     query GetUserSnapshot($date: Date, $filters: UserReportFilter, $after: Int, $limit: Int){
   userSnapshot(date: $date, filters: $filters, after: $after, limit: $limit){
     results{
       id
       name
       email
       createdAt
       enabled
       roles
       datasets{
         datasetId
         role
       }
-      
+
     }
     pageInfo{
       startCursor
       endCursor
       hasNextPage
       aggregateCount
     }
   }
 }
     """
 
-    def __init__(self, *, date: datetime, filters: Union[Dict, UserMetricsFilter] = None, limit: int = None):
+    def __init__(
+        self,
+        *,
+        date: "datetime",
+        filters: "Optional[Union[AnyDict, UserMetricsFilter]]" = None,
+        limit: "Optional[int]" = None,
+    ):
         variables = {
-            "date": date.strftime('%Y-%m-%d') if date is not None else None,
+            "date": date.strftime("%Y-%m-%d") if date is not None else None,
             "filters": filters,
-            "limit": limit
+            "limit": limit,
         }
         super().__init__(self.query, variables=variables)
 
-    def process_response(self, response) -> List[UserSnapshot]:
-        return _PagedUserSnapshots(**super().process_response(response)["userSnapshot"]).results
+    def process_response(self, response: "Payload") -> "List[UserSnapshot]":
+        return _PagedUserSnapshots(
+            **super().parse_payload(response)["userSnapshot"]
+        ).results
 
 
-class GetUserChangelog(PagedRequest):
+class GetUserChangelog(PagedRequest["List[UserChangelog]"]):
     """
 
-        Gets paged detailed information about app users.
+    Gets paged detailed information about app users.
+
+    Args:
+        filters (UserSnapshotFilter): filter the query based on UserMetricsFilter criteria.
+        start_date (datetime): specific start date for query.
+        end_date (datetime): specific end date for query.
+        limit (int): limit how many come back per query or per page.
+    """
 
-        Args:
-            filters (UserSnapshotFilter): filter the query based on UserMetricsFilter criteria.
-            start_date (datetime): specific start date for query.
-            end_date (datetime): specific end date for query.
-            limit (int): limit how many come back per query or per page.
-        """
     query = """
         query GetUserChangelog($sdate: Date, $edate: Date, $filters: UserReportFilter, $after: Int, $limit: Int){
         userChangelog(startDate: $sdate, endDate: $edate, filters: $filters, after:$after, limit:$limit){
             results {
             id
             date
             userEmail
@@ -136,58 +156,79 @@
             endCursor
         }
 
         }
     }
         """
 
-    def __init__(self, *, start_date: datetime, end_date: datetime, filters: Union[Dict, UserMetricsFilter] = None,
-                 limit: int = None):
+    def __init__(
+        self,
+        *,
+        start_date: "datetime",
+        end_date: "datetime",
+        filters: "Optional[Union[AnyDict, UserMetricsFilter]]" = None,
+        limit: "Optional[int]" = None,
+    ):
         variables = {
-            "sdate": start_date.strftime('%Y-%m-%d') if start_date is not None else None,
-            "edate": end_date.strftime('%Y-%m-%d') if end_date is not None else None,
+            "sdate": start_date.strftime("%Y-%m-%d")
+            if start_date is not None
+            else None,
+            "edate": end_date.strftime("%Y-%m-%d") if end_date is not None else None,
             "filters": filters,
-            "limit": limit
+            "limit": limit,
         }
         super().__init__(self.query, variables=variables)
 
-    def process_response(self, response) -> List[UserSnapshot]:
-        return _PagedUserChangelog(**super().process_response(response)["userChangelog"]).results
+    def process_response(self, response: "Payload") -> "List[UserChangelog]":
+        return _PagedUserChangelog(
+            **super().parse_payload(response)["userChangelog"]
+        ).results
 
 
-class GenerateChangelogReport(GraphQLRequest):
+class GenerateChangelogReport(GraphQLRequest["UserChangelogReport"]):
     """
 
-        Creates a job to generate a report of detailed information about app users
-        
-        Args:
-            filters (UserSnapshotFilter): filter the query based on UserMetricsFilter criteria.
-            start_date (datetime): specific start date for query.
-            end_date (datetime): specific end date for query.
-            report_format (str): specific format of the report, JSON or CSV.
+    Creates a job to generate a report of detailed information about app users
+
+    Args:
+        filters (UserSnapshotFilter): filter the query based on UserMetricsFilter criteria.
+        start_date (datetime): specific start date for query.
+        end_date (datetime): specific end date for query.
+        report_format (str): specific format of the report, JSON or CSV.
+
+    """
 
-        """
     query = """
         mutation GenerateChangeReport ($sdate: Date, $edate: Date, $filters: UserReportFilter){
     userChangelogReport(
         startDate: $sdate,
         endDate: $edate,
         filters: $filters,
         reportFormat: JSON
     ){
         jobId
     }
 }
         """
 
-    def __init__(self, *, start_date: datetime, end_date: datetime, filters: Union[Dict, UserMetricsFilter] = None,
-                 report_format: str = "csv"):
+    def __init__(
+        self,
+        *,
+        start_date: "datetime",
+        end_date: "datetime",
+        filters: "Optional[Union[AnyDict, UserMetricsFilter]]" = None,
+        report_format: str = "csv",
+    ):
         variables = {
-            "sdate": start_date.strftime('%Y-%m-%d') if start_date is not None else None,
-            "edate": end_date.strftime('%Y-%m-%d') if end_date is not None else None,
+            "sdate": start_date.strftime("%Y-%m-%d")
+            if start_date is not None
+            else None,
+            "edate": end_date.strftime("%Y-%m-%d") if end_date is not None else None,
             "filters": filters,
-            "format": report_format
+            "format": report_format,
         }
         super().__init__(self.query, variables=variables)
 
-    def process_response(self, response) -> List[UserSnapshot]:
-        return UserChangelogReport(**super().process_response(response)["userChangelogReport"])
+    def process_response(self, response: "Payload") -> "UserChangelogReport":
+        return UserChangelogReport(
+            **super().parse_payload(response)["userChangelogReport"]
+        )
```

### Comparing `indico-client-6.1.0a1/indico/queries/workflow.py` & `indico-client-6.7.0a0/indico/queries/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import io
-import json
-from typing import List, Union, Dict
 import tempfile
+from typing import TYPE_CHECKING
 
-from indico.client.request import GraphQLRequest, RequestChain, Debouncer
+from indico.client.request import Delay, GraphQLRequest, RequestChain
 from indico.errors import IndicoError, IndicoInputError
-from indico.queries.storage import UploadDocument
-from indico.types import Job, Submission, Workflow, SUBMISSION_RESULT_VERSIONS
+from indico.queries.storage import UploadBatched, UploadDocument
+from indico.types import SUBMISSION_RESULT_VERSIONS, Submission, Workflow
 from indico.types.utils import cc_to_snake, snake_to_cc
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, ClassVar, Dict, Iterator, List, Optional, Union
 
-class ListWorkflows(GraphQLRequest):
+    from indico.typing import Payload
+
+
+class ListWorkflows(GraphQLRequest["List[Workflow]"]):
     """
     List all workflows visible to authenticated user
 
     Options:
         dataset_ids (List[int]): List of dataset ids to filter by
         workflow_ids (List[int]): List of workflow ids to filter by
 
@@ -54,67 +58,77 @@
                                       taskType
                                       questionnaireId
                                       classNames
                                       selectedModel{
                                         id
                                       }
                                 }
-                            
+
                         }
-                
+
                     }
                   componentLinks{
                     id
                     headComponentId
                     tailComponentId
                     filters{
                       classes
                     }
-                    
+
                   }
                 }
             }
         }
     """
 
     def __init__(
-            self, *, dataset_ids: List[int] = None, workflow_ids: List[int] = None, limit=100
+        self,
+        *,
+        dataset_ids: "Optional[List[int]]" = None,
+        workflow_ids: "Optional[List[int]]" = None,
+        limit: int = 100,
     ):
         super().__init__(
             self.query,
-            variables={"datasetIds": dataset_ids,
-                       "workflowIds": workflow_ids, "limit": limit},
+            variables={
+                "datasetIds": dataset_ids,
+                "workflowIds": workflow_ids,
+                "limit": limit,
+            },
         )
 
-    def process_response(self, response) -> List[Workflow]:
+    def process_response(self, response: "Payload") -> "List[Workflow]":
         return [
             Workflow(**w)
-            for w in super().process_response(response)["workflows"]["workflows"]
+            for w in super().parse_payload(response)["workflows"]["workflows"]
         ]
 
 
-class GetWorkflow(ListWorkflows):
+class GetWorkflow(GraphQLRequest["Workflow"]):
     """
     Query for Workflow by id
 
     Args:
         workflow_id (int): Workflow id to query for
 
     Returns:
         Workflow: Found Workflow object
     """
 
     def __init__(self, workflow_id: int):
-        super().__init__(workflow_ids=[workflow_id])
+        super().__init__(
+            ListWorkflows.query,
+            variables={"datasetIds": None, "workflowIds": [workflow_id], "limit": 100},
+        )
 
-    def process_response(self, response) -> Workflow:
-        return super().process_response(response)[0]
+    def process_response(self, response: "Payload") -> "Workflow":
+        return Workflow(**super().parse_payload(response)["workflows"]["workflows"][0])
 
 
-class _ToggleReview(GraphQLRequest):
+class _ToggleReview(GraphQLRequest["Workflow"]):
     toggle = "enableReview"
     query_name = "toggleWorkflowReview"
     query = """
         mutation ToggleReview($workflowId: Int!, $reviewState: Boolean!){
             <QUERY NAME>(workflowId: $workflowId, <TOGGLE>: $reviewState){
                 id
                 name
@@ -125,28 +139,27 @@
     """
 
     def __init__(self, workflow_id: int, enable_review: bool):
         query = self.query.replace("<QUERY NAME>", self.query_name)
         query = query.replace("<TOGGLE>", self.toggle)
         super().__init__(
             query,
-            variables={"workflowId": workflow_id,
-                       "reviewState": enable_review},
+            variables={"workflowId": workflow_id, "reviewState": enable_review},
         )
 
-    def process_response(self, response) -> Workflow:
-        return Workflow(**super().process_response(response)[self.query_name])
+    def process_response(self, response: "Payload") -> "Workflow":
+        return Workflow(**super().parse_payload(response)[self.query_name])
 
 
 class _ToggleAutoReview(_ToggleReview):
     toggle = "enableAutoReview"
     query_name = "toggleWorkflowAutoReview"
 
 
-class UpdateWorkflowSettings(RequestChain):
+class UpdateWorkflowSettings(RequestChain["Workflow"]):
     """
     Mutation to toggle review and auto-review on a workflow
 
     Args:
         workflow (int|Workflow): Workflow or workflow id to update
 
     Options:
@@ -154,35 +167,34 @@
         enable_auto_review (bool): Enable auto_review
 
     Returns:
         Workflow: Updated Workflow object
     """
 
     def __init__(
-            self,
-            workflow: Union[Workflow, int],
-            enable_review: bool = None,
-            enable_auto_review: bool = None,
+        self,
+        workflow: "Union[Workflow, int]",
+        enable_review: "Optional[bool]" = None,
+        enable_auto_review: "Optional[bool]" = None,
     ):
-        self.workflow_id = workflow.id if isinstance(
-            workflow, Workflow) else workflow
+        self.workflow_id = workflow.id if isinstance(workflow, Workflow) else workflow
         if enable_review is None and enable_auto_review is None:
             raise IndicoInputError("Must provide at least one review option")
 
         self.enable_review = enable_review
         self.enable_auto_review = enable_auto_review
 
-    def requests(self):
+    def requests(self) -> "Iterator[_ToggleReview]":
         if self.enable_review is not None:
             yield _ToggleReview(self.workflow_id, self.enable_review)
         if self.enable_auto_review is not None:
             yield _ToggleAutoReview(self.workflow_id, self.enable_auto_review)
 
 
-class _WorkflowSubmission(GraphQLRequest):
+class _WorkflowSubmission(GraphQLRequest["Union[List[Submission], List[int]]"]):
     query = """
         mutation workflowSubmissionMutation({signature}) {{
             {mutation_name}({args}) {{
                 jobIds
                 submissionIds
             }}
         }}
@@ -219,68 +231,70 @@
         "workflowId": "Int!",
         "files": "[FileInput]!",
         "bundle": "Boolean",
         "resultVersion": "SubmissionResultVersion",
     }
 
     def __init__(
-            self,
-            detailed_response: bool,
-            **kwargs,
+        self,
+        detailed_response: bool,
+        **kwargs: "Any",
     ):
         self.workflow_id = kwargs["workflow_id"]
 
         # construct mutation signature and args based on provided kwargs to ensure
         # backwards-compatible graphql calls
         #
-        # inputFiles, bundle, and resultVersion only avaliable on IPA 4.9.0+
+        # inputFiles, bundle, and resultVersion only available on IPA 4.9.0+
         subq = (
             self.files_subquery
             if kwargs.get("bundle") or kwargs.get("result_version")
             else ""
         )
         q = (
             self.detailed_query.replace("<SUBQUERY>", subq)
             if detailed_response
             else self.query
         )
 
-        args = [
+        args_list: "List[str]" = [
             _arg for _arg in self.mutation_args.keys() if kwargs.get(cc_to_snake(_arg))
         ]
-        signature = ",".join(
-            f"${_arg}: {self.mutation_args[_arg]}" for _arg in args)
-        args = ",".join(f"{_arg}: ${_arg}" for _arg in args)
+        signature: str = ",".join(
+            f"${_arg}: {self.mutation_args[_arg]}" for _arg in args_list
+        )
+        args: str = ",".join(f"{_arg}: ${_arg}" for _arg in args_list)
 
         super().__init__(
             query=q.format(
                 mutation_name=self.mutation_name, signature=signature, args=args
             ),
             variables={snake_to_cc(var): val for var, val in kwargs.items()},
         )
 
-    def process_response(self, response):
-        response = super().process_response(response)[self.mutation_name]
+    def process_response(
+        self, response: "Payload"
+    ) -> "Union[List[Submission], List[int]]":
+        response = super().parse_payload(response)[self.mutation_name]
         if "submissions" in response:
             return [Submission(**s) for s in response["submissions"]]
         if not response["submissionIds"]:
-            raise IndicoError(
-                f"Failed to submit to workflow {self.workflow_id}")
+            raise IndicoError(f"Failed to submit to workflow {self.workflow_id}")
         else:
-            return response["submissionIds"]
-        return [Job(id=job_id) for job_id in response["jobIds"]]
+            sub_ids: "List[int]" = response["submissionIds"]
+            return sub_ids
 
 
 class _WorkflowUrlSubmission(_WorkflowSubmission):
     mutation_name = "workflowUrlSubmission"
     mutation_args = {**_WorkflowSubmission.mutation_args, "urls": "[String]!"}
     del mutation_args["files"]
 
 
-class WorkflowSubmission(RequestChain):
+class WorkflowSubmission(RequestChain["Union[List[Submission], List[int]]"]):
     f"""
     Submit files to a workflow for processing.
     One of `files`, `urls`, `stream`, or `text` is required.
 
     Args:
         workflow_id (int): Id of workflow to submit files to
         files (List[str], optional): List of local file paths to submit
@@ -288,69 +302,75 @@
         submission (bool, optional): DEPRECATED - AsyncJobs are no longer supported.
         bundle (bool, optional): Batch all files under a single submission id
         result_version (str, optional):
             The format of the submission result file. One of:
                 {SUBMISSION_RESULT_VERSIONS}
             If bundle is enabled, this must be version TWO or later.
         streams (Dict[str, io.BufferedIOBase]): List of filename keys mapped to streams
-            for upload. Similar to files but mutually exclusive with files. 
+            for upload. Similar to files but mutually exclusive with files.
             Can take for example: io.BufferedReader, io.BinaryIO, or io.BytesIO.
         text (str, optional): text to submit. Note: submission may still go through OCR.
+        batch_size (int, optional): If submitting files, specifies the amount of files to submit in a single batch. Defaults to 10. A call with a batch exceeding 500mb total will fail with an error.
 
     Returns:
         List[int]: If `submission`, these will be submission ids.
             Otherwise, they will be AsyncJob ids.
 
     """
 
-    detailed_response = False
+    detailed_response: "ClassVar[bool]" = False
 
     def __init__(
-            self,
-            workflow_id: int,
-            files: List[str] = None,
-            urls: List[str] = None,
-            submission: bool = True,
-            bundle: bool = False,
-            result_version: str = None,
-            streams: Dict[str, io.BufferedIOBase] = None,
-            text: str = ""
+        self,
+        workflow_id: int,
+        files: "Optional[List[str]]" = None,
+        urls: "Optional[List[str]]" = None,
+        submission: bool = True,
+        bundle: bool = False,
+        result_version: "Optional[str]" = None,
+        streams: "Optional[Dict[str, io.BufferedIOBase]]" = None,
+        text: str = "",
+        batch_size: int = 10,
     ):
         self.workflow_id = workflow_id
         self.files = files
         self.urls = urls
         self.submission = submission
         self.bundle = bundle
         self.result_version = result_version
         self.has_streams = False
         if streams is not None:
             self.streams = streams.copy()
             self.has_streams = True
-        else:
-            self.streams = None
         self.text = text
+        self.batch_size = batch_size
         if not submission:
-            raise IndicoInputError(
-                "This option is deprecated and no longer supported.")
+            raise IndicoInputError("This option is deprecated and no longer supported.")
         if not self.files and not self.urls and not self.has_streams and not self.text:
             raise IndicoInputError(
-                "One of 'files', 'streams', 'urls', or 'text' must be specified")
+                "One of 'files', 'streams', 'urls', or 'text' must be specified"
+            )
         elif (self.files or self.urls or self.text) and self.has_streams:
             raise IndicoInputError(
-                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified.")
+                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified."
+            )
         elif (self.files or self.text) and self.urls:
             raise IndicoInputError(
-                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified")
+                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified"
+            )
         elif self.files and self.text:
             raise IndicoInputError(
-                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified")
+                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified"
+            )
 
-    def requests(self):
+    def requests(
+        self,
+    ) -> "Iterator[Union[UploadBatched, UploadDocument, _WorkflowSubmission]]":
         if self.files:
-            yield UploadDocument(files=self.files)
+            yield UploadBatched(files=self.files, batch_size=self.batch_size)
             yield _WorkflowSubmission(
                 self.detailed_response,
                 workflow_id=self.workflow_id,
                 files=self.previous,
                 bundle=self.bundle,
                 result_version=self.result_version,
             )
@@ -368,15 +388,15 @@
                 self.detailed_response,
                 workflow_id=self.workflow_id,
                 files=self.previous,
                 bundle=self.bundle,
                 result_version=self.result_version,
             )
         elif self.text:
-            temp = tempfile.NamedTemporaryFile(mode='w+', suffix='.txt')
+            temp = tempfile.NamedTemporaryFile(mode="w+", suffix=".txt")
             try:
                 temp.write(self.text)
                 temp.seek(0)
                 yield UploadDocument(files=[temp.name])
                 yield _WorkflowSubmission(
                     self.detailed_response,
                     workflow_id=self.workflow_id,
@@ -405,35 +425,35 @@
             If bundle is enabled, this must be version TWO or later.
 
     Returns:
         List[Submission]: Submission objects created
 
     """
 
-    detailed_response = True
+    detailed_response: "ClassVar[bool]" = True
 
     def __init__(
-            self,
-            workflow_id: int,
-            files: List[str] = None,
-            urls: List[str] = None,
-            bundle: bool = False,
-            result_version: str = None,
+        self,
+        workflow_id: int,
+        files: "Optional[List[str]]" = None,
+        urls: "Optional[List[str]]" = None,
+        bundle: bool = False,
+        result_version: "Optional[str]" = None,
     ):
         super().__init__(
             workflow_id,
             files=files,
             urls=urls,
             submission=True,
             bundle=bundle,
             result_version=result_version,
         )
 
 
-class _AddDataToWorkflow(GraphQLRequest):
+class _AddDataToWorkflow(GraphQLRequest["Workflow"]):
     query = """
         mutation addDataToWorkflow($workflowId: Int!) {
             addDataToWorkflow(workflowId: $workflowId){
                 workflow{
                     id
                     name
                     status
@@ -444,21 +464,21 @@
 
     def __init__(self, workflow_id: int):
         super().__init__(
             self.query,
             variables={"workflowId": workflow_id},
         )
 
-    def process_response(self, response) -> Workflow:
+    def process_response(self, response: "Payload") -> "Workflow":
         return Workflow(
-            **super().process_response(response)["addDataToWorkflow"]["workflow"]
+            **super().parse_payload(response)["addDataToWorkflow"]["workflow"]
         )
 
 
-class AddDataToWorkflow(RequestChain):
+class AddDataToWorkflow(RequestChain["Workflow"]):
     """
     Mutation to update data in a workflow, presumably
     after new data is added to the dataset.
 
     Args:
         workflow_id (int): Workflow id to update
 
@@ -469,97 +489,94 @@
         Workflow: Updated Workflow object
     """
 
     def __init__(self, workflow_id: int, wait: bool = False):
         self.workflow_id = workflow_id
         self.wait = wait
 
-    def requests(self):
+    def requests(self) -> "Iterator[Union[_AddDataToWorkflow, Delay, GetWorkflow]]":
         yield _AddDataToWorkflow(self.workflow_id)
 
         if self.wait:
-            debouncer = Debouncer()
-
             while self.previous.status != "COMPLETE":
+                yield Delay()
                 yield GetWorkflow(workflow_id=self.workflow_id)
-                debouncer.backoff()
 
 
-class CreateWorkflow(GraphQLRequest):
+class CreateWorkflow(GraphQLRequest["Workflow"]):
     """
     Mutation to create workflow given an existing dataset.
 
     Args:
         dataset_id(int): dataset to create workflow for
         name(str): name for the workflow
 
     """
+
     query = """  mutation createWorkflow($datasetId: Int!, $name: String!) {
     createWorkflow(datasetId: $datasetId, name: $name) {
            workflow {
                     id
                     name
                     status
                     reviewEnabled
                     autoReviewEnabled
                     submissionRunnable
                 components {
                         id
                         componentType
                         reviewable
                         filteredClasses
-                        
+
                         ... on ModelGroupComponent {
                             taskType
                             modelType
                         }
-                
+
                     }
                   componentLinks{
                     id
                     headComponentId
                     tailComponentId
                     filters {
                       classes
                     }
-                    
+
                   }
                 }
     }
     }
     """
 
     def __init__(self, dataset_id: int, name: str):
         super().__init__(
             self.query,
-            variables={"datasetId": dataset_id,
-                       "name": name},
+            variables={"datasetId": dataset_id, "name": name},
         )
 
-    def process_response(self, response) -> Workflow:
-        return Workflow(
-            **super().process_response(response)["createWorkflow"]["workflow"]
-        )
+    def process_response(self, response: "Payload") -> "Workflow":
+        return Workflow(**super().parse_payload(response)["createWorkflow"]["workflow"])
 
 
-class DeleteWorkflow(GraphQLRequest):
+class DeleteWorkflow(GraphQLRequest[bool]):
     """
-    Mutation to delete workflow given workflow id. Note that this operation includes deleting 
+    Mutation to delete workflow given workflow id. Note that this operation includes deleting
     all components and models associated with this workflow.
 
     Args:
         workflow_id(int): id of workflow to delete
     """
 
-    query = """        
+    query = """
         mutation deleteWorkflow($workflowId: Int!){
             deleteWorkflow(workflowId: $workflowId){
                 success
             }
         }
     """
 
     def __init__(self, workflow_id: int):
         super().__init__(self.query, variables={"workflowId": workflow_id})
 
-    def process_response(self, response) -> bool:
-        return super().process_response(response)["deleteWorkflow"]["success"]
+    def process_response(self, response: "Payload") -> bool:
+        status: bool = super().parse_payload(response)["deleteWorkflow"]["success"]
+        return status
```

### Comparing `indico-client-6.1.0a1/indico/queries/workflow_components.py` & `indico-client-6.7.0a0/indico/queries/workflow_components.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import TYPE_CHECKING
+
 import jsons
-from typing import List
 
 from indico import GraphQLRequest, RequestChain
 from indico.errors import IndicoInputError
 from indico.types import (
+    LinkedLabelGroup,
     NewLabelsetArguments,
     NewQuestionnaireArguments,
     Workflow,
-    LinkedLabelGroup,
 )
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Iterator, List, Optional, Union
 
-class _AddWorkflowComponent(GraphQLRequest):
+    from indico.typing import AnyDict, Payload
+
+
+class _AddWorkflowComponent(GraphQLRequest["Workflow"]):
     query = """mutation addWorkflowComponent($afterComponentId:Int, $afterComponentLinkId: Int, $component: JSONString!, $workflowId: Int!){
   addWorkflowComponent(afterComponentId: $afterComponentId,
   component: $component,
   workflowId:$workflowId
   afterComponentLinkId: $afterComponentLinkId){
   workflow {
                 id
@@ -60,123 +66,124 @@
 
             }
   }
 }"""
 
     def __init__(
         self,
-        after_component_id: int,
-        after_component_link: int,
+        after_component_id: "Optional[int]",
+        after_component_link: "Optional[int]",
         workflow_id: int,
-        component: dict,
+        component: "AnyDict",
     ):
         super().__init__(
             self.query,
             variables={
                 "afterComponentId": after_component_id,
                 "afterComponentLink": after_component_link,
                 "workflowId": workflow_id,
                 "component": jsons.dumps(component),
             },
         )
 
-    def process_response(self, response) -> Workflow:
+    def process_response(self, response: "Payload") -> "Workflow":
         return Workflow(
-            **super().process_response(response)["addWorkflowComponent"]["workflow"]
+            **super().parse_payload(response)["addWorkflowComponent"]["workflow"]
         )
 
 
-class AddLinkedLabelComponent(RequestChain):
+class AddLinkedLabelComponent(RequestChain["Workflow"]):
     """
     Adds a linked label transformer that groups together labels
 
     Args:
         after_component_id(int): the component this component follows.
         workflow_id(int): the workflow id.
         labelset_id(int): the labelset to source classes from.
         model_group_id(int): the model group to source classes from.
         groups (List[LinkedLabelGroup]): configuration for how to group labels.
     """
+
     def __init__(
         self,
         after_component_id: int,
         workflow_id: int,
         labelset_id: int,
         model_group_id: int,
-        groups: List[LinkedLabelGroup],
-        after_component_link_id: int = None,
+        groups: "List[LinkedLabelGroup]",
+        after_component_link_id: "Optional[int]" = None,
     ):
-
         self.workflow_id = workflow_id
         self.after_component_id = after_component_id
         self.after_component_link_id = after_component_link_id
         self.component = {
             "component_type": "link_label",
             "config": {
                 "labelset_id": labelset_id,
                 "model_group_id": model_group_id,
                 "groups": [self.__groups_to_json(group) for group in groups],
             },
         }
 
-    def __groups_to_json(self, group: LinkedLabelGroup):
+    def __groups_to_json(self, group: "LinkedLabelGroup") -> "AnyDict":
         return {
             "name": group.name,
             "strategy": group.strategy.name.lower(),
             "class_names": group.class_ids,
             "strategy_settings": group.strategy_settings,
         }
 
-    def requests(self):
+    def requests(self) -> "Iterator[_AddWorkflowComponent]":
         yield _AddWorkflowComponent(
             after_component_id=self.after_component_id,
             after_component_link=self.after_component_link_id,
             workflow_id=self.workflow_id,
             component=self.component,
         )
 
 
-class AddContentLengthFilterComponent(RequestChain):
+class AddContentLengthFilterComponent(RequestChain["Workflow"]):
     """
     Adds a content length filter.
 
     Args:
         workflow_id(int): the workflow id.
         after_component_id(int): the component this component follows.
         minimum(int): minimum length of content to accept. Defaults to None.
         maximum(int): maximum length of content to accept. Defaults to None.
     """
+
     def __init__(
         self,
         workflow_id: int,
         after_component_id: int,
-        after_component_link_id: int = None,
-        minimum: int = None,
-        maximum: int = None,
+        after_component_link_id: "Optional[int]" = None,
+        minimum: "Optional[int]" = None,
+        maximum: "Optional[int]" = None,
     ):
         self.workflow_id = workflow_id
         self.after_component_id = after_component_id
         self.after_component_link_id = after_component_link_id
         self.minimum = minimum
         self.maximum = maximum
         self.component = {
             "component_type": "content_length",
             "config": {"minimum": minimum, "maximum": maximum},
         }
 
-    def requests(self):
+    def requests(self) -> "Iterator[_AddWorkflowComponent]":
         yield _AddWorkflowComponent(
             after_component_id=self.after_component_id,
             after_component_link=self.after_component_link_id,
             workflow_id=self.workflow_id,
             component=self.component,
         )
 
 
-class AddLinkClassificationComponent(RequestChain):
+class AddLinkClassificationComponent(RequestChain["Workflow"]):
     """
     Adds a link classification model component with filtered classes.
 
     Args:
         workflow_id(int): the workflow id.
         after_component_id(int): the component this component follows.
         model_group_id(int): the model group to source classes from.
@@ -185,40 +192,40 @@
     """
 
     def __init__(
         self,
         workflow_id: int,
         after_component_id: int,
         model_group_id: int,
-        filtered_classes: List[List[str]],
-        labels: str = None,
-        after_component_link_id: int = None,
+        filtered_classes: "List[List[str]]",
+        labels: "Optional[str]" = None,
+        after_component_link_id: "Optional[int]" = None,
     ):
         self.workflow_id = workflow_id
         self.after_component_id = after_component_id
         self.after_component_link_id = after_component_link_id
         self.component = {
             "component_type": "link_classification_model",
             "config": {
                 "model_group_id": model_group_id,
                 "filtered_classes": filtered_classes,
                 "labels": labels,
             },
         }
 
-    def requests(self):
+    def requests(self) -> "Iterator[_AddWorkflowComponent]":
         yield _AddWorkflowComponent(
             after_component_id=self.after_component_id,
             after_component_link=self.after_component_link_id,
             workflow_id=self.workflow_id,
             component=self.component,
         )
 
 
-class AddModelGroupComponent(GraphQLRequest):
+class AddModelGroupComponent(GraphQLRequest["Workflow"]):
     """
     Adds a new model group to a workflow, optionally with a customized questionnaire.
     Available on 5.0+ only.
     Returns workflow with updated component list, which will contain the added Model Group.
 
     Args:
         workflow_id(int): the id of the workflow to add the component to.
@@ -301,84 +308,90 @@
 
     def __init__(
         self,
         workflow_id: int,
         dataset_id: int,
         name: str,
         source_column_id: int,
-        after_component_id: int = None,
-        after_link_id: int = None,
-        labelset_column_id: int = None,
-        new_labelset_args: NewLabelsetArguments = None,
-        new_questionnaire_args: NewQuestionnaireArguments = None,
-        model_training_options: str = None,
-        model_type: str = None,
+        after_component_id: "Optional[int]" = None,
+        after_link_id: "Optional[int]" = None,
+        labelset_column_id: "Optional[int]" = None,
+        new_labelset_args: "Optional[NewLabelsetArguments]" = None,
+        new_questionnaire_args: "Optional[NewQuestionnaireArguments]" = None,
+        model_training_options: "Optional[Union[str, AnyDict]]" = None,
+        model_type: "Optional[str]" = None,
     ):
-
         if labelset_column_id is not None and new_labelset_args is not None:
             raise IndicoInputError(
                 "Cannot define both labelset_column_id and new_labelset_args, must be one "
                 "or the other."
             )
         if labelset_column_id is None and new_labelset_args is None:
             raise IndicoInputError(
                 "Must define one of either labelset_column_id or new_labelset_args."
             )
 
+        model_training_options_json: "Optional[str]" = None
         if model_training_options:
-            model_training_options = jsons.dumps(model_training_options)
+            if isinstance(model_training_options, dict):
+                model_training_options_json = jsons.dumps(model_training_options)
+            else:
+                model_training_options_json = model_training_options
 
         super().__init__(
             self.query,
             variables={
                 "workflowId": workflow_id,
                 "name": name,
                 "datasetId": dataset_id,
                 "sourceColumnId": source_column_id,
                 "labelsetColumnId": labelset_column_id,
                 "afterComponentId": after_component_id,
                 "afterLinkId": after_link_id,
-                "modelTrainingOptions": model_training_options,
+                "modelTrainingOptions": model_training_options_json,
                 "modelType": model_type,
-                "newLabelsetArgs": self.__labelset_to_json(new_labelset_args)
-                if new_labelset_args is not None
-                else None,
-                "questionnaireArgs": self.__questionnaire_to_json(
-                    new_questionnaire_args
-                )
-                if new_questionnaire_args is not None
-                else None,
+                "newLabelsetArgs": (
+                    self.__labelset_to_json(new_labelset_args)
+                    if new_labelset_args is not None
+                    else None
+                ),
+                "questionnaireArgs": (
+                    self.__questionnaire_to_json(new_questionnaire_args)
+                    if new_questionnaire_args is not None
+                    else None
+                ),
             },
         )
 
-    def __labelset_to_json(self, labelset: NewLabelsetArguments):
+    def __labelset_to_json(self, labelset: "NewLabelsetArguments") -> "AnyDict":
         return {
             "name": labelset.name,
             "numLabelersRequired": labelset.num_labelers_required,
             "datacolumnId": labelset.datacolumn_id,
             "taskType": labelset.task_type.name,
             "targetNames": labelset.target_names,
         }
 
-    def __questionnaire_to_json(self, questionnaire: NewQuestionnaireArguments):
+    def __questionnaire_to_json(
+        self, questionnaire: "NewQuestionnaireArguments"
+    ) -> "AnyDict":
         return {
             "instructions": questionnaire.instructions,
             "forceTextMode": questionnaire.force_text_mode,
             "showPredictions": questionnaire.show_predictions,
             "users": questionnaire.users,
         }
 
-    def process_response(self, response) -> Workflow:
+    def process_response(self, response: "Payload") -> "Workflow":
         return Workflow(
-            **super().process_response(response)["addModelGroupComponent"]["workflow"]
+            **super().parse_payload(response)["addModelGroupComponent"]["workflow"]
         )
 
 
-class DeleteWorkflowComponent(GraphQLRequest):
-
+class DeleteWorkflowComponent(GraphQLRequest["Workflow"]):
     """
     Deletes a component from a workflow. If the component has an associated model, the model is deleted as well.
     Available on 5.3+ only.
     Returns workflow with updated list of components and links
 
     Args:
         workflow_id(int): the id of the workflow to delete the component from.
@@ -436,11 +449,11 @@
 
     def __init__(self, workflow_id: int, component_id: int):
         super().__init__(
             self.query,
             variables={"workflowId": workflow_id, "componentId": component_id},
         )
 
-    def process_response(self, response) -> Workflow:
+    def process_response(self, response: "Payload") -> "Workflow":
         return Workflow(
-            **super().process_response(response)["deleteWorkflowComponent"]["workflow"]
+            **super().parse_payload(response)["deleteWorkflowComponent"]["workflow"]
         )
```

### Comparing `indico-client-6.1.0a1/indico/queries/workflow_metrics.py` & `indico-client-6.7.0a0/indico/queries/workflow_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 from datetime import datetime
-from indico.errors import IndicoInputError
+from typing import TYPE_CHECKING, List
+
 from indico.client.request import GraphQLRequest
+from indico.errors import IndicoInputError
 from indico.types import BaseType
-from indico.types.workflow_metrics import WorkflowMetricsOptions, WorkflowMetrics
-from typing import List
+from indico.types.workflow_metrics import WorkflowMetrics, WorkflowMetricsOptions
+
+if TYPE_CHECKING:  # pragma: no cover
+    from indico.typing import Payload
 
 
 class _WorkflowMetric(BaseType):
     metrics: WorkflowMetrics
 
 
 class _TopWorkflowMetric(BaseType):
     workflows: List[_WorkflowMetric]
 
 
-class GetWorkflowMetrics(GraphQLRequest):
+class GetWorkflowMetrics(GraphQLRequest["List[WorkflowMetrics]"]):
     """
     Requests detailed workflow metric data, including daily and total submission counts, review queue counts, and straight through processing details.
     Query can be configured to include only specific metrics by passing in one of WorkflowOptions for SUBMISSIONS, REVIEW, or STRAIGHT_THROUGH_PROCESSING.
 
     Args:
         options (List[WorkflowMetricsOptions]): specific metrics to return.
         start_date (datetime): start date for metrics data.
         end_date (datetime): end date for metrics data. defaults to today.
         workflow_ids (List[int]): ids of specific workflows to query.
 
     """
+
     __MAP_WORKFLOW_KEYS = {
         WorkflowMetricsOptions.SUBMISSIONS: """
         firstSubmittedDate
-               submissions {               
+               submissions {
                   aggregate {
                     submitted
                     completed
                     completedInReview
                     completedReviewQueue
                     completedExceptionQueue
                     rejectedInReview
@@ -94,15 +99,15 @@
                     className
                     aggregate {
                       reviewNumerator
                       autoReviewNumerator
                       reviewDenom
                       autoReviewDenom
                       reviewStpPct
-                      autoReviewStpPct                    
+                      autoReviewStpPct
                     }
                     daily {
                       date
                       reviewNumerator
                       autoReviewNumerator
                       reviewDenom
                       autoReviewDenom
@@ -111,28 +116,27 @@
                     }
                   }
                 }
             }
                 """,
         WorkflowMetricsOptions.TIME_ON_TASK: """
                timeOnTask {
-                  aggregate { 
+                  aggregate {
                     avgMinsPerDoc
                     avgMinsPerDocReview
                     avgMinsPerDocExceptions
                   }
                   daily {
                     date
                     avgMinsPerDoc
                     avgMinsPerDocReview
                     avgMinsPerDocExceptions
                   }
                }
-        """
-
+        """,
     }
     query = """
 query ($workflowIds: [Int]!, $startDate: Date, $endDate:Date) {
     workflows(workflowIds: $workflowIds){
         workflows {
             metrics(startDate:$startDate, endDate:$endDate){
                firstSubmittedDate
@@ -140,29 +144,47 @@
                __QUERY_OPTS__
               }
             }
         }
 }
 """
 
-    def __init__(self, options: List[WorkflowMetricsOptions], start_date: datetime, end_date: datetime,
-                 workflow_ids: List[int]):
+    def __init__(
+        self,
+        options: "List[WorkflowMetricsOptions]",
+        start_date: datetime,
+        end_date: datetime,
+        workflow_ids: "List[int]",
+    ):
         self.query = self.__map_query_values(options)
         if workflow_ids is None or start_date is None:
             raise IndicoInputError("Must specify date and workflow id")
         if end_date is None:
             end_date = datetime.now()
-        super().__init__(self.query, variables={"startDate": start_date.strftime('%Y-%m-%d'),
-                                                "endDate": end_date.strftime('%Y-%m-%d'), "workflowIds": workflow_ids})
 
-    def process_response(self, response) -> List[WorkflowMetrics]:
-        list_of_metrics = _TopWorkflowMetric(**super().process_response(response)["workflows"]).workflows
-        return list(map(lambda x: x.metrics, list_of_metrics))
+        super().__init__(
+            self.query,
+            variables={
+                "startDate": start_date.strftime("%Y-%m-%d"),
+                "endDate": end_date.strftime("%Y-%m-%d"),
+                "workflowIds": workflow_ids,
+            },
+        )
 
-    def __map_query_values(self, options: List[WorkflowMetricsOptions]):
-        daily = ' '
+    def __map_query_values(self, options: "List[WorkflowMetricsOptions]") -> str:
+        daily = " "
         if len(options) < 1:
-            daily = ' '.join([self.__MAP_WORKFLOW_KEYS[a] for a in self.__MAP_WORKFLOW_KEYS.keys()])
+            daily = " ".join(
+                [self.__MAP_WORKFLOW_KEYS[a] for a in self.__MAP_WORKFLOW_KEYS.keys()]
+            )
         else:
-            daily = ' '.join([self.__MAP_WORKFLOW_KEYS[a] for a in options])
-        query = self.query.replace("__QUERY_OPTS__", daily)
+            daily = " ".join([self.__MAP_WORKFLOW_KEYS[a] for a in options])
+
+        query: str = self.query.replace("__QUERY_OPTS__", daily)
         return query
+
+    def process_response(self, response: "Payload") -> "List[WorkflowMetrics]":
+        list_of_metrics = _TopWorkflowMetric(
+            **super().parse_payload(response)["workflows"]
+        ).workflows
+
+        return [x.metrics for x in list_of_metrics]
```

### Comparing `indico-client-6.1.0a1/indico/types/datafile.py` & `indico-client-6.7.0a0/indico/types/datafile.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a1/indico/types/dataset.py` & `indico-client-6.7.0a0/indico/types/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from typing import List
 
+from indico.errors import IndicoInputError
 from indico.types.base import BaseType
 from indico.types.datafile import Datafile
-from indico.errors import IndicoInputError
 
 
 class DataColumn(BaseType):
     """
     A DataColumn in the Indico Platform
 
     Attributes:
@@ -53,36 +53,43 @@
     permissions: str
     files: List[Datafile]
     labelsets: List[LabelSet]
     datacolumns: List[DataColumn]
 
     def labelset_by_name(self, name: str) -> LabelSet:
         if name not in [lab.name for lab in self.labelsets]:
-            raise IndicoInputError(f"No labelset found for {name}. Current labelset names include {[lab.name for lab in self.labelsets]}.")
+            raise IndicoInputError(
+                f"No labelset found for {name}. Current labelset names include {[lab.name for lab in self.labelsets]}."
+            )
         return next(lab for lab in self.labelsets if lab.name == name)
 
     def datacolumn_by_name(self, name: str) -> DataColumn:
         if name not in [datacol.name for datacol in self.datacolumns]:
-            raise IndicoInputError(f"No datacolumn found for {name}. Current datacolumn names include {[datacol.name for datacol in self.datacolumns]}.")
+            raise IndicoInputError(
+                f"No datacolumn found for {name}. Current datacolumn names include {[datacol.name for datacol in self.datacolumns]}."
+            )
         return next(datacol for datacol in self.datacolumns if datacol.name == name)
 
 
 class TableReadOrder(Enum):
     ROW = 0
     COLUMN = 1
 
+
 class OcrEngine(Enum):
     """
     Enum representing available OCR engines.
     """
+
     OMNIPAGE = 0
     READAPI = 1
     READAPI_V2 = 2
     READAPI_TABLES_V1 = 3
 
+
 class OmnipageOcrOptionsInput(BaseType):
     """
     Omnipage specific OCR options for dataset creation.
 
     Args:
         auto_rotate(bool): auto rotate.
         single_colum(bool): Read table as a single column.
@@ -91,44 +98,49 @@
         cells(bool): Return table information for post-processing rules
         force_render(bool): Force rednering.
         native_layout(bool): Native layout.
         native_pdf(bool): Native pdf.
         table_read_order(TableReadOrder): Read table by row or column.
 
     """
+
     auto_rotate: bool
     single_column: bool
     upscale_images: bool
     languages: List[str]
     cells: bool
     force_render: bool
     native_layout: bool
     native_pdf: bool
     table_read_order: TableReadOrder
 
+
 class ReadApiOcrOptionsInput(BaseType):
     """
     Read API OCR options.
 
     Args:
         auto_rotate(bool): Auto rotate
         single_column(bool): Read table as a single column.
         upscale_images(bool): Scale up low resolution images.
         languages(List[str]): List of languages to use.
     """
+
     auto_rotate: bool
     single_column: bool
     upscale_images: bool
     languages: List[str]
 
+
 class OcrInputLanguage(BaseType):
     name: str
     code: str
 
-class OcrOptionsInput():
+
+class OcrOptionsInput:
     """
     Input options for OCR engine.
     """
+
     ocr_engine: OcrEngine
     omnipage_options: OmnipageOcrOptionsInput
     readapi_options: ReadApiOcrOptionsInput
-
```

### Comparing `indico-client-6.1.0a1/indico/types/export.py` & `indico-client-6.7.0a0/indico/types/export.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import List
 from enum import Enum
+from typing import List
 
 from indico.types.base import BaseType
 
 
 class LabelResolutionStrategy(Enum):
     MAJORITY_VOTE_WITH_TIES = "majority_vote_with_ties"
     MAJORITY_VOTE_WITHOUT_TIES = "majority_vote_without_ties"
```

### Comparing `indico-client-6.1.0a1/indico/types/integration.py` & `indico-client-6.7.0a0/indico/types/integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from datetime import datetime
 from enum import Enum
+
 from indico.types import BaseType
 
 
 class IntegrationType(Enum):
     EXCHANGE = 1
 
+
 class ExchangeIntegrationCredentials(BaseType):
     """
     Credentials needed to connect a Microsoft Exchange server to an Indico workflow using
     """
+
     client_id: str
     client_secret: str
     tenant_id: str
 
+
 class ExchangeIntegrationConfiguration(BaseType):
     """
     Configuration options available for an integration with Microsoft Exchange
     """
+
     user_id: str
     folder_id: str
-    folder_name: str = None
-    filters: str = None
+    folder_name: str
+    filters: str
 
 
 class Integration(BaseType):
     """
     An integration pulls document from a third-party data source and submits them to a workflow
 
     Args:
-        id(int): ID of the integration 
+        id(int): ID of the integration
         workflow_id(int): ID of the workflow to submit to.
         enabled(bool): Whether Indico is currently sending documents from this datasource to the workflow.
         created_at(datetime): When this integration was created.
         integration_type(IntegrationType): Type of the data source for this integration
     """
 
     id: int
     workflow_id: int
     enabled: bool
     created_at: datetime
     integration_type: IntegrationType
 
+
 class ExchangeIntegration(Integration):
     config: ExchangeIntegrationConfiguration
```

### Comparing `indico-client-6.1.0a1/indico/types/model_group.py` & `indico-client-6.7.0a0/indico/types/model_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     task_type: str
     questionnaire_id: int
     class_names: List[str]
 
 
 class ModelTaskType(Enum):
     """A list of valid task types for a model group."""
+
     CLASSIFICATION = 1
     FORM_EXTRACTION = 2
     OBJECT_DETECTION = 3
     CLASSIFICATION_MULTIPLE = 4
     REGRESSION = 5
     ANNOTATION = 6
     CLASSIFICATION_UNBUNDLING = 7
@@ -50,32 +51,38 @@
     DOCUMENT = 5
     TFIDF_LR = 6
     TFIDF_GBT = 7
 
 
 class NewQuestionnaireArguments(BaseType):
     """instructions: String
-Questionnaire instructions
+    Questionnaire instructions
 
-forceTextMode: Boolean = false
-Always use Text Labeling UI
+    forceTextMode: Boolean = false
+    Always use Text Labeling UI
 
-showPredictions: Boolean = true
-Show predictions at the global level
+    showPredictions: Boolean = true
+    Show predictions at the global level
 
-users: [Int]
-User IDs to add to the questionnaire"""
+    users: [Int]
+    User IDs to add to the questionnaire"""
 
     instructions: str
     force_text_mode: bool = False
     show_predictions: bool = True
     users: List[int]
 
 
-class NewLabelsetArguments():
-    def __init__(self, name: str, task_type: ModelTaskType,
-                 target_names: List[str], datacolumn_id: int, num_labelers_required: int = 1):
+class NewLabelsetArguments:
+    def __init__(
+        self,
+        name: str,
+        task_type: ModelTaskType,
+        target_names: List[str],
+        datacolumn_id: int,
+        num_labelers_required: int = 1,
+    ):
         self.name = name
         self.num_labelers_required = num_labelers_required
         self.task_type = task_type
         self.target_names = target_names
         self.datacolumn_id = datacolumn_id
```

### Comparing `indico-client-6.1.0a1/indico/types/model_metrics.py` & `indico-client-6.7.0a0/indico/types/model_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+
 from indico.types.base import BaseType
 
 
 class PerClassSeqMetrics(BaseType):
     """
     Metrics per class
```

### Comparing `indico-client-6.1.0a1/indico/types/questionnaire.py` & `indico-client-6.7.0a0/indico/types/questionnaire.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+
 from indico.types.base import BaseType
 
 
 class TargetName(BaseType):
     id: int
     name: str
```

### Comparing `indico-client-6.1.0a1/indico/types/submission_file.py` & `indico-client-6.7.0a0/indico/types/submission_file.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a1/indico/types/user_metrics.py` & `indico-client-6.7.0a0/indico/types/user_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,99 @@
-import datetime
+from datetime import datetime
+from typing import List
 
 from indico.types.base import BaseType
-from typing import List
 
 
 class AppRoles(BaseType):
     """Info about roles. Name and how many users have this role.
-    
+
     Attributes:
         role (str): A role name
         count (int): Count of how many users have said role.
     """
+
     role: str
     count: int
 
 
 class UserDatasets(BaseType):
     """Dataset Id and roles assigned to user in that dataset.
-    
+
     Attributes:
         dataset_id (int): The id of a particular dataset
         role (str): A dataset assigned to said dataset.
     """
+
     dataset_id: int
     role: str
 
 
 class UserSummaryCounts(BaseType):
     """
     Summary of user counts
 
     Attributes:
         enabled (int): How many user accounts are enabled.
         disabled (int): How many user accounts are disabled.
     """
+
     enabled: int
     disabled: int
 
 
 class UserSnapshot(BaseType):
     """Individual information about a user and their dataset access
-    
+
     Attributes:
         id (int): The user's id.
         name (str): The user's name.
         email (str): The user's email.
         created_at (str): Time of creation.
         enabled (bool): True if user account is enabled.
         roles (List[str]): List of roles assigned to this user.
         datasets (List[UserDatasets]): List of datasets this user can access.
     """
+
     id: int
     name: str
     email: str
     created_at: str
     enabled: bool
     roles: List[str]
     datasets: List[UserDatasets]
 
 
 class UserSummary(BaseType):
     """Summary data on users and app roles
-    
+
     Attributes:
         users (UserSummarycounts): Counts of enabled/disabled users.
         app_roles (List[AppRoles]): List of all available user roles.
     """
+
     users: UserSummaryCounts
     app_roles: List[AppRoles]
 
 
 class DatasetRole(BaseType):
     """Dataset role information
-    
+
     Attributes:
         dataset_id (int): Id of a particular dataset.
         role (str): Role name which has access to this dataset.
     """
+
     dataset_id: int
     role: str
 
 
 class UserChangelog(BaseType):
     """Log entry of a change made to a user's permission
-    
+
     Attributes:
         id (str): Id of the log entry
         date (datetime): Time of long entry.
         user_id (int): Id of the user whose attributes were changed.
         user_email (str): Email of the user whose attributes were changed.
         updated_by (id): Id of the account which made the change.
         updater_email (str): Email of the account which made the change.
@@ -96,14 +102,15 @@
         previous_roles (List[str]): Roles assigned prior to the change.
         roles (List[str]): Roles assigned after the change.
         previous_datasets (List[DatasetRole]): List of dataset/role mappings prior to the change.
         datasets (List[DatasetRole]): List of dataset/role mappings after the change.
         changes_made (List[str]): A list of changed made.
 
     """
+
     id: str
     date: datetime
     user_id: int
     user_email: str
     updated_by: int
     updater_email: str
     previously_enabled: bool
@@ -113,12 +120,13 @@
     previous_datasets: List[DatasetRole]
     datasets: List[DatasetRole]
     changes_made: List[str]
 
 
 class UserChangelogReport(BaseType):
     """Job id of a request for a changelog report file for download
-    
+
     Attributes:
         job_id (str): The job id. Use for fetching JobStatus.
     """
+
     job_id: str
```

### Comparing `indico-client-6.1.0a1/indico/types/utils.py` & `indico-client-6.7.0a0/indico/types/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import re
-from typing import Union
 import time
+from typing import TYPE_CHECKING
+
 from indico.errors import IndicoTimeoutError
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Match, NoReturn, Optional, Union
+
 _cc_to_snake_re = re.compile(r"(?<!^)(?=[A-Z])")
 _snake_to_cc_re = re.compile(r"(.*?)_([a-zA-Z])")
 
 
-def cc_to_snake(string: str):
+def cc_to_snake(string: str) -> str:
     return re.sub(_cc_to_snake_re, "_", string).lower()
 
 
-def _camel(match):
+def _camel(match: "Match[str]") -> str:
     return match.group(1) + match.group(2).upper()
 
 
-def snake_to_cc(string: str):
+def snake_to_cc(string: str) -> str:
     return re.sub(_snake_to_cc_re, _camel, string, 0)
 
 
-
 class Timer:
-    def __init__(self, timeout: Union[int, float]):
-        self.timeout = timeout
-        self.start = time.time()
-        self.elapsed = 0
+    def __init__(self, timeout: "Union[int, float]"):
+        self.timeout: "Union[int, float]" = timeout
+        self.start: float = time.time()
+        self.elapsed: float = 0
 
-    def check(self):
+    def check(self) -> "Optional[NoReturn]":
         self.elapsed = time.time() - self.start
         if self.timeout < self.elapsed:
-            raise IndicoTimeoutError(self.elapsed)
+            raise IndicoTimeoutError(self.elapsed)
+
+        return None
```

### Comparing `indico-client-6.1.0a1/indico/types/workflow.py` & `indico-client-6.7.0a0/indico/types/workflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from enum import Enum
-from typing import List, Union
 from datetime import datetime
-from indico.types import BaseType, ModelGroup, ModelTaskType
+from enum import Enum
+from typing import TYPE_CHECKING, List
+
+from indico.types import BaseType, ModelGroup
+
+if TYPE_CHECKING:  # pragma: no cover
+    from indico.typing import AnyDict
 
 
 class WorkflowComponent(BaseType):
     """
     A component, such as a Model Group or Content Length filter, that is present on a workflow.
     This is essentially a step in the workflow process, such as OCR
     or predicting with a model group.
@@ -13,16 +17,14 @@
     """
 
     id: int
     component_type: str
     task_type: str
     model_type: str
     model_group: ModelGroup
-    task_type: str
-    model_type: str
     minimum: int
     maximum: int
 
 
 class WorkflowComponentLinks(BaseType):
     """
     Represents a link between two components.
@@ -67,31 +69,31 @@
             component
             for component in self.components
             if hasattr(component, "model_group") and component.model_group.name == name
         )
 
 
 class LinkedLabelStrategy(Enum):
-    BY_ROW = 0,
+    BY_ROW = (0,)
     BY_KEY = 1
 
 
 class LinkedLabelGroup:
     def __init__(
         self,
         name: str,
         strategy: LinkedLabelStrategy,
         class_ids: List[int],
-        strategy_settings: dict,
+        strategy_settings: "AnyDict",
     ):
         self.name = name
         self.strategy = strategy
         self.class_ids = class_ids
         self.strategy_settings = strategy_settings
 
 
 class ComponentFamily(Enum):
-    MODEL = 0,
-    FILTER = 1,
-    TRANSFORMER = 2,
-    REVIEW = 3,
+    MODEL = (0,)
+    FILTER = (1,)
+    TRANSFORMER = (2,)
+    REVIEW = (3,)
     OUTPUT = 4
```

### Comparing `indico-client-6.1.0a1/indico/types/workflow_metrics.py` & `indico-client-6.7.0a0/indico/types/workflow_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from enum import Enum
-from indico.types.base import BaseType
 from typing import List
 
+from indico.types.base import BaseType
+
 
 class WorkflowMetricsOptions(Enum):
     """
     Options for pulling back specific metrics.
 
     Attributes:
         SUBMISSIONS: Generates SubmissionMetrics in the response.
         REIVEW: Generates review Queue metrics in the response.
         STRAIGHT_THROUGH_PROCESSING: Generates StraightThroughProcessing metrics in the response.
         TIME_ON_TASK: Average time spent by reviewers on documents.
     """
+
     SUBMISSIONS = 1
     REVIEW = 2
     STRAIGHT_THROUGH_PROCESSING = 3
     TIME_ON_TASK = 4
 
 
 class TimeOnTaskMetric(BaseType):
@@ -27,43 +29,46 @@
         avg_mins_per_doc(float): Average amount of minutes reviewers spend on documents in this workflow
             across review and exceptions queue.
         avg_mins_per_doc_review(float): Average amount of minutes reviewers spend on documents in this workflow
             in the review queue.
         avg_min_per_doc_exceptions(float): Average amount of minutes reviewers spend on ducments for this workflow in
             the exceptions queue.
     """
+
     avg_mins_per_doc: float
     avg_mins_per_doc_review: float
     avg_min_per_doc_exceptions: float
 
 
 class DailyTimeOnTaskMetric(TimeOnTaskMetric):
     """
     Daily time on task metrics.
-    
+
     Attributes:
         avg_mins_per_doc(float): Average amount of minutes reviewers spend on documents in this workflow
             across review and exceptions queue.
         avg_mins_per_doc_review(float): Average amount of minutes reviewers spend on documents in this workflow
             in the review queue.
         avg_min_per_doc_exceptions(float): Average amount of minutes reviewers spend on ducments for this workflow in
             the exceptions queue.
         date(str): Date.
     """
+
     date: str
 
 
 class TimeOnTaskMetrics(BaseType):
     """
     Time on task metrics.
 
     Attributes:
         aggregate(TimeOnTaskMetric): Aggregate level time on task metrics.
         daily(List[DailyTimeOnTaskMetric): Daily level time on task metrics.
     """
+
     aggregate: TimeOnTaskMetric
     daily: List[DailyTimeOnTaskMetric]
 
 
 class SubmissionMetric(BaseType):
     """
     Submission metric.
@@ -73,14 +78,15 @@
         completed(int): Number of items completed in this workflow on this day.
         completed_in_review(int): Number of items accepted in the review or the exceptions queue.
         completed_review_queue(int): Number of items accepted in the review queue.
         completed_exception_queue(int): Number of items accepted in the exceptions queue.
         rejected_in_review(int): Number of items rejected in the exceptions queue.
         date(str): Date.
     """
+
     submitted: int
     completed: int
     completed_in_review: int
     completed_review_queue: int
     completed_exception_queue: int
     rejected_in_review: int
 
@@ -94,80 +100,87 @@
         completed(int): Number of items completed in this workflow on this day.
         completed_in_review(int): Number of items accepted in the review or the exceptions queue.
         completed_review_queue(int): Number of items accepted in the review queue.
         completed_exception_queue(int): Number of items accepted in the exceptions queue.
         rejected_in_review(int): Number of items rejected in the exceptions queue.
         date(str): Date.
     """
+
     date: str
 
 
 class SubmissionMetrics(BaseType):
     """
     Submission metrics.
 
     Attributes:
         aggregate(SubmissionMetric): Aggregate level submission metrics.
         daily(List[SubmissionMetric]): Daily submission metrics.
     """
+
     aggregate: SubmissionMetric
     daily: List[DailySubmissionMetric]
 
 
 class DailyQueueMetric(BaseType):
     """
     Daily cumulative metrics for queues
     Attributes:
         date (str): the date.
         subs_on_queue(int): Number of submissions queued for review
         hours_on_queue(float): Cumulative hours items wait on queue for review.
         avg_age_in_queue(float): Average cumulative age of items waiting in review queues.
     """
+
     date: str
     subs_on_queue: int
     hours_on_queue: float
     avg_age_in_queue: float
 
 
 class QueueMetrics(BaseType):
     """
     Daily cumulative metrics for queues.
     Attributes:
         daily_cumulative(List[DailyQueueMetric]): list of cumulative queue metrics per day
     """
+
     daily_cumulative: List[DailyQueueMetric]
 
 
 class PredictionMetric(BaseType):
     """
     The total number of model-generated predictions for specified workflow.
     Attributes:
         num_preds(int): the total number of model-generated predictions.
     """
+
     num_preds: int
 
 
 class DailyPredictionMetric(PredictionMetric):
     """
     The total number of model-generated predictions for specified workflow for this date.
     Attributes:
         date(str): the date of the prediction.
         num_preds(int): the total number of model-generated predictions.
     """
+
     date: str
 
 
 class PredictionMetrics(BaseType):
     """
     Prediction metrics.
 
     Attributes:
         aggregate(PredictionMetric): Total number of predictions generated for this workflow.
         daily(List[PredictionMetrics]): Number of predictions generated per-date.
     """
+
     aggregate: PredictionMetric
     daily: List[PredictionMetric]
 
 
 class StpMetric(BaseType):
     """
     Base Straight through processing (STP) metric for a model, class, or workflow.
@@ -176,14 +189,15 @@
         review_numerator(int): The number of human accepted model predictions.
         auto_review_numerator(int): The number of human accepted auto review labels.
         review_denom(int): Total of user supplied labels and model predictions.
         auto_review_denom(int) Total of user supplied labels and auto review labels.
         review_stp_pct(float): Percent of human accepted model predictions. Present if auto review is disabled.
         auto_review_stp_pct(float): Percent of auto review labels accepted. Present if auto review is enabled.
     """
+
     review_numerator: int
     auto_review_numerator: int
     review_denom: int
     auto_review_denom: int
     review_stp_pct: float
     auto_review_stp_pct: float
 
@@ -197,26 +211,28 @@
         auto_review_numerator(int): The number of human accepted auto review labels.
         review_denom(int): Total of user supplied labels and model predictions.
         auto_review_denom(int) Total of user supplied labels and auto review labels.
         review_stp_pct(float): Percent of human accepted model predictions. Present if auto review is disabled.
         auto_review_stp_pct(float): Percent of auto review labels accepted. Present if auto review is enabled.
         date(str): The date these metrics are applicable.
     """
+
     date: str
 
 
 class ClassStpMetrics(BaseType):
     """
     STP Metrics per class.
 
     Attributes:
         class_name(str): Name of the class.
         aggregate(StpMetric): Aggregate level metrics about this class.
         daily(List[DailyStpMetric]): Per-date STP metrics for this class.
     """
+
     class_name: str
     aggregate: StpMetric
     daily: List[DailyStpMetric]
 
 
 class ModelStpMetrics(BaseType):
     """
@@ -225,39 +241,42 @@
     Attributes:
         model_group_id(int): Id of the model group.
         name(str): Name of the model.
         aggregate(StpMetric): Aggregate level STP metrics for the model.
         daily(List[DailyStpMetric]): Daily STP metrics for the model.
         class_metrics(List[ClassStpMetrics]): Metrics per model class.
     """
+
     model_group_id: int
     name: str
     aggregate: StpMetric
     daily: List[DailyStpMetric]
     class_metrics: List[ClassStpMetrics]
 
 
 class WorkflowStpMetrics(BaseType):
     """
     Daily workflow STP metrics.
 
     Attributes:
         daily(List[DailyStpMetric]): List of daily metrics.
     """
+
     daily: List[DailyStpMetric]
 
 
 class StraightThroughProcessing(BaseType):
     """
     Straight Through Processing (STP) metrics.
 
     Attributes:
         workflow(WorkflowStpMetrics): Daily aggregate workflow level STP metrics.
         model(List[ModelStpMetrics]): Model STP metrics (including class STP).
     """
+
     workflow: WorkflowStpMetrics
     model: List[ModelStpMetrics]
 
 
 class WorkflowMetrics(BaseType):
     """
     Workflow metrics for the requested workflow id and dates.
@@ -268,14 +287,15 @@
         submissions(SubmissionMetrics): Submission specific metrics.
         queues(QueueMetrics): Review queue metrics.
         predictions(PredictionMetrics): Prediction metrics.
         straight_through_processing(StraightThroughProcessing): Straight through processing (STP) metrics.
         first_submitted_date(str): The earliest date of submission to this workflow.
 
     """
+
     workflow_id: int
     time_on_task: TimeOnTaskMetrics
     submissions: SubmissionMetrics
     queues: QueueMetrics
     predictions: PredictionMetrics
     straight_through_processing: StraightThroughProcessing
     first_submitted_date: str
```

### Comparing `indico-client-6.1.0a1/indico_client.egg-info/PKG-INFO` & `indico-client-6.7.0a0/indico_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indico-client
-Version: 6.1.0a1
+Version: 6.7.0a0
 Summary: A Python Wrapper for indico app API.
 Home-page: https://github.com/IndicoDataSolutions/indico-client-python
 Author: indico
 Author-email: engineering@indico.io
 License: MIT License (See LICENSE)
 Platform: UNKNOWN
 License-File: LICENSE
@@ -29,7 +29,8 @@
 From source:
 
 .. code:: bash
 
     git clone https://github.com/IndicoDataSolutions/indico-client-python.git
     python setup.py install
 
+
```

### Comparing `indico-client-6.1.0a1/indico_client.egg-info/SOURCES.txt` & `indico-client-6.7.0a0/indico_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 indico/__init__.py
 indico/_version.py
 indico/errors.py
+indico/py.typed
+indico/typing.py
 indico/client/__init__.py
 indico/client/client.py
 indico/client/request.py
 indico/config/__init__.py
 indico/config/config.py
 indico/filters/__init__.py
 indico/http/__init__.py
@@ -46,14 +49,15 @@
 indico/types/document_report.py
 indico/types/export.py
 indico/types/integration.py
 indico/types/jobs.py
 indico/types/model.py
 indico/types/model_group.py
 indico/types/model_metrics.py
+indico/types/output_file.py
 indico/types/questionnaire.py
 indico/types/submission.py
 indico/types/submission_file.py
 indico/types/user_metrics.py
 indico/types/utils.py
 indico/types/workflow.py
 indico/types/workflow_metrics.py
@@ -75,13 +79,14 @@
 tests/integration/queries/test_document.py
 tests/integration/queries/test_document_report.py
 tests/integration/queries/test_export.py
 tests/integration/queries/test_integration.py
 tests/integration/queries/test_job.py
 tests/integration/queries/test_model_group.py
 tests/integration/queries/test_questionnaire.py
+tests/integration/queries/test_submission.py
 tests/integration/queries/test_user_metrics.py
 tests/integration/queries/test_workflow.py
 tests/integration/queries/test_workflow_component.py
 tests/integration/queries/test_workflow_metrics.py
 tests/unit/__init__.py
 tests/unit/test_filters.py
```

### Comparing `indico-client-6.1.0a1/setup.py` & `indico-client-6.7.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """
 Setup for indico apis
 """
-import versioneer
+
 from pathlib import Path
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
+
+import versioneer
 
 setup(
     name="indico-client",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     packages=find_packages(exclude=["tests"]),
     description="""A Python Wrapper for indico app API.""",
     license="MIT License (See LICENSE)",
     long_description=open(Path(__file__).parent.absolute() / "README.rst").read(),
     url="https://github.com/IndicoDataSolutions/indico-client-python",
     author="indico",
     author_email="engineering@indico.io",
-    tests_require=["pytest>=5.2.1", "requests-mock>=1.8.0", "pytest-asyncio"],
+    tests_require=["pytest<8", "requests-mock>=1.8.0", "pytest-asyncio>0.21"],
     install_requires=[
         "msgpack>=0.5.6",
         "msgpack-numpy==0.4.4.3",
         "numpy>=1.16.0",
         "Pillow>=6.2.0",
         "requests>=2.22.0",
         "setuptools>=41.4.0",
         "pandas>=1.0.3",
         'importlib-metadata ~= 1.0 ; python_version < "3.8"',
         "deprecation>=2.1.0",
         "jsons",
-        "aiohttp[speedups]"
+        "aiohttp[speedups]",
     ],
 )
```

### Comparing `indico-client-6.1.0a1/tests/integration/conftest.py` & `indico-client-6.7.0a0/tests/integration/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
-import pytest
 import os
 
+import pytest
+
 from indico.client import IndicoClient
 from indico.queries.datasets import GetAvailableOcrEngines
-from .data.datasets import *
+
 from .data.async_datasets import *
+from .data.datasets import *
 
 logging.getLogger("indico").setLevel(logging.DEBUG)
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--host",
```

### Comparing `indico-client-6.1.0a1/tests/integration/data/async_datasets.py` & `indico-client-6.7.0a0/tests/integration/data/async_datasets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pytest_asyncio
 import time
 from pathlib import Path
+
+import pytest_asyncio
+
 from indico.client import AsyncIndicoClient
-from indico.queries import (
-    CreateDataset,
-)
+from indico.queries import CreateDataset
 
 
 @pytest_asyncio.fixture(scope="module")
 async def aio_org_annotate_dataset(indico):
     dataset_filepath = str(Path(__file__).parents[0]) + "/org-annotate-labeled.csv"
     async with AsyncIndicoClient() as client:
         response = await client.call(
```

### Comparing `indico-client-6.1.0a1/tests/integration/data/datasets.py` & `indico-client-6.7.0a0/tests/integration/data/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
-import pytest
 import time
 from pathlib import Path
+
+import pytest
+
 from indico.client import IndicoClient
 from indico.queries import (
+    AddExchangeIntegration,
+    AddModelGroupComponent,
     CreateDataset,
     CreateWorkflow,
-    AddModelGroupComponent,
     GetModelGroup,
-    AddExchangeIntegration,
-    StartIntegration,
     GetWorkflow,
+    StartIntegration,
 )
 from indico.queries.workflow_components import _AddWorkflowComponent
-from indico.types import ModelGroup, Dataset, Workflow, Integration
+from indico.types import Dataset, Integration, ModelGroup, Workflow
 
 PUBLIC_URL = "https://github.com/IndicoDataSolutions/indico-client-python/raw/master/tests/integration/data/"
 
 
 @pytest.fixture(scope="module")
 def airlines_dataset(indico):
     client = IndicoClient()
@@ -266,53 +268,39 @@
 
 @pytest.fixture(scope="module")
 def exchange_integration_to_delete(org_annotate_workflow: Workflow) -> Integration:
     client = IndicoClient()
     creds = {
         "clientId": os.getenv("EXCH_CLIENT_ID"),
         "clientSecret": os.getenv("EXCH_CLIENT_SECRET"),
-        "tenantId": os.getenv("EXCH_TENANT_ID")
+        "tenantId": os.getenv("EXCH_TENANT_ID"),
     }
 
-    config = {
-        "userId": os.getenv("EXCH_USER_ID"),
-        "folderId": "mailFolders('inbox')"
-    }
+    config = {"userId": os.getenv("EXCH_USER_ID"), "folderId": "mailFolders('inbox')"}
 
     integ: Integration = client.call(
         AddExchangeIntegration(
-            workflow_id=org_annotate_workflow.id,
-            config=config,
-            credentials=creds
+            workflow_id=org_annotate_workflow.id, config=config, credentials=creds
         )
     )
 
     return integ
 
 
 @pytest.fixture(scope="module")
 def started_exchange_integration(org_annotate_workflow: Workflow) -> Integration:
     client = IndicoClient()
     creds = {
         "clientId": os.getenv("EXCH_CLIENT_ID"),
         "clientSecret": os.getenv("EXCH_CLIENT_SECRET"),
-        "tenantId": os.getenv("EXCH_TENANT_ID")
+        "tenantId": os.getenv("EXCH_TENANT_ID"),
     }
 
-    config = {
-        "userId": os.getenv("EXCH_USER_ID"),
-        "folderId": "mailFolders('inbox')"
-    }
+    config = {"userId": os.getenv("EXCH_USER_ID"), "folderId": "mailFolders('inbox')"}
 
     integ: Integration = client.call(
         AddExchangeIntegration(
-            workflow_id=org_annotate_workflow.id,
-            config=config,
-            credentials=creds
-        )
-    )
-    client.call(
-        StartIntegration(
-            integration_id=integ.id
+            workflow_id=org_annotate_workflow.id, config=config, credentials=creds
         )
     )
+    client.call(StartIntegration(integration_id=integ.id))
     yield integ
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_custom_blueprint.py` & `indico-client-6.7.0a0/tests/integration/queries/test_custom_blueprint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import pytest
+
 from indico.client import IndicoClient
 from indico.errors import IndicoInputError
 from indico.queries.custom_blueprint import RegisterCustomBlueprint
 from indico.types.workflow import ComponentFamily
 
 
 def test_register_blueprint(indico):
     client = IndicoClient()
     bpreq = RegisterCustomBlueprint(
-        component_family=ComponentFamily.OUTPUT, 
-        name="Meowtput", 
-        description="adds 'cat' to the result file", 
+        component_family=ComponentFamily.OUTPUT,
+        name="Meowtput",
+        description="adds 'cat' to the result file",
         config={
             "inputs": [{"name": "result_file", "ioClass": "PartitionStream"}],
             "outputs": [{"name": "result_file", "ioClass": "PartitionStream"}],
-            "submissionLauncher": {"service": "customizer_default", "name": "cat_output"}
+            "submissionLauncher": {
+                "service": "customizer_default",
+                "name": "cat_output",
+            },
         },
-        tags= ["custom"],
+        tags=["custom"],
         all_access=True,
-        footer="version 2"
+        footer="version 2",
     )
     bp = client.call(bpreq)
     print(bp.__dict__)
     assert bp.id
 
+
 def test_register_blueprint_bad_config(indico):
     with pytest.raises(IndicoInputError):
         RegisterCustomBlueprint(
-            component_family=ComponentFamily.OUTPUT, 
-            name="Meowtput", 
-            description="adds 'cat' to the result file", 
+            component_family=ComponentFamily.OUTPUT,
+            name="Meowtput",
+            description="adds 'cat' to the result file",
             config={
                 "inputs": [{"name": "result_file", "ioClass": "PartitionStream"}],
                 "outputs": [{"name": "result_file", "ioClass": "PartitionStream"}],
-                "submissionLauncher": {}
+                "submissionLauncher": {},
             },
-            tags= ["custom"],
+            tags=["custom"],
             all_access=True,
-            footer="version 2"
+            footer="version 2",
         )
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_dataset.py` & `indico-client-6.7.0a0/tests/integration/queries/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-import time
 import json
-from indico.filters import DatasetFilter
-import pytest
-import pandas as pd
-from pathlib import Path
 import os
+import time
+from pathlib import Path
+
+import pandas as pd
+import pytest
+
 from indico.client import IndicoClient
+from indico.errors import IndicoRequestError
+from indico.filters import DatasetFilter
 from indico.queries.datasets import (
+    AddFiles,
+    CreateDataset,
+    CreateEmptyDataset,
+    DeleteDataset,
     GetDataset,
     GetDatasetFileStatus,
-    CreateDataset,
     ListDatasets,
-    DeleteDataset,
-    CreateEmptyDataset,
-    AddFiles,
-    ProcessFiles,
 )
 from indico.queries.export import CreateExport, DownloadExport
 from indico.types.dataset import (
     Dataset,
-    OmnipageOcrOptionsInput,
-    TableReadOrder,
     OcrEngine,
+    OmnipageOcrOptionsInput,
     ReadApiOcrOptionsInput,
+    TableReadOrder,
 )
-from indico.errors import IndicoRequestError
 from tests.integration.data.datasets import airlines_dataset  # noqa: F401
 
 
 def test_create_dataset(indico):
     client = IndicoClient()
     dataset_filepath = str(Path(__file__).parents[1]) + "/data/AirlineComplaints.csv"
 
@@ -261,45 +262,14 @@
     dataset = client.call(
         AddFiles(dataset_id=dataset.id, files=[dataset_filepaths[1]], autoprocess=True)
     )
 
     _dataset_complete(dataset)
 
 
-def test_create_from_files_document_without_autoprocess(indico):
-    client = IndicoClient()
-    dataset = client.call(CreateEmptyDataset(name=f"dataset-{int(time.time())}"))
-    file_names = ["us_doi.tiff", "mock.pdf"]
-    parent_path = str(Path(__file__).parent.parent / "data")
-    dataset_filepaths = [
-        os.path.join(parent_path, file_name) for file_name in file_names
-    ]
-
-    dataset = client.call(AddFiles(dataset_id=dataset.id, files=[dataset_filepaths[0]]))
-
-    for f in dataset.files:
-        assert f.status == "DOWNLOADED"
-
-    datafile_ids = [f.id for f in dataset.files]
-
-    dataset = client.call(
-        ProcessFiles(dataset_id=dataset.id, datafile_ids=datafile_ids, wait=True)
-    )
-
-    dataset = client.call(AddFiles(dataset_id=dataset.id, files=[dataset_filepaths[1]]))
-
-    datafile_ids = [f.id for f in dataset.files if f.status == "DOWNLOADED"]
-
-    dataset = client.call(
-        ProcessFiles(dataset_id=dataset.id, datafile_ids=datafile_ids, wait=True)
-    )
-
-    _dataset_complete(dataset)
-
-
 def test_create_from_files_document(indico):
     client = IndicoClient()
     dataset = client.call(CreateEmptyDataset(name=f"dataset-{int(time.time())}"))
     file_names = ["us_doi.tiff", "mock.pdf"]
     parent_path = str(Path(__file__).parent.parent / "data")
     dataset_filepaths = [
         os.path.join(parent_path, file_name) for file_name in file_names
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_document.py` & `indico-client-6.7.0a0/tests/integration/queries/test_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import unittest
-import pytest
 import os
+import unittest
 from pathlib import Path
+
+import pytest
+
 from indico.client import IndicoClient
 from indico.queries import (
-    RetrieveStorageObject,
-    JobStatus,
     DocumentExtraction,
+    JobStatus,
+    RetrieveStorageObject,
     UploadBatched,
     UploadDocument,
 )
 
 
 def test_document_extraction(indico):
     client = IndicoClient()
@@ -140,15 +142,18 @@
     for job in jobs:
         assert job.id is not None
         job = client.call(JobStatus(id=job.id, wait=True))
         assert job.status == "SUCCESS"
         assert job.ready is True
         assert isinstance(job.result["url"], str)
 
-@unittest.skip("Expected to fail pending https://indicodata.atlassian.net/browse/SUP-437")
+
+@unittest.skip(
+    "Expected to fail pending https://indicodata.atlassian.net/browse/SUP-437"
+)
 def test_document_extraction_images(indico):
     client = IndicoClient()
     dataset_filepath = str(Path(__file__).parents[1]) + "/data/mock.pdf"
     jobs = client.call(
         DocumentExtraction(
             files=[dataset_filepath], json_config='{"preset_config": "simple"}'
         )
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_document_report.py` & `indico-client-6.7.0a0/tests/integration/queries/test_document_report.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import List
 
 from indico import IndicoClient
+from indico.filters import DocumentReportFilter
 from indico.queries.document_report import GetDocumentReport
 from indico.types.document_report import DocumentReport
-from indico.filters import DocumentReportFilter
 
 
 def test_fetch_docs(indico):
     """
     NOTE: this test will fail if the cluster hasn't yet processed any submissions
     """
     client = IndicoClient()
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_export.py` & `indico-client-6.7.0a0/tests/integration/queries/test_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-import pytest
 import json
+import re
 from unittest import mock
+
+import pytest
+
 from indico.client import IndicoClient
-from indico.types.dataset import Dataset
-from indico.types.export import Export
 from indico.errors import IndicoRequestError
 from indico.queries.export import CreateExport, DownloadExport
+from indico.types.dataset import Dataset
+from indico.types.export import Export
+
 from ..data.datasets import airlines_dataset
-import re
 
 
 def test_create_and_download_export(airlines_dataset: Dataset):
     client = IndicoClient()
     export = client.call(
         CreateExport(
             dataset_id=airlines_dataset.id,
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_integration.py` & `indico-client-6.7.0a0/tests/integration/queries/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 
 from indico.client import IndicoClient
 from indico.queries import (
     AddExchangeIntegration,
-    StartIntegration,
     DeleteIntegration,
     PauseIntegration,
+    StartIntegration,
 )
-
-from indico.types import Workflow, Integration, ModelGroup
+from indico.types import Integration, ModelGroup, Workflow
 from tests.integration.data.datasets import (
-    airlines_workflow,
     airlines_dataset,
-    org_annotate_workflow,
+    airlines_workflow,
+    exchange_integration_to_delete,
     org_annotate_dataset,
     org_annotate_exchange_integration,
     org_annotate_model_group,
-    exchange_integration_to_delete,
-    started_exchange_integration
+    org_annotate_workflow,
+    started_exchange_integration,
 )
 
+
 def test_add_integration(airlines_workflow: Workflow):
     client = IndicoClient()
     creds = {
         "clientId": os.getenv("EXCH_CLIENT_ID"),
         "clientSecret": os.getenv("EXCH_CLIENT_SECRET"),
         "tenantId": os.getenv("EXCH_TENANT_ID"),
     }
@@ -44,35 +44,23 @@
     org_annotate_exchange_integration: Integration,
     org_annotate_model_group: ModelGroup,
     org_annotate_workflow: Workflow,
 ):
     integ = org_annotate_exchange_integration
     assert not integ.enabled
     client = IndicoClient()
-    resp = client.call(
-        StartIntegration(
-            integration_id=integ.id
-        )
-    )
+    resp = client.call(StartIntegration(integration_id=integ.id))
     assert resp["startWorkflowIntegration"]["success"]
-    
+
 
 def test_delete_integration(exchange_integration_to_delete: Integration):
     integ = exchange_integration_to_delete
     client = IndicoClient()
-    resp = client.call(
-        DeleteIntegration(
-            integration_id=integ.id
-        )
-    )
+    resp = client.call(DeleteIntegration(integration_id=integ.id))
     assert resp["deleteWorkflowIntegration"]["success"]
 
 
 def test_pause_integration(started_exchange_integration: Integration):
     integ = started_exchange_integration
     client = IndicoClient()
-    resp = client.call(
-        PauseIntegration(
-            integration_id=integ.id
-        )
-    )
+    resp = client.call(PauseIntegration(integration_id=integ.id))
     assert resp["pauseWorkflowIntegration"]["success"]
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_job.py` & `indico-client-6.7.0a0/tests/integration/queries/test_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import pytest
 
 from indico.client import IndicoClient
-from indico.queries import JobStatus, DocumentExtraction
-from indico.types.jobs import Job
 from indico.errors import IndicoTimeoutError
+from indico.queries import DocumentExtraction, JobStatus
+from indico.types.jobs import Job
 
 
 def test_job_wait_on_success(indico):
     client = IndicoClient()
     dataset_filepath = str(Path(__file__).parents[1]) + "/data/mock.pdf"
 
     jobs = client.call(
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_model_group.py` & `indico-client-6.7.0a0/tests/integration/queries/test_model_group.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,34 @@
-import pytest
-import time
-import os
 import json
+import os
+import time
 from pathlib import Path
+
+import pytest
+
 from indico.client import IndicoClient
+from indico.errors import IndicoRequestError
+from indico.queries.jobs import JobStatus
 from indico.queries.model_groups import (
+    AddModelGroupComponent,
     GetModelGroup,
-    CreateModelGroup,
-    ModelGroupPredict,
     GetTrainingModelWithProgress,
-    LoadModel,
+    ModelGroupPredict,
+    UpdateModelGroupSettings,
 )
 from indico.queries.model_groups.metrics import (
     AnnotationModelGroupMetrics,
-    ObjectDetectionMetrics,
     GetModelGroupMetrics,
+    ObjectDetectionMetrics,
 )
-from indico.queries.storage import UploadDocument, URL_PREFIX
-from indico.queries.jobs import JobStatus
+from indico.queries.storage import URL_PREFIX, UploadDocument
 from indico.types import Workflow
 from indico.types.dataset import Dataset
+from indico.types.model import Model, ModelOptions, TrainingProgress
 from indico.types.model_group import ModelGroup
-from indico.types.model import Model, TrainingProgress
-from ..data.datasets import (
-    airlines_dataset,
-    too_small_dataset,
-    too_small_workflow,
-    airlines_model_group,
-    cats_dogs_image_dataset,
-    cats_dogs_image_workflow,
-    cats_dogs_modelgroup,
-    org_annotate_model_group,
-    org_annotate_workflow,
-    org_annotate_dataset,
-    cats_dogs_image_workflow,
-    airlines_workflow,
-)
-from indico.errors import IndicoRequestError
-
-
-def test_create_model_group(airlines_dataset: Dataset, airlines_workflow: Workflow):
-    client = IndicoClient()
-
-    name = f"TestCreateModelGroup-{int(time.time())}"
-    after_component = airlines_workflow.component_by_type("INPUT_OCR_EXTRACTION")
-    mg: ModelGroup = client.call(
-        CreateModelGroup(
-            name=name,
-            workflow_id=airlines_workflow.id,
-            dataset_id=airlines_dataset.id,
-            after_component_id=after_component.id,
-            source_column_id=airlines_dataset.datacolumn_by_name("Text").id,
-            labelset_id=airlines_dataset.labelset_by_name("Target_1").id,
-        )
-    )
-
-    assert mg.name == name
 
 
 def test_get_missing_model_group(indico):
     client = IndicoClient()
 
     with pytest.raises(IndicoRequestError):
         client.call(GetModelGroup(id=500000))
@@ -75,98 +44,51 @@
         "max_iter": 2000,
         "lr": 0.1,
         "batch_size": 1,
         "filter_empty": False,
         "test_size": 0.2,
         "use_small_model": False,
     }
-
+    after_component_id = cats_dogs_image_workflow.component_by_type("INPUT_IMAGE").id
     mg: ModelGroup = client.call(
-        CreateModelGroup(
+        AddModelGroupComponent(
             name=name,
-            workflow_id=cats_dogs_image_workflow.id,
-            after_component_id=cats_dogs_image_workflow.component_by_type(
-                "INPUT_IMAGE"
-            ).id,
             dataset_id=cats_dogs_image_dataset.id,
+            after_component_id=after_component_id,
             source_column_id=cats_dogs_image_dataset.datacolumn_by_name("urls").id,
-            labelset_id=cats_dogs_image_dataset.labelset_by_name("label").id,
+            labelset_column_id=cats_dogs_image_dataset.labelset_by_name("label").id,
+            workflow_id=cats_dogs_image_workflow.id,
             model_training_options=model_training_options,
         )
     )
 
-    assert mg.name == name
-
-
-def test_create_model_group_with_wait(
-    indico, airlines_dataset: Dataset, airlines_workflow: Workflow
-):
-    client = IndicoClient()
-
-    name = f"TestCreateModelGroup-{int(time.time())}"
-    after_component = airlines_workflow.component_by_type("INPUT_OCR_EXTRACTION").id
-    mg: ModelGroup = client.call(
-        CreateModelGroup(
-            name=name,
-            dataset_id=airlines_dataset.id,
-            source_column_id=airlines_dataset.datacolumn_by_name("Text").id,
-            labelset_id=airlines_dataset.labelset_by_name("Target_1").id,
-            wait=True,
-            workflow_id=airlines_workflow.id,
-            after_component_id=after_component,
-        )
-    )
-
-    assert mg.name == name
-    assert mg.selected_model.status == "COMPLETE"
-
-
-def test_create_model_group_with_wait_not_enough_data(
-    indico, too_small_dataset: Dataset, too_small_workflow: Workflow
-):
-    client = IndicoClient()
-
-    name = f"TestCreateModelGroup-{int(time.time())}"
-    after_component_id = too_small_workflow.component_by_type("INPUT_OCR_EXTRACTION").id
-    mg: ModelGroup = client.call(
-        CreateModelGroup(
-            name=name,
-            workflow_id=too_small_workflow.id,
-            dataset_id=too_small_dataset.id,
-            source_column_id=too_small_dataset.datacolumn_by_name("Text").id,
-            labelset_id=too_small_dataset.labelset_by_name("Target_1").id,
-            after_component_id=after_component_id,
-            wait=True,
-        )
-    )
-
-    assert mg.name == name
-    assert mg.selected_model.status == "NOT_ENOUGH_DATA"
+    assert mg.model_group_by_name(name) is not None
 
 
 def test_model_group_progress(
     indico, airlines_dataset: Dataset, airlines_workflow: Workflow
 ):
     client = IndicoClient()
 
     name = f"TestCreateModelGroup-{int(time.time())}"
     after_component_id = airlines_workflow.component_by_type("INPUT_OCR_EXTRACTION").id
     mg: ModelGroup = client.call(
-        CreateModelGroup(
+        AddModelGroupComponent(
             name=name,
-            workflow_id=airlines_workflow.id,
             dataset_id=airlines_dataset.id,
-            source_column_id=airlines_dataset.datacolumn_by_name("Text").id,
-            labelset_id=airlines_dataset.labelset_by_name("Target_1").id,
-            wait=False,
             after_component_id=after_component_id,
+            source_column_id=airlines_dataset.datacolumn_by_name("Text").id,
+            labelset_column_id=airlines_dataset.labelset_by_name("Target_1").id,
+            workflow_id=airlines_workflow.id,
         )
     )
     time.sleep(1)
-    model: Model = client.call((GetTrainingModelWithProgress(id=mg.id)))
+    model: Model = client.call(
+        GetTrainingModelWithProgress(id=mg.model_group_by_name(name).id)
+    )
 
     assert type(model) == Model
     assert model.status in ["CREATING", "TRAINING", "COMPLETE"]
     assert type(model.training_progress) == TrainingProgress
     assert model.training_progress.percent_complete < 101.0
 
 
@@ -219,26 +141,14 @@
 
     result = client.call(JobStatus(job.id, wait=True))
 
     assert result.status != "FAILURE"
     assert len(result.result) == 5
 
 
-def test_load_model(indico, airlines_dataset, airlines_model_group):
-    client = IndicoClient()
-
-    status = client.call(
-        LoadModel(
-            model_id=airlines_model_group.selected_model.id,
-        )
-    )
-
-    assert status == "ready"
-
-
 def test_annotation_metrics(
     indico, org_annotate_dataset, org_annotate_workflow, org_annotate_model_group
 ):
     client = IndicoClient()
     result = client.call(
         AnnotationModelGroupMetrics(model_group_id=org_annotate_model_group.id)
     )
@@ -281,7 +191,23 @@
     assert isinstance(result.class_metrics[0].metrics[0].span_type, str)
 
     assert isinstance(result.model_level_metrics[0].span_type, str)
     assert isinstance(result.model_level_metrics[0].micro_f1, float)
     assert isinstance(result.model_level_metrics[0].macro_f1, float)
     assert isinstance(result.model_level_metrics[0].weighted_f1, float)
     assert result.retrain_for_metrics is False
+
+
+def test_update_model_group_settings(indico, org_annotate_model_group):
+    client = IndicoClient()
+    model_training_options = {"use_autolabeled_data": True, "use_partial_data": True}
+    result = client.call(
+        UpdateModelGroupSettings(
+            model_group_id=org_annotate_model_group.id,
+            model_training_options=model_training_options,
+        )
+    )
+    assert isinstance(result, ModelOptions)
+    assert result.model_training_options == {
+        "use_autolabeled_data": True,
+        "use_partial_data": True,
+    }
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_questionnaire.py` & `indico-client-6.7.0a0/tests/integration/queries/test_questionnaire.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-import time
-import pytest
-import typing as t
 import json
+import time
 from pathlib import Path
 
 import pandas as pd
+import pytest
 
 from indico.client import IndicoClient
-from indico.queries import CreateWorkflow
+from indico.errors import IndicoError
+from indico.queries import AddModelGroupComponent, CreateWorkflow
 from indico.queries.datasets import CreateDataset, GetDataset
 from indico.queries.questionnaire import (
-    CreateQuestionaire,
+    AddLabels,
     GetQuestionnaire,
     GetQuestionnaireExamples,
-    AddLabels,
 )
-from indico.errors import IndicoError
-from indico.types import Workflow
-from indico.types.questionnaire import Questionnaire, Example, TargetName
+from indico.types import ModelTaskType, NewLabelsetArguments, Workflow
+from indico.types.questionnaire import Example, Questionnaire
 
 
 @pytest.fixture
 def unlabeled_questionnaire(indico):
     client = IndicoClient()
     datasets_dir = Path(__file__).parents[1] / "data"
     files = [str(datasets_dir / f"pdf{f}.pdf") for f in range(3)]
@@ -31,29 +29,46 @@
     )
     workflow: Workflow = client.call(
         CreateWorkflow(
             name=f"CreateWorkflow-test{int(time.time())}", dataset_id=dataset.id
         )
     )
     after_component_id = workflow.component_by_type("INPUT_OCR_EXTRACTION").id
+    source_col_id = dataset.datacolumn_by_name("text").id
+    classifier_name = f"CreateDatasetTeach-test-{int(time.time())}"
+
+    new_labelset_args = {
+        "datacolumn_id": source_col_id,
+        "name": classifier_name,
+        "num_labelers_required": 1,
+        "task_type": ModelTaskType.CLASSIFICATION,
+        "target_names": ["A", "B", "C"],
+    }
 
     questionnaire = client.call(
-        CreateQuestionaire(
-            name=f"CreateDatasetTeach-test-{int(time.time())}",
+        AddModelGroupComponent(
+            name=classifier_name,
             dataset_id=dataset.id,
-            targets=["A", "B", "C"],
             workflow_id=workflow.id,
+            new_labelset_args=NewLabelsetArguments(**new_labelset_args),
+            source_column_id=source_col_id,
             after_component_id=after_component_id,
         )
     )
-    return {"dataset": dataset, "questionnaire": questionnaire}
+    questionnaire_id = questionnaire.model_group_by_name(
+        classifier_name
+    ).model_group.questionnaire_id
+    return {
+        "dataset": dataset,
+        "questionnaire_id": questionnaire_id,
+    }
 
 
 def test_create_questionnaire_no_labels(unlabeled_questionnaire):
-    assert isinstance(unlabeled_questionnaire["questionnaire"], Questionnaire)
+    assert isinstance(unlabeled_questionnaire["questionnaire_id"], int)
 
 
 def test_create_questionnaire_labeled(indico):
     client = IndicoClient()
     datasets_dir = Path(__file__).parents[1] / "data"
     csv_path = datasets_dir / "staffer_large.csv"
     files = [str(datasets_dir / f"pdf{f}.pdf") for f in range(3)]
@@ -62,77 +77,86 @@
         CreateDataset(name=f"CreateDataset-test-{int(time.time())}", files=files)
     )
     workflow: Workflow = client.call(
         CreateWorkflow(
             name=f"CreateWorkflow-test{int(time.time())}", dataset_id=dataset.id
         )
     )
-    after_component = workflow.component_by_type("INPUT_OCR_EXTRACTION").id
+    source_col_id = dataset.datacolumn_by_name("text").id
+    after_component_id = workflow.component_by_type("INPUT_OCR_EXTRACTION").id
     csv = pd.read_csv(csv_path)
     data = {
         string: json.loads(label) for string, label in zip(csv["text"], csv["labels"])
     }
+    classifier_name = f"CreateDatasetTeach-test-{int(time.time())}"
     targets = list(set(t["label"] for sample in data.values() for t in sample))
+    new_labelset_args = {
+        "datacolumn_id": source_col_id,
+        "name": classifier_name,
+        "num_labelers_required": 1,
+        "task_type": ModelTaskType.CLASSIFICATION,
+        "target_names": targets,
+    }
 
     response = client.call(
-        CreateQuestionaire(
-            name=f"CreateDatasetTeach-test-{int(time.time())}",
+        AddModelGroupComponent(
+            name=classifier_name,
             dataset_id=dataset.id,
-            target_lookup=data,
-            targets=targets,
             workflow_id=workflow.id,
-            after_component_id=after_component,
+            new_labelset_args=NewLabelsetArguments(**new_labelset_args),
+            source_column_id=source_col_id,
+            after_component_id=after_component_id,
         )
     )
 
-    assert isinstance(response, Questionnaire)
+    assert isinstance(response, Workflow)
 
 
 def test_get_nonexistent_questionnaire(indico):
     client = IndicoClient()
     with pytest.raises(IndicoError):
         client.call(GetQuestionnaire(123454321))
 
 
 def test_get_questionnaire(indico, unlabeled_questionnaire):
     client = IndicoClient()
     response = client.call(
-        GetQuestionnaire(unlabeled_questionnaire["questionnaire"].id)
+        GetQuestionnaire(unlabeled_questionnaire["questionnaire_id"])
     )
     assert isinstance(response, Questionnaire)
-    assert response.id == unlabeled_questionnaire["questionnaire"].id
+    assert response.id == unlabeled_questionnaire["questionnaire_id"]
     assert not response.odl
     assert response.num_total_examples == 3
     assert response.num_fully_labeled == 0
 
 
 def test_get_examples(indico, unlabeled_questionnaire):
     client = IndicoClient()
     examples = client.call(
         GetQuestionnaireExamples(
-            questionnaire_id=unlabeled_questionnaire["questionnaire"].id, num_examples=3
+            questionnaire_id=unlabeled_questionnaire["questionnaire_id"], num_examples=3
         )
     )
     assert len(examples) == 3
     for example in examples:
         assert isinstance(example, Example)
         assert isinstance(example.source, str)
         assert isinstance(example.row_index, int)
         assert isinstance(example.datafile_id, int)
 
 
 def test_add_labels(indico, unlabeled_questionnaire):
     client = IndicoClient()
     questionnaire = client.call(
-        GetQuestionnaire(questionnaire_id=unlabeled_questionnaire["questionnaire"].id)
+        GetQuestionnaire(questionnaire_id=unlabeled_questionnaire["questionnaire_id"])
     )
     targets = questionnaire.question.labelset.target_names
     example = client.call(
         GetQuestionnaireExamples(
-            questionnaire_id=unlabeled_questionnaire["questionnaire"].id, num_examples=1
+            questionnaire_id=unlabeled_questionnaire["questionnaire_id"], num_examples=1
         )
     )
     targets = [
         {
             "clsId": next(t.id for t in targets if t.name == "A"),
             "spans": [{"start": 0, "end": 10, "pageNum": 0}],
         }
@@ -151,11 +175,11 @@
         AddLabels(
             labelset_id=labelset_id,
             dataset_id=dataset_id,
             labels=labels,
         )
     )
     questionnaire = client.call(
-        GetQuestionnaire(unlabeled_questionnaire["questionnaire"].id)
+        GetQuestionnaire(unlabeled_questionnaire["questionnaire_id"])
     )
     assert questionnaire.num_total_examples == 3
     assert questionnaire.num_fully_labeled == 1
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_user_metrics.py` & `indico-client-6.7.0a0/tests/integration/queries/test_user_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from datetime import datetime
+
 import pytest
+
 from indico.client import IndicoClient
-from indico.filters import or_, UserMetricsFilter
+from indico.filters import UserMetricsFilter, or_
 from indico.queries import JobStatus, RetrieveStorageObject
-from indico.types.user_metrics import UserSummary
 from indico.queries.usermetrics import (
-    GetUserSummary,
-    GetUserSnapshots,
-    GetUserChangelog,
     GenerateChangelogReport,
+    GetUserChangelog,
+    GetUserSnapshots,
+    GetUserSummary,
 )
-from datetime import datetime
+from indico.types.user_metrics import UserSummary
 
 
 def test_fetch_summary(indico):
     client = IndicoClient()
     user_summary: UserSummary = client.call(GetUserSummary())
     assert user_summary is not None
     assert len(user_summary.app_roles) > 0
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_workflow.py` & `indico-client-6.7.0a0/tests/integration/queries/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import os
+import time
 from datetime import datetime
-from indico.queries.workflow import GetWorkflow
-import pytest
 from pathlib import Path
-import time
+
+import pytest
 
 from indico.client import IndicoClient
 from indico.errors import IndicoError, IndicoInputError, IndicoTimeoutError
 from indico.filters import SubmissionFilter, SubmissionReviewFilter
 from indico.queries import (
+    AddDataToWorkflow,
+    AddFiles,
+    CreateDataset,
+    DeleteWorkflow,
     GetSubmission,
     JobStatus,
     ListSubmissions,
     ListWorkflows,
     RetrieveStorageObject,
     SubmissionResult,
     SubmitReview,
     UpdateSubmission,
     UpdateWorkflowSettings,
     WaitForSubmissions,
     WorkflowSubmission,
     WorkflowSubmissionDetailed,
-    AddDataToWorkflow,
-    AddFiles,
-    CreateDataset,
-    DeleteWorkflow,
 )
-from indico.queries.questionnaire import CreateQuestionaire, GetQuestionnaire
+from indico.queries.questionnaire import GetQuestionnaire
+from indico.queries.workflow import GetWorkflow
 from indico.queries.workflow_components import _AddWorkflowComponent
-from indico.types import ModelGroup
+from indico.types import ModelGroup, ModelTaskType, NewLabelsetArguments
 from indico.types.submission import Submission
 
 from ..data.datasets import *  # noqa
 from ..data.datasets import PUBLIC_URL
 
 
 def test_list_workflows(indico, airlines_dataset, airlines_model_group: ModelGroup):
@@ -82,15 +83,15 @@
     result = client.call(RetrieveStorageObject(result_url.result))
     assert isinstance(result, dict)
     assert result["submission_id"] == submission_id
     assert result["file_version"] == 1
     sub = client.call(GetSubmission(submission_id))
     assert isinstance(sub, Submission)
     assert sub.retrieved is False
-    assert sub.deleted is False
+    assert sub.files_deleted is False
     client.call(UpdateSubmission(submission_id, retrieved=True))
     sub = client.call(GetSubmission(submission_id))
     assert sub.retrieved is True
 
 
 def test_workflow_submission_with_streams(
     indico, airlines_dataset, airlines_model_group: ModelGroup
@@ -270,21 +271,21 @@
     submission_id = submission_ids[0]
     assert submission_id
 
     with pytest.raises(IndicoTimeoutError):
         start = time.time()
         client.call(WaitForSubmissions(submission_id, timeout=1))
         end = time.time()
-        assert(end - start >= 1 and end - start < 2)
+        assert end - start >= 1 and end - start < 2
 
     with pytest.raises(IndicoTimeoutError):
         start = time.time()
         client.call(SubmissionResult(submission_id, "COMPLETE", wait=True, timeout=1))
         end = time.time()
-        assert(end - start >= 1 and end - start < 2)
+        assert end - start >= 1 and end - start < 2
 
 
 def test_list_workflow_submission_retrieved(
     indico, airlines_dataset, airlines_workflow, airlines_model_group: ModelGroup
 ):
     client = IndicoClient()
 
@@ -375,27 +376,28 @@
 def test_workflow_submission_auto_review_v1(
     indico,
     force_complete,
     org_annotate_dataset,
     org_annotate_workflow,
     org_annotate_model_group,
 ):
-
     client = IndicoClient()
 
     wf = client.call(
         UpdateWorkflowSettings(
             org_annotate_workflow.id, enable_review=True, enable_auto_review=True
         )
     )
     assert wf.review_enabled and wf.auto_review_enabled
 
     _file = str(Path(__file__).parents[1]) + "/data/org-sample.pdf"
 
-    sub_ids = client.call(WorkflowSubmission(workflow_id=wf.id, files=[_file], result_version="ONE"))
+    sub_ids = client.call(
+        WorkflowSubmission(workflow_id=wf.id, files=[_file], result_version="ONE")
+    )
     subs = client.call(WaitForSubmissions(sub_ids, timeout=120))
     sub = subs[0]
     assert sub.status == "PENDING_AUTO_REVIEW"
     raw_result = client.call(RetrieveStorageObject(sub.result_file))
     changes = raw_result["results"]["document"]["results"]
     for model, preds in changes.items():
         if isinstance(preds, dict):
@@ -404,41 +406,48 @@
             for pred in preds:
                 pred["accepted"] = True
     job = client.call(
         SubmitReview(sub.id, changes=changes, force_complete=force_complete)
     )
     job = client.call(JobStatus(job.id))
     submission = client.call(WaitForSubmissions([sub.id]))[0]
-    assert submission.status == "COMPLETE" if force_complete else submission.status == "PENDING_REVIEW"
+    assert (
+        submission.status == "COMPLETE"
+        if force_complete
+        else submission.status == "PENDING_REVIEW"
+    )
 
 
 @pytest.mark.parametrize("force_complete", [None, True])
 def test_workflow_submission_auto_review_v3_result(
     indico,
     force_complete,
     org_annotate_dataset,
     org_annotate_workflow,
     org_annotate_model_group,
 ):
-
     client = IndicoClient()
 
     wf = client.call(
         UpdateWorkflowSettings(
             org_annotate_workflow.id, enable_review=True, enable_auto_review=True
         )
     )
     assert wf.review_enabled and wf.auto_review_enabled
 
     _file = str(Path(__file__).parents[1]) + "/data/org-sample.pdf"
 
-    sub_ids = client.call(WorkflowSubmission(workflow_id=wf.id, files=[_file], result_version="THREE"))
+    sub_ids = client.call(
+        WorkflowSubmission(workflow_id=wf.id, files=[_file], result_version="THREE")
+    )
     subs = client.call(WaitForSubmissions(sub_ids, timeout=120))
     sub = subs[0]
-    assert sub.status == "PENDING_AUTO_REVIEW" or sub.status == "COMPLETE" # sub status will be set to COMPLETE if v3 is not supported
+    assert (
+        sub.status == "PENDING_AUTO_REVIEW" or sub.status == "COMPLETE"
+    )  # sub status will be set to COMPLETE if v3 is not supported
     if sub.status == "PENDING_AUTO_REVIEW":
         raw_result = client.call(RetrieveStorageObject(sub.result_file))
         changes = raw_result["submission_results"]
         assert isinstance(changes, list)
         for change in changes:
             # use original values
             change["model_results"] = change["model_results"]["ORIGINAL"]
@@ -450,15 +459,19 @@
                     for pred in preds:
                         pred["accepted"] = True
         job = client.call(
             SubmitReview(sub.id, changes=changes, force_complete=force_complete)
         )
         job = client.call(JobStatus(job.id))
         submission = client.call(WaitForSubmissions([sub.id]))[0]
-        assert submission.status == "COMPLETE" if force_complete else submission.status == "PENDING_REVIEW"
+        assert (
+            submission.status == "COMPLETE"
+            if force_complete
+            else submission.status == "PENDING_REVIEW"
+        )
 
 
 def test_list_workflow_submission_rejected(org_annotate_dataset):
     client = IndicoClient()
     wfs = client.call(ListWorkflows(dataset_ids=[org_annotate_dataset.id]))
     wf = max(wfs, key=lambda w: w.id)
     wf = client.call(
@@ -492,51 +505,73 @@
     )
 
     workflowreq = CreateWorkflow(
         dataset_id=dataset.id, name=f"Update-test-{int(time.time())}"
     )
     wf = client.call(workflowreq)
 
+    after_component_id = wf.component_by_type("INPUT_OCR_EXTRACTION").id
+    source_col_id = dataset.datacolumn_by_name("Text").id
+    classifier_name = f"CreateDatasetTeach-test-{int(time.time())}"
+
+    new_labelset_args = {
+        "datacolumn_id": source_col_id,
+        "name": classifier_name,
+        "num_labelers_required": 1,
+        "task_type": ModelTaskType.CLASSIFICATION,
+        "target_names": ["A", "B", "C"],
+    }
+
     questionnaire = client.call(
-        CreateQuestionaire(
-            name=f"CreateDatasetTeach-test-{int(time.time())}",
+        AddModelGroupComponent(
+            name=classifier_name,
             dataset_id=dataset.id,
-            targets=["A", "B", "C"],
             workflow_id=wf.id,
-            after_component_id=wf.component_by_type("INPUT_OCR_EXTRACTION").id,
+            new_labelset_args=NewLabelsetArguments(**new_labelset_args),
+            source_column_id=source_col_id,
+            after_component_id=after_component_id,
         )
     )
 
     client.call(
         _AddWorkflowComponent(
             after_component_id=wf.component_by_type("OUTPUT_JSON_FORMATTER").id,
             component='{"component_type":"default_output","config":{}}',
             workflow_id=wf.id,
             after_component_link=None,
         )
     )
 
+    questionnaire = client.call(
+        GetQuestionnaire(
+            questionnaire.model_group_by_name(
+                classifier_name
+            ).model_group.questionnaire_id
+        )
+    )
+
     # add data to dataset and process
     dataset = client.call(
         AddFiles(dataset_id=dataset.id, files=[airline_csv], autoprocess=True)
     )
-
     assert dataset.status == "COMPLETE"
+
     return dataset, wf, questionnaire
 
 
 def test_add_data_to_workflow_wait(indico):
     client = IndicoClient()
     _, wf, q1 = _new_dataset_for_updating(client)
 
     wf = client.call(AddDataToWorkflow(wf.id, wait=True))
     assert wf.status == "COMPLETE"
 
     q2 = client.call(GetQuestionnaire(q1.id))
-    # the total num avaliable should double, since we re-add the same data
+
+    # the total num available should double, since we re-add the same data
     assert q1.num_total_examples * 2 == q2.num_total_examples
 
 
 def test_add_data_to_workflow_nowait(indico):
     client = IndicoClient()
     _, wf, _ = _new_dataset_for_updating(client)
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_workflow_component.py` & `indico-client-6.7.0a0/tests/integration/queries/test_workflow_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from indico.client import IndicoClient
-from indico.queries import DeleteWorkflowComponent, GetWorkflow, GetDataset
+from indico.queries import DeleteWorkflowComponent, GetDataset, GetWorkflow
 from indico.queries.workflow_components import AddLinkClassificationComponent
 from indico.types import ModelGroup, ModelTaskType, NewLabelsetArguments
 
 from ..data.datasets import *  # noqa
 
 
 def test_add_mg_new_labelset(indico, org_annotate_dataset):
@@ -51,23 +51,26 @@
             workflow_id=airlines_workflow.id, component_id=mg_comp_id
         )
     )
     assert len(wf.components) == num_components - 1
     assert mg_comp_id not in {c.id for c in wf.components}
     assert len(wf.component_links) == num_links - 1
 
+
 def test_add_many_filtered_classes(indico, org_annotate_dataset):
     client = IndicoClient()
     workflowreq = CreateWorkflow(
         dataset_id=org_annotate_dataset.id, name=f"OrgAnnotate-test-{int(time.time())}"
     )
     wf = client.call(workflowreq)
     mg_name = f"TestAnnotationModelGroup-{int(time.time())}"
     labelset_name = "test-filtered-classes"
-    after_component_id = next(c.id for c in wf.components if c.component_type == "INPUT_OCR_EXTRACTION")
+    after_component_id = next(
+        c.id for c in wf.components if c.component_type == "INPUT_OCR_EXTRACTION"
+    )
     source_column_id = org_annotate_dataset.datacolumn_by_name(
         "News Headlines w/Company Names"
     ).id
     modelgroupreq = AddModelGroupComponent(
         name=mg_name,
         dataset_id=org_annotate_dataset.id,
         workflow_id=wf.id,
@@ -77,41 +80,43 @@
             name=labelset_name,
             task_type=ModelTaskType.CLASSIFICATION_MULTIPLE,
             target_names=["type 1", "type 2", "type 3"],
             datacolumn_id=source_column_id,
         ),
     )
     wf = client.call(modelgroupreq)
-    mg = next(c for c in wf.components if c.component_type == 'MODEL_GROUP')
+    mg = next(c for c in wf.components if c.component_type == "MODEL_GROUP")
     after_component_id = mg.id
-    
-    classes_to_filter = [
-            ["type 1"],
-            ["type 3"]
-        ]
+
+    classes_to_filter = [["type 1"], ["type 3"]]
     filtered = AddLinkClassificationComponent(
-            workflow_id=wf.id,
-            after_component_id=after_component_id,
-            model_group_id=mg.model_group.id,
-            filtered_classes=classes_to_filter,
-            labels="actual",
-        )
+        workflow_id=wf.id,
+        after_component_id=after_component_id,
+        model_group_id=mg.model_group.id,
+        filtered_classes=classes_to_filter,
+        labels="actual",
+    )
     wf = client.call(filtered)
-    new_component = next(c.id for c in wf.components if c.component_type == "LINK_CLASSIFICATION_MODEL")
+    new_component = next(
+        c.id for c in wf.components if c.component_type == "LINK_CLASSIFICATION_MODEL"
+    )
     assert new_component is not None
 
+
 def test_add_single_filtered_class(indico, org_annotate_dataset):
     client = IndicoClient()
     workflowreq = CreateWorkflow(
         dataset_id=org_annotate_dataset.id, name=f"OrgAnnotate-test-{int(time.time())}"
     )
     wf = client.call(workflowreq)
     mg_name = f"TestAnnotationModelGroup-{int(time.time())}"
     labelset_name = "test-filtered-classes"
-    after_component_id = next(c.id for c in wf.components if c.component_type == "INPUT_OCR_EXTRACTION")
+    after_component_id = next(
+        c.id for c in wf.components if c.component_type == "INPUT_OCR_EXTRACTION"
+    )
     source_column_id = org_annotate_dataset.datacolumn_by_name(
         "News Headlines w/Company Names"
     ).id
     modelgroupreq = AddModelGroupComponent(
         name=mg_name,
         dataset_id=org_annotate_dataset.id,
         workflow_id=wf.id,
@@ -121,41 +126,43 @@
             name=labelset_name,
             task_type=ModelTaskType.CLASSIFICATION_MULTIPLE,
             target_names=["type 1", "type 2", "type 3"],
             datacolumn_id=source_column_id,
         ),
     )
     wf = client.call(modelgroupreq)
-    mg = next(c for c in wf.components if c.component_type == 'MODEL_GROUP')
+    mg = next(c for c in wf.components if c.component_type == "MODEL_GROUP")
     after_component_id = mg.id
-    
-    classes_to_filter = [
-            ["type 1"]
-        ]
+
+    classes_to_filter = [["type 1"]]
     filtered = AddLinkClassificationComponent(
-            workflow_id=wf.id,
-            after_component_id=after_component_id,
-            model_group_id=mg.model_group.id,
-            filtered_classes=classes_to_filter,
-            labels="actual",
-        )
+        workflow_id=wf.id,
+        after_component_id=after_component_id,
+        model_group_id=mg.model_group.id,
+        filtered_classes=classes_to_filter,
+        labels="actual",
+    )
     wf = client.call(filtered)
-    new_component =  next(c.id for c in wf.components if c.component_type == 'LINK_CLASSIFICATION_MODEL')
+    new_component = next(
+        c.id for c in wf.components if c.component_type == "LINK_CLASSIFICATION_MODEL"
+    )
     assert new_component is not None
 
 
 def test_add_bad_syntax_filtered_classes(indico, org_annotate_dataset):
     client = IndicoClient()
     workflowreq = CreateWorkflow(
         dataset_id=org_annotate_dataset.id, name=f"OrgAnnotate-test-{int(time.time())}"
     )
     wf = client.call(workflowreq)
     mg_name = f"TestAnnotationModelGroup-{int(time.time())}"
     labelset_name = "test-filtered-classes"
-    after_component_id = next(c.id for c in wf.components if c.component_type == "INPUT_OCR_EXTRACTION")
+    after_component_id = next(
+        c.id for c in wf.components if c.component_type == "INPUT_OCR_EXTRACTION"
+    )
     source_column_id = org_annotate_dataset.datacolumn_by_name(
         "News Headlines w/Company Names"
     ).id
     modelgroupreq = AddModelGroupComponent(
         name=mg_name,
         dataset_id=org_annotate_dataset.id,
         workflow_id=wf.id,
@@ -165,24 +172,20 @@
             name=labelset_name,
             task_type=ModelTaskType.CLASSIFICATION_MULTIPLE,
             target_names=["type 1", "type 2", "type 3"],
             datacolumn_id=source_column_id,
         ),
     )
     wf = client.call(modelgroupreq)
-    mg = next(c for c in wf.components if c.component_type == 'MODEL_GROUP')
+    mg = next(c for c in wf.components if c.component_type == "MODEL_GROUP")
     after_component_id = mg.id
-    
-    classes_to_filter = [
-            ["type 1"],
-            ["type 2"]
-        ]
+
+    classes_to_filter = [["type 1"], ["type 2"]]
     filtered = AddLinkClassificationComponent(
-            workflow_id=wf.id,
-            after_component_id=after_component_id,
-            model_group_id=6108,
-            filtered_classes=[classes_to_filter],
-            labels="actual",
-        )
+        workflow_id=wf.id,
+        after_component_id=after_component_id,
+        model_group_id=6108,
+        filtered_classes=[classes_to_filter],
+        labels="actual",
+    )
     with pytest.raises(Exception):
         wf = client.call(filtered)
-
```

### Comparing `indico-client-6.1.0a1/tests/integration/queries/test_workflow_metrics.py` & `indico-client-6.7.0a0/tests/integration/queries/test_workflow_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from pathlib import Path
 import time
+from datetime import datetime
+from pathlib import Path
 from typing import List
 
 import pytest
+
 from indico.client import IndicoClient
 from indico.queries import (
     JobStatus,
     RetrieveStorageObject,
+    SubmitReview,
     UpdateWorkflowSettings,
-    WorkflowSubmission,
     WaitForSubmissions,
-    SubmitReview,
+    WorkflowSubmission,
 )
-
-from indico.types.workflow_metrics import WorkflowMetrics, WorkflowMetricsOptions
 from indico.queries.workflow_metrics import GetWorkflowMetrics
-from datetime import datetime
+from indico.types.workflow_metrics import WorkflowMetrics, WorkflowMetricsOptions
+
 from ..data.datasets import *  # noqa
 from ..data.datasets import PUBLIC_URL
-import time
 
 
 @pytest.fixture
-def workflow(indico, org_annotate_dataset, org_annotate_workflow, org_annotate_model_group):
+def workflow(
+    indico, org_annotate_dataset, org_annotate_workflow, org_annotate_model_group
+):
     client = IndicoClient()
 
     wf = client.call(
-        UpdateWorkflowSettings(org_annotate_workflow.id, enable_review=True, enable_auto_review=True)
+        UpdateWorkflowSettings(
+            org_annotate_workflow.id, enable_review=True, enable_auto_review=True
+        )
     )
     assert wf.review_enabled and wf.auto_review_enabled
 
     _file = str(Path(__file__).parents[1]) + "/data/org-sample.pdf"
 
     sub_ids = client.call(WorkflowSubmission(workflow_id=wf.id, files=[_file]))
     subs = client.call(WaitForSubmissions(sub_ids, timeout=900))
```

### Comparing `indico-client-6.1.0a1/tests/integration/test_base_aioclient.py` & `indico-client-6.7.0a0/tests/integration/test_base_aioclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 
 from indico.client import AsyncIndicoClient, IndicoConfig
-from indico.client.request import HTTPRequest, HTTPMethod, GraphQLRequest
+from indico.client.request import GraphQLRequest, HTTPMethod, HTTPRequest
 from indico.errors import IndicoAuthenticationFailed
 
-
 pytestmark = pytest.mark.asyncio(scope="module")
 
 
 async def test_http_request(indico):
     async with AsyncIndicoClient() as client:
         response = await client.call(
             HTTPRequest(method=HTTPMethod.GET, path="/auth/users/details")
```

### Comparing `indico-client-6.1.0a1/tests/integration/test_base_client.py` & `indico-client-6.7.0a0/tests/integration/test_base_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from indico.client import IndicoClient, IndicoConfig
-from indico.client.request import HTTPRequest, HTTPMethod, GraphQLRequest
+from indico.client.request import GraphQLRequest, HTTPMethod, HTTPRequest
 from indico.errors import IndicoAuthenticationFailed
 from tests.integration.data.datasets import org_annotate_dataset
 
 
 def test_http_request(indico):
     client = IndicoClient()
     response = client.call(
```

### Comparing `indico-client-6.1.0a1/tests/unit/test_filters.py` & `indico-client-6.7.0a0/tests/unit/test_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import pytest
 from datetime import datetime
 
+import pytest
+
 from indico.errors import IndicoInputError
-from indico.filters import Filter, SubmissionFilter, and_, or_, DocumentReportFilter
+from indico.filters import DocumentReportFilter, Filter, SubmissionFilter, and_, or_
 
 
 def test_filter():
     with pytest.raises(IndicoInputError):
         Filter()
     f = Filter(key="value")
     assert dict(f) == {"key": "value"}
@@ -27,15 +28,15 @@
     assert dict(f) == {"status": "COMPLETE"}
 
 
 def test_doc_report_filter():
     todays_date = datetime.now().strftime("%Y-%m-%d")
 
     filter_opts = DocumentReportFilter(created_at_start_date=datetime(2021, 7, 1))
-    assert filter_opts['createdAt']['to'] == todays_date
+    assert filter_opts["createdAt"]["to"] == todays_date
     with pytest.raises(IndicoInputError):
         DocumentReportFilter(created_at_end_date=datetime.now())
 
     filter_opts = DocumentReportFilter(updated_at_start_date=datetime(2021, 8, 1))
-    assert filter_opts['updatedAt']['to'] == todays_date
+    assert filter_opts["updatedAt"]["to"] == todays_date
     with pytest.raises(IndicoInputError):
         DocumentReportFilter(updated_at_end_date=datetime.now())
```

### Comparing `indico-client-6.1.0a1/versioneer.py` & `indico-client-6.7.0a0/versioneer.py`

 * *Files identical despite different names*

