# Comparing `tmp/safe-mol-0.1.5.tar.gz` & `tmp/safe-mol-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-mol-0.1.5.tar", last modified: Sun Jan 14 00:22:21 2024, max compression
+gzip compressed data, was "safe-mol-0.1.6.tar", last modified: Thu Apr 11 15:23:04 2024, max compression
```

## Comparing `safe-mol-0.1.5.tar` & `safe-mol-0.1.6.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.539872 safe-mol-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.527872 safe-mol-0.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.527872 safe-mol-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-14 00:18:24.000000 safe-mol-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-14 00:18:24.000000 safe-mol-0.1.5/DATA_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-01-14 00:18:24.000000 safe-mol-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-01-14 00:22:21.539872 safe-mol-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-01-14 00:18:24.000000 safe-mol-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.531872 safe-mol-0.1.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.531872 safe-mol-0.1.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/api/safe.md
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/api/safe.models.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/api/safe.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.531872 safe-mol-0.1.5/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    36030 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/assets/safe-construction.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86699 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/assets/safe-tasks.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/data_license.md
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.535872 safe-mol-0.1.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)  1793089 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/tutorials/design-with-safe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36563 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/tutorials/extracting-representation-molfeat.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   138661 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/tutorials/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    91753 2024-01-14 00:18:24.000000 safe-mol-0.1.5/docs/tutorials/how-it-works.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-14 00:18:24.000000 safe-mol-0.1.5/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.527872 safe-mol-0.1.5/expts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.535872 safe-mol-0.1.5/expts/config/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/config/accelerate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.535872 safe-mol-0.1.5/expts/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/slurm-data-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/slurm-notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/slurm-tokenizer-train-custom.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/slurm-tokenizer-train-small.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1168 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/slurm-tokenizer-train.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/train-small.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/scripts/train.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.535872 safe-mol-0.1.5/expts/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/tokenizer/_tokenizer-custom-mini-test.json
--rw-r--r--   0 runner    (1001) docker     (127)    46319 2024-01-14 00:18:24.000000 safe-mol-0.1.5/expts/tokenizer/tokenizer-custom.json
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-01-14 00:18:24.000000 safe-mol-0.1.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-01-14 00:18:24.000000 safe-mol-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.535872 safe-mol-0.1.5/safe/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39190 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.539872 safe-mol-0.1.5/safe/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/collator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.539872 safe-mol-0.1.5/safe/trainer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/configs/default_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/trainer/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-01-14 00:18:24.000000 safe-mol-0.1.5/safe/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.539872 safe-mol-0.1.5/safe_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-01-14 00:22:21.000000 safe-mol-0.1.5/safe_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-14 00:22:21.000000 safe-mol-0.1.5/safe_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 00:22:21.000000 safe-mol-0.1.5/safe_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-14 00:22:21.000000 safe-mol-0.1.5/safe_mol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 00:22:17.000000 safe-mol-0.1.5/safe_mol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-14 00:22:21.000000 safe-mol-0.1.5/safe_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-14 00:22:21.000000 safe-mol-0.1.5/safe_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 00:22:21.539872 safe-mol-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:22:21.539872 safe-mol-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-14 00:18:24.000000 safe-mol-0.1.5/tests/test_hgf_load.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-14 00:18:24.000000 safe-mol-0.1.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-14 00:18:24.000000 safe-mol-0.1.5/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-01-14 00:18:24.000000 safe-mol-0.1.5/tests/test_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.472078 safe-mol-0.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.472078 safe-mol-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 15:19:06.000000 safe-mol-0.1.6/DATA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-11 15:19:06.000000 safe-mol-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-11 15:23:04.484078 safe-mol-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-11 15:19:06.000000 safe-mol-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/api/safe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/api/safe.models.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/api/safe.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36030 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/assets/safe-construction.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86699 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/assets/safe-tasks.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/data_license.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1793089 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/design-with-safe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36563 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/extracting-representation-molfeat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   138661 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    91753 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/how-it-works.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-11 15:19:06.000000 safe-mol-0.1.6/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.472078 safe-mol-0.1.6/expts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/expts/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/config/accelerate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/expts/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-data-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-custom.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-small.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1168 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/train-small.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/train.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/expts/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/tokenizer/_tokenizer-custom-mini-test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46319 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/tokenizer/tokenizer-custom.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-11 15:19:06.000000 safe-mol-0.1.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-11 15:19:06.000000 safe-mol-0.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/safe/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17588 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39204 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/safe/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/collator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/safe/trainer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/configs/default_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/safe_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:23:00.000000 safe-mol-0.1.6/safe_mol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:23:04.484078 safe-mol-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_hgf_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_safe.py
```

### Comparing `safe-mol-0.1.5/.github/PULL_REQUEST_TEMPLATE.md` & `safe-mol-0.1.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/.github/workflows/code-check.yml` & `safe-mol-0.1.6/.github/workflows/code-check.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: Install black
         run: |
-          pip install black>=23
+          pip install black>=24
 
       - name: Lint
         run: black --check .
 
   python-lint-ruff:
     name: Python lint [ruff]
     runs-on: ubuntu-latest
```

### Comparing `safe-mol-0.1.5/.github/workflows/doc.yml` & `safe-mol-0.1.6/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/.github/workflows/release.yml` & `safe-mol-0.1.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/.github/workflows/test.yml` & `safe-mol-0.1.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/.gitignore` & `safe-mol-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/LICENSE` & `safe-mol-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/PKG-INFO` & `safe-mol-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-mol
-Version: 0.1.5
+Version: 0.1.6
 Summary: Implementation of the 'Gotta be SAFE: a new framework for molecular design' paper
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/datamol-io/safe
 Project-URL: Bug Tracker, https://github.com/datamol-io/safe/issues
 Project-URL: Documentation, https://safe-docs.datamol.io/
 Keywords: safe,smiles,de novo,design,molecules
@@ -100,17 +100,17 @@
 The construction of a SAFE strings requires defining a molecular fragmentation algorithm. By default, we use [BRICS], but any other fragmentation algorithm can be used. The image below illustrates the process of building a SAFE string. The resulting string is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/datamol) or [RDKit](https://github.com/rdkit/rdkit).
 
 </br>
 <div align="center">
     <img src="docs/assets/safe-construction.svg" width="100%">
 </div>
 
-## News 
+## News 🚀
 
-#### 2024/01/15
+#### 💥 2024/01/15 💥
 1. [@IanAWatson](https://github.com/IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a custom fragmentation algorithm. Follow the installation instruction on the repo and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/SAFE.md)
 
 
 ### Installation
 
 You can install `safe` using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: safe-mol Version: 0.1.5 Summary: Implementation of
+Metadata-Version: 2.1 Name: safe-mol Version: 0.1.6 Summary: Implementation of
 the 'Gotta be SAFE: a new framework for molecular design' paper Author-email:
 Emmanuel Noutahi
 gmail.com> License: Apache-2.0 Project-URL: Source Code, https://github.com/
 datamol-io/safe Project-URL: Bug Tracker, https://github.com/datamol-io/safe/
 issues Project-URL: Documentation, https://safe-docs.datamol.io/ Keywords:
 safe,smiles,de novo,design,molecules Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
@@ -61,19 +61,19 @@
 motif extension - linker generation - scaffold morphing. The construction of a
 SAFE strings requires defining a molecular fragmentation algorithm. By default,
 we use [BRICS], but any other fragmentation algorithm can be used. The image
 below illustrates the process of building a SAFE string. The resulting string
 is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/
 datamol) or [RDKit](https://github.com/rdkit/rdkit).
                       [docs/assets/safe-construction.svg]
-## News #### 2024/01/15 1. [@IanAWatson](https://github.com/IanAWatson) has a
-C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/
-LillyMol/tree/bazel_version_float) that is quite fast and use a custom
-fragmentation algorithm. Follow the installation instruction on the repo and
-checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
+## News ð #### ð¥ 2024/01/15 ð¥ 1. [@IanAWatson](https://github.com/
+IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/
+IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a
+custom fragmentation algorithm. Follow the installation instruction on the repo
+and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
 github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/
 SAFE.md) ### Installation You can install `safe` using pip: ```bash pip install
 safe-mol ``` You can use conda/mamba: ```bash mamba install -c conda-forge
 safe-mol ``` ### Datasets and Models | Type | Name | Infos | Size | Comment | |
 ---------------------- | ------------------------------------------------------
 ------------------------ | ---------- | ----- | -------------------- | | Model
 | [datamol-io/safe-gpt](https://huggingface.co/datamol-io/safe-gpt) | 87M
```

### Comparing `safe-mol-0.1.5/README.md` & `safe-mol-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
 The construction of a SAFE strings requires defining a molecular fragmentation algorithm. By default, we use [BRICS], but any other fragmentation algorithm can be used. The image below illustrates the process of building a SAFE string. The resulting string is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/datamol) or [RDKit](https://github.com/rdkit/rdkit).
 
 </br>
 <div align="center">
     <img src="docs/assets/safe-construction.svg" width="100%">
 </div>
 
-## News 
+## News 🚀
 
-#### 2024/01/15
+#### 💥 2024/01/15 💥
 1. [@IanAWatson](https://github.com/IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a custom fragmentation algorithm. Follow the installation instruction on the repo and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/SAFE.md)
 
 
 ### Installation
 
 You can install `safe` using pip:
```

#### html2text {}

```diff
@@ -37,19 +37,19 @@
 motif extension - linker generation - scaffold morphing. The construction of a
 SAFE strings requires defining a molecular fragmentation algorithm. By default,
 we use [BRICS], but any other fragmentation algorithm can be used. The image
 below illustrates the process of building a SAFE string. The resulting string
 is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/
 datamol) or [RDKit](https://github.com/rdkit/rdkit).
                       [docs/assets/safe-construction.svg]
-## News #### 2024/01/15 1. [@IanAWatson](https://github.com/IanAWatson) has a
-C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/
-LillyMol/tree/bazel_version_float) that is quite fast and use a custom
-fragmentation algorithm. Follow the installation instruction on the repo and
-checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
+## News ð #### ð¥ 2024/01/15 ð¥ 1. [@IanAWatson](https://github.com/
+IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/
+IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a
+custom fragmentation algorithm. Follow the installation instruction on the repo
+and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
 github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/
 SAFE.md) ### Installation You can install `safe` using pip: ```bash pip install
 safe-mol ``` You can use conda/mamba: ```bash mamba install -c conda-forge
 safe-mol ``` ### Datasets and Models | Type | Name | Infos | Size | Comment | |
 ---------------------- | ------------------------------------------------------
 ------------------------ | ---------- | ----- | -------------------- | | Model
 | [datamol-io/safe-gpt](https://huggingface.co/datamol-io/safe-gpt) | 87M
```

### Comparing `safe-mol-0.1.5/docs/api/safe.models.md` & `safe-mol-0.1.6/docs/api/safe.models.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/assets/safe-construction.svg` & `safe-mol-0.1.6/docs/assets/safe-construction.svg`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/assets/safe-tasks.svg` & `safe-mol-0.1.6/docs/assets/safe-tasks.svg`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/cli.md` & `safe-mol-0.1.6/docs/cli.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/index.md` & `safe-mol-0.1.6/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 The construction of a SAFE strings requires defining a molecular fragmentation algorithm. By default, we use [BRICS], but any other fragmentation algorithm can be used. The image below illustrates the process of building a SAFE string. The resulting string is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/datamol) or [RDKit](https://github.com/rdkit/rdkit).
 
 </br>
 <div align="center">
     <img src="assets/safe-construction.svg" width="100%">
 </div>
 
+
+## News 🚀
+
+#### 💥 2024/01/15 💥
+1. [@IanAWatson](https://github.com/IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a custom fragmentation algorithm. Follow the installation instruction on the repo and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/SAFE.md)
+
 ### Installation
 
 You can install `safe` using pip:
 
 ```bash
 pip install safe-mol
 ```
```

#### html2text {}

```diff
@@ -38,23 +38,29 @@
 decoration - motif extension - linker generation - scaffold morphing. The
 construction of a SAFE strings requires defining a molecular fragmentation
 algorithm. By default, we use [BRICS], but any other fragmentation algorithm
 can be used. The image below illustrates the process of building a SAFE string.
 The resulting string is a valid SMILES that can be read by [datamol](https://
 github.com/datamol-io/datamol) or [RDKit](https://github.com/rdkit/rdkit).
                         [assets/safe-construction.svg]
-### Installation You can install `safe` using pip: ```bash pip install safe-mol
-``` You can use conda/mamba: ```bash mamba install -c conda-forge safe-mol ```
-### Datasets and Models | Type | Name | Infos | Size | Comment | | ------------
----------- | ------------------------------------------------------------------
------------- | ---------- | ----- | -------------------- | | Model | [datamol-
-io/safe-gpt](https://huggingface.co/datamol-io/safe-gpt) | 87M params | 350M |
-Default model | | Training Dataset | [datamol-io/safe-gpt](https://
-huggingface.co/datasets/datamol-io/safe-gpt) | 1.1B rows | 250GB | Training
-dataset | | Drug Benchmark Dataset | [datamol-io/safe-drugs](https://
+## News ð #### ð¥ 2024/01/15 ð¥ 1. [@IanAWatson](https://github.com/
+IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/
+IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a
+custom fragmentation algorithm. Follow the installation instruction on the repo
+and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
+github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/
+SAFE.md) ### Installation You can install `safe` using pip: ```bash pip install
+safe-mol ``` You can use conda/mamba: ```bash mamba install -c conda-forge
+safe-mol ``` ### Datasets and Models | Type | Name | Infos | Size | Comment | |
+---------------------- | ------------------------------------------------------
+------------------------ | ---------- | ----- | -------------------- | | Model
+| [datamol-io/safe-gpt](https://huggingface.co/datamol-io/safe-gpt) | 87M
+params | 350M | Default model | | Training Dataset | [datamol-io/safe-gpt]
+(https://huggingface.co/datasets/datamol-io/safe-gpt) | 1.1B rows | 250GB |
+Training dataset | | Drug Benchmark Dataset | [datamol-io/safe-drugs](https://
 huggingface.co/datasets/datamol-io/safe-drugs) | 26 rows | 20 kB | Benchmarking
 dataset | ## Usage The tutorials in the [documentation](https://safe-
 docs.datamol.io/) can help you get started with `safe` and `SAFE-GPT`. ### API
 We summarize some key functions provided by the `safe` package below. |
 Function | Description | | ------------- | ------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
```

### Comparing `safe-mol-0.1.5/docs/tutorials/design-with-safe.ipynb` & `safe-mol-0.1.6/docs/tutorials/design-with-safe.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/tutorials/extracting-representation-molfeat.ipynb` & `safe-mol-0.1.6/docs/tutorials/extracting-representation-molfeat.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/tutorials/getting-started.ipynb` & `safe-mol-0.1.6/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/docs/tutorials/how-it-works.ipynb` & `safe-mol-0.1.6/docs/tutorials/how-it-works.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/env.yml` & `safe-mol-0.1.6/env.yml`

 * *Files 19% similar despite different names*

```diff
@@ -7,29 +7,30 @@
   - tqdm
   - loguru
   - typer
   - universal_pathlib
 
   # Scientific
   - datamol
+  - pandas <=2.1.1
   - numpy
   - pytorch >=2.0
   - transformers
   - datasets
   - tokenizers
   - accelerate
   - evaluate
   - wandb
   - huggingface_hub
 
   # Optional
   - deepspeed
 
   # dev
-  - black >=23
+  - black >=24
   - ruff
   - pytest >=6.0
   - nbconvert
   - jupyterlab
   - nbconvert
   - ipywidgets
```

### Comparing `safe-mol-0.1.5/expts/scripts/slurm-tokenizer-train-custom.sh` & `safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-custom.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/expts/scripts/slurm-tokenizer-train-small.sh` & `safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-small.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/expts/scripts/slurm-tokenizer-train.sh` & `safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/expts/scripts/train-small.sh` & `safe-mol-0.1.6/expts/scripts/train-small.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/expts/scripts/train.sh` & `safe-mol-0.1.6/expts/scripts/train.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/expts/tokenizer/_tokenizer-custom-mini-test.json` & `safe-mol-0.1.6/expts/tokenizer/_tokenizer-custom-mini-test.json`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/expts/tokenizer/tokenizer-custom.json` & `safe-mol-0.1.6/expts/tokenizer/tokenizer-custom.json`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/mkdocs.yml` & `safe-mol-0.1.6/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
   - Data License: data_license.md
 
 theme:
   name: material
   features:
     - navigation.expand
 
+extra_javascript:
+  - assets/js/google-analytics.js
+  
 markdown_extensions:
   - admonition
   - markdown_include.include
   - pymdownx.emoji
   - pymdownx.highlight
   - pymdownx.magiclink
   - pymdownx.superfences
```

### Comparing `safe-mol-0.1.5/pyproject.toml` & `safe-mol-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -77,35 +77,33 @@
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose --color yes"
 testpaths = ["tests"]
 
-[tool.ruff.pycodestyle]
-max-doc-length = 150
 
 [tool.ruff]
 line-length = 120
 # Enable Pyflakes `E` and `F` codes by default.
-select = [
+lint.select = [
     "E",
     "W", # see: https://pypi.org/project/pycodestyle
     "F", # see: https://pypi.org/project/pyflakes
 ]
-extend-select = [
+lint.extend-select = [
     "C4",  # see: https://pypi.org/project/flake8-comprehensions
     "SIM", # see: https://pypi.org/project/flake8-simplify
     "RET", # see: https://pypi.org/project/flake8-return
     "PT",  # see: https://pypi.org/project/flake8-pytest-style
 ]
-ignore = [
+lint.ignore = [
     "E731", # Do not assign a lambda expression, use a def
     "S108",
     "F401",
     "S105",
     "E501",
     "E722",
 ]
 # Exclude a variety of commonly ignored directories.
 exclude = [".git", "docs", "_notebooks"]
-ignore-init-module-imports = true
+lint.ignore-init-module-imports = true
```

### Comparing `safe-mol-0.1.5/safe/converter.py` & `safe-mol-0.1.6/safe/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,24 +284,24 @@
         for i_a, i_b in matching_bonds:
             # if both atoms of the bond are found in a disallowed substructure, we cannot consider them
             # on the other end, a bond between two substructure to preserved independently is perfectly fine
             if any((i_a in ignore_x and i_b in ignore_x) for ignore_x in substructed_ignored):
                 continue
             obond = mol.GetBondBetweenAtoms(i_a, i_b)
             bonds.append(obond.GetIdx())
+
         if len(bonds) > 0:
             mol = Chem.FragmentOnBonds(
                 mol,
                 bonds,
                 dummyLabels=[(i + bond_map_id, i + bond_map_id) for i in range(len(bonds))],
             )
         # here we need to be clever and disable rooted atom as the atom with mapping
 
         frags = list(Chem.GetMolFrags(mol, asMols=True))
-
         if randomize:
             frags = rng.permutation(frags).tolist()
         elif canonical:
             frags = sorted(
                 frags,
                 key=lambda x: x.GetNumAtoms(),
                 reverse=True,
@@ -318,26 +318,31 @@
                     isomericSmiles=True,
                     canonical=True,  # needs to always be true
                     rootedAtAtom=non_map_atom_idxs[0],
                 )
             )
 
         scaffold_str = ".".join(frags_str)
+        # EN: fix for https://github.com/datamol-io/safe/issues/37
+        # we were using the wrong branch number count which did not take into account
+        # possible change in digit utilization after bond slicing
+        scf_branch_num = self._find_branch_number(scaffold_str) + branch_numbers
+
         # don't capture atom mapping in the scaffold
         attach_pos = set(re.findall(r"(\[\d+\*\]|!\[[^:]*:\d+\])", scaffold_str))
-
         if canonical:
             attach_pos = sorted(attach_pos)
-        starting_num = 1 if len(branch_numbers) == 0 else max(branch_numbers) + 1
+        starting_num = 1 if len(scf_branch_num) == 0 else max(scf_branch_num) + 1
         for attach in attach_pos:
             val = str(starting_num) if starting_num < 10 else f"%{starting_num}"
             # we cannot have anything of the form "\([@=-#-$/\]*\d+\)"
             attach_regexp = re.compile(r"(" + re.escape(attach) + r")")
             scaffold_str = attach_regexp.sub(val, scaffold_str)
             starting_num += 1
+
         # now we need to remove all the parenthesis around digit only number
         wrong_attach = re.compile(r"\(([\%\d]*)\)")
         scaffold_str = wrong_attach.sub(r"\g<1>", scaffold_str)
         # furthermore, we autoapply rdkit-compatible digit standardization.
         if rdkit_safe:
             pattern = r"\(([=-@#]?)(%?\d{1,2})\)"
             replacement = r"\g<1>\g<2>"
```

### Comparing `safe-mol-0.1.5/safe/sample.py` & `safe-mol-0.1.6/safe/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,18 +38,18 @@
         Args:
             model: input SAFEDoubleHeadsModel to use for generation
             tokenizer: input SAFETokenizer to use for generation
             generation_config: input GenerationConfig to use for generation
             safe_encoder: custom safe encoder to use
             verbose: whether to print out logging information during generation
         """
-        if isinstance(model, os.PathLike):
+        if isinstance(model, (str, os.PathLike)):
             model = SAFEDoubleHeadsModel.from_pretrained(model)
 
-        if isinstance(tokenizer, os.PathLike):
+        if isinstance(tokenizer, (str, os.PathLike)):
             tokenizer = SAFETokenizer.load(tokenizer)
 
         model.eval()
         self.model = model
         self.tokenizer = tokenizer
         if isinstance(generation_config, os.PathLike):
             generation_config = GenerationConfig.from_pretrained(generation_config)
```

### Comparing `safe-mol-0.1.5/safe/tokenizer.py` & `safe-mol-0.1.6/safe/tokenizer.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe/trainer/cli.py` & `safe-mol-0.1.6/safe/trainer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,17 +338,17 @@
         dispatch_batches=(data_args.streaming is not True),
         train_dataset=train_dataset.shuffle(seed=(training_args.seed or 42)),
         eval_dataset=dataset.get(eval_dataset_key_name, None),
         args=training_args,
         prop_loss_coeff=model_args.prop_loss_coeff,
         compute_metrics=compute_metrics if training_args.do_eval else None,
         data_collator=data_collator,
-        preprocess_logits_for_metrics=preprocess_logits_for_metrics
-        if training_args.do_eval
-        else None,
+        preprocess_logits_for_metrics=(
+            preprocess_logits_for_metrics if training_args.do_eval else None
+        ),
     )
 
     if training_args.do_train:
         checkpoint = None
         if training_args.resume_from_checkpoint is not None:
             checkpoint = training_args.resume_from_checkpoint
         elif last_checkpoint is not None:
```

### Comparing `safe-mol-0.1.5/safe/trainer/collator.py` & `safe-mol-0.1.6/safe/trainer/collator.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe/trainer/configs/default_config.json` & `safe-mol-0.1.6/safe/trainer/configs/default_config.json`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe/trainer/data_utils.py` & `safe-mol-0.1.6/safe/trainer/data_utils.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe/trainer/model.py` & `safe-mol-0.1.6/safe/trainer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         labels: Optional[torch.LongTensor] = None,
         mc_labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         inputs: Optional[Any] = None,  # do not remove because of trainer
+        encoder_hidden_states: Optional[torch.Tensor] = None,
         **kwargs,
     ) -> Union[Tuple, GPT2DoubleHeadsModelOutput]:
         r"""
 
         Args:
             mc_token_ids (`torch.LongTensor` of shape `(batch_size, num_choices)`, *optional*, default to index of the last token of the input):
                 Index of the classification token in each input sequence. Selected in the range `[0, input_ids.size(-1) -
@@ -160,14 +161,15 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
+            encoder_hidden_states=encoder_hidden_states,
         )
 
         hidden_states = transformer_outputs[0]
         lm_logits = self.lm_head(hidden_states)
 
         if mc_token_ids is None and self.config.pad_token_id is not None and input_ids is not None:
             mc_token_ids = (torch.ne(input_ids, self.config.pad_token_id).sum(-1) - 1).to(
```

### Comparing `safe-mol-0.1.5/safe/trainer/trainer_utils.py` & `safe-mol-0.1.6/safe/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe/utils.py` & `safe-mol-0.1.6/safe/utils.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe/viz.py` & `safe-mol-0.1.6/safe/viz.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/safe_mol.egg-info/PKG-INFO` & `safe-mol-0.1.6/safe_mol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-mol
-Version: 0.1.5
+Version: 0.1.6
 Summary: Implementation of the 'Gotta be SAFE: a new framework for molecular design' paper
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/datamol-io/safe
 Project-URL: Bug Tracker, https://github.com/datamol-io/safe/issues
 Project-URL: Documentation, https://safe-docs.datamol.io/
 Keywords: safe,smiles,de novo,design,molecules
@@ -100,17 +100,17 @@
 The construction of a SAFE strings requires defining a molecular fragmentation algorithm. By default, we use [BRICS], but any other fragmentation algorithm can be used. The image below illustrates the process of building a SAFE string. The resulting string is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/datamol) or [RDKit](https://github.com/rdkit/rdkit).
 
 </br>
 <div align="center">
     <img src="docs/assets/safe-construction.svg" width="100%">
 </div>
 
-## News 
+## News 🚀
 
-#### 2024/01/15
+#### 💥 2024/01/15 💥
 1. [@IanAWatson](https://github.com/IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a custom fragmentation algorithm. Follow the installation instruction on the repo and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/SAFE.md)
 
 
 ### Installation
 
 You can install `safe` using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: safe-mol Version: 0.1.5 Summary: Implementation of
+Metadata-Version: 2.1 Name: safe-mol Version: 0.1.6 Summary: Implementation of
 the 'Gotta be SAFE: a new framework for molecular design' paper Author-email:
 Emmanuel Noutahi
 gmail.com> License: Apache-2.0 Project-URL: Source Code, https://github.com/
 datamol-io/safe Project-URL: Bug Tracker, https://github.com/datamol-io/safe/
 issues Project-URL: Documentation, https://safe-docs.datamol.io/ Keywords:
 safe,smiles,de novo,design,molecules Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
@@ -61,19 +61,19 @@
 motif extension - linker generation - scaffold morphing. The construction of a
 SAFE strings requires defining a molecular fragmentation algorithm. By default,
 we use [BRICS], but any other fragmentation algorithm can be used. The image
 below illustrates the process of building a SAFE string. The resulting string
 is a valid SMILES that can be read by [datamol](https://github.com/datamol-io/
 datamol) or [RDKit](https://github.com/rdkit/rdkit).
                       [docs/assets/safe-construction.svg]
-## News #### 2024/01/15 1. [@IanAWatson](https://github.com/IanAWatson) has a
-C++ implementation of SAFE in [LillyMol](https://github.com/IanAWatson/
-LillyMol/tree/bazel_version_float) that is quite fast and use a custom
-fragmentation algorithm. Follow the installation instruction on the repo and
-checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
+## News ð #### ð¥ 2024/01/15 ð¥ 1. [@IanAWatson](https://github.com/
+IanAWatson) has a C++ implementation of SAFE in [LillyMol](https://github.com/
+IanAWatson/LillyMol/tree/bazel_version_float) that is quite fast and use a
+custom fragmentation algorithm. Follow the installation instruction on the repo
+and checkout the docs of the CLI here: [docs/Molecule_Tools/SAFE.md](https://
 github.com/IanAWatson/LillyMol/blob/bazel_version_float/docs/Molecule_Tools/
 SAFE.md) ### Installation You can install `safe` using pip: ```bash pip install
 safe-mol ``` You can use conda/mamba: ```bash mamba install -c conda-forge
 safe-mol ``` ### Datasets and Models | Type | Name | Infos | Size | Comment | |
 ---------------------- | ------------------------------------------------------
 ------------------------ | ---------- | ----- | -------------------- | | Model
 | [datamol-io/safe-gpt](https://huggingface.co/datamol-io/safe-gpt) | 87M
```

### Comparing `safe-mol-0.1.5/safe_mol.egg-info/SOURCES.txt` & `safe-mol-0.1.6/safe_mol.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 docs/index.md
 docs/license.md
 docs/api/safe.md
 docs/api/safe.models.md
 docs/api/safe.viz.md
 docs/assets/safe-construction.svg
 docs/assets/safe-tasks.svg
+docs/assets/js/google-analytics.js
 docs/tutorials/design-with-safe.ipynb
 docs/tutorials/extracting-representation-molfeat.ipynb
 docs/tutorials/getting-started.ipynb
 docs/tutorials/how-it-works.ipynb
 expts/config/accelerate.yaml
 expts/scripts/slurm-data-build.sh
 expts/scripts/slurm-notebook.sh
```

### Comparing `safe-mol-0.1.5/tests/test_hgf_load.py` & `safe-mol-0.1.6/tests/test_hgf_load.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/tests/test_notebooks.py` & `safe-mol-0.1.6/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.5/tests/test_safe.py` & `safe-mol-0.1.6/tests/test_safe.py`

 * *Files 11% similar despite different names*

```diff
@@ -106,7 +106,18 @@
                 remove_added_hs=True,
             )
             fragments.append(f)
     input_mol = dm.to_mol(input_sm)
     assert safe.decode(safe_str) is not None
     assert dm.same_mol(dm.to_mol(safe_str), input_mol)
     assert None not in fragments
+
+
+def test_fused_ring_issue():
+    FUSED_RING_LIST = [
+        "[H][C@@]12CC[C@@]3(CCC(=O)O3)[C@@]1(C)CC[C@@]1([H])[C@@]2([H])[C@@]([H])(CC2=CC(=O)CC[C@]12C)SC(C)=O",
+        "[H][C@@]12C[C@H](C)[C@](OC(=O)CC)(C(=O)COC(=O)CC)[C@@]1(C)C[C@H](O)[C@@]1(Cl)[C@@]2([H])CCC2=CC(=O)C=C[C@]12C",
+        "[H][C@@]12CC[C@@](O)(C#C)[C@@]1(CC)CC[C@]1([H])[C@@]3([H])CCC(=O)C=C3CC[C@@]21[H]",
+    ]
+    for fused_ring in FUSED_RING_LIST:
+        output_string = safe.decode(safe.encode(fused_ring))
+        assert dm.same_mol(fused_ring, output_string)
```

