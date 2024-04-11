# Comparing `tmp/PGCacheWatch-0.4.0.tar.gz` & `tmp/PGCacheWatch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PGCacheWatch-0.4.0.tar", last modified: Wed Apr 10 20:23:09 2024, max compression
+gzip compressed data, was "PGCacheWatch-0.4.1.tar", last modified: Thu Apr 11 11:28:04 2024, max compression
```

## Comparing `PGCacheWatch-0.4.0.tar` & `PGCacheWatch-0.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.185156 PGCacheWatch-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.185156 PGCacheWatch-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.189156 PGCacheWatch-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)   124806 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/logo.webp
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/pged.md
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/docs/strategies.md
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.185156 PGCacheWatch-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/src/pgcachewatch/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 20:23:09.000000 PGCacheWatch-0.4.0/src/pgcachewatch/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/pg_event_distributor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/src/pgcachewatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:09.193156 PGCacheWatch-0.4.0/tests/db/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_decoraters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_pg_event_distributor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-10 20:22:59.000000 PGCacheWatch-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.287127 PGCacheWatch-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.275127 PGCacheWatch-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.275127 PGCacheWatch-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-11 11:28:04.287127 PGCacheWatch-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.279127 PGCacheWatch-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)   124806 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/logo.webp
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/pged.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/docs/strategies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:28:04.287127 PGCacheWatch-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.275127 PGCacheWatch-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.283127 PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-11 11:28:04.000000 PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-11 11:28:04.000000 PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:28:04.000000 PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-11 11:28:04.000000 PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 11:28:04.000000 PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.283127 PGCacheWatch-0.4.1/src/pgcachewatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 11:28:04.000000 PGCacheWatch-0.4.1/src/pgcachewatch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/pg_event_distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/src/pgcachewatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.283127 PGCacheWatch-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:28:04.283127 PGCacheWatch-0.4.1/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_decoraters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_pg_event_distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-11 11:27:55.000000 PGCacheWatch-0.4.1/tests/test_utils.py
```

### Comparing `PGCacheWatch-0.4.0/.github/workflows/ci.yml` & `PGCacheWatch-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/.github/workflows/linting.yml` & `PGCacheWatch-0.4.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/.github/workflows/release.yml` & `PGCacheWatch-0.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/.gitignore` & `PGCacheWatch-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/LICENSE` & `PGCacheWatch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/PKG-INFO` & `PGCacheWatch-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PGCacheWatch
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library for real-time PostgreSQL event-driven cache invalidation.
 Author: janbjorge
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Homepage, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Issues, https://github.com/janbjorge/pgcachewatch/issues
 Project-URL: Repository, https://github.com/janbjorge/pgcachewatch/
```

### Comparing `PGCacheWatch-0.4.0/README.md` & `PGCacheWatch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/Makefile` & `PGCacheWatch-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/configuration.md` & `PGCacheWatch-0.4.1/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/examples.md` & `PGCacheWatch-0.4.1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/index.rst` & `PGCacheWatch-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/introduction.md` & `PGCacheWatch-0.4.1/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/logo.webp` & `PGCacheWatch-0.4.1/docs/logo.webp`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/make.bat` & `PGCacheWatch-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/pged.md` & `PGCacheWatch-0.4.1/docs/pged.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/setup.md` & `PGCacheWatch-0.4.1/docs/setup.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/docs/strategies.md` & `PGCacheWatch-0.4.1/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/pyproject.toml` & `PGCacheWatch-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/PKG-INFO` & `PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PGCacheWatch
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library for real-time PostgreSQL event-driven cache invalidation.
 Author: janbjorge
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Homepage, https://github.com/janbjorge/pgcachewatch/
 Project-URL: Issues, https://github.com/janbjorge/pgcachewatch/issues
 Project-URL: Repository, https://github.com/janbjorge/pgcachewatch/
```

### Comparing `PGCacheWatch-0.4.0/src/PGCacheWatch.egg-info/SOURCES.txt` & `PGCacheWatch-0.4.1/src/PGCacheWatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/cli.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/cli.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/decorators.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/decorators.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/listeners.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/listeners.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/models.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/models.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/pg_event_distributor.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/pg_event_distributor.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/queries.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/queries.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/strategies.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/strategies.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/src/pgcachewatch/utils.py` & `PGCacheWatch-0.4.1/src/pgcachewatch/utils.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/conftest.py` & `PGCacheWatch-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/db/init_db.sh` & `PGCacheWatch-0.4.1/tests/db/init_db.sh`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_decoraters.py` & `PGCacheWatch-0.4.1/tests/test_decoraters.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_fastapi.py` & `PGCacheWatch-0.4.1/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_integration.py` & `PGCacheWatch-0.4.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_listeners.py` & `PGCacheWatch-0.4.1/tests/test_listeners.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_pg_event_distributor.py` & `PGCacheWatch-0.4.1/tests/test_pg_event_distributor.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_strategies.py` & `PGCacheWatch-0.4.1/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `PGCacheWatch-0.4.0/tests/test_utils.py` & `PGCacheWatch-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

