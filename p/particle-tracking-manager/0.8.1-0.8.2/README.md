# Comparing `tmp/particle_tracking_manager-0.8.1.tar.gz` & `tmp/particle_tracking_manager-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particle_tracking_manager-0.8.1.tar", last modified: Fri Apr  5 18:00:33 2024, max compression
+gzip compressed data, was "particle_tracking_manager-0.8.2.tar", last modified: Thu Apr 11 02:15:04 2024, max compression
```

## Comparing `particle_tracking_manager-0.8.1.tar` & `particle_tracking_manager-0.8.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/ci/environment-py3.11.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/ci/environment-py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/more_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/whats_new.md
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    49101 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    24422 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-05 18:00:33.363611 particle_tracking_manager-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_realistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.126199 particle_tracking_manager-0.8.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/ci/environment-py3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/ci/environment-py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/more_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/whats_new.md
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/particle_tracking_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/particle_tracking_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51864 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24422 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_realistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_seeding.py
```

### Comparing `particle_tracking_manager-0.8.1/.github/workflows/release.yaml` & `particle_tracking_manager-0.8.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/.github/workflows/test.yaml` & `particle_tracking_manager-0.8.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/.gitignore` & `particle_tracking_manager-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/.pre-commit-config.yaml` & `particle_tracking_manager-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/LICENSE.txt` & `particle_tracking_manager-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/PKG-INFO` & `particle_tracking_manager-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.8.1
+Version: 0.8.2
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.8.1/README.md` & `particle_tracking_manager-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/ci/environment-py3.10.yml` & `particle_tracking_manager-0.8.2/ci/environment-py3.10.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/ci/environment-py3.11.yml` & `particle_tracking_manager-0.8.2/ci/environment-py3.11.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/ci/environment-py3.9.yml` & `particle_tracking_manager-0.8.2/ci/environment-py3.9.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/docs/Makefile` & `particle_tracking_manager-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/docs/conf.py` & `particle_tracking_manager-0.8.2/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,21 @@
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "**.ipynb_checkpoints", "Thumbs.db", ".DS_Store"]
+exclude_patterns = [
+    "*.ipynb",
+    "_build",
+    "**.ipynb_checkpoints",
+    "Thumbs.db",
+    ".DS_Store",
+]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `particle_tracking_manager-0.8.1/docs/configuration.md` & `particle_tracking_manager-0.8.2/docs/configuration.md`

 * *Files 4% similar despite different names*

```diff
@@ -169,26 +169,26 @@
 
 ```
 import particle_tracking_manager as ptm
 import xroms
 
 m = ptm.OpenDriftModel(lon=-90, lat=28.7, number=1, steps=2)
 url = xroms.datasets.CLOVER.fetch("ROMS_example_full_grid.nc")
-reader_kwargs = dict(loc=url, kwargs_xarray={})
-m.add_reader(**reader_kwargs)
+ds = xr.open_dataset(url, decode_times=False)
+m.add_reader(ds=ds)
 m.run_all()
 ```
 
 
 To run an idealized scenario, no reader should be added (`ocean_model` should be left as None), then fallback configuration parameters (which are not surfaced specifically in `particle-tracking-manager`) can be manually changed, for example:
 
 ```
 from datetime import datetime
 m = ptm.OpenDriftModel(lon=4.0, lat=60.0, start_time=datetime(2015, 9, 22, 6),
-                       use_auto_landmask=True,)
+                       use_auto_landmask=True, steps=5)
 
 # idealized simulation, provide a fake current
 m.o.set_config('environment:fallback:y_sea_water_velocity', 1)
 
 # seed
 m.seed()
 
@@ -197,15 +197,15 @@
 ```
 
 For testing purposes, all steps can be run (including added a "reader") with the selections above plus including `ocean_model="test"`.
 
 ```
 from datetime import datetime
 m = ptm.OpenDriftModel(lon=4.0, lat=60.0, start_time=datetime(2015, 9, 22, 6),
-                       use_auto_landmask=True, ocean_model="test")
+                       use_auto_landmask=True, ocean_model="test", steps=5)
 
 m.run_all()
 ```
 
 ### OpenDriftModel options
 
 #### Drift model
@@ -242,15 +242,15 @@
 ```
 
 The default list of `export_variables` is set in `config_model` but is modified depending on the `drift_model` set.
 
 
 #### How to modify details for Stokes Drift
 
-Turn on (on by default):
+Turn on (on by default, drift model-dependent):
 
 ```
 m = ptm.OpenDriftModel(stokes_drift=True)
 ```
 
 If Stokes drift is on, the following is also turned on in OpenDriftModel:
```

### Comparing `particle_tracking_manager-0.8.1/docs/environment.yml` & `particle_tracking_manager-0.8.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/docs/index.rst` & `particle_tracking_manager-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/docs/more_examples.md` & `particle_tracking_manager-0.8.2/docs/more_examples.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/docs/quick_start.md` & `particle_tracking_manager-0.8.2/docs/quick_start.md`

 * *Files 14% similar despite different names*

```diff
@@ -26,28 +26,35 @@
 ## Python Package
 
 Run directly from the Lagrangian model you want to use, which will inherit from the manager class. For now there is one option of `OpenDriftModel`.
 
 ```
 import particle_tracking_manager as ptm
 
-m = ptm.OpenDriftModel(ocean_model="NWGOA", lon=-151, lat=59)
+m = ptm.OpenDriftModel(ocean_model="NWGOA", lon=-151, lat=59, steps=1)
+# Can modify `m` between these steps, or look at `OpenDrift` config with `m.drift_model_config()`
 m.run_all()
 ```
 
 Then find results in file `m.outfile_name`.
 
 +++
 
 ## Command Line Interface
 
 The equivalent for the set up above for using the command line is:
 
 ```
-ptm lon=-151 lat=59 ocean_model=NWGOA
+ptm lon=-151 lat=59 ocean_model=NWGOA steps=1
+```
+
+To just initialize the simulation and print the `OpenDrift` configuration to screen without running the simulation, add the `--dry-run` flag:
+
+```
+ptm lon=-151 lat=59 ocean_model=NWGOA steps=1 --dry-run
 ```
 
 `m.outfile_name` is printed to the screen after the command has been run. `ptm` is installed as an entry point with `particle-tracking-manager`.
 
 +++
 
 (new_reader)=
@@ -118,15 +125,21 @@
 ```
 m.reader
 ```
 
 Get reader/ocean model properties (gathered metadata about model):
 
 ```
-m.reader_metadata(key)
+m.reader_metadata(<key>)
 ```
 
 Show configuration details — many more details on this in {doc}`configuration`:
 
 ```
 m.show_config()
 ```
+
+Show `OpenDrift` configuration for selected `drift_model`:
+
+```
+m.drift_model_config()
+```
```

### Comparing `particle_tracking_manager-0.8.1/docs/tutorial.md` & `particle_tracking_manager-0.8.2/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/docs/whats_new.md` & `particle_tracking_manager-0.8.2/docs/whats_new.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # What's New
 
+## v0.8.2 (April 10, 2024)
+
+* updated docs
+* improved `drift_model_config()`
+* updated tests
+* now include PTM metadata with output file
+
 ## v0.8.1 (April 5, 2024)
 
 * updated docs
 
 ## v0.8.0 (April 2, 2024)
 
 * `time_step_output` behavior has changed — 1 hour by default
```

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager/cli.py` & `particle_tracking_manager-0.8.2/particle_tracking_manager/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,27 +102,40 @@
     parser.add_argument(
         "kwargs",
         nargs="*",
         action=ParseKwargs,
         help="Input keyword arguments for running PTM. Available options are specific to the `catalog_type`. Dictionary-style input, e.g. `case='Oil'`. Format for list items is e.g. standard_names='[sea_water_practical_salinity,sea_water_temperature]'.",
     )
 
+    parser.add_argument(
+        "--dry-run",
+        help="Return configuration parameters without running the model.",
+        action=argparse.BooleanOptionalAction,
+        default=False,
+    )
+
     args = parser.parse_args()
 
     to_bool = {
         key: ast.literal_eval(value)
         for key, value in args.kwargs.items()
         if value in ["True", "False"]
     }
     args.kwargs.update(to_bool)
 
-    # # set default
-    # if "model" not in args:
-    #     args.kwargs["model"] = "opendrift"
+    m = ptm.OpenDriftModel(**args.kwargs)
+
+    if args.dry_run:
 
-    # if args.kwargs["ocean_model"] is None and args.kwargs["start_time"] is None:
-    #     raise KeyError("Need to either use a reader or input a start_time to avoid error.")
+        # run this to make sure everything is updated fully
+        m.add_reader()
+        print(m.drift_model_config())
 
-    m = ptm.OpenDriftModel(**args.kwargs)
-    m.run_all()
+    else:
+
+        m.add_reader()
+        print(m.drift_model_config())
+
+        m.seed()
+        m.run()
 
-    print(m.outfile_name)
+        print(m.outfile_name)
```

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/config.json` & `particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/config.json`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/opendrift.py` & `particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/opendrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Using OpenDrift for particle tracking."""
 import copy
 import datetime
+import gc
 import json
 import logging
+import os
+import platform
+import tempfile
 
 from pathlib import Path
 from typing import Optional, Union
 
 import appdirs
 
 # using my own version of ROMS reader
@@ -731,19 +735,25 @@
                         decode_times=False,
                     )
 
                 # otherwise remote
                 else:
                     if ".nc" in loc_remote:
                         ds = xr.open_dataset(
-                            loc_remote, chunks={}, drop_variables=drop_vars
+                            loc_remote,
+                            chunks={},
+                            drop_variables=drop_vars,
+                            decode_times=False,
                         )
                     else:
                         ds = xr.open_zarr(
-                            loc_remote, chunks={}, drop_variables=drop_vars
+                            loc_remote,
+                            chunks={},
+                            drop_variables=drop_vars,
+                            decode_times=False,
                         )
 
             # For NWGOA, need to calculate wetdry mask from a variable
             if self.ocean_model == "NWGOA" and not self.use_static_masks:
                 ds["wetdry_mask_rho"] = (~ds.zeta.isnull()).astype(int)
 
             # For CIOFSOP need to rename u/v to have "East" and "North" in the variable names
@@ -807,65 +817,89 @@
             # can find reader at manager.o.env.readers[self.ocean_model]
 
             self.oceanmodel_lon0_360 = oceanmodel_lon0_360
 
         else:
             raise ValueError("reader did not set an ocean_model")
 
-    def run_seed(self):
-        """Seed drifters for model."""
+    @property
+    def seed_kws(self):
+        """Gather seed input kwargs.
+
+        This could be run more than once.
+        """
 
         already_there = [
             "seed:number",
             "seed:z",
             "seed:seafloor",
             "seed:droplet_diameter_mu",
             "seed:droplet_diameter_min_subsea",
             "seed:droplet_size_distribution",
             "seed:droplet_diameter_sigma",
             "seed:droplet_diameter_max_subsea",
             "seed:object_type",
+            "seed_flag",
+            "drift:use_tabularised_stokes_drift",
+            "drift:vertical_advection",
+            "drift:truncate_ocean_model_below_m",
         ]
 
-        seed_kws = {
-            "time": self.start_time.to_pydatetime(),
+        _seed_kws = {
+            "time": self.start_time.to_pydatetime()
+            if self.start_time is not None
+            else None,
             "z": self.z,
         }
 
         # update seed_kws with drift_model-specific seed parameters
         seedlist = self.drift_model_config(prefix="seed")
         seedlist = [(one, two) for one, two in seedlist if one not in already_there]
         seedlist = [(one.replace("seed:", ""), two) for one, two in seedlist]
-        seed_kws.update(seedlist)
+        _seed_kws.update(seedlist)
 
         if self.seed_flag == "elements":
             # add additional seed parameters
-            seed_kws.update(
+            _seed_kws.update(
                 {
                     "lon": self.lon,
                     "lat": self.lat,
                     "radius": self.radius,
                     "radius_type": self.radius_type,
                 }
             )
 
-            self.o.seed_elements(**seed_kws)
+        elif self.seed_flag == "geojson":
+
+            # geojson needs string representation of time
+            _seed_kws["time"] = (
+                self.start_time.isoformat() if self.start_time is not None else None
+            )
+
+        self._seed_kws = _seed_kws
+        return self._seed_kws
+
+    def run_seed(self):
+        """Actually seed drifters for model."""
+
+        if self.seed_flag == "elements":
+
+            self.o.seed_elements(**self.seed_kws)
 
         elif self.seed_flag == "geojson":
 
             # geojson needs string representation of time
-            seed_kws["time"] = self.start_time.isoformat()
-            self.geojson["properties"] = seed_kws
+            self.seed_kws["time"] = self.start_time.isoformat()
+            self.geojson["properties"] = self.seed_kws
             json_string_dumps = json.dumps(self.geojson)
             self.o.seed_from_geojson(json_string_dumps)
 
         else:
             raise ValueError(f"seed_flag {self.seed_flag} not recognized.")
 
-        self.seed_kws = seed_kws
         self.initial_drifters = self.o.elements_scheduled
 
     def run_drifters(self):
         """Run the drifters!"""
 
         if self.steps is None and self.duration is None and self.end_time is None:
             raise ValueError(
@@ -881,29 +915,55 @@
         full_config = copy.deepcopy(self._config)  # save
         config_input_to_opendrift = {
             k: full_config[k] for k in self._config_orig.keys()
         }
 
         self.o._config = config_input_to_opendrift  # only OpenDrift config
 
-        output_file = (
-            self.output_file
+        output_file_initial = (
+            f"{self.output_file}_initial"
             or f"output-results_{datetime.datetime.utcnow():%Y-%m-%dT%H%M:%SZ}.nc"
         )
 
         self.o.run(
             time_step=timedir * self.time_step,
             time_step_output=self.time_step_output,
             steps=self.steps,
             export_variables=self.export_variables,
-            outfile=output_file,
+            outfile=output_file_initial,
         )
 
         self.o._config = full_config  # reinstate config
 
+        # open outfile file and add config to it
+        # config can't be present earlier because it breaks opendrift
+        ds = xr.open_dataset(output_file_initial)
+        for k, v in self.drift_model_config():
+            if isinstance(v, (bool, type(None), pd.Timestamp, pd.Timedelta)):
+                v = str(v)
+            ds.attrs[f"ptm_config_{k}"] = v
+
+        # Make new output file
+        output_file = (
+            self.output_file
+            or f"output-results_{datetime.datetime.utcnow():%Y-%m-%dT%H%M:%SZ}.nc"
+        )
+
+        ds.to_netcdf(output_file)
+
+        # update with new path name
+        self.o.outfile_name = output_file
+
+        try:
+            # remove initial file to save space
+            os.remove(output_file_initial)
+        except PermissionError:
+            # windows issue
+            pass
+
     @property
     def _config(self):
         """Surface the model configuration."""
 
         # save for reinstatement when running the drifters
         if self._config_orig is None:
             self._config_orig = copy.deepcopy(self.o._config)
@@ -1007,33 +1067,57 @@
         return self.o.export_variables
 
     def drift_model_config(self, ptm_level=[1, 2, 3], prefix=""):
         """Show config for this drift model selection.
 
         This shows all PTM-controlled parameters for the OpenDrift
         drift model selected and their current values, at the selected ptm_level
-        of importance.
+        of importance. It includes some additional configuration parameters
+        that are indirectly controlled by PTM parameters.
 
         Parameters
         ----------
         ptm_level : int, list, optional
             Options are 1, 2, 3, or lists of combinations. Use [1,2,3] for all.
             Default is 1.
         prefix : str, optional
             prefix to search config for, only for OpenDrift parameters (not PTM).
         """
 
-        return [
+        outlist = [
             (key, value_dict["value"])
             for key, value_dict in self.show_config(
                 substring=":", ptm_level=ptm_level, level=[1, 2, 3], prefix=prefix
             ).items()
             if "value" in value_dict
         ]
 
+        # also PTM config parameters that are separate from OpenDrift parameters
+        outlist2 = [
+            (key, value_dict["value"])
+            for key, value_dict in self.show_config(
+                ptm_level=ptm_level, prefix=prefix
+            ).items()
+            if "od_mapping" not in value_dict and "value" in value_dict
+        ]
+
+        # extra parameters that are not in the config_model but are set by PTM indirectly
+        extra_keys = [
+            "drift:vertical_advection",
+            "drift:truncate_ocean_model_below_m",
+            "drift:use_tabularised_stokes_drift",
+        ]
+        outlist += [
+            (key, self.show_config(key=key)["value"])
+            for key in extra_keys
+            if "value" in self.show_config(key=key)
+        ]
+
+        return outlist + outlist2
+
     def get_configspec(self, prefix, substring, excludestring, level, ptm_level):
         """Copied from OpenDrift, then modified."""
 
         if not isinstance(level, list) and level is not None:
             level = [level]
         if not isinstance(ptm_level, list) and ptm_level is not None:
             ptm_level = [ptm_level]
```

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager/plotting.py` & `particle_tracking_manager-0.8.2/particle_tracking_manager/plotting.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager.py` & `particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager_config.json` & `particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager_config.json`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/PKG-INFO` & `particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.8.1
+Version: 0.8.2
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/SOURCES.txt` & `particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/pyproject.toml` & `particle_tracking_manager-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/setup.cfg` & `particle_tracking_manager-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/tests/conftest.py` & `particle_tracking_manager-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/tests/test_cli.py` & `particle_tracking_manager-0.8.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/tests/test_config.py` & `particle_tracking_manager-0.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/tests/test_manager.py` & `particle_tracking_manager-0.8.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/tests/test_opendrift.py` & `particle_tracking_manager-0.8.2/tests/test_opendrift.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,47 +229,45 @@
         m = OpenDriftModel(drift_model="not_a_real_model")
 
 
 class TestTheManager(unittest.TestCase):
     def setUp(self):
         self.m = OpenDriftModel()
         # self.m.config_model = {"test_key": {"value": "old_value"}}
+        # test m.drift_model_config()
+        # also test in other sub tests
 
     def test_set_drift_model(self):
         """can't change the drift_model after class initialization"""
         with self.assertRaises(KeyError):
             self.m.drift_model = "new_model"
 
     def test_set_o(self):
         with self.assertRaises(KeyError):
             self.m.o = "new_o"
 
     def test_stokes_drift_true_not_leeway(self):
         self.m.stokes_drift = True
-        self.m.drift_model = "OceanDrift"
         assert self.m.show_config(key="drift:use_tabularised_stokes_drift")
 
     def test_surface_only_true_not_leeway(self):
         self.m.surface_only = True
-        self.m.drift_model = "OceanDrift"
         assert (
             self.m.show_config(key="drift:truncate_ocean_model_below_m")["value"] == 0.5
         )
 
     def test_surface_only_false_not_leeway(self):
         self.m.surface_only = False
-        self.m.drift_model = "OceanDrift"
         assert (
             self.m.show_config(key="drift:truncate_ocean_model_below_m")["value"]
             is None
         )
 
     def test_do3D_false_not_leeway(self):
         self.m.do3D = False
-        self.m.drift_model = "OceanDrift"
         assert not self.m.show_config(key="drift:vertical_advection")["value"]
         assert not self.m.show_config(key="drift:vertical_mixing")["value"]
 
     def test_do3D_true(self):
         self.m.do3D = True
         # assert self.m.show_config(key="drift:vertical_advection")["value"]
 
@@ -387,14 +385,15 @@
         droplet_diameter_min_subsea=0.01,
         droplet_diameter_mu=0.01,
         droplet_size_distribution="normal",
         droplet_diameter_sigma=10,
         oil_film_thickness=5,
         oil_type="GENERIC DIESEL",
     )
+
     m.o.set_config("environment:constant:x_wind", -1)
     m.o.set_config("environment:constant:y_wind", -1)
     m.o.set_config("environment:constant:x_sea_water_velocity", -1)
     m.o.set_config("environment:constant:y_sea_water_velocity", -1)
     m.seed()
 
     # to check impact of m3_per_hour: mass_oil for m3_per_hour of 1 * 5
```

### Comparing `particle_tracking_manager-0.8.1/tests/test_realistic.py` & `particle_tracking_manager-0.8.2/tests/test_realistic.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.1/tests/test_seeding.py` & `particle_tracking_manager-0.8.2/tests/test_seeding.py`

 * *Files identical despite different names*

