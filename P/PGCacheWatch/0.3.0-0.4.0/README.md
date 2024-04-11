# Comparing `tmp/PGCacheWatch-0.3.0.tar.gz` & `tmp/PGCacheWatch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PGCacheWatch-0.3.0.tar", last modified: Mon Apr  8 15:48:25 2024, max compression
+gzip compressed data, was "PGCacheWatch-0.4.0.tar", last modified: Wed Apr 10 20:23:09 2024, max compression
```

## Comparing `PGCacheWatch-0.3.0.tar` & `PGCacheWatch-0.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.820888 PGCacheWatch-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.820888 PGCacheWatch-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.824888 PGCacheWatch-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)   124806 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/logo.webp
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/pgb.md
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/docs/strategies.md
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.820888 PGCacheWatch-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.824888 PGCacheWatch-0.3.0/src/pgcachewatch/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 15:48:25.000000 PGCacheWatch-0.3.0/src/pgcachewatch/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/pg_bouncer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/src/pgcachewatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:48:25.828888 PGCacheWatch-0.3.0/tests/db/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_decoraters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_pg_bouncer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-08 15:48:14.000000 PGCacheWatch-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.185156 PGCacheWatch-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.185156 PGCacheWatch-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.189156 PGCacheWatch-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)   124806 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/logo.webp
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/pged.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/strategies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.185156 PGCacheWatch-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/src/pgcachewatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/pgcachewatch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/pg_event_distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_decoraters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_pg_event_distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_utils.py
```

### Comparing `PGCacheWatch-0.3.0/.github/workflows/ci.yml` & `PGCacheWatch-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/.github/workflows/linting.yml` & `PGCacheWatch-0.4.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/.github/workflows/release.yml` & `PGCacheWatch-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/.gitignore` & `PGCacheWatch-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/LICENSE` & `PGCacheWatch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/PKG-INFO` & `PGCacheWatch-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PGCacheWatch
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for real-time PostgreSQL event-driven cache invalidation.
 Author: janbjorge
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Homepage, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Issues, https://github.com/janbjorge/pgcachewatch/issues
 Project-URL: Repository, https://github.com/janbjorge/pgcachewatch/
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `PGCacheWatch-0.3.0/README.md` & `PGCacheWatch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/Makefile` & `PGCacheWatch-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/configuration.md` & `PGCacheWatch-0.4.0/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/examples.md` & `PGCacheWatch-0.4.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/index.rst` & `PGCacheWatch-0.4.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -14,9 +14,9 @@
    :maxdepth: 1
    :caption: Contents:
 
    introduction
    setup
    configuration
    strategies
-   pgb
+   pged
    examples
```

### Comparing `PGCacheWatch-0.3.0/docs/introduction.md` & `PGCacheWatch-0.4.0/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/logo.webp` & `PGCacheWatch-0.4.0/docs/logo.webp`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/make.bat` & `PGCacheWatch-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/pgb.md` & `PGCacheWatch-0.4.0/docs/pged.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-## PG-Bouncer Service
+## PG Event Distributor
 
-The new PG-Bouncer service, is designed to enhance PGCacheWatch by enabling efficient distribution of PostgreSQL notifications to multiple clients. This service acts as a middleware, receiving notifications from PostgreSQL and broadcasting them to connected clients via WebSockets. This "fan-out" effect ensures real-time cache invalidation across all clients with minimal database connections.
+The PG event distributor, is designed to enhance PGCacheWatch by enabling efficient distribution of PostgreSQL notifications to multiple clients. This service acts as a middleware, receiving notifications from PostgreSQL and broadcasting them to connected clients via WebSockets. This "fan-out" effect ensures real-time cache invalidation across all clients with minimal database connections.
 
 ###  Key Benefits:
 
 - **Scalability**: Handles numerous clients without increasing load on the PostgreSQL server.
 - **Efficiency**: Reduces the need for multiple direct connections to PostgreSQL for NOTIFY/LISTEN.
 - **Real-time**: Ensures immediate cache invalidation across services upon database changes.
 
@@ -14,31 +14,31 @@
                                       +-------------------+
                                       |   PostgreSQL DB   |
                                       | - NOTIFY on event |
                                       +---------+---------+
                                                 |
                                                 | NOTIFY
                                                 |
-                                      +---------v---------+
-                                      |  PG-Bouncer       |
-                                      |  Service          |
-                                      | - Fan-out NOTIFY  |
-                                      +---------+---------+
+                                      +---------v-------------+
+                                      |  PG Event Distributor |
+                                      |  Service              |
+                                      | - Fan-out NOTIFY      |
+                                      +---------+-------------+
                                                 |
                                   +-------------+-------------+
                                   |                           |
                           +-------v-------+           +-------v-------+
                           | WebSocket     |           | WebSocket     |
                           | Client 1      |           | Client N      |
                           | - Invalidate  |           | - Invalidate  |
                           |   Cache       |           |   Cache       |
                           +---------------+           +---------------+
 ```
 
-To leverage the PG-Bouncer service within your PGCacheWatch setup, ensure it's running and accessible by your application. Configure PGCacheWatch to connect to PG-Bouncer instead of directly to PostgreSQL for notifications. This setup amplifies the effectiveness of your cache invalidation strategy by ensuring timely updates across all client caches with optimized resource usage.
+To leverage the PG Event Distributor within your PGCacheWatch setup, ensure it's running and accessible by your application. Configure PGCacheWatch to connect to the PG Event Distributor instead of directly to PostgreSQL for notifications. This setup amplifies the effectiveness of your cache invalidation strategy by ensuring timely updates across all client caches with optimized resource usage.
 
-### Running the PG-Bouncer Service
-To start the PG-Bouncer service, use the following command in your terminal. This command utilizes uvicorn, an ASGI server, to run the service defined in the `pgcachewatch.pg_bouncer:main` module. The --factory flag is used to indicate that uvicorn should call the provided application factory function to get the ASGI application instance.
+### Running the PG Event Distributor
+To start the PG Event Distributor service, use the following command in your terminal. This command utilizes uvicorn, an ASGI server, to run the service defined in the `pgcachewatch.pg_event_distributor:main` module. The --factory flag is used to indicate that uvicorn should call the provided application factory function to get the ASGI application instance.
 
 ```bash
-uvicorn pgcachewatch.pg_bouncer:main --factory
+uvicorn pgcachewatch.pg_event_distributor:main --factory
 ```
```

### Comparing `PGCacheWatch-0.3.0/docs/setup.md` & `PGCacheWatch-0.4.0/docs/setup.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/docs/strategies.md` & `PGCacheWatch-0.4.0/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/pyproject.toml` & `PGCacheWatch-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dynamic = ["version"]
 license = { text = "Apache 2.0" }
 name = "PGCacheWatch"
 readme = "README.md"
 requires-python = ">=3.10"
 
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Other Environment",
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
```

### Comparing `PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/PKG-INFO` & `PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PGCacheWatch
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for real-time PostgreSQL event-driven cache invalidation.
 Author: janbjorge
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Homepage, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Issues, https://github.com/janbjorge/pgcachewatch/issues
 Project-URL: Repository, https://github.com/janbjorge/pgcachewatch/
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `PGCacheWatch-0.3.0/src/PGCacheWatch.egg-info/SOURCES.txt` & `PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 docs/conf.py
 docs/configuration.md
 docs/examples.md
 docs/index.rst
 docs/introduction.md
 docs/logo.webp
 docs/make.bat
-docs/pgb.md
+docs/pged.md
 docs/setup.md
 docs/strategies.md
 src/PGCacheWatch.egg-info/PKG-INFO
 src/PGCacheWatch.egg-info/SOURCES.txt
 src/PGCacheWatch.egg-info/dependency_links.txt
 src/PGCacheWatch.egg-info/requires.txt
 src/PGCacheWatch.egg-info/top_level.txt
@@ -27,21 +27,21 @@
 src/pgcachewatch/__main__.py
 src/pgcachewatch/_version.py
 src/pgcachewatch/cli.py
 src/pgcachewatch/decorators.py
 src/pgcachewatch/listeners.py
 src/pgcachewatch/logconfig.py
 src/pgcachewatch/models.py
-src/pgcachewatch/pg_bouncer.py
+src/pgcachewatch/pg_event_distributor.py
 src/pgcachewatch/queries.py
 src/pgcachewatch/strategies.py
 src/pgcachewatch/utils.py
 tests/conftest.py
 tests/test_decoraters.py
 tests/test_fastapi.py
 tests/test_integration.py
 tests/test_listeners.py
-tests/test_pg_bouncer.py
+tests/test_pg_event_distributor.py
 tests/test_strategies.py
 tests/test_utils.py
 tests/db/Dockerfile
 tests/db/init_db.sh
```

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/cli.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import argparse
 import sys
 
 import asyncpg
 
-from pgcachewatch import queries
+from pgcachewatch import models, queries
 
 
 def cliparser() -> argparse.Namespace:
-    common_arguments = argparse.ArgumentParser(add_help=False)
+    common_arguments = argparse.ArgumentParser(
+        add_help=False,
+        prog="pgcachewatch",
+    )
     common_arguments.add_argument(
         "--channel-name",
-        default="ch_pgcachewatch_table_change",
+        default=models.DEFAULT_PG_CHANNE,
         help=(
             "The PGNotify channel that will be used by pgcachewatch to listen "
             "for changes on tables, this should be uniq to pgcachewatch clients."
         ),
     )
     common_arguments.add_argument(
         "--function-name",
         default="fn_pgcachewatch_table_change",
         help=(
-            "The name of postgres 'helper function' that emits the on change evnets. "
-            "This must be uniq."
+            "The prefix of the postgres 'helper function' that emits "
+            "the on change evnets."
         ),
     )
     common_arguments.add_argument(
         "--trigger-name",
-        default="tg_pgcachewatch_table_change_",
+        default="tg_pgcachewatch_table_change",
         help="All triggers installed on tables will start with this prefix.",
     )
     common_arguments.add_argument(
         "--commit",
         action="store_true",
-        help="Commit changes to DB.",
+        help="Commit changes to database.",
     )
 
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        prog="pgcachewatch",
     )
 
     subparsers = parser.add_subparsers(dest="command", required=True)
 
     install = subparsers.add_parser(
         "install",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -56,54 +60,57 @@
 
     return parser.parse_args()
 
 
 async def main() -> None:
     parsed = cliparser()
 
+    pg_fn_name = f"{parsed.function_name}_{parsed.channel_name}"
+    pg_tg_name = f"{parsed.trigger_name}_{parsed.channel_name}"
+
     match parsed.command:
         case "install":
-            install = [
-                queries.create_notify_function(
-                    channel_name=parsed.channel_name,
-                    function_name=parsed.function_name,
-                )
-            ]
-
-            for table in parsed.tables:
-                install.append(
+            install = "\n".join(
+                [
+                    queries.create_notify_function(
+                        channel_name=parsed.channel_name,
+                        function_name=pg_fn_name,
+                    )
+                ]
+                + [
                     queries.create_after_change_trigger(
+                        trigger_name=pg_tg_name,
                         table_name=table,
-                        channel_name=parsed.channel_name,
-                        function_name=parsed.function_name,
-                        trigger_name_prefix=parsed.trigger_name,
+                        function_name=pg_fn_name,
                     )
-                )
+                    for table in parsed.tables
+                ]
+            )
+
+            print(install, flush=True)
 
-            combined = "\n".join(install)
-            print(combined, flush=True)
             if parsed.commit:
-                await (await asyncpg.connect()).execute(combined)
+                await (await asyncpg.connect()).execute(install)
             else:
                 print(
                     "::: Use '--commit' to write changes to db. :::",
                     file=sys.stderr,
                 )
 
         case "uninstall":
             trigger_names = await (await asyncpg.connect()).fetch(
-                queries.fetch_trigger_names(parsed.trigger_name),
+                queries.fetch_trigger_names(pg_tg_name),
             )
             combined = "\n".join(
                 (
                     "\n".join(
                         queries.drop_trigger(t["trigger_name"], t["table"])
                         for t in trigger_names
                     ),
-                    queries.drop_function(parsed.function_name),
+                    queries.drop_function(pg_fn_name),
                 )
             )
             print(combined, flush=True)
             if parsed.commit:
                 await (await asyncpg.connect()).execute(combined)
             else:
                 print(
```

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/listeners.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/listeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         self._pg_channel: None | models.PGChannel = None
         self._pg_connection: None | asyncpg.Connection = None
         self._max_latency = max_latency
 
     async def connect(
         self,
         connection: asyncpg.Connection,
-        channel: models.PGChannel = models.PGChannel("ch_pgcachewatch_table_change"),
+        channel: models.PGChannel = models.DEFAULT_PG_CHANNE,
     ) -> None:
         """
         Asynchronously connects the PGEventQueue to a specified
         PostgreSQL channel and connection.
 
         This method establishes a listener on a PostgreSQL channel
         using the provided connection. It is designed to be called
@@ -201,15 +201,15 @@
         self._max_latency = max_latency
         self._handler_task: asyncio.Task | None = None
         self._ws: websockets.WebSocketClientProtocol | None = None
 
     async def connect(
         self,
         ws: websockets.WebSocketClientProtocol,
-        channel: models.PGChannel = models.PGChannel("ch_pgcachewatch_table_change"),
+        channel: models.PGChannel = models.DEFAULT_PG_CHANNE,
     ) -> None:
         async def _handler(ws: websockets.WebSocketClientProtocol) -> None:
             event_handler = create_event_inserter(self, self._max_latency)
             while True:
                 try:
                     event_handler(self._pg_channel, await ws.recv())
                 except websockets.ConnectionClosedOK:
```

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/models.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 
 import pydantic
 
 OPERATIONS = Literal[
     "insert",
     "update",
     "delete",
+    "truncate",
 ]
 
 PGChannel = NewType(
     "PGChannel",
     str,
 )
 
+DEFAULT_PG_CHANNE = PGChannel("ch_pgcachewatch_table_change")
+
 
 class DeadlineSetting(pydantic.BaseModel):
     """
     A data class representing settings for a deadline.
 
     Attributes:
         max_iter: Maximum number of iterations allowed.
```

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/pg_bouncer.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/pg_event_distributor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Facilitates WebSocket clients subscribing to PostgreSQL notifications via
 a single connection. Reduces PostgreSQL server load by sharing one connection
 among multiple clients
 
 Usage example:
-`uvicorn pgcachewatch.pg_bouncer:main --factory`
+`uvicorn pgcachewatch.pg_event_distributor:main --factory`
 """
 
 import asyncio
 from contextlib import asynccontextmanager
 from typing import AsyncGenerator
 
 import asyncpg
```

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/queries.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 def create_notify_function(
     channel_name: str,
     function_name: str,
 ) -> str:
     return f"""
-CREATE OR REPLACE FUNCTION {function_name}_{channel_name}() RETURNS TRIGGER AS $$
+CREATE OR REPLACE FUNCTION {function_name}() RETURNS TRIGGER AS $$
   BEGIN
     PERFORM pg_notify(
       '{channel_name}',
       json_build_object(
         'operation', lower(TG_OP),
         'table', TG_TABLE_NAME,
         'sent_at', NOW()
@@ -15,23 +15,22 @@
     RETURN NEW;
   END;
   $$ LANGUAGE plpgsql;
 """
 
 
 def create_after_change_trigger(
+    trigger_name: str,
     table_name: str,
-    channel_name: str,
     function_name: str,
-    trigger_name_prefix: str,
 ) -> str:
     return f"""
-CREATE OR REPLACE TRIGGER {trigger_name_prefix}{table_name}
+CREATE OR REPLACE TRIGGER {trigger_name}
   AFTER INSERT OR UPDATE OR DELETE OR TRUNCATE ON {table_name}
-  EXECUTE FUNCTION {function_name}_{channel_name}();
+  EXECUTE FUNCTION {function_name}();
 """
 
 
 def fetch_trigger_names(prefix: str) -> str:
     return f"""
 SELECT
   event_object_table AS table,
```

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/strategies.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/strategies.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/src/pgcachewatch/utils.py` & `PGCacheWatch-0.4.0/src/pgcachewatch/utils.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/tests/conftest.py` & `PGCacheWatch-0.4.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pytest
 
 
 def pgb_address() -> str:
     return "127.0.0.1:8000"
 
 
-async def pg_bouncer_isup() -> bool:
+async def pg_event_distributor_isup() -> bool:
     timeout = timedelta(seconds=1)
     deadline = datetime.now() + timeout
 
     async with httpx.AsyncClient(base_url=f"http://{pgb_address()}") as client:
         while datetime.now() < deadline:
             with suppress(httpx.ConnectError):
                 if (await client.get("/up")).is_success:
@@ -57,19 +57,19 @@
         monkeypatch.setenv("PGPASSWORD", "testpassword")
 
     if os.environ.get("PGDATABASE", Unset) is Unset:
         monkeypatch.setenv("PGDATABASE", "testdb")
 
 
 @pytest.fixture(scope="function")
-async def pgbapp() -> AsyncGenerator[Popen, None]:
+async def pgedapp() -> AsyncGenerator[Popen, None]:
     with Popen(
-        "uvicorn pgcachewatch.pg_bouncer:main --factory".split(),
+        "uvicorn pgcachewatch.pg_event_distributor:main --factory".split(),
         stderr=PIPE,
         stdout=PIPE,
     ) as p:
-        await pg_bouncer_isup()
+        await pg_event_distributor_isup()
         try:
             yield p
         finally:
             p.kill()
             p.wait()
```

### Comparing `PGCacheWatch-0.3.0/tests/db/init_db.sh` & `PGCacheWatch-0.4.0/tests/db/init_db.sh`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/tests/test_decoraters.py` & `PGCacheWatch-0.4.0/tests/test_decoraters.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/tests/test_fastapi.py` & `PGCacheWatch-0.4.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/tests/test_integration.py` & `PGCacheWatch-0.4.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/tests/test_listeners.py` & `PGCacheWatch-0.4.0/tests/test_listeners.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         key=lambda x: x.sent_at,
     )
 
 
 @pytest.mark.parametrize("N", (1, 8, 32))
 @pytest.mark.parametrize("operation", get_args(models.OPERATIONS))
 async def test_eventqueue_and_wslistner(
-    pgbapp: Popen,
+    pgedapp: Popen,
     N: int,
     operation: models.OPERATIONS,
     pgpool: asyncpg.Pool,
 ) -> None:
     channel = models.PGChannel(f"test_eventqueue_and_pglistner_{N}_{operation}")
     listener = listeners.WSEventQueue()
```

### Comparing `PGCacheWatch-0.3.0/tests/test_pg_bouncer.py` & `PGCacheWatch-0.4.0/tests/test_pg_event_distributor.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from datetime import datetime, timezone
 from subprocess import Popen
 from typing import get_args
 
 import asyncpg
 import pytest
 import websockets
-from conftest import pg_bouncer_isup, pgb_address
+from conftest import pg_event_distributor_isup, pgb_address
 from pgcachewatch import listeners, models, utils
 
 
-async def test_up_endpoint(pgbapp: Popen) -> None:
-    assert await pg_bouncer_isup()
+async def test_up_endpoint(pgedapp: Popen) -> None:
+    assert await pg_event_distributor_isup()
 
 
 @pytest.mark.parametrize("operation", get_args(models.OPERATIONS))
 @pytest.mark.parametrize("N", (1, 8))
 async def test_ws_broadcast(
-    pgbapp: Popen,
+    pgedapp: Popen,
     N: int,
     pgpool: asyncpg.Pool,
     operation: models.OPERATIONS,
     channel: models.PGChannel = models.PGChannel("test_ws_broadcast"),
 ) -> None:
     async with websockets.connect(f"ws://{pgb_address()}/pgpubsub/{channel}") as ws:
         to_emit = [
@@ -95,15 +95,15 @@
 
     assert que.qsize() == N
 
 
 @pytest.mark.parametrize("operation", get_args(models.OPERATIONS))
 @pytest.mark.parametrize("N", (1, 64))
 async def test_put_on_event_ws_event_queue(
-    pgbapp: Popen,
+    pgedapp: Popen,
     N: int,
     pgpool: asyncpg.Pool,
     operation: models.OPERATIONS,
     channel: models.PGChannel = models.PGChannel("test_put_on_event_ws_event_queue"),
 ) -> None:
     async with websockets.connect(f"ws://{pgb_address()}/pgpubsub/{channel}") as ws:
         lisn = listeners.WSEventQueue()
@@ -129,15 +129,15 @@
         assert to_emit == sorted(
             (lisn.get_nowait() for _ in range(N)),
             key=lambda x: x.sent_at,
         )
 
 
 async def test_ws_event_queue_connection_healthy(
-    pgbapp: Popen,
+    pgedapp: Popen,
     channel: models.PGChannel = models.PGChannel(
         "test_ws_event_queue_connection_healthy"
     ),
 ) -> None:
     async with websockets.connect(f"ws://{pgb_address()}/pgpubsub/{channel}") as ws:
         lisn = listeners.WSEventQueue()
         await lisn.connect(ws, channel)
```

### Comparing `PGCacheWatch-0.3.0/tests/test_strategies.py` & `PGCacheWatch-0.4.0/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.3.0/tests/test_utils.py` & `PGCacheWatch-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

