# Comparing `tmp/scmallet-0.0.2.tar.gz` & `tmp/scmallet-0.0.3.tar.gz`

## Comparing `scmallet-0.0.2.tar` & `scmallet-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.2/.codecov.yaml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.0.2/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.0.2/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/__init__.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/binarize.py
--rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/eval_model.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/infer.py
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/input.py
--rw-r--r--   0        0        0    20237 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/mallet.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/topic_metrices.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.0.2/tests/test_basic.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.0.2/LICENSE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 scmallet-0.0.2/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 scmallet-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.3/.codecov.yaml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.0.3/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.0.3/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/__init__.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/binarize.py
+-rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/eval_model.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/infer.py
+-rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/input.py
+-rw-r--r--   0        0        0    26591 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/mallet.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/topic_metrices.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.0.3/tests/test_basic.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.0.3/LICENSE
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 scmallet-0.0.3/README.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 scmallet-0.0.3/PKG-INFO
```

### Comparing `scmallet-0.0.2/.cruft.json` & `scmallet-0.0.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/.pre-commit-config.yaml` & `scmallet-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `scmallet-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/.github/workflows/build.yaml` & `scmallet-0.0.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/.github/workflows/release.yaml` & `scmallet-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/.github/workflows/test.yaml` & `scmallet-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/src/scmallet/binarize.py` & `scmallet-0.0.3/src/scmallet/binarize.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/src/scmallet/eval_model.py` & `scmallet-0.0.3/src/scmallet/eval_model.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/src/scmallet/infer.py` & `scmallet-0.0.3/src/scmallet/infer.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/src/scmallet/input.py` & `scmallet-0.0.3/src/scmallet/input.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/src/scmallet/topic_metrices.py` & `scmallet-0.0.3/src/scmallet/topic_metrices.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/src/scmallet/utils.py` & `scmallet-0.0.3/src/scmallet/utils.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/LICENSE` & `scmallet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/README.md` & `scmallet-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/pyproject.toml` & `scmallet-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.2/PKG-INFO` & `scmallet-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scmallet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper of MALLET for LDA analysis on single-cell data
 Project-URL: Source, https://github.com/lhqing/scmallet
 Project-URL: Home-page, https://github.com/lhqing/scmallet
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanqingliu@fas.harvard.edu>
 License: MIT License
```

