# Comparing `tmp/lsst-rsp-0.4.3.tar.gz` & `tmp/lsst-rsp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-rsp-0.4.3.tar", last modified: Fri Mar 22 21:47:47 2024, max compression
+gzip compressed data, was "lsst-rsp-0.5.0.tar", last modified: Thu Apr 11 19:18:30 2024, max compression
```

## Comparing `lsst-rsp-0.4.3.tar` & `lsst-rsp-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.016677 lsst-rsp-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.012677 lsst-rsp-0.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.012677 lsst-rsp-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.github/workflows/periodic-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-03-22 21:47:47.016677 lsst-rsp-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.012677 lsst-rsp-0.4.3/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/changelog.d/_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 21:47:47.016677 lsst-rsp-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.008677 lsst-rsp-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.012677 lsst-rsp-0.4.3/src/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/src/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.012677 lsst-rsp-0.4.3/src/lsst/rsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/src/lsst/rsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/src/lsst/rsp/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/src/lsst/rsp/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/src/lsst/rsp/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/src/lsst/rsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.016677 lsst-rsp-0.4.3/src/lsst_rsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-03-22 21:47:46.000000 lsst-rsp-0.4.3/src/lsst_rsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-22 21:47:47.000000 lsst-rsp-0.4.3/src/lsst_rsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:47:46.000000 lsst-rsp-0.4.3/src/lsst_rsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-22 21:47:46.000000 lsst-rsp-0.4.3/src/lsst_rsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-22 21:47:46.000000 lsst-rsp-0.4.3/src/lsst_rsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:47:47.016677 lsst-rsp-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/tests/version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-22 21:47:41.000000 lsst-rsp-0.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.452279 lsst-rsp-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-11 19:18:30.452279 lsst-rsp-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/changelog.d/_template.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:30.452279 lsst-rsp-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.440279 lsst-rsp-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/src/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/src/lsst/rsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/src/lsst/rsp/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/src/lsst/rsp/startup/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/models/noninteractive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/src/lsst/rsp/startup/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/services/labrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.444279 lsst-rsp-0.5.0/src/lsst/rsp/startup/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/storage/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/startup/storage/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/src/lsst/rsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.452279 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-11 19:18:30.000000 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-11 19:18:30.000000 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:30.000000 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 19:18:30.000000 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-11 19:18:30.000000 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 19:18:30.000000 lsst-rsp-0.5.0/src/lsst_rsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/startup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.440279 lsst-rsp-0.5.0/tests/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/etc/dircolors.ansi-universal
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/etc/skel/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/etc/skel/.gitconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/etc/skel/.pythonrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/etc/skel/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/etc/skel/notebooks/.user_setups
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.440279 lsst-rsp-0.5.0/tests/support/files/homedir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/homedir/.lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/homedir/.lsst/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/homedir/.lsst/postgres-credentials.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.440279 lsst-rsp-0.5.0/tests/support/files/stack_top/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/stack_top/jupyterlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/stack_top/jupyterlab/20-logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:30.448279 lsst-rsp-0.5.0/tests/support/files/stack_top/jupyterlab/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tests/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 19:18:25.000000 lsst-rsp-0.5.0/tox.ini
```

### Comparing `lsst-rsp-0.4.3/.github/CONTRIBUTING.md` & `lsst-rsp-0.5.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/.github/workflows/ci.yaml` & `lsst-rsp-0.5.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/.github/workflows/periodic-ci.yaml` & `lsst-rsp-0.5.0/.github/workflows/periodic-ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/.gitignore` & `lsst-rsp-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/.pre-commit-config.yaml` & `lsst-rsp-0.5.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     rev: v4.5.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.16.0
```

### Comparing `lsst-rsp-0.4.3/CHANGELOG.md` & `lsst-rsp-0.5.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/LICENSE` & `lsst-rsp-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/PKG-INFO` & `lsst-rsp-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.4.3
+Version: 0.5.0
 Summary: Utility functions for the Rubin Science Platform
+Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -39,14 +40,16 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Deprecated<2
 Requires-Dist: IPython<9
 Requires-Dist: pyvo<2,>=1.5.0
+Requires-Dist: structlog
+Requires-Dist: symbolicmode<3
 Provides-Extra: dev
 Requires-Dist: types-deprecated; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `lsst-rsp-0.4.3/README.md` & `lsst-rsp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/pyproject.toml` & `lsst-rsp-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,27 @@
     "Operating System :: POSIX",
     "Typing :: Typed",
 ]
 requires-python = ">=3.11"
 dependencies = [
     "Deprecated<2",
     "IPython<9",
-    "pyvo>=1.5.0,<2"
+    "pyvo>=1.5.0,<2",
+    "structlog",  # Uses CalVer, not SemVer
+    "symbolicmode<3",
 ]
 dynamic = ["version"]
 
+[[project.authors]]
+name = "Association of Universities for Research in Astronomy, Inc. (AURA)"
+email = "sqre-admin@lists.lsst.org"
+
+[project.scripts]
+launch-rubin-jupyterlab = "lsst.rsp.startup.cli:main"
+
 [project.optional-dependencies]
 dev = [
     # Typing
     "types-deprecated",
     "types-requests",
     # Testing
     "coverage[toml]",
@@ -101,14 +110,15 @@
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:"
 ]
 
 [tool.mypy]
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
+exclude = "tests/support/files"
 ignore_missing_imports = true
 local_partial_types = true
 no_implicit_reexport = true
 show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_unreachable = true
@@ -132,14 +142,17 @@
 # errs on the side of disabling legitimate lints.
 #
 # Reference for settings: https://docs.astral.sh/ruff/settings/
 # Reference for rules: https://docs.astral.sh/ruff/rules/
 [tool.ruff]
 line-length = 79
 target-version = "py311"
+exclude = [
+    "tests/support/files/*"
+]
 
 [tool.ruff.lint]
 ignore = [
     "ANN101",  # self should not have a type annotation
     "ANN102",  # cls should not have a type annotation
     "ANN401",  # sometimes Any is the right type
     "ARG001",  # unused function arguments are often legitimate
@@ -151,15 +164,14 @@
     "D102",    # sometimes we use docstring inheritence
     "D104",    # don't see the point of documenting every package
     "D105",    # our style doesn't require docstrings for magic methods
     "D106",    # Pydantic uses a nested Config class that doesn't warrant docs
     "D205",    # our documentation style allows a folded first line
     "EM101",   # justification (duplicate string in traceback) is silly
     "EM102",   # justification (duplicate string in traceback) is silly
-    "FBT003",  # positional booleans are normal for Pydantic field defaults
     "FIX002",  # point of a TODO comment is that we're not ready to fix it
     "G004",    # forbidding logging f-strings is appealing, but not our style
     "RET505",  # disagree that omitting else always makes code more readable
     "PLR0911", # often many returns is clearer and simpler style
     "PLR0913", # factory pattern uses constructors with many arguments
     "PLR2004", # too aggressive about magic values
     "PLW0603", # yes global is discouraged but if needed, it's needed
@@ -204,28 +216,32 @@
     "D103",    # tests don't need docstrings
     "PLR0915", # tests are allowed to be long, sometimes that's convenient
     "PT012",   # way too aggressive about limiting pytest.raises blocks
     "S101",    # tests should use assert
     "S106",    # tests are allowed to hard-code dummy passwords
     "SLF001",  # tests are allowed to access private members
 ]
-
+"src/lsst/rsp/startup/**" = [
+    "S606",    # Sometimes we really mean os.execve(), not subprocess.run()
+]
 [tool.ruff.lint.isort]
 known-first-party = ["lsst.rsp", "tests"]
 split-on-trailing-comma = false
 
 # These are too useful as attributes or methods to allow the conflict with the
 # built-in to rule out their use.
 [tool.ruff.lint.flake8-builtins]
 builtins-ignorelist = [
     "all",
     "any",
+    "dict",
     "help",
     "id",
     "list",
+    "open",
     "type",
 ]
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
```

### Comparing `lsst-rsp-0.4.3/src/lsst/rsp/__init__.py` & `lsst-rsp-0.5.0/src/lsst/rsp/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/src/lsst/rsp/catalog.py` & `lsst-rsp-0.5.0/src/lsst/rsp/catalog.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/src/lsst/rsp/log.py` & `lsst-rsp-0.5.0/src/lsst/rsp/log.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/src/lsst/rsp/service.py` & `lsst-rsp-0.5.0/src/lsst/rsp/service.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.4.3/src/lsst/rsp/utils.py` & `lsst-rsp-0.5.0/src/lsst/rsp/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,20 @@
 
     Returns
     -------
     str
         Digest of the Docker image this code is running inside, or the empty
         string if the digest could not be determined.
     """
-    return os.environ.get("JUPYTER_IMAGE_SPEC", "")
+    spec = os.environ.get("JUPYTER_IMAGE_SPEC", "")
+    hash_marker = "@sha256:"
+    hash_pos = spec.find(hash_marker)
+    if hash_pos == -1:
+        return ""
+    return spec[hash_pos + len(hash_marker) :]
 
 
 def get_access_token(
     tokenfile: str | Path | None = None, log: Any | None = None
 ) -> str:
     """Get the Gafaelfawr access token for the user.
```

### Comparing `lsst-rsp-0.4.3/src/lsst_rsp.egg-info/PKG-INFO` & `lsst-rsp-0.5.0/src/lsst_rsp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.4.3
+Version: 0.5.0
 Summary: Utility functions for the Rubin Science Platform
+Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -39,14 +40,16 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Deprecated<2
 Requires-Dist: IPython<9
 Requires-Dist: pyvo<2,>=1.5.0
+Requires-Dist: structlog
+Requires-Dist: symbolicmode<3
 Provides-Extra: dev
 Requires-Dist: types-deprecated; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `lsst-rsp-0.4.3/tests/utils_test.py` & `lsst-rsp-0.5.0/tests/utils_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 """Tests for utility functions."""
 
 from __future__ import annotations
 
 import pytest
 
 from lsst.rsp import format_bytes
-from lsst.rsp.utils import get_service_url
+from lsst.rsp.utils import get_digest, get_service_url
 
 
 def test_format_bytes() -> None:
     """Test human-readable names for numeric byte inputs."""
     assert format_bytes(1) == "1 B"
     assert format_bytes(1234) == "1.23 kB"
     assert format_bytes(12345678) == "12.35 MB"
     assert format_bytes(1234567890) == "1.23 GB"
     assert format_bytes(1234567890000) == "1.23 TB"
     assert format_bytes(1234567890000000) == "1.23 PB"
 
 
+def test_get_digest(monkeypatch: pytest.MonkeyPatch) -> None:
+    monkeypatch.setenv("JUPYTER_IMAGE_SPEC", "sciplat-lab@sha256:abcde")
+    digest = get_digest()
+    assert digest == "abcde"
+
+
+def test_get_digest_fail(monkeypatch: pytest.MonkeyPatch) -> None:
+    monkeypatch.setenv("JUPYTER_IMAGE_SPEC", "sciplat-lab:w_2024_01")
+    digest = get_digest()
+    assert digest == ""
+
+
 def test_get_service_url(monkeypatch: pytest.MonkeyPatch) -> None:
     """Ensure there are no doubled slashes."""
     monkeypatch.setenv("EXTERNAL_INSTANCE_URL", "https://test.example.com/")
     monkeypatch.setenv("TAP_ROUTE", "/api/tap")
     assert get_service_url("tap") == "https://test.example.com/api/tap"
```

### Comparing `lsst-rsp-0.4.3/tox.ini` & `lsst-rsp-0.5.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tox]
 envlist = py,coverage-report,typing,lint
 isolated_build = True
 
 [testenv]
 description = Run pytest against {envname}.
-extras =
-    dev
+extras = dev
 
 [testenv:py]
 description = Run pytest
 commands =
     coverage run -m pytest {posargs}
 
 [testenv:coverage-report]
```

