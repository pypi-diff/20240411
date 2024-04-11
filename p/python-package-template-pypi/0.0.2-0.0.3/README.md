# Comparing `tmp/python_package_template_pypi-0.0.2.tar.gz` & `tmp/python_package_template_pypi-0.0.3.tar.gz`

## Comparing `python_package_template_pypi-0.0.2.tar` & `python_package_template_pypi-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,26 @@
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/readthedocs.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/.github/CODEOWNERS
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/docs/add_five.rst
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/docs/conf.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/docs/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/src/python_package_template/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/src/python_package_template/main.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/tests/main_test.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/LICENSE
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/README.md
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/readthedocs.yml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/ruff.toml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/tox.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/add_five.rst
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/src/python_package_template/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/src/python_package_template/main.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/tests/main_test.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/README.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/hatch.toml
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/PKG-INFO
```

### Comparing `python_package_template_pypi-0.0.2/.pre-commit-config.yaml` & `python_package_template_pypi-0.0.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # See https://pre-commit.com/hooks.html for more hooks
 
 # exclude: ""
 
 # pre-commit
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
         args: [--maxkb=2000]
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: name-tests-test
       - id: trailing-whitespace
 
   # ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.1
+    rev: v0.3.5
     hooks:
       # Ruff linting
       - id: ruff
         args: [--line-length=120]
       # Ruff formatting
       - id: ruff-format
```

### Comparing `python_package_template_pypi-0.0.2/.github/workflows/release.yml` & `python_package_template_pypi-0.0.3/.github/workflows/release.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 name: release
 on:
   push:
     tags:
       - "*"
 
 jobs:
@@ -32,7 +33,15 @@
 
       - name: Build the package.
         run: >
           python -m build
 
       - name: Publish the package.
         uses: pypa/gh-action-pypi-publish@release/v1
+
+  gh-pages:
+    permissions:
+      contents: write
+
+    uses: daniel-mizsak/workflows/.github/workflows/gh-pages.yml@main
+    with:
+      python-version: "3.12"
```

### Comparing `python_package_template_pypi-0.0.2/docs/conf.py` & `python_package_template_pypi-0.0.3/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Configuration file for the Sphinx documentation builder.
 
 For the full list of built-in configuration values, see the documentation:
 https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 Built docs locally with:
-sphinx-build -b html docs/source/ docs/build/html
+sphinx-build -b html docs docs/build/html
 
 @author "Daniel Mizsak" <info@pythonvilag.hu>
 """
 
 from datetime import UTC, datetime
 
 from python_package_template import __version__
```

### Comparing `python_package_template_pypi-0.0.2/LICENSE` & `python_package_template_pypi-0.0.3/LICENSE`

 * *Files identical despite different names*

