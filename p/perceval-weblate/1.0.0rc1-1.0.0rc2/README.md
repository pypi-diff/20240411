# Comparing `tmp/perceval_weblate-1.0.0rc1.tar.gz` & `tmp/perceval_weblate-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_weblate-1.0.0rc1.tar", max compression
+gzip compressed data, was "perceval_weblate-1.0.0rc2.tar", max compression
```

## Comparing `perceval_weblate-1.0.0rc1.tar` & `perceval_weblate-1.0.0rc2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      196 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     2653 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/NEWS
--rw-r--r--   0        0        0     2187 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/README.md
--rw-r--r--   0        0        0        0 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/perceval/backends/weblate/__init__.py
--rw-r--r--   0        0        0       91 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/perceval/backends/weblate/_version.py
--rw-r--r--   0        0        0    14043 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/perceval/backends/weblate/weblate.py
--rw-r--r--   0        0        0     1403 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     1832 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/base.py
--rw-r--r--   0        0        0      981 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes.json
--rw-r--r--   0        0        0     1922 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_archived.json
--rw-r--r--   0        0        0     8490 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_expected.json
--rw-r--r--   0        0        0     1086 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_page_2.json
--rw-r--r--   0        0        0      719 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_unit.json
--rw-r--r--   0        0        0      359 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_user_1.json
--rw-r--r--   0        0        0      354 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_user_2.json
--rw-r--r--   0        0        0       31 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_user_no_permission.json
--rw-r--r--   0        0        0     1007 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/run_tests.py
--rw-r--r--   0        0        0    16895 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/test_weblate.py
--rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 perceval_weblate-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      196 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     2653 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/NEWS
+-rw-r--r--   0        0        0     2187 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/perceval/backends/weblate/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/perceval/backends/weblate/_version.py
+-rw-r--r--   0        0        0    14043 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/perceval/backends/weblate/weblate.py
+-rw-r--r--   0        0        0     1403 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     1832 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/base.py
+-rw-r--r--   0        0        0      981 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes.json
+-rw-r--r--   0        0        0     1922 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes_archived.json
+-rw-r--r--   0        0        0     8490 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes_expected.json
+-rw-r--r--   0        0        0     1086 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes_page_2.json
+-rw-r--r--   0        0        0      719 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_unit.json
+-rw-r--r--   0        0        0      359 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_user_1.json
+-rw-r--r--   0        0        0      354 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_user_2.json
+-rw-r--r--   0        0        0       31 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_user_no_permission.json
+-rw-r--r--   0        0        0     1007 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/run_tests.py
+-rw-r--r--   0        0        0    16895 2024-04-11 10:48:53.992782 perceval_weblate-1.0.0rc2/tests/test_weblate.py
+-rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 perceval_weblate-1.0.0rc2/PKG-INFO
```

### Comparing `perceval_weblate-1.0.0rc1/LICENSE` & `perceval_weblate-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/NEWS` & `perceval_weblate-1.0.0rc2/NEWS`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/README.md` & `perceval_weblate-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/perceval/backends/weblate/weblate.py` & `perceval_weblate-1.0.0rc2/perceval/backends/weblate/weblate.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/pyproject.toml` & `perceval_weblate-1.0.0rc2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-weblate"
-version = "1.0.0-rc.1"
+version = "1.0.0-rc.2"
 description = "Bundle of Perceval backends for Weblate."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_weblate-1.0.0rc1/tests/base.py` & `perceval_weblate-1.0.0rc2/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes.json` & `perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_archived.json` & `perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes_archived.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_expected.json` & `perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes_expected.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_page_2.json` & `perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_changes_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_unit.json` & `perceval_weblate-1.0.0rc2/tests/data/weblate/weblate_unit.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/run_tests.py` & `perceval_weblate-1.0.0rc2/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/tests/test_weblate.py` & `perceval_weblate-1.0.0rc2/tests/test_weblate.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-1.0.0rc1/PKG-INFO` & `perceval_weblate-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-weblate
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Bundle of Perceval backends for Weblate.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

