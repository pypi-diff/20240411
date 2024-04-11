# Comparing `tmp/dyff-storage-0.5.0.tar.gz` & `tmp/dyff-storage-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-storage-0.5.0.tar", last modified: Tue Apr  9 20:48:18 2024, max compression
+gzip compressed data, was "dyff-storage-0.5.1.tar", last modified: Thu Apr 11 02:32:43 2024, max compression
```

## Comparing `dyff-storage-0.5.0.tar` & `dyff-storage-0.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.902431 dyff-storage-0.5.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.909431 dyff-storage-0.5.0/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.909431 dyff-storage-0.5.0/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.910431 dyff-storage-0.5.0/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     5781 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.911431 dyff-storage-0.5.0/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.911431 dyff-storage-0.5.0/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8770 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.912431 dyff-storage-0.5.0/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.912431 dyff-storage-0.5.0/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    20262 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.913431 dyff-storage-0.5.0/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13410 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2088 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.914431 dyff-storage-0.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.386708 dyff-storage-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-04-11 02:32:43.385707 dyff-storage-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.374708 dyff-storage-0.5.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.380708 dyff-storage-0.5.1/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.380708 dyff-storage-0.5.1/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.381708 dyff-storage-0.5.1/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.381708 dyff-storage-0.5.1/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.382708 dyff-storage-0.5.1/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.382708 dyff-storage-0.5.1/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.383708 dyff-storage-0.5.1/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    20365 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.383708 dyff-storage-0.5.1/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13410 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.385707 dyff-storage-0.5.1/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-11 02:32:43.000000 dyff-storage-0.5.1/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:32:43.386708 dyff-storage-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:32:43.385707 dyff-storage-0.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-11 02:32:37.000000 dyff-storage-0.5.1/tests/test_import.py
```

### Comparing `dyff-storage-0.5.0/.gitignore` & `dyff-storage-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/.gitlab-ci.yml` & `dyff-storage-0.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/.licenserc.yaml` & `dyff-storage-0.5.1/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/.pre-commit-config.yaml` & `dyff-storage-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/.secrets.baseline` & `dyff-storage-0.5.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/CODE_OF_CONDUCT.md` & `dyff-storage-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/LICENSE` & `dyff-storage-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/PKG-INFO` & `dyff-storage-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff-storage-0.5.0/README.md` & `dyff-storage-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/__init__.py` & `dyff-storage-0.5.1/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/base/auth.py` & `dyff-storage-0.5.1/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/base/command.py` & `dyff-storage-0.5.1/dyff/storage/backend/base/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 import abc
 from typing import Optional
 
 from dyff.schema.platform import (
-    Analysis,
     Audit,
     Dataset,
     DataSource,
     EntityStatus,
     EntityStatusReason,
     Evaluation,
     InferenceService,
     InferenceSession,
     Labeled,
+    Measurement,
     Method,
     Model,
     Module,
     Report,
+    SafetyCase,
 )
 
 
 class CommandBackend(abc.ABC):
     @abc.abstractmethod
     def update_status(
         self, id: str, *, status: str, reason: Optional[str] = None
@@ -42,26 +43,14 @@
         :param id: The ID of the entity to update.
         :type id: str
         :param labels: The labels to update.
         :type labels: Labeled
         """
 
     @abc.abstractmethod
-    def create_analysis(self, spec: Analysis) -> Analysis:
-        """Create a new Analysis entity in the system.
-
-        Parameters:
-          spec: Specification of the Analysis. The system fields of the spec
-            such as ``.id`` must be **unset**.
-
-        Returns:
-          A copy of ``spec`` with all system fields set.
-        """
-
-    @abc.abstractmethod
     def create_audit(self, spec: Audit) -> Audit:
         """Create a new Audit entity in the system.
 
         Parameters:
           spec: Specification of the Audit. The system fields of the spec
             such as ``.id`` must be **unset**.
 
@@ -126,14 +115,26 @@
             such as ``.id`` must be **unset**.
 
         Returns:
           A copy of ``spec`` with all system fields set.
         """
 
     @abc.abstractmethod
+    def create_measurement(self, spec: Measurement) -> Measurement:
+        """Create a new Measurement entity in the system.
+
+        Parameters:
+          spec: Specification of the Measurement. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+
+    @abc.abstractmethod
     def create_method(self, spec: Method) -> Method:
         """Create a new Method entity in the system.
 
         Parameters:
           spec: Specification of the Method. The system fields of the spec
             such as ``.id`` must be **unset**.
 
@@ -173,14 +174,26 @@
           spec: Specification of the Report. The system fields of the spec
             such as ``.id`` must be **unset**.
 
         Returns:
           A copy of ``spec`` with all system fields set.
         """
 
+    @abc.abstractmethod
+    def create_safetycase(self, spec: SafetyCase) -> SafetyCase:
+        """Create a new SafetyCase entity in the system.
+
+        Parameters:
+          spec: Specification of the SafetyCase. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+
     def terminate_workflow(self, id: str) -> None:
         """Terminate a running workflow.
 
         :param id: The ID of the workflow.
         :type id: str
         """
         self.update_status(
```

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/base/query.py` & `dyff-storage-0.5.1/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/base/storage.py` & `dyff-storage-0.5.1/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/gcloud/storage.py` & `dyff-storage-0.5.1/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/kafka/command.py` & `dyff-storage-0.5.1/dyff/storage/backend/kafka/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 from typing import Optional, TypeVar
 
 import pydantic
 from confluent_kafka import Producer
 
 from dyff.schema import ids
 from dyff.schema.platform import (
-    Analysis,
     Audit,
     Dataset,
     DataSource,
     DyffEntity,
     DyffEntityType,
     EntityStatus,
     EntityStatusReason,
     Evaluation,
     InferenceService,
     InferenceSession,
     Labeled,
+    Measurement,
     Method,
     Model,
     Module,
     Report,
+    SafetyCase,
 )
 from dyff.storage import timestamp
 from dyff.storage.config import config
 from dyff.storage.typing import YAMLObject
 
 from ..base.command import CommandBackend
 
@@ -139,26 +140,14 @@
         :type labels: Labeled
         """
         update = labels.dict()
         self._kafka_producer.produce(
             topic=self.events_topic, value=serialize_value(update), key=serialize_id(id)
         )
 
-    def create_analysis(self, spec: Analysis) -> Analysis:
-        """Create a new Analysis entity in the system.
-
-        Parameters:
-          spec: Specification of the Analysis. The system fields of the spec
-            such as ``.id`` must be **unset**.
-
-        Returns:
-          A copy of ``spec`` with all system fields set.
-        """
-        return self._produce_create_event(spec)
-
     def create_audit(self, spec: Audit) -> Audit:
         """Create a new Audit entity in the system.
 
         Parameters:
           spec: Specification of the Audit. The system fields of the spec
             such as ``.id`` must be **unset**.
 
@@ -223,14 +212,26 @@
             such as ``.id`` must be **unset**.
 
         Returns:
           A copy of ``spec`` with all system fields set.
         """
         return self._produce_create_event(spec)
 
+    def create_measurement(self, spec: Measurement) -> Measurement:
+        """Create a new Measurement entity in the system.
+
+        Parameters:
+          spec: Specification of the Measurement. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+        return self._produce_create_event(spec)
+
     def create_method(self, spec: Method) -> Method:
         """Create a new Method entity in the system.
 
         Parameters:
           spec: Specification of the Method. The system fields of the spec
             such as ``.id`` must be **unset**.
 
@@ -270,7 +271,19 @@
           spec: Specification of the Report. The system fields of the spec
             such as ``.id`` must be **unset**.
 
         Returns:
           A copy of ``spec`` with all system fields set.
         """
         return self._produce_create_event(spec)
+
+    def create_safetycase(self, spec: SafetyCase) -> SafetyCase:
+        """Create a new SafetyCase entity in the system.
+
+        Parameters:
+          spec: Specification of the SafetyCase. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+        return self._produce_create_event(spec)
```

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/mock/command.py` & `dyff-storage-0.5.1/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/mongodb/auth.py` & `dyff-storage-0.5.1/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/mongodb/query.py` & `dyff-storage-0.5.1/dyff/storage/backend/mongodb/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,23 @@
                 for label_key, label_value in labeled.labels.items():
                     mongo_conjunction.append(
                         {k: {"$elemMatch": {"key": label_key, "value": label_value}}}
                     )
             # TODO:
             # elif k == "annotations":
             #     pass
+            elif k == "inputsAnyOf":
+                # This is a special query for Analysis-related entities. It
+                # selects entities that reference any of the listed IDs in
+                # their .inputs field.
+                entity_list = v.split(",")
+                for entity in entity_list:
+                    mongo_conjunction.append(
+                        {"inputs": {"$elemMatch": {"key": "entity", "value": entity}}}
+                    )
             elif isinstance(v, list):
                 mongo_conjunction.append({k: {"$in": list(v)}})
             else:
                 mongo_conjunction.append({k: v})
 
         query = {"$and": mongo_conjunction} if mongo_conjunction else {}
         print(f"query: {query}")
@@ -363,23 +372,16 @@
           whitelist: The set of accounts and entities that the caller has
             been granted access to.
           **query: Equality constraints on fields of the Measurement entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
         qdict = query.dict()
-        self._rename_query_key(qdict, "dataset", "dataset.id")
-        self._rename_query_key(qdict, "datasetName", "dataset.name")
-        self._rename_query_key(qdict, "evaluation", "evaluation.id")
-        self._rename_query_key(qdict, "inferenceService", "inferenceService.id")
-        self._rename_query_key(qdict, "inferenceServiceName", "inferenceService.name")
         self._rename_query_key(qdict, "method", "method.id")
         self._rename_query_key(qdict, "methodName", "method.name")
-        self._rename_query_key(qdict, "model", "model.id")
-        self._rename_query_key(qdict, "modelName", "model.name")
         results = self._query_entities(Entities.Measurement, whitelist, qdict)
         return [Measurement.parse_obj(result) for result in results]
 
     def get_method(self, id: str) -> Optional[Method]:
         """Retrieve a Method entity.
 
         Parameters:
@@ -513,9 +515,11 @@
           whitelist: The set of accounts and entities that the caller has
             been granted access to.
           **query: Equality constraints on fields of the SafetyCase entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
         qdict = query.dict()
+        self._rename_query_key(qdict, "method", "method.id")
+        self._rename_query_key(qdict, "methodName", "method.name")
         results = self._query_entities(Entities.SafetyCase, whitelist, qdict)
         return [SafetyCase.parse_obj(result) for result in results]
```

### Comparing `dyff-storage-0.5.0/dyff/storage/backend/s3/storage.py` & `dyff-storage-0.5.1/dyff/storage/backend/s3/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/config.py` & `dyff-storage-0.5.1/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/paths.py` & `dyff-storage-0.5.1/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff/storage/timestamp.py` & `dyff-storage-0.5.1/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/dyff_storage.egg-info/PKG-INFO` & `dyff-storage-0.5.1/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff-storage-0.5.0/dyff_storage.egg-info/SOURCES.txt` & `dyff-storage-0.5.1/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/makefile` & `dyff-storage-0.5.1/makefile`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/pyproject.toml` & `dyff-storage-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.5.0/tests/test_import.py` & `dyff-storage-0.5.1/tests/test_import.py`

 * *Files identical despite different names*

