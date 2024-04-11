# Comparing `tmp/dyff-audit-0.2.0.tar.gz` & `tmp/dyff-audit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-audit-0.2.0.tar", last modified: Mon Apr  8 22:16:12 2024, max compression
+gzip compressed data, was "dyff-audit-0.2.1.tar", last modified: Thu Apr 11 17:06:06 2024, max compression
```

## Comparing `dyff-audit-0.2.0.tar` & `dyff-audit-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.846786 dyff-audit-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3438 2024-04-08 22:16:12.845786 dyff-audit-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.836786 dyff-audit-0.2.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.841786 dyff-audit-0.2.0/dyff/audit/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4602 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.841786 dyff-audit-0.2.0/dyff/audit/data/
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/data/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.842786 dyff-audit-0.2.0/dyff/audit/metrics/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/metrics/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/metrics/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.843786 dyff-audit-0.2.0/dyff/audit/scoring/
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/scoring/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/scoring/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/scoring/example.py
--rw-rw-rw-   0 root         (0) root         (0)    11999 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/scoring/text.py
--rw-rw-rw-   0 root         (0) root         (0)     5756 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/dyff/audit/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.845786 dyff-audit-0.2.0/dyff_audit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3438 2024-04-08 22:16:12.000000 dyff-audit-0.2.0/dyff_audit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      715 2024-04-08 22:16:12.000000 dyff-audit-0.2.0/dyff_audit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 22:16:12.000000 dyff-audit-0.2.0/dyff_audit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-08 22:16:12.000000 dyff-audit-0.2.0/dyff_audit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 22:16:12.000000 dyff-audit-0.2.0/dyff_audit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 22:16:12.846786 dyff-audit-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:16:12.845786 dyff-audit-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-08 22:16:06.000000 dyff-audit-0.2.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.321524 dyff-audit-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3438 2024-04-11 17:06:06.320523 dyff-audit-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.312523 dyff-audit-0.2.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.316523 dyff-audit-0.2.1/dyff/audit/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6569 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.317523 dyff-audit-0.2.1/dyff/audit/data/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/data/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.317523 dyff-audit-0.2.1/dyff/audit/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/metrics/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/metrics/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.318524 dyff-audit-0.2.1/dyff/audit/scoring/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/scoring/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/scoring/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/scoring/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    11999 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/scoring/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     5756 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/dyff/audit/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.320523 dyff-audit-0.2.1/dyff_audit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3438 2024-04-11 17:06:06.000000 dyff-audit-0.2.1/dyff_audit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      715 2024-04-11 17:06:06.000000 dyff-audit-0.2.1/dyff_audit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:06:06.000000 dyff-audit-0.2.1/dyff_audit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-11 17:06:06.000000 dyff-audit-0.2.1/dyff_audit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-11 17:06:06.000000 dyff-audit-0.2.1/dyff_audit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 17:06:06.321524 dyff-audit-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:06:06.320523 dyff-audit-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-11 17:06:00.000000 dyff-audit-0.2.1/tests/test_import.py
```

### Comparing `dyff-audit-0.2.0/.gitlab-ci.yml` & `dyff-audit-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/.pre-commit-config.yaml` & `dyff-audit-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/.secrets.baseline` & `dyff-audit-0.2.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/CODE_OF_CONDUCT.md` & `dyff-audit-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/LICENSE` & `dyff-audit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/PKG-INFO` & `dyff-audit-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-audit-0.2.0/README.md` & `dyff-audit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/data/text.py` & `dyff-audit-0.2.1/dyff/audit/data/text.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/metrics/base.py` & `dyff-audit-0.2.1/dyff/audit/metrics/base.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/metrics/text.py` & `dyff-audit-0.2.1/dyff/audit/metrics/text.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/scoring/base.py` & `dyff-audit-0.2.1/dyff/audit/scoring/base.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/scoring/classification.py` & `dyff-audit-0.2.1/dyff/audit/scoring/classification.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/scoring/example.py` & `dyff-audit-0.2.1/dyff/audit/scoring/example.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/scoring/text.py` & `dyff-audit-0.2.1/dyff/audit/scoring/text.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff/audit/workflows.py` & `dyff-audit-0.2.1/dyff/audit/workflows.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/dyff_audit.egg-info/PKG-INFO` & `dyff-audit-0.2.1/dyff_audit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-audit-0.2.0/dyff_audit.egg-info/SOURCES.txt` & `dyff-audit-0.2.1/dyff_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/makefile` & `dyff-audit-0.2.1/makefile`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/pyproject.toml` & `dyff-audit-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.2.0/tests/test_import.py` & `dyff-audit-0.2.1/tests/test_import.py`

 * *Files identical despite different names*

