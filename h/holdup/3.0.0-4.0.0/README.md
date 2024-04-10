# Comparing `tmp/holdup-3.0.0.tar.gz` & `tmp/holdup-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holdup-3.0.0.tar", last modified: Sun Mar 20 15:58:58 2022, max compression
+gzip compressed data, was "holdup-4.0.0.tar", last modified: Mon Feb 13 22:22:54 2023, max compression
```

## Comparing `holdup-3.0.0.tar` & `holdup-4.0.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.225861 holdup-3.0.0/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      630 2022-03-20 15:58:49.000000 holdup-3.0.0/.bumpversion.cfg
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1825 2022-03-18 14:48:13.000000 holdup-3.0.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      174 2022-03-18 14:48:12.000000 holdup-3.0.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2019-05-22 22:01:47.000000 holdup-3.0.0/.dockerignore
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2022-03-18 14:48:12.000000 holdup-3.0.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.220861 holdup-3.0.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.222861 holdup-3.0.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3690 2022-03-20 14:58:16.000000 holdup-3.0.0/.github/workflows/github-actions.yml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      666 2022-03-18 14:48:12.000000 holdup-3.0.0/.gitignore
--rw-r--r--   0 ionel     (1000) ionel     (1000)      637 2022-03-18 14:50:29.000000 holdup-3.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2022-03-18 14:48:12.000000 holdup-3.0.0/.readthedocs.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      162 2022-03-18 14:50:29.000000 holdup-3.0.0/AUTHORS.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2398 2022-03-20 15:55:02.000000 holdup-3.0.0/CHANGELOG.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2402 2022-03-18 14:48:12.000000 holdup-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      456 2022-03-20 15:21:16.000000 holdup-3.0.0/Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2022-03-18 14:50:29.000000 holdup-3.0.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)      448 2022-03-20 15:21:10.000000 holdup-3.0.0/MANIFEST.in
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7152 2022-03-20 15:58:58.225861 holdup-3.0.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     5073 2022-03-20 15:58:49.000000 holdup-3.0.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.222861 holdup-3.0.0/ci/
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     3063 2022-03-18 14:48:12.000000 holdup-3.0.0/ci/bootstrap.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       66 2022-03-18 14:48:12.000000 holdup-3.0.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.220861 holdup-3.0.0/ci/templates/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.220861 holdup-3.0.0/ci/templates/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.222861 holdup-3.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1977 2022-03-20 14:58:05.000000 holdup-3.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.223861 holdup-3.0.0/docs/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/authors.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/changelog.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1264 2022-03-20 15:58:49.000000 holdup-3.0.0/docs/conf.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/contributing.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      244 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       86 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/installation.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/readme.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.223861 holdup-3.0.0/docs/reference/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       94 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/reference/holdup.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       58 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/reference/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       41 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/requirements.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       64 2022-03-18 14:48:12.000000 holdup-3.0.0/docs/usage.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      160 2022-03-18 14:48:12.000000 holdup-3.0.0/pyproject.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      564 2022-03-20 15:58:58.225861 holdup-3.0.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     3198 2022-03-20 15:58:49.000000 holdup-3.0.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.221861 holdup-3.0.0/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.223861 holdup-3.0.0/src/holdup/
--rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2022-03-20 15:58:49.000000 holdup-3.0.0/src/holdup/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      381 2022-03-18 14:50:29.000000 holdup-3.0.0/src/holdup/__main__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    14981 2022-03-18 15:50:56.000000 holdup-3.0.0/src/holdup/cli.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.224861 holdup-3.0.0/src/holdup.egg-info/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     7152 2022-03-20 15:58:58.000000 holdup-3.0.0/src/holdup.egg-info/PKG-INFO
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1031 2022-03-20 15:58:58.000000 holdup-3.0.0/src/holdup.egg-info/SOURCES.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2022-03-20 15:58:58.000000 holdup-3.0.0/src/holdup.egg-info/dependency_links.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       44 2022-03-20 15:58:58.000000 holdup-3.0.0/src/holdup.egg-info/entry_points.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2018-11-23 21:50:52.000000 holdup-3.0.0/src/holdup.egg-info/not-zip-safe
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      115 2022-03-20 15:58:58.000000 holdup-3.0.0/src/holdup.egg-info/requires.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        7 2022-03-20 15:58:58.000000 holdup-3.0.0/src/holdup.egg-info/top_level.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2022-03-20 15:58:58.224861 holdup-3.0.0/tests/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3024 2022-03-20 15:20:45.000000 holdup-3.0.0/tests/Dockerfile
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      233 2019-05-23 16:13:09.000000 holdup-3.0.0/tests/conftest.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      299 2020-12-16 14:31:22.000000 holdup-3.0.0/tests/docker-compose.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     8743 2022-03-18 20:50:57.000000 holdup-3.0.0/tests/test_holdup.py
--rwxrwxr-x   0 ionel     (1000) ionel     (1000)      650 2019-05-26 20:51:27.000000 holdup-3.0.0/tests/test_pg.py
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)      520 2022-03-20 14:58:27.000000 holdup-3.0.0/tests/test_pg.sh
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1784 2022-03-20 15:42:50.000000 holdup-3.0.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.595526 holdup-4.0.0/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      630 2023-02-13 22:22:39.000000 holdup-4.0.0/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1891 2023-02-13 20:53:55.000000 holdup-4.0.0/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      174 2022-03-18 14:48:12.000000 holdup-4.0.0/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2019-05-22 22:01:47.000000 holdup-4.0.0/.dockerignore
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2022-03-18 14:48:12.000000 holdup-4.0.0/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.590526 holdup-4.0.0/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.593526 holdup-4.0.0/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     6556 2023-02-13 20:53:55.000000 holdup-4.0.0/.github/workflows/github-actions.yml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      666 2022-03-18 14:48:12.000000 holdup-4.0.0/.gitignore
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      637 2023-02-13 20:53:55.000000 holdup-4.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2022-03-18 14:48:12.000000 holdup-4.0.0/.readthedocs.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      162 2022-03-18 14:50:29.000000 holdup-4.0.0/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2640 2023-02-13 22:21:24.000000 holdup-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2397 2023-02-13 20:53:55.000000 holdup-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      456 2022-03-20 15:21:16.000000 holdup-4.0.0/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2023-02-13 20:53:55.000000 holdup-4.0.0/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      468 2023-02-13 20:53:55.000000 holdup-4.0.0/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7395 2023-02-13 22:22:54.595526 holdup-4.0.0/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     5073 2023-02-13 22:22:39.000000 holdup-4.0.0/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.593526 holdup-4.0.0/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2930 2023-02-13 20:53:55.000000 holdup-4.0.0/ci/bootstrap.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       72 2023-02-13 20:53:55.000000 holdup-4.0.0/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.591526 holdup-4.0.0/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.591526 holdup-4.0.0/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.593526 holdup-4.0.0/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1977 2023-02-13 20:53:55.000000 holdup-4.0.0/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.594526 holdup-4.0.0/docs/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/authors.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/changelog.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1233 2023-02-13 22:22:39.000000 holdup-4.0.0/docs/conf.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/contributing.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      244 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       86 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/installation.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/readme.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.594526 holdup-4.0.0/docs/reference/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       94 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/reference/holdup.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       58 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/reference/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       41 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/requirements.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       64 2022-03-18 14:48:12.000000 holdup-4.0.0/docs/usage.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      127 2023-02-13 20:53:55.000000 holdup-4.0.0/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      825 2023-02-13 20:53:55.000000 holdup-4.0.0/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      314 2023-02-13 22:22:54.595526 holdup-4.0.0/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     3085 2023-02-13 22:22:39.000000 holdup-4.0.0/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.591526 holdup-4.0.0/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.594526 holdup-4.0.0/src/holdup/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2023-02-13 22:22:39.000000 holdup-4.0.0/src/holdup/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      381 2022-03-18 14:50:29.000000 holdup-4.0.0/src/holdup/__main__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    15135 2023-02-13 20:53:55.000000 holdup-4.0.0/src/holdup/cli.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.595526 holdup-4.0.0/src/holdup.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7395 2023-02-13 22:22:54.000000 holdup-4.0.0/src/holdup.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1042 2023-02-13 22:22:54.000000 holdup-4.0.0/src/holdup.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-02-13 22:22:54.000000 holdup-4.0.0/src/holdup.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       44 2023-02-13 22:22:54.000000 holdup-4.0.0/src/holdup.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2023-02-13 22:22:53.000000 holdup-4.0.0/src/holdup.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       14 2023-02-13 22:22:54.000000 holdup-4.0.0/src/holdup.egg-info/requires.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2023-02-13 22:22:54.000000 holdup-4.0.0/src/holdup.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2023-02-13 22:22:54.595526 holdup-4.0.0/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3024 2022-03-20 15:20:45.000000 holdup-4.0.0/tests/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      233 2023-02-13 20:53:55.000000 holdup-4.0.0/tests/conftest.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      299 2020-12-16 14:31:22.000000 holdup-4.0.0/tests/docker-compose.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    10421 2023-02-13 21:49:55.000000 holdup-4.0.0/tests/test_holdup.py
+-rwxrwxr-x   0 ionel     (1000) ionel     (1000)      650 2019-05-26 20:51:27.000000 holdup-4.0.0/tests/test_pg.py
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)      520 2022-03-20 14:58:27.000000 holdup-4.0.0/tests/test_pg.sh
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1878 2023-02-13 20:53:55.000000 holdup-4.0.0/tox.ini
```

### Comparing `holdup-3.0.0/.bumpversion.cfg` & `holdup-4.0.0/.bumpversion.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [bumpversion]
-current_version = 3.0.0
+current_version = 4.0.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
-search = version='{current_version}'
-replace = version='{new_version}'
+search = version="{current_version}"
+replace = version="{new_version}"
 
 [bumpversion:file (badge):README.rst]
 search = /v{current_version}.svg
 replace = /v{new_version}.svg
 
 [bumpversion:file (link):README.rst]
 search = /v{current_version}...master
 replace = /v{new_version}...master
 
 [bumpversion:file:docs/conf.py]
-search = version = release = '{current_version}'
-replace = version = release = '{new_version}'
+search = version = release = "{current_version}"
+replace = version = release = "{new_version}"
 
 [bumpversion:file:src/holdup/__init__.py]
-search = __version__ = '{current_version}'
-replace = __version__ = '{new_version}'
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
```

### Comparing `holdup-3.0.0/.cookiecutterrc` & `holdup-4.0.0/.cookiecutterrc`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # Generated by cookiepatcher, a small shim around cookiecutter (pip install cookiepatcher)
 
 default_context:
-    allow_tests_inside_package: no
-    appveyor: no
+    allow_tests_inside_package: 'no'
+    appveyor: 'no'
     c_extension_function: '-'
     c_extension_module: '-'
-    c_extension_optional: no
-    c_extension_support: no
-    c_extension_test_pypi: no
+    c_extension_optional: 'no'
+    c_extension_support: 'no'
+    c_extension_test_pypi: 'no'
     c_extension_test_pypi_username: ionelmc
-    codacy: no
+    codacy: 'no'
     codacy_projectid: '[Get ID from https://app.codacy.com/app/ionelmc/python-holdup/settings]'
-    codeclimate: no
-    codecov: no
+    codeclimate: 'no'
+    codecov: 'no'
     command_line_interface: argparse
     command_line_interface_bin_name: holdup
-    coveralls: yes
+    coveralls: 'yes'
     distribution_name: holdup
     email: contact@ionelmc.ro
     full_name: Ionel Cristian Mărieș
-    github_actions: yes
-    legacy_python: no
+    github_actions: 'yes'
+    github_actions_osx: 'yes'
+    github_actions_windows: 'yes'
     license: BSD 2-Clause License
     linter: flake8
     package_name: holdup
-    pre_commit: yes
+    pre_commit: 'yes'
     pre_commit_formatter: black
     project_name: Holdup
     project_short_description: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
-    pypi_badge: yes
-    pypi_disable_upload: no
+    pypi_badge: 'yes'
+    pypi_disable_upload: 'no'
     release_date: '2021-04-08'
     repo_hosting: github.com
     repo_hosting_domain: github.com
     repo_main_branch: master
     repo_name: python-holdup
     repo_username: ionelmc
-    requiresio: yes
-    scrutinizer: no
-    setup_py_uses_setuptools_scm: no
-    setup_py_uses_test_runner: no
-    sphinx_docs: yes
+    requiresio: 'yes'
+    scrutinizer: 'no'
+    setup_py_uses_pytest_runner: 'no'
+    setup_py_uses_setuptools_scm: 'no'
+    sphinx_docs: 'yes'
     sphinx_docs_hosting: https://python-holdup.readthedocs.io/
-    sphinx_doctest: no
+    sphinx_doctest: 'no'
     sphinx_theme: sphinx-py3doc-enhanced-theme
-    test_matrix_configurator: no
-    test_matrix_separate_coverage: no
-    test_runner: pytest
-    travis: no
-    travis_osx: no
-    version: 2.0.0
+    test_matrix_configurator: 'no'
+    test_matrix_separate_coverage: 'no'
+    travis: 'no'
+    travis_osx: 'no'
+    version: 3.0.0
     version_manager: bump2version
     website: https://blog.ionelmc.ro
     year_from: '2016'
-    year_to: '2022'
+    year_to: '2023'
```

### Comparing `holdup-3.0.0/.gitignore` & `holdup-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `holdup-3.0.0/.pre-commit-config.yaml` & `holdup-4.0.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # To install the git pre-commit hook run:
 #   pre-commit install
 # To update the pre-commit hooks run:
 #   pre-commit install-hooks
 exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
-    hooks:
-      - id: flake8
   - repo: https://github.com/psf/black
-    rev: 22.1.0
+    rev: 23.1.0
     hooks:
       - id: black
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
+    hooks:
+      - id: flake8
```

### Comparing `holdup-3.0.0/CHANGELOG.rst` & `holdup-4.0.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 Changelog
 =========
 
+4.0.0 (2023-02-14)
+------------------
+
+* Added support for psycopg 3 (now the ``holdup[pg]`` extra will require that). The old psycopg2 is still supported for now.
+* Dropped support for Python 3.6 and added in Python 3.11 in the test suite.
+
 3.0.0 (2022-03-20)
 ------------------
 
 * Dropped support for Python 2.
 * Switched CI from Travis to GitHub Actions.
 * Fixed bugs with password masking (it wasn't working for postgresql URIs).
```

### Comparing `holdup-3.0.0/CONTRIBUTING.rst` & `holdup-4.0.0/CONTRIBUTING.rst`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-4. When you're done making changes run all the checks and docs builder with `tox <https://tox.readthedocs.io/en/latest/install.html>`_ one command::
+4. When you're done making changes run all the checks and docs builder with `tox <https://tox.wiki/en/latest/installation.html>`_ one command::
 
     tox
 
 5. Commit your changes and push your branch to GitHub::
 
     git add .
     git commit -m "Your detailed description of your changes."
```

### Comparing `holdup-3.0.0/LICENSE` & `holdup-4.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2016-2022, Ionel Cristian Mărieș. All rights reserved.
+Copyright (c) 2016-2023, Ionel Cristian Mărieș. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
 following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
 disclaimer.
```

### Comparing `holdup-3.0.0/PKG-INFO` & `holdup-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holdup
-Version: 3.0.0
+Version: 4.0.0
 Summary: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
 Home-page: https://github.com/ionelmc/python-holdup
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-holdup.readthedocs.io/
 Project-URL: Changelog, https://python-holdup.readthedocs.io/en/latest/changelog.html
@@ -16,23 +16,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: pg
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
@@ -135,14 +135,20 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+4.0.0 (2023-02-14)
+------------------
+
+* Added support for psycopg 3 (now the ``holdup[pg]`` extra will require that). The old psycopg2 is still supported for now.
+* Dropped support for Python 3.6 and added in Python 3.11 in the test suite.
+
 3.0.0 (2022-03-20)
 ------------------
 
 * Dropped support for Python 2.
 * Switched CI from Travis to GitHub Actions.
 * Fixed bugs with password masking (it wasn't working for postgresql URIs).
```

### Comparing `holdup-3.0.0/README.rst` & `holdup-4.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/holdup
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/holdup.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/holdup
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-holdup/v3.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-holdup/v4.0.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-holdup/compare/v3.0.0...master
+    :target: https://github.com/ionelmc/python-holdup/compare/v4.0.0...master
 
 
 
 .. end-badges
 
 A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services
 (like almost everything).
```

### Comparing `holdup-3.0.0/ci/bootstrap.py` & `holdup-4.0.0/ci/bootstrap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,81 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from __future__ import absolute_import
-from __future__ import print_function
-from __future__ import unicode_literals
-
 import os
+import pathlib
 import subprocess
 import sys
-from os.path import abspath
-from os.path import dirname
-from os.path import exists
-from os.path import join
-from os.path import relpath
 
-base_path = dirname(dirname(abspath(__file__)))
-templates_path = join(base_path, "ci", "templates")
+base_path: pathlib.Path = pathlib.Path(__file__).resolve().parent.parent
+templates_path = base_path / "ci" / "templates"
 
 
 def check_call(args):
     print("+", *args)
     subprocess.check_call(args)
 
 
 def exec_in_env():
-    env_path = join(base_path, ".tox", "bootstrap")
+    env_path = base_path / ".tox" / "bootstrap"
     if sys.platform == "win32":
-        bin_path = join(env_path, "Scripts")
+        bin_path = env_path / "Scripts"
     else:
-        bin_path = join(env_path, "bin")
-    if not exists(env_path):
+        bin_path = env_path / "bin"
+    if not env_path.exists():
         import subprocess
 
         print("Making bootstrap env in: {0} ...".format(env_path))
         try:
             check_call([sys.executable, "-m", "venv", env_path])
         except subprocess.CalledProcessError:
             try:
                 check_call([sys.executable, "-m", "virtualenv", env_path])
             except subprocess.CalledProcessError:
                 check_call(["virtualenv", env_path])
         print("Installing `jinja2` into bootstrap environment...")
-        check_call([join(bin_path, "pip"), "install", "jinja2", "tox"])
-    python_executable = join(bin_path, "python")
-    if not os.path.exists(python_executable):
-        python_executable += '.exe'
+        check_call([bin_path / "pip", "install", "jinja2", "tox"])
+    python_executable = bin_path / "python"
+    if not python_executable.exists():
+        python_executable = python_executable.with_suffix(".exe")
 
     print("Re-executing with: {0}".format(python_executable))
     print("+ exec", python_executable, __file__, "--no-env")
     os.execv(python_executable, [python_executable, __file__, "--no-env"])
 
 
 def main():
     import jinja2
 
     print("Project path: {0}".format(base_path))
 
     jinja = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(templates_path),
+        loader=jinja2.FileSystemLoader(str(templates_path)),
         trim_blocks=True,
         lstrip_blocks=True,
         keep_trailing_newline=True,
     )
 
     tox_environments = [
         line.strip()
         # 'tox' need not be installed globally, but must be importable
         # by the Python that is running this script.
         # This uses sys.executable the same way that the call in
         # cookiecutter-pylibrary/hooks/post_gen_project.py
         # invokes this bootstrap.py itself.
-        for line in subprocess.check_output([sys.executable, '-m', 'tox', '--listenvs'], universal_newlines=True).splitlines()
+        for line in subprocess.check_output([sys.executable, "-m", "tox", "--listenvs"], universal_newlines=True).splitlines()
     ]
-    tox_environments = [line for line in tox_environments if line.startswith('py')]
+    tox_environments = [line for line in tox_environments if line.startswith("py")]
 
-    for root, _, files in os.walk(templates_path):
-        for name in files:
-            relative = relpath(root, templates_path)
-            with open(join(base_path, relative, name), "w") as fh:
-                fh.write(jinja.get_template(join(relative, name)).render(tox_environments=tox_environments))
-            print("Wrote {}".format(name))
+    for template in templates_path.rglob("*"):
+        if template.is_file():
+            template_path = str(template.relative_to(templates_path))
+            destination = base_path / template_path
+            destination.parent.mkdir(parents=True, exist_ok=True)
+            destination.write_text(jinja.get_template(template_path).render(tox_environments=tox_environments))
+            print("Wrote {}".format(template_path))
     print("DONE.")
 
 
 if __name__ == "__main__":
     args = sys.argv[1:]
     if args == ["--no-env"]:
         main()
```

### Comparing `holdup-3.0.0/ci/templates/.github/workflows/github-actions.yml` & `holdup-4.0.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,18 @@
             toxpython: '{{ toxpython }}'
             python_arch: '{{ python_arch }}'
             tox_env: '{{ env }}{% if 'cover' in env %},codecov{% endif %}'
             os: '{{ os }}-latest'
 {% endfor %}
 {% endfor %}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       with:
         python-version: {{ '${{ matrix.python }}' }}
         architecture: {{ '${{ matrix.python_arch }}' }}
     - name: install dependencies
       run: |
         python -mpip install --progress-bar=off -r ci/requirements.txt
         virtualenv --version
```

### Comparing `holdup-3.0.0/docs/conf.py` & `holdup-4.0.0/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
-
 import sphinx_py3doc_enhanced_theme
 
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.extlinks',
-    'sphinx.ext.ifconfig',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.todo',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.extlinks",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
 ]
-source_suffix = '.rst'
-master_doc = 'index'
-project = 'Holdup'
-year = '2016-2022'
-author = 'Ionel Cristian Mărieș'
-copyright = '{0}, {1}'.format(year, author)
-version = release = '3.0.0'
+source_suffix = ".rst"
+master_doc = "index"
+project = "Holdup"
+year = "2016-2023"
+author = "Ionel Cristian Mărieș"
+copyright = "{0}, {1}".format(year, author)
+version = release = "4.0.0"
 
-pygments_style = 'trac'
-templates_path = ['.']
+pygments_style = "trac"
+templates_path = ["."]
 extlinks = {
-    'issue': ('https://github.com/ionelmc/python-holdup/issues/%s', '#'),
-    'pr': ('https://github.com/ionelmc/python-holdup/pull/%s', 'PR #'),
+    "issue": ("https://github.com/ionelmc/python-holdup/issues/%s", "issue #%s"),
+    "pr": ("https://github.com/ionelmc/python-holdup/pull/%s", "PR #%s"),
 }
 html_theme = "sphinx_py3doc_enhanced_theme"
 html_theme_path = [sphinx_py3doc_enhanced_theme.get_html_theme_path()]
 html_theme_options = {
-    'githuburl': 'https://github.com/ionelmc/python-holdup/',
+    "githuburl": "https://github.com/ionelmc/python-holdup/",
 }
 
 html_use_smartypants = True
-html_last_updated_fmt = '%b %d, %Y'
+html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
 html_sidebars = {
-    '**': ['searchbox.html', 'globaltoc.html', 'sourcelink.html'],
+    "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
 }
-html_short_title = '%s-%s' % (project, version)
+html_short_title = "%s-%s" % (project, version)
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
```

### Comparing `holdup-3.0.0/setup.py` & `holdup-4.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,75 +10,74 @@
 from os.path import splitext
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 def read(*names, **kwargs):
-    with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
+    with io.open(join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
-    name='holdup',
-    version='3.0.0',
-    license='BSD-2-Clause',
+    name="holdup",
+    version="4.0.0",
+    license="BSD-2-Clause",
     description=(
-        'A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services '
-        '(like almost everything).'
+        "A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services "
+        "(like almost everything)."
     ),
-    long_description='{}\n{}'.format(
-        re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
-        re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
+    long_description="{}\n{}".format(
+        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
+        re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
-    author='Ionel Cristian Mărieș',
-    author_email='contact@ionelmc.ro',
-    url='https://github.com/ionelmc/python-holdup',
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
-    py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
+    author="Ionel Cristian Mărieș",
+    author_email="contact@ionelmc.ro",
+    url="https://github.com/ionelmc/python-holdup",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: Unix',
-        'Operating System :: POSIX',
-        'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: Unix",
+        "Operating System :: POSIX",
+        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
         # uncomment if you test on these interpreters:
         # 'Programming Language :: Python :: Implementation :: IronPython',
         # 'Programming Language :: Python :: Implementation :: Jython',
         # 'Programming Language :: Python :: Implementation :: Stackless',
-        'Topic :: Utilities',
+        "Topic :: Utilities",
     ],
     project_urls={
-        'Documentation': 'https://python-holdup.readthedocs.io/',
-        'Changelog': 'https://python-holdup.readthedocs.io/en/latest/changelog.html',
-        'Issue Tracker': 'https://github.com/ionelmc/python-holdup/issues',
+        "Documentation": "https://python-holdup.readthedocs.io/",
+        "Changelog": "https://python-holdup.readthedocs.io/en/latest/changelog.html",
+        "Issue Tracker": "https://github.com/ionelmc/python-holdup/issues",
     },
-    keywords=['wait', 'port', 'service', 'docker', 'unix', 'domain', 'socket', 'tcp', 'waiter', 'holdup', 'hold-up'],
-    python_requires='>=3.6',
+    keywords=["wait", "port", "service", "docker", "unix", "domain", "socket", "tcp", "waiter", "holdup", "hold-up"],
+    python_requires=">=3.7",
     install_requires=[
         # eg: 'aspectlib==1.1.1', 'six>=1.7',
     ],
     extras_require={
-        'pg:platform_python_implementation=="PyPy"': ['psycopg2cffi'],
-        'pg:platform_python_implementation=="CPython"': ['psycopg2'],
+        "pg": ["psycopg"],
     },
     entry_points={
-        'console_scripts': [
-            'holdup = holdup.cli:main',
+        "console_scripts": [
+            "holdup = holdup.cli:main",
         ]
     },
 )
```

### Comparing `holdup-3.0.0/src/holdup/cli.py` & `holdup-4.0.0/src/holdup/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,40 +11,43 @@
     ``holdup.__main__`` in ``sys.modules``.
   - When you import __main__ it will get executed again (as a module) because
     there's no ``holdup.__main__`` in ``sys.modules``.
 
   Also see (1) from http://click.pocoo.org/5/setuptools/#setuptools-integration
 """
 
-from __future__ import print_function
-
 import argparse
 import ast
 import os
 import re
 import socket
 import ssl
 import sys
 from contextlib import closing
 from operator import methodcaller
 from time import sleep
 from time import time
 
 try:
-    import psycopg2
+    import psycopg
 except ImportError:
     try:
-        import psycopg2cffi as psycopg2
+        import psycopg2 as psycopg
     except ImportError:
-        psycopg2 = None
-
+        try:
+            import psycopg2cffi as psycopg
+        except ImportError:
+            psycopg = None
 try:
-    from psycopg2.extensions import make_dsn
+    from psycopg.conninfo import make_conninfo
 except ImportError:
-    make_dsn = lambda value: value  # noqa
+    try:
+        from psycopg2.extensions import make_dsn as make_conninfo
+    except ImportError:
+        make_conninfo = lambda value: value  # noqa
 
 import builtins
 from pipes import quote
 from urllib.parse import urlparse
 from urllib.parse import urlunparse
 from urllib.request import HTTPBasicAuthHandler
 from urllib.request import HTTPDigestAuthHandler
@@ -60,39 +63,39 @@
         try:
             self.run(options)
         except Exception as exc:
             self.error = exc
         else:
             self.error = False
             if options.verbose:
-                print(f'holdup: Passed check: {self.display(verbose=True, verbose_passwords=options.verbose_passwords)}')
+                print(f"holdup: Passed check: {self.display(verbose=True, verbose_passwords=options.verbose_passwords)}")
             return True
 
     def run(self, options):
         raise NotImplementedError
 
     @property
     def status(self):
         if self.error:
-            return f'{self.error}'
+            return f"{self.error}"
         elif self.error is None:
-            return 'PENDING'
+            return "PENDING"
         else:
-            return 'PASSED'
+            return "PASSED"
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({repr(self.__dict__)[1:-1]})'
+        return f"{self.__class__.__name__}({repr(self.__dict__)[1:-1]})"
 
     def display_definition(self, **kwargs):
         raise NotImplementedError
 
     def display(self, *, verbose, **kwargs):
         definition = self.display_definition(**kwargs)
         if verbose:
-            return f'{definition!r} -> {self.status}'
+            return f"{definition!r} -> {self.status}"
         else:
             return definition
 
 
 class TcpCheck(Check):
     def __init__(self, host, port):
         self.host = host
@@ -101,62 +104,62 @@
     def run(self, options):
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(options.check_timeout)
         with closing(sock):
             sock.connect((self.host, self.port))
 
     def __repr__(self):
-        return f'TcpCheck(host={self.host!r}, port={self.port!r})'
+        return f"TcpCheck(host={self.host!r}, port={self.port!r})"
 
     def display(self, *, verbose, **_):
-        definition = f'tcp://{self.host}:{self.port}'
+        definition = f"tcp://{self.host}:{self.port}"
         if verbose:
-            return f'{definition!r} -> {self.status}'
+            return f"{definition!r} -> {self.status}"
         else:
             return definition
 
 
 class PgCheck(Check):
     def __init__(self, connection_string):
         self.connection_string = connection_string
-        if '?' in connection_string.rsplit('/', 1)[1]:
-            self.separator = '&'
+        if "?" in connection_string.rsplit("/", 1)[1]:
+            self.separator = "&"
         else:
-            self.separator = '?'
+            self.separator = "?"
 
     def run(self, options):
         with closing(
-            psycopg2.connect(f'{self.connection_string}{self.separator}connect_timeout={max(1, int(options.check_timeout))}')
+            psycopg.connect(f"{self.connection_string}{self.separator}connect_timeout={max(1, int(options.check_timeout))}")
         ) as conn:
             with closing(conn.cursor()) as cur:
-                cur.execute('SELECT version()')
+                cur.execute("SELECT version()")
                 cur.fetchone()
 
     def __repr__(self):
-        return f'PgCheck({self.connection_string})'
+        return f"PgCheck({self.connection_string})"
 
-    def display_definition(self, *, verbose_passwords, _password_re=re.compile(r':[^@:]+@')):
+    def display_definition(self, *, verbose_passwords, _password_re=re.compile(r":[^@:]+@")):
         definition = str(self.connection_string)
         if not verbose_passwords:
-            definition = _password_re.sub(':******@', definition, 1)
+            definition = _password_re.sub(":******@", definition, 1)
         return definition
 
 
 class HttpCheck(Check):
     def __init__(self, url):
         self.handlers = []
         self.parsed_url = url = urlparse(url)
         self.scheme = url.scheme
         self.insecure = False
-        if url.scheme == 'https+insecure':
+        if url.scheme == "https+insecure":
             self.insecure = True
-            url = url._replace(scheme='https')
+            url = url._replace(scheme="https")
 
         if url.port:
-            self.netloc = f'{self.hostname}:{self.port}'
+            self.netloc = f"{self.hostname}:{self.port}"
         else:
             self.netloc = url.hostname
 
         cleaned_url = urlunparse(url._replace(netloc=self.netloc))
 
         if url.username or url.password:
             password_mgr = HTTPPasswordMgrWithDefaultRealm()
@@ -177,61 +180,61 @@
         handlers.append(HTTPSHandler(context=ssl_ctx))
 
         opener = build_opener(*handlers)
 
         with closing(opener.open(self.url, timeout=options.check_timeout)) as req:
             status = req.getcode()
             if status != 200:
-                raise Exception(f'Expected status code 200, got {status!r}')
+                raise Exception(f"Expected status code 200, got {status!r}")
 
     def __repr__(self):
-        return f'HttpCheck({self.url}, insecure={self.do_insecure}, status={self.status})'
+        return f"HttpCheck({self.url}, insecure={self.do_insecure}, status={self.status})"
 
     def display_definition(self, *, verbose_passwords):
         url = self.parsed_url
         if not verbose_passwords:
             if not url.password:
-                mask = '******'
+                mask = "******"
             else:
-                mask = f'{url.username}:******'
-            url = url._replace(netloc=f'{mask}@{self.netloc}')
+                mask = f"{url.username}:******"
+            url = url._replace(netloc=f"{mask}@{self.netloc}")
         return urlunparse(url)
 
 
 class UnixCheck(Check):
     def __init__(self, path):
         self.path = path
 
     def run(self, options):
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.settimeout(options.check_timeout)
         with closing(sock):
             sock.connect(self.path)
 
     def __repr__(self):
-        return f'UnixCheck({self.path!r}, status={self.status})'
+        return f"UnixCheck({self.path!r}, status={self.status})"
 
     def display_definition(self, **_):
-        return f'unix://{self.path}'
+        return f"unix://{self.path}"
 
 
 class PathCheck(Check):
     def __init__(self, path):
         self.path = path
 
     def run(self, _):
         os.stat(self.path)
         if not os.access(self.path, os.R_OK):
-            raise Exception(f'Failed access({self.path!r}, R_OK) test')
+            raise Exception(f"Failed access({self.path!r}, R_OK) test")
 
     def __repr__(self):
-        return f'PathCheck({self.path!r}, status={self.status})'
+        return f"PathCheck({self.path!r}, status={self.status})"
 
     def display_definition(self, **_):
-        return f'path://{self.path}'
+        return f"path://{self.path}"
 
 
 class EvalCheck(Check):
     def __init__(self, expr):
         self.expr = expr
         self.ns = {}
         try:
@@ -240,150 +243,150 @@
             raise argparse.ArgumentTypeError(f'Invalid service spec {expr!r}. Parse error:\n  {exc.text} {" " * exc.offset}^\n{exc}')
         for node in ast.walk(tree):
             if isinstance(node, ast.Name):
                 if not hasattr(builtins, node.id):
                     try:
                         __import__(node.id)
                     except ImportError as exc:
-                        raise argparse.ArgumentTypeError(f'Invalid service spec {expr!r}. Import error: {exc}')
+                        raise argparse.ArgumentTypeError(f"Invalid service spec {expr!r}. Import error: {exc}")
                     self.ns[node.id] = sys.modules[node.id]
 
     def run(self, _):
         result = eval(self.expr, dict(self.ns), dict(self.ns))
         if not result:
-            raise Exception(f'Failed to evaluate {self.expr!r}. Result {result!r} is falsey')
+            raise Exception(f"Failed to evaluate {self.expr!r}. Result {result!r} is falsey")
 
     def __repr__(self):
-        return f'EvalCheck({self.expr!r}, ns={self.ns!r}, status={self.status})'
+        return f"EvalCheck({self.expr!r}, ns={self.ns!r}, status={self.status})"
 
     def display_definition(self, **_):
-        return f'eval://{self.expr}'
+        return f"eval://{self.expr}"
 
 
 class AnyCheck(Check):
     def __init__(self, checks):
         self.checks = checks
 
     def run(self, options):
         for check in self.checks:
             if check.is_passing(options):
                 break
         else:
-            raise Exception('ALL FAILED')
+            raise Exception("ALL FAILED")
 
     def __repr__(self):
         return f'AnyCheck({", ".join(map(repr, self.checks))}, status={self.status})'
 
     def display(self, *, verbose, **kwargs):
-        checks = ', '.join(map(methodcaller('display', verbose=verbose, **kwargs), self.checks))
+        checks = ", ".join(map(methodcaller("display", verbose=verbose, **kwargs), self.checks))
         if verbose:
-            return f'any({checks}) -> {self.status}'
+            return f"any({checks}) -> {self.status}"
         else:
-            return f'any({checks})'
+            return f"any({checks})"
 
 
 def parse_service(service):
-    if '://' not in service:
+    if "://" not in service:
         raise argparse.ArgumentTypeError(f'Invalid service spec {service!r}. Must have "://".')
-    proto, value = service.split('://', 1)
+    proto, value = service.split("://", 1)
 
-    if ',' in value and proto != 'eval':
-        parts = value.split(',')
+    if "," in value and proto != "eval":
+        parts = value.split(",")
         for pos, part in enumerate(parts):
-            if part.startswith('eval://'):
-                parts[pos] = ','.join(parts[pos:])
+            if part.startswith("eval://"):
+                parts[pos] = ",".join(parts[pos:])
                 del parts[pos + 1 :]
                 break
         return AnyCheck([parse_value(part, proto) for part in parts])
     else:
         return parse_value(value, proto)
 
 
 def parse_value(value, proto):
-    if '://' in value:
-        proto, value = value.split('://', 1)
-    display_value = f'{proto}://{value}'
+    if "://" in value:
+        proto, value = value.split("://", 1)
+    display_value = f"{proto}://{value}"
 
-    if proto == 'tcp':
-        if ':' not in value:
+    if proto == "tcp":
+        if ":" not in value:
             raise argparse.ArgumentTypeError(f'Invalid service spec {display_value!r}. Must have ":". Where\'s the port?')
-        host, port = value.strip('/').split(':', 1)
+        host, port = value.strip("/").split(":", 1)
         if not port.isdigit():
-            raise argparse.ArgumentTypeError(f'Invalid service spec {display_value!r}. Port must be a number not {port!r}.')
+            raise argparse.ArgumentTypeError(f"Invalid service spec {display_value!r}. Port must be a number not {port!r}.")
         port = int(port)
         return TcpCheck(host, port)
-    elif proto in ('pg', 'postgresql', 'postgres'):
-        if psycopg2 is None:
-            raise argparse.ArgumentTypeError(f'Protocol {proto} unusable. Install holdup[pg].')
+    elif proto in ("pg", "postgresql", "postgres"):
+        if psycopg is None:
+            raise argparse.ArgumentTypeError(f"Protocol {proto} unusable. Install holdup[pg].")
 
-        uri = f'postgresql://{value}'
+        uri = f"postgresql://{value}"
         try:
-            connection_uri = make_dsn(uri)
+            connection_uri = make_conninfo(uri)
         except Exception as exc:
-            raise argparse.ArgumentTypeError(f'Failed to parse {display_value!r}: {exc}. Must be a valid connection URI.')
+            raise argparse.ArgumentTypeError(f"Failed to parse {display_value!r}: {exc}. Must be a valid connection URI.")
         return PgCheck(connection_uri)
-    elif proto == 'unix':
+    elif proto == "unix":
         return UnixCheck(value)
-    elif proto == 'path':
+    elif proto == "path":
         return PathCheck(value)
-    elif proto in ('http', 'https', 'https+insecure'):
-        return HttpCheck('%s://%s' % (proto, value))
-    elif proto == 'eval':
+    elif proto in ("http", "https", "https+insecure"):
+        return HttpCheck("%s://%s" % (proto, value))
+    elif proto == "eval":
         return EvalCheck(value)
     else:
         raise argparse.ArgumentTypeError(f'Unknown protocol {proto!r} in {display_value!r}. Must be "tcp", "path", "unix" or "pg".')
 
 
 parser = argparse.ArgumentParser(
-    usage='%(prog)s [-h] [-t SECONDS] [-T SECONDS] [-i SECONDS] [-n] service [service ...] ' '[-- command [arg [arg ...]]]',
-    description='Wait for services to be ready and optionally exec command.',
+    usage="%(prog)s [-h] [-t SECONDS] [-T SECONDS] [-i SECONDS] [-n] service [service ...] " "[-- command [arg [arg ...]]]",
+    description="Wait for services to be ready and optionally exec command.",
 )
 parser.add_argument(
-    'service',
+    "service",
     nargs=argparse.ONE_OR_MORE,
     type=parse_service,
-    help='A service to wait for. '
-    'Supported protocols: '
+    help="A service to wait for. "
+    "Supported protocols: "
     '"tcp://host:port/", '
     '"path:///path/to/something", '
     '"unix:///path/to/domain.sock", '
     '"eval://expr", '
     '"pg://user:password@host:port/dbname" ("postgres" and "postgresql" also allowed), '
     '"http://urn", '
     '"https://urn", '
     '"https+insecure://urn" (status 200 expected for http*). '
-    'Join protocols with a comma to make holdup exit at the first '
+    "Join protocols with a comma to make holdup exit at the first "
     'passing one, eg: "tcp://host:1,host:2" or "tcp://host:1,tcp://host:2" are equivalent and mean '
-    '`any that pass`.',
+    "`any that pass`.",
 )
-parser.add_argument('command', nargs=argparse.OPTIONAL, help='An optional command to exec.')
+parser.add_argument("command", nargs=argparse.OPTIONAL, help="An optional command to exec.")
 parser.add_argument(
-    '-t', '--timeout', metavar='SECONDS', type=float, default=60.0, help='Time to wait for services to be ready. Default: %(default)s'
+    "-t", "--timeout", metavar="SECONDS", type=float, default=60.0, help="Time to wait for services to be ready. Default: %(default)s"
 )
 parser.add_argument(
-    '-T', '--check-timeout', metavar='SECONDS', type=float, default=1.0, help='Time to wait for a single check. Default: %(default)s'
+    "-T", "--check-timeout", metavar="SECONDS", type=float, default=1.0, help="Time to wait for a single check. Default: %(default)s"
 )
-parser.add_argument('-i', '--interval', metavar='SECONDS', type=float, default=0.2, help='How often to check. Default: %(default)s')
-parser.add_argument('-v', '--verbose', action='store_true', help='Verbose mode.')
-parser.add_argument('--verbose-passwords', action='store_true', help='Disable PostgreSQL/HTTP password masking.')
+parser.add_argument("-i", "--interval", metavar="SECONDS", type=float, default=0.2, help="How often to check. Default: %(default)s")
+parser.add_argument("-v", "--verbose", action="store_true", help="Verbose mode.")
+parser.add_argument("--verbose-passwords", action="store_true", help="Disable PostgreSQL/HTTP password masking.")
 parser.add_argument(
-    '-n',
-    '--no-abort',
-    action='store_true',
-    help='Ignore failed services. ' 'This makes `holdup` return 0 exit code regardless of services actually responding.',
+    "-n",
+    "--no-abort",
+    action="store_true",
+    help="Ignore failed services. " "This makes `holdup` return 0 exit code regardless of services actually responding.",
 )
-parser.add_argument('--insecure', action='store_true', help='Disable SSL Certificate verification for HTTPS services.')
+parser.add_argument("--insecure", action="store_true", help="Disable SSL Certificate verification for HTTPS services.")
 
 
 def add_version_argument(parser):
     import holdup
 
     parser.add_argument(
-        '--version',
-        action='version',
+        "--version",
+        action="version",
         version=f"%(prog)s {holdup.__version__} from {holdup.__file__}",
         help="display the version of the holdup package and its location, then exit.",
     )
 
 
 def main():
     """
@@ -392,31 +395,31 @@
 
     Returns:
         int: A return code
 
     Does stuff.
     """
     add_version_argument(parser)
-    if '--' in sys.argv:
-        pos = sys.argv.index('--')
+    if "--" in sys.argv:
+        pos = sys.argv.index("--")
         argv, command = sys.argv[1:pos], sys.argv[pos + 1 :]
     else:
         argv, command = sys.argv[1:], None
     options = parser.parse_args(args=argv)
     if options.timeout < options.check_timeout:
         if options.check_timeout == 1.0:
             options.check_timeout = options.timeout
         else:
-            parser.error('--timeout value must be greater than --check-timeout value!')
+            parser.error("--timeout value must be greater than --check-timeout value!")
     pending = list(options.service)
-    brief_representer = methodcaller('display', verbose=False, verbose_passwords=options.verbose_passwords)
-    verbose_representer = methodcaller('display', verbose=True, verbose_passwords=options.verbose_passwords)
+    brief_representer = methodcaller("display", verbose=False, verbose_passwords=options.verbose_passwords)
+    verbose_representer = methodcaller("display", verbose=True, verbose_passwords=options.verbose_passwords)
     if options.verbose:
         print(
-            f'holdup: Waiting for {options.timeout}s ({options.check_timeout}s per check, {options.interval}s sleep between loops) '
+            f"holdup: Waiting for {options.timeout}s ({options.check_timeout}s per check, {options.interval}s sleep between loops) "
             f'for these services: {", ".join(map(brief_representer, pending))}'
         )
     start = time()
     at_least_once = True
     while at_least_once or pending and time() - start < options.timeout:
         lapse = time()
         pending = [check for check in pending if not check.is_passing(options)]
```

### Comparing `holdup-3.0.0/src/holdup.egg-info/PKG-INFO` & `holdup-4.0.0/src/holdup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holdup
-Version: 3.0.0
+Version: 4.0.0
 Summary: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
 Home-page: https://github.com/ionelmc/python-holdup
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-holdup.readthedocs.io/
 Project-URL: Changelog, https://python-holdup.readthedocs.io/en/latest/changelog.html
@@ -16,23 +16,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: pg
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
@@ -135,14 +135,20 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+4.0.0 (2023-02-14)
+------------------
+
+* Added support for psycopg 3 (now the ``holdup[pg]`` extra will require that). The old psycopg2 is still supported for now.
+* Dropped support for Python 3.6 and added in Python 3.11 in the test suite.
+
 3.0.0 (2022-03-20)
 ------------------
 
 * Dropped support for Python 2.
 * Switched CI from Travis to GitHub Actions.
 * Fixed bugs with password masking (it wasn't working for postgresql URIs).
```

### Comparing `holdup-3.0.0/src/holdup.egg-info/SOURCES.txt` & `holdup-4.0.0/src/holdup.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 Dockerfile
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
+pytest.ini
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
```

### Comparing `holdup-3.0.0/tests/Dockerfile` & `holdup-4.0.0/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `holdup-3.0.0/tests/test_pg.py` & `holdup-4.0.0/tests/test_pg.py`

 * *Files identical despite different names*

### Comparing `holdup-3.0.0/tests/test_pg.sh` & `holdup-4.0.0/tests/test_pg.sh`

 * *Files identical despite different names*

### Comparing `holdup-3.0.0/tox.ini` & `holdup-4.0.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -10,54 +10,57 @@
 ; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py36,py37,py38,py39,py310,pypy37,pypy38},
+    {py37,py38,py39,py310,py311,pypy38,pypy39}-{pg2,pg3},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
     pypy37: {env:TOXPYTHON:pypy3.7}
     pypy38: {env:TOXPYTHON:pypy3.8}
-    py36: {env:TOXPYTHON:python3.6}
+    pypy39: {env:TOXPYTHON:pypy3.9}
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
     py39: {env:TOXPYTHON:python3.9}
+    py310: {env:TOXPYTHON:python3.10}
+    py311: {env:TOXPYTHON:python3.11}
     {bootstrap,clean,check,report,docs,coveralls}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = false
 deps =
     pytest
     pytest-cov
     hunter
-    {py36,py37,py38,py39,py310}: psycopg2-binary==2.9.3
-    {pypy37,pypy38}: psycopg2cffi==2.8.1
+    pg3: psycopg
+    {py36,py37,py38,py39,py310,py311}-pg2: psycopg2-binary
+    {pypy38,pypy39}-pg2: psycopg2cffi
 commands =
     {posargs:pytest --cov --cov-report=term-missing -vv tests}
 
 [testenv:check]
 deps =
     docutils
     check-manifest
     flake8
     readme-renderer
     pygments
     isort
 skip_install = true
 commands =
     python setup.py check --strict --metadata --restructuredtext
-    check-manifest {toxinidir}
+    check-manifest .
     flake8
     isort --verbose --check-only --diff --filter-files .
 
 [testenv:docs]
 usedevelop = true
 deps =
     -r{toxinidir}/docs/requirements.txt
```

