# Comparing `tmp/dplutils-0.5.1.tar.gz` & `tmp/dplutils-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dplutils-0.5.1.tar", last modified: Tue Apr  9 00:48:43 2024, max compression
+gzip compressed data, was "dplutils-0.5.2.tar", last modified: Thu Apr 11 15:11:21 2024, max compression
```

## Comparing `dplutils-0.5.1.tar` & `dplutils-0.5.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.231753 dplutils-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 00:48:32.000000 dplutils-0.5.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 00:48:32.000000 dplutils-0.5.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.219753 dplutils-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 00:48:32.000000 dplutils-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.219753 dplutils-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-09 00:48:32.000000 dplutils-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-09 00:48:32.000000 dplutils-0.5.1/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 00:48:32.000000 dplutils-0.5.1/.github/workflows/security.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-09 00:48:32.000000 dplutils-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 00:48:32.000000 dplutils-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 00:48:32.000000 dplutils-0.5.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-09 00:48:32.000000 dplutils-0.5.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 00:48:32.000000 dplutils-0.5.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-09 00:48:32.000000 dplutils-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 00:48:32.000000 dplutils-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-09 00:48:43.231753 dplutils-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-09 00:48:32.000000 dplutils-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.219753 dplutils-0.5.1/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-09 00:48:32.000000 dplutils-0.5.1/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-04-09 00:48:32.000000 dplutils-0.5.1/docker/startray.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.219753 dplutils-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.219753 dplutils-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/_static/.DS_Store
--rwxr-xr-x   0 runner    (1001) docker     (127)    33376 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/_static/SSEC_logo_horiz_blue_1152x263.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    72437 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/_static/SSEC_logo_vert_white_lg_1184x661.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.223753 dplutils-0.5.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/api_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/api_observers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/api_pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/api_streaming.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/execution.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/tasks_graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 00:48:32.000000 dplutils-0.5.1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.223753 dplutils-0.5.1/dplutils/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 00:48:43.000000 dplutils-0.5.1/dplutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.227753 dplutils-0.5.1/dplutils/observer/
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/observer/aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/observer/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/observer/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.227753 dplutils-0.5.1/dplutils/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 00:48:32.000000 dplutils-0.5.1/dplutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.231753 dplutils-0.5.1/dplutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-09 00:48:43.000000 dplutils-0.5.1/dplutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-09 00:48:43.000000 dplutils-0.5.1/dplutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:48:43.000000 dplutils-0.5.1/dplutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:48:42.000000 dplutils-0.5.1/dplutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 00:48:43.000000 dplutils-0.5.1/dplutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 00:48:43.000000 dplutils-0.5.1/dplutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.227753 dplutils-0.5.1/githooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-04-09 00:48:32.000000 dplutils-0.5.1/githooks/pre-push
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 00:48:32.000000 dplutils-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.227753 dplutils-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 00:48:32.000000 dplutils-0.5.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 00:48:32.000000 dplutils-0.5.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 00:48:32.000000 dplutils-0.5.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 00:48:32.000000 dplutils-0.5.1/requirements/prd.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 00:48:32.000000 dplutils-0.5.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:48:43.231753 dplutils-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.227753 dplutils-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.227753 dplutils-0.5.1/tests/observer/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/observer/test_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/observer/test_observer_aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/observer/test_observer_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/observer/test_observer_ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:48:43.231753 dplutils-0.5.1/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_executor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_ray_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_ray_stream_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_stream_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/pipeline/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 00:48:32.000000 dplutils-0.5.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 00:48:32.000000 dplutils-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.352961 dplutils-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 15:11:10.000000 dplutils-0.5.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-11 15:11:10.000000 dplutils-0.5.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-11 15:11:10.000000 dplutils-0.5.2/.github/workflows/security.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-11 15:11:10.000000 dplutils-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 15:11:10.000000 dplutils-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-11 15:11:10.000000 dplutils-0.5.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-11 15:11:10.000000 dplutils-0.5.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 15:11:10.000000 dplutils-0.5.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-11 15:11:10.000000 dplutils-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-11 15:11:10.000000 dplutils-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-11 15:11:21.352961 dplutils-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-11 15:11:10.000000 dplutils-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-11 15:11:10.000000 dplutils-0.5.2/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-04-11 15:11:10.000000 dplutils-0.5.2/docker/startray.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.340961 dplutils-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/.DS_Store
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33376 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/SSEC_logo_horiz_blue_1152x263.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72437 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/SSEC_logo_vert_white_lg_1184x661.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.344961 dplutils-0.5.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_observers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/api_streaming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/execution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/tasks_graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 15:11:10.000000 dplutils-0.5.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.344961 dplutils-0.5.2/dplutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/dplutils/observer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/observer/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/dplutils/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-11 15:11:10.000000 dplutils-0.5.2/dplutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.352961 dplutils-0.5.2/dplutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 15:11:21.000000 dplutils-0.5.2/dplutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/githooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-04-11 15:11:10.000000 dplutils-0.5.2/githooks/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-11 15:11:10.000000 dplutils-0.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/prd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 15:11:10.000000 dplutils-0.5.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:11:21.352961 dplutils-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.348961 dplutils-0.5.2/tests/observer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer_aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/observer/test_observer_ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:11:21.352961 dplutils-0.5.2/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_executor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_ray_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_ray_stream_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_stream_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/pipeline/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-11 15:11:10.000000 dplutils-0.5.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-11 15:11:10.000000 dplutils-0.5.2/tox.ini
```

### Comparing `dplutils-0.5.1/.github/workflows/ci.yml` & `dplutils-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/.github/workflows/dist.yml` & `dplutils-0.5.2/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/.github/workflows/security.yml` & `dplutils-0.5.2/.github/workflows/security.yml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/.gitignore` & `dplutils-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/.readthedocs.yaml` & `dplutils-0.5.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/.zenodo.json` & `dplutils-0.5.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/CITATION.cff` & `dplutils-0.5.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/CODE_OF_CONDUCT.md` & `dplutils-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/LICENSE` & `dplutils-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/PKG-INFO` & `dplutils-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplutils
-Version: 0.5.1
+Version: 0.5.2
 Author-email: Scientifc Software Engineering Center at JHU <ssec@jhu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Software Engineering Center at JHU
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `dplutils-0.5.1/README.md` & `dplutils-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docker/Dockerfile` & `dplutils-0.5.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/Makefile` & `dplutils-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/_static/.DS_Store` & `dplutils-0.5.2/docs/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/_static/SSEC_logo_horiz_blue_1152x263.png` & `dplutils-0.5.2/docs/_static/SSEC_logo_horiz_blue_1152x263.png`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/_static/SSEC_logo_vert_white_lg_1184x661.png` & `dplutils-0.5.2/docs/_static/SSEC_logo_vert_white_lg_1184x661.png`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/make.bat` & `dplutils-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/source/api_observers.rst` & `dplutils-0.5.2/docs/source/api_observers.rst`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/source/conf.py` & `dplutils-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/docs/source/quickstart.rst` & `dplutils-0.5.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/cli.py` & `dplutils-0.5.2/dplutils/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 from argparse import ArgumentParser, Namespace
-from dplutils.pipeline.utils import dict_from_coord
 from dplutils.pipeline import PipelineExecutor
 
 
 def add_generic_args(argparser):
     """Add Pipeline generic args to parser
 
     The generic set of CLI arguments are as follows:
@@ -45,22 +44,14 @@
     try:
         v = json.loads(v)
     except json.decoder.JSONDecodeError:
         pass
     return k, v
 
 
-def config_dict_from_args(args):
-    config = {}
-    for conf in args.set_config:
-        k,v = parse_config_element(conf)
-        config.update(dict_from_coord(k, v))
-    return config
-
-
 def set_config_from_args(pipeline: PipelineExecutor, args: Namespace):
     """Configure pipeline using config from arguments
 
     Set context from the ``set-context`` argument and config from
     ``set-config``. Each will be parset as ``name=value`` pair, where the value
     is parsed as a JSON object, falling back to string.
 
@@ -68,17 +59,16 @@
     ``task.param[.subparam[...]]`` where ``task`` is the taskname, ``param`` is
     a parameter of :class:`PipelineTask<dplutils.pipeline.PipelineTask>`
     and ``subparam`` is a key within a dictionary of such a parameter (where
     applicable).
     """
     for ctx in args.set_context:
         pipeline.set_context(*parse_config_element(ctx))
-    config = config_dict_from_args(args)
-    if config:
-        pipeline.set_config_from_dict(config)
+    for conf in args.set_config:
+        pipeline.set_config(*parse_config_element(conf))
 
 
 def cli_run(pipeline: PipelineExecutor, args: Namespace|None = None,  **argparse_kwargs):
     """Run pipeline from cli args
 
     If ``args`` is None, this function runs the pipeline for the standard set of
     workload-independent arguments (e.g. those that are generic to pipleines in
```

### Comparing `dplutils-0.5.1/dplutils/observer/__init__.py` & `dplutils-0.5.2/dplutils/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/observer/aim.py` & `dplutils-0.5.2/dplutils/observer/aim.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/observer/mlflow.py` & `dplutils-0.5.2/dplutils/observer/mlflow.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/observer/ray.py` & `dplutils-0.5.2/dplutils/observer/ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/pipeline/executor.py` & `dplutils-0.5.2/dplutils/pipeline/executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/pipeline/graph.py` & `dplutils-0.5.2/dplutils/pipeline/graph.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/pipeline/ray.py` & `dplutils-0.5.2/dplutils/pipeline/ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/pipeline/stream.py` & `dplutils-0.5.2/dplutils/pipeline/stream.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils/pipeline/task.py` & `dplutils-0.5.2/dplutils/pipeline/task.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/dplutils.egg-info/PKG-INFO` & `dplutils-0.5.2/dplutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dplutils
-Version: 0.5.1
+Version: 0.5.2
 Author-email: Scientifc Software Engineering Center at JHU <ssec@jhu.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Software Engineering Center at JHU
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `dplutils-0.5.1/dplutils.egg-info/SOURCES.txt` & `dplutils-0.5.2/dplutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/pyproject.toml` & `dplutils-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/conftest.py` & `dplutils-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/observer/test_observer.py` & `dplutils-0.5.2/tests/observer/test_observer.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/observer/test_observer_aim.py` & `dplutils-0.5.2/tests/observer/test_observer_aim.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/observer/test_observer_mlflow.py` & `dplutils-0.5.2/tests/observer/test_observer_mlflow.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/observer/test_observer_ray.py` & `dplutils-0.5.2/tests/observer/test_observer_ray.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_executor_base.py` & `dplutils-0.5.2/tests/pipeline/test_executor_base.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_pipeline_graph.py` & `dplutils-0.5.2/tests/pipeline/test_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_pipeline_task.py` & `dplutils-0.5.2/tests/pipeline/test_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_ray_executor.py` & `dplutils-0.5.2/tests/pipeline/test_ray_executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_ray_stream_executor.py` & `dplutils-0.5.2/tests/pipeline/test_ray_stream_executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_stream_executor.py` & `dplutils-0.5.2/tests/pipeline/test_stream_executor.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tests/pipeline/test_suite.py` & `dplutils-0.5.2/tests/pipeline/test_suite.py`

 * *Files identical despite different names*

### Comparing `dplutils-0.5.1/tox.ini` & `dplutils-0.5.2/tox.ini`

 * *Files identical despite different names*

