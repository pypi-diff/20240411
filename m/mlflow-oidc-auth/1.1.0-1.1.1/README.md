# Comparing `tmp/mlflow-oidc-auth-1.1.0.tar.gz` & `tmp/mlflow-oidc-auth-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-oidc-auth-1.1.0.tar", last modified: Wed Apr 10 02:47:14 2024, max compression
+gzip compressed data, was "mlflow-oidc-auth-1.1.1.tar", last modified: Wed Apr 10 20:05:52 2024, max compression
```

## Comparing `mlflow-oidc-auth-1.1.0.tar` & `mlflow-oidc-auth-1.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.916981 mlflow-oidc-auth-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-04-10 02:47:14.916981 mlflow-oidc-auth-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.908981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.908981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.908981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.908981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/sqlalchemy_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.908981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.912981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/templates/_footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/templates/_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/templates/auth.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.912981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/398.70c7e628915a6c39.js
--rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/3rdpartylicenses.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/953.eb8714051ee666a2.js
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-10 02:47:12.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   703409 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/main.ff1acef2e224ca42.js
--rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/runtime.5064f1f60b88aea4.js
--rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-10 02:47:11.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:47:14.912981 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-04-10 02:47:14.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 02:47:14.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:47:14.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 02:47:14.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 02:47:14.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 02:47:14.000000 mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-10 02:46:04.000000 mlflow-oidc-auth-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:47:14.916981 mlflow-oidc-auth-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.320966 mlflow-oidc-auth-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-04-10 20:05:52.320966 mlflow-oidc-auth-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.312966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.316966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.316966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.316966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/sqlalchemy_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.316966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.316966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/templates/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/templates/_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/templates/auth.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.320966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/398.70c7e628915a6c39.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/3rdpartylicenses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   703509 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/main.84383ebc03062e87.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/runtime.0cd10aef5e6b1db8.js
+-rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-10 20:05:49.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:05:52.320966 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-04-10 20:05:52.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 20:05:52.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:05:52.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 20:05:52.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 20:05:52.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 20:05:52.000000 mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-10 20:04:47.000000 mlflow-oidc-auth-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:05:52.320966 mlflow-oidc-auth-1.1.1/setup.cfg
```

### Comparing `mlflow-oidc-auth-1.1.0/LICENSE` & `mlflow-oidc-auth-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/PKG-INFO` & `mlflow-oidc-auth-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.1.0
+Version: 1.1.1
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -253,14 +253,17 @@
 | OIDC_AUTHORIZATION_URL | OIDC Auth URL (if discovery URL is not defined) |
 | OIDC_TOKEN_URL         | OIDC Token URL (if discovery URL is not defined) |
 | OIDC_USER_URL          | OIDC User info URL (if discovery URL is not defined) |
 | SECRET_KEY             | Key to perform cookie encryption |
 | OAUTHLIB_INSECURE_TRANSPORT | Development only. Allow to use insecure endpoints for OIDC |
 | LOG_LEVEL                   | Application log level |
 | OIDC_USERS_DB_URI | Database connection string |
+| MLFLOW_TRACKING_USERNAME | Credentials for internal communications via API |
+| MLFLOW_TRACKING_PASSWORD | Credentials for internal communications via API |
+| MLFLOW_TRACKING_URI | URI for internal communications via API |
 
 # Configuration examples
 
 ## Okta
 
 ```bash
 OIDC_DISCOVERY_URL = 'https://<your_domain>.okta.com/.well-known/openid-configuration'
@@ -285,22 +288,27 @@
 OIDC_GROUP_NAME = "mlflow_users_group_name"
 OIDC_ADMIN_GROUP_NAME = "mlflow_admins_group_name"
 ```
 
 > please note, that for getting group membership information, the application should have "GroupMember.Read.All" permission
 
 # Development
+
+Preconditions:
+
+The following tools should be installed for local development:
+
+* git
+* nodejs
+* python
+
 ```shell
 git clone https://github.com/data-platform-hq/mlflow-oidc-auth
 cd mlflow-oidc-auth
-python3 -m venv venv
-source venv/bin/activate
-pip install --editable .
-mlflow server --dev --app-name oidc-auth --host 0.0.0.0 --port 8080
+./scripts/run-dev-server.sh
 ```
 
-
 # License
 Apache 2 Licensed. For more information please see [LICENSE](./LICENSE)
 
 ### Based on MLFlow basic-auth plugin
 https://github.com/mlflow/mlflow/tree/master/mlflow/server/auth
```

### Comparing `mlflow-oidc-auth-1.1.0/README.md` & `mlflow-oidc-auth-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 | OIDC_AUTHORIZATION_URL | OIDC Auth URL (if discovery URL is not defined) |
 | OIDC_TOKEN_URL         | OIDC Token URL (if discovery URL is not defined) |
 | OIDC_USER_URL          | OIDC User info URL (if discovery URL is not defined) |
 | SECRET_KEY             | Key to perform cookie encryption |
 | OAUTHLIB_INSECURE_TRANSPORT | Development only. Allow to use insecure endpoints for OIDC |
 | LOG_LEVEL                   | Application log level |
 | OIDC_USERS_DB_URI | Database connection string |
+| MLFLOW_TRACKING_USERNAME | Credentials for internal communications via API |
+| MLFLOW_TRACKING_PASSWORD | Credentials for internal communications via API |
+| MLFLOW_TRACKING_URI | URI for internal communications via API |
 
 # Configuration examples
 
 ## Okta
 
 ```bash
 OIDC_DISCOVERY_URL = 'https://<your_domain>.okta.com/.well-known/openid-configuration'
@@ -52,22 +55,27 @@
 OIDC_GROUP_NAME = "mlflow_users_group_name"
 OIDC_ADMIN_GROUP_NAME = "mlflow_admins_group_name"
 ```
 
 > please note, that for getting group membership information, the application should have "GroupMember.Read.All" permission
 
 # Development
+
+Preconditions:
+
+The following tools should be installed for local development:
+
+* git
+* nodejs
+* python
+
 ```shell
 git clone https://github.com/data-platform-hq/mlflow-oidc-auth
 cd mlflow-oidc-auth
-python3 -m venv venv
-source venv/bin/activate
-pip install --editable .
-mlflow server --dev --app-name oidc-auth --host 0.0.0.0 --port 8080
+./scripts/run-dev-server.sh
 ```
 
-
 # License
 Apache 2 Licensed. For more information please see [LICENSE](./LICENSE)
 
 ### Based on MLFlow basic-auth plugin
 https://github.com/mlflow/mlflow/tree/master/mlflow/server/auth
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/app.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/app.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/client.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/config.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import secrets
 import requests
+import secrets
 
 from dotenv import load_dotenv
 from mlflow_oidc_auth.app import app
 
 load_dotenv()  # take environment variables from .env.
 
 
@@ -30,11 +31,14 @@
     else:
         OIDC_AUTHORIZATION_URL = os.environ.get("OIDC_AUTHORIZATION_URL", None)
         OIDC_TOKEN_URL = os.environ.get("OIDC_TOKEN_URL", None)
         OIDC_USER_URL = os.environ.get("OIDC_USER_URL", None)
     OIDC_REDIRECT_URI = os.environ.get("OIDC_REDIRECT_URI", None)
     OIDC_CLIENT_ID = os.environ.get("OIDC_CLIENT_ID", None)
     OIDC_CLIENT_SECRET = os.environ.get("OIDC_CLIENT_SECRET", None)
+    MLFLOW_TRACKING_URI = os.environ.get("MLFLOW_TRACKING_URI", "http://localhost:8080")
+    MLFLOW_TRACKING_USERNAME = os.environ.get("MLFLOW_TRACKING_USERNAME", secrets.token_urlsafe(32))
+    MLFLOW_TRACKING_PASSWORD = os.environ.get("MLFLOW_TRACKING_PASSWORD", secrets.token_urlsafe(72))
 
     @staticmethod
     def get_property(property_name):
         return getattr(AppConfig, property_name, None)
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/alembic.ini` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/env.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/models.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/db/utils.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/entities.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/permissions.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/routes.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/sqlalchemy_store.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/static/favicon.ico` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/static/style.css` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/static/style.css`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/398.70c7e628915a6c39.js` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/398.70c7e628915a6c39.js`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/3rdpartylicenses.txt` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/953.eb8714051ee666a2.js` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,66 @@
 "use strict";
 (self.webpackChunkmlflow_oidc_auth_front = self.webpackChunkmlflow_oidc_auth_front || []).push([
     [953], {
-        2953: (T, l, n) => {
-            n.r(l), n.d(l, {
-                HomePageModule: () => I
+        2953: (Z, m, n) => {
+            n.r(m), n.d(m, {
+                HomePageModule: () => w
             });
             var i = n(6895),
                 r = n(9197),
                 u = n(3732);
             const g = [{
                     title: "Experiment Name",
                     key: "name"
                 }, {
                     title: "Permission",
                     key: "permission"
                 }],
-                p = [{
+                d = [{
                     title: "Model name",
                     key: "name"
                 }, {
                     title: "Permissions",
                     key: "permission"
                 }];
             var e = n(4650),
-                d = n(5938),
+                p = n(5938),
                 f = n(705),
                 h = n(5419),
                 C = n(6709),
                 v = n(4859),
                 c = n(3848);
 
-            function P(t, a) {
+            function M(t, a) {
                 if (1 & t && e._UZ(0, "ml-table", 9), 2 & t) {
                     const o = e.oxw();
                     e.Q6J("columnConfig", o.experimentsColumnConfig)("data", o.experimentsDataSource)
                 }
             }
 
-            function y(t, a) {
+            function P(t, a) {
                 if (1 & t && e._UZ(0, "ml-table", 9), 2 & t) {
                     const o = e.oxw();
                     e.Q6J("columnConfig", o.modelsColumnConfig)("data", o.modelsDataSource)
                 }
             }
 
-            function M(t, a) {
+            function y(t, a) {
                 1 & t && (e.TgZ(0, "div", 10)(1, "span"), e._uU(2, "You have no experiments"), e.qZA()())
             }
 
-            function x(t, a) {
+            function b(t, a) {
                 1 & t && (e.TgZ(0, "div", 10)(1, "span"), e._uU(2, "You have no models"), e.qZA()())
             }
-            const b = [{
+            const x = [{
                 path: "",
                 component: (() => {
                     class t {
-                        constructor(o, s, m) {
-                            this.dialog = o, this.authService = s, this.userDataService = m, this.currentUserInfo = null, this.experimentsColumnConfig = g, this.modelsColumnConfig = p, this.experimentsDataSource = [], this.modelsDataSource = []
+                        constructor(o, s, l) {
+                            this.dialog = o, this.authService = s, this.userDataService = l, this.currentUserInfo = null, this.experimentsColumnConfig = g, this.modelsColumnConfig = d, this.experimentsDataSource = [], this.modelsDataSource = []
                         }
                         ngOnInit() {
                             if (this.currentUserInfo = this.authService.getUserInfo(), this.currentUserInfo) {
                                 const {
                                     experiment_permissions: o,
                                     registered_model_permissions: s
                                 } = this.currentUserInfo;
@@ -74,68 +74,73 @@
                                 this.dialog.open(u.eN, {
                                     data: {
                                         token: o
                                     }
                                 })
                             })
                         }
+                        redirectToMLFlow() {
+                            window.location.href = "/"
+                        }
                     }
                     return t.\u0275fac = function(o) {
-                        return new(o || t)(e.Y36(d.uw), e.Y36(f.e8), e.Y36(h.M))
+                        return new(o || t)(e.Y36(p.uw), e.Y36(f.e8), e.Y36(h.M))
                     }, t.\u0275cmp = e.Xpm({
                         type: t,
                         selectors: [
                             ["ml-home-page"]
                         ],
                         decls: 19,
                         vars: 4,
                         consts: [
                             [1, "controls-container", "pb-3"],
-                            ["mat-flat-button", "", "aria-label", "login", "color", "primary", 1, "me-2"],
+                            ["mat-flat-button", "", "aria-label", "login", "color", "primary", 1, "me-2", 3, "click"],
                             ["mat-flat-button", "", "aria-label", "login", "color", "primary", 3, "click"],
                             ["label", "Experiments"],
                             [1, "my-3"],
                             [3, "columnConfig", "data", 4, "ngIf", "ngIfElse"],
                             ["label", "Models"],
                             ["noExperimentData", ""],
                             ["noModelData", ""],
                             [3, "columnConfig", "data"],
                             [1, "d-flex", "w-100", "justify-content-center", "py-5"]
                         ],
                         template: function(o, s) {
-                            if (1 & o && (e.TgZ(0, "div", 0)(1, "button", 1)(2, "span"), e._uU(3, "Login to MLFlow"), e.qZA()(), e.TgZ(4, "button", 2), e.NdJ("click", function() {
+                            if (1 & o && (e.TgZ(0, "div", 0)(1, "button", 1), e.NdJ("click", function() {
+                                    return s.redirectToMLFlow()
+                                }), e.TgZ(2, "span"), e._uU(3, "Login to MLFlow"), e.qZA()(), e.TgZ(4, "button", 2), e.NdJ("click", function() {
                                     return s.showAccessKeyModal()
-                                }), e.TgZ(5, "span"), e._uU(6, "Create access key"), e.qZA()()(), e.TgZ(7, "div")(8, "mat-tab-group")(9, "mat-tab", 3)(10, "div", 4), e.YNc(11, P, 1, 2, "ml-table", 5), e.qZA()(), e.TgZ(12, "mat-tab", 6)(13, "div", 4), e.YNc(14, y, 1, 2, "ml-table", 5), e.qZA()()()(), e.YNc(15, M, 3, 0, "ng-template", null, 7, e.W1O), e.YNc(17, x, 3, 0, "ng-template", null, 8, e.W1O)), 2 & o) {
-                                const m = e.MAs(16),
-                                    Z = e.MAs(18);
-                                e.xp6(11), e.Q6J("ngIf", s.experimentsDataSource.length)("ngIfElse", m), e.xp6(3), e.Q6J("ngIf", s.modelsDataSource.length)("ngIfElse", Z)
+                                }), e.TgZ(5, "span"), e._uU(6, "Create access key"), e.qZA()()(), e.TgZ(7, "div")(8, "mat-tab-group")(9, "mat-tab", 3)(10, "div", 4), e.YNc(11, M, 1, 2, "ml-table", 5), e.qZA()(), e.TgZ(12, "mat-tab", 6)(13, "div", 4), e.YNc(14, P, 1, 2, "ml-table", 5), e.qZA()()()(), e.YNc(15, y, 3, 0, "ng-template", null, 7, e.W1O), e.YNc(17, b, 3, 0, "ng-template", null, 8, e.W1O)), 2 & o) {
+                                const l = e.MAs(16),
+                                    S = e.MAs(18);
+                                e.xp6(11), e.Q6J("ngIf", s.experimentsDataSource.length)("ngIfElse", l), e.xp6(3), e.Q6J("ngIf", s.modelsDataSource.length)("ngIfElse", S)
                             }
                         },
                         dependencies: [i.O5, C.a, v.lW, c.SP, c.uX],
                         styles: [".mat-column-experiment_id[_ngcontent-%COMP%], .mat-column-name[_ngcontent-%COMP%]{white-space:unset!important;width:50%!important;overflow-wrap:break-word;word-wrap:break-word;word-break:break-word;-webkit-hyphens:auto;hyphens:auto}"]
                     }), t
                 })()
             }];
             let H = (() => {
                 class t {}
                 return t.\u0275fac = function(o) {
                     return new(o || t)
                 }, t.\u0275mod = e.oAB({
                     type: t
                 }), t.\u0275inj = e.cJS({
-                    imports: [r.Bz.forChild(b), r.Bz]
+                    imports: [r.Bz.forChild(x), r.Bz]
                 }), t
             })();
-            var S = n(3912);
-            let I = (() => {
+            var T = n(3912);
+            let w = (() => {
                 class t {}
                 return t.\u0275fac = function(o) {
                     return new(o || t)
                 }, t.\u0275mod = e.oAB({
                     type: t
                 }), t.\u0275inj = e.cJS({
-                    imports: [i.ez, S.m, H]
+                    imports: [i.ez, T.m, H]
                 }), t
             })()
         }
     }
 ]);
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/favicon.ico` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/index.html` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -6,10 +6,10 @@
   <link rel="icon" type="image/x-icon" href="favicon.ico">
   <link rel="preconnect" href="https://fonts.gstatic.com">
   <style type="text/css">@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fCRc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fABc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fCBc4AMP6lbBP.woff2) format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fBxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fCxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fChc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:300;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmSU5fBBc4AMP6lQ.woff2) format('woff2');unicode-range:U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu72xKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu5mxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu7mxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4WxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu7WxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu7GxKKTU1Kvnz.woff2) format('woff2');unicode-range:U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4mxKKTU1Kg.woff2) format('woff2');unicode-range:U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fCRc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fABc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fCBc4AMP6lbBP.woff2) format('woff2');unicode-range:U+1F00-1FFF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fBxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0370-0377, U+037A-037F, U+0384-038A, U+038C, U+038E-03A1, U+03A3-03FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fCxc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fChc4AMP6lbBP.woff2) format('woff2');unicode-range:U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;}@font-face{font-family:'Roboto';font-style:normal;font-weight:500;font-display:swap;src:url(https://fonts.gstatic.com/s/roboto/v30/KFOlCnqEu92Fr1MmEU9fBBc4AMP6lQ.woff2) format('woff2');unicode-range:U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;}</style>
   <style type="text/css">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v142/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2');}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
 <style>.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}@charset "UTF-8";html,body{height:100%}body{margin:0;font-family:Roboto,Helvetica Neue,sans-serif}:root{--bs-blue:#0d6efd;--bs-indigo:#6610f2;--bs-purple:#6f42c1;--bs-pink:#d63384;--bs-red:#dc3545;--bs-orange:#fd7e14;--bs-yellow:#ffc107;--bs-green:#198754;--bs-teal:#20c997;--bs-cyan:#0dcaf0;--bs-black:#000;--bs-white:#fff;--bs-gray:#6c757d;--bs-gray-dark:#343a40;--bs-gray-100:#f8f9fa;--bs-gray-200:#e9ecef;--bs-gray-300:#dee2e6;--bs-gray-400:#ced4da;--bs-gray-500:#adb5bd;--bs-gray-600:#6c757d;--bs-gray-700:#495057;--bs-gray-800:#343a40;--bs-gray-900:#212529;--bs-primary:#0d6efd;--bs-secondary:#6c757d;--bs-success:#198754;--bs-info:#0dcaf0;--bs-warning:#ffc107;--bs-danger:#dc3545;--bs-light:#f8f9fa;--bs-dark:#212529;--bs-primary-rgb:13, 110, 253;--bs-secondary-rgb:108, 117, 125;--bs-success-rgb:25, 135, 84;--bs-info-rgb:13, 202, 240;--bs-warning-rgb:255, 193, 7;--bs-danger-rgb:220, 53, 69;--bs-light-rgb:248, 249, 250;--bs-dark-rgb:33, 37, 41;--bs-primary-text-emphasis:#052c65;--bs-secondary-text-emphasis:#2b2f32;--bs-success-text-emphasis:#0a3622;--bs-info-text-emphasis:#055160;--bs-warning-text-emphasis:#664d03;--bs-danger-text-emphasis:#58151c;--bs-light-text-emphasis:#495057;--bs-dark-text-emphasis:#495057;--bs-primary-bg-subtle:#cfe2ff;--bs-secondary-bg-subtle:#e2e3e5;--bs-success-bg-subtle:#d1e7dd;--bs-info-bg-subtle:#cff4fc;--bs-warning-bg-subtle:#fff3cd;--bs-danger-bg-subtle:#f8d7da;--bs-light-bg-subtle:#fcfcfd;--bs-dark-bg-subtle:#ced4da;--bs-primary-border-subtle:#9ec5fe;--bs-secondary-border-subtle:#c4c8cb;--bs-success-border-subtle:#a3cfbb;--bs-info-border-subtle:#9eeaf9;--bs-warning-border-subtle:#ffe69c;--bs-danger-border-subtle:#f1aeb5;--bs-light-border-subtle:#e9ecef;--bs-dark-border-subtle:#adb5bd;--bs-white-rgb:255, 255, 255;--bs-black-rgb:0, 0, 0;--bs-font-sans-serif:system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";--bs-font-monospace:SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;--bs-gradient:linear-gradient(180deg, rgba(255, 255, 255, .15), rgba(255, 255, 255, 0));--bs-body-font-family:var(--bs-font-sans-serif);--bs-body-font-size:1rem;--bs-body-font-weight:400;--bs-body-line-height:1.5;--bs-body-color:#212529;--bs-body-color-rgb:33, 37, 41;--bs-body-bg:#fff;--bs-body-bg-rgb:255, 255, 255;--bs-emphasis-color:#000;--bs-emphasis-color-rgb:0, 0, 0;--bs-secondary-color:rgba(33, 37, 41, .75);--bs-secondary-color-rgb:33, 37, 41;--bs-secondary-bg:#e9ecef;--bs-secondary-bg-rgb:233, 236, 239;--bs-tertiary-color:rgba(33, 37, 41, .5);--bs-tertiary-color-rgb:33, 37, 41;--bs-tertiary-bg:#f8f9fa;--bs-tertiary-bg-rgb:248, 249, 250;--bs-heading-color:inherit;--bs-link-color:#0d6efd;--bs-link-color-rgb:13, 110, 253;--bs-link-decoration:underline;--bs-link-hover-color:#0a58ca;--bs-link-hover-color-rgb:10, 88, 202;--bs-code-color:#d63384;--bs-highlight-color:#212529;--bs-highlight-bg:#fff3cd;--bs-border-width:1px;--bs-border-style:solid;--bs-border-color:#dee2e6;--bs-border-color-translucent:rgba(0, 0, 0, .175);--bs-border-radius:.375rem;--bs-border-radius-sm:.25rem;--bs-border-radius-lg:.5rem;--bs-border-radius-xl:1rem;--bs-border-radius-xxl:2rem;--bs-border-radius-2xl:var(--bs-border-radius-xxl);--bs-border-radius-pill:50rem;--bs-box-shadow:0 .5rem 1rem rgba(0, 0, 0, .15);--bs-box-shadow-sm:0 .125rem .25rem rgba(0, 0, 0, .075);--bs-box-shadow-lg:0 1rem 3rem rgba(0, 0, 0, .175);--bs-box-shadow-inset:inset 0 1px 2px rgba(0, 0, 0, .075);--bs-focus-ring-width:.25rem;--bs-focus-ring-opacity:.25;--bs-focus-ring-color:rgba(13, 110, 253, .25);--bs-form-valid-color:#198754;--bs-form-valid-border-color:#198754;--bs-form-invalid-color:#dc3545;--bs-form-invalid-border-color:#dc3545}*,*:before,*:after{box-sizing:border-box}@media (prefers-reduced-motion: no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:var(--bs-body-font-family);font-size:var(--bs-body-font-size);font-weight:var(--bs-body-font-weight);line-height:var(--bs-body-line-height);color:var(--bs-body-color);text-align:var(--bs-body-text-align);background-color:var(--bs-body-bg);-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:rgba(0,0,0,0)}:root{--bs-breakpoint-xs:0;--bs-breakpoint-sm:576px;--bs-breakpoint-md:768px;--bs-breakpoint-lg:992px;--bs-breakpoint-xl:1200px;--bs-breakpoint-xxl:1400px}</style><link rel="stylesheet" href="styles.68f068b304676cf1.css" media="print" onload="this.media='all'"><noscript><link rel="stylesheet" href="styles.68f068b304676cf1.css"></noscript></head>
 <body class="mat-typography">
   <app-root></app-root>
-<script src="runtime.5064f1f60b88aea4.js" type="module"></script><script src="polyfills.90a0049d0bf863c4.js" type="module"></script><script src="main.ff1acef2e224ca42.js" type="module"></script>
+<script src="runtime.0cd10aef5e6b1db8.js" type="module"></script><script src="polyfills.90a0049d0bf863c4.js" type="module"></script><script src="main.84383ebc03062e87.js" type="module"></script>
 
 </body></html>
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/main.ff1acef2e224ca42.js` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/main.84383ebc03062e87.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -53,14 +53,17 @@
                 };
             let L = (() => {
                 class be {
                     constructor() {
                         this.name = ""
                     }
                     ngOnInit() {}
+                    logout() {
+                        window.location.href = "/logout"
+                    }
                 }
                 return be.\u0275fac = function(fe) {
                     return new(fe || be)
                 }, be.\u0275cmp = s.Xpm({
                     type: be,
                     selectors: [
                         ["ml-header"]
@@ -71,18 +74,20 @@
                     decls: 14,
                     vars: 6,
                     consts: [
                         [1, "py-3"],
                         [1, "col-12", "d-flex", "align-items-center"],
                         [1, "mx-3"],
                         ["mat-button", "", 3, "routerLink"],
-                        ["mat-button", "", "aria-label", "logout", 1, "logout", 3, "routerLink"]
+                        ["mat-button", "", "aria-label", "logout", 1, "logout", 3, "routerLink", "click"]
                     ],
-                    template: function(fe, Oe) {
-                        1 & fe && (s.TgZ(0, "header", 0)(1, "div", 1)(2, "span"), s._uU(3), s.qZA(), s.TgZ(4, "nav", 2)(5, "a", 3), s._uU(6, "Home"), s.qZA(), s.TgZ(7, "a", 3), s._uU(8, "Admin panel"), s.qZA()(), s.TgZ(9, "button", 4)(10, "mat-icon"), s._uU(11, "exit_to_app"), s.qZA(), s.TgZ(12, "span"), s._uU(13, "Logout"), s.qZA()()()()), 2 & fe && (s.xp6(3), s.hij("Hello, ", Oe.name, ""), s.xp6(2), s.Q6J("routerLink", s.DdM(4, O)), s.xp6(2), s.Q6J("routerLink", s.DdM(5, De)), s.xp6(2), s.Q6J("routerLink", "/logout"))
+                    template: function(fe, Te) {
+                        1 & fe && (s.TgZ(0, "header", 0)(1, "div", 1)(2, "span"), s._uU(3), s.qZA(), s.TgZ(4, "nav", 2)(5, "a", 3), s._uU(6, "Home"), s.qZA(), s.TgZ(7, "a", 3), s._uU(8, "Admin panel"), s.qZA()(), s.TgZ(9, "button", 4), s.NdJ("click", function() {
+                            return Te.logout()
+                        }), s.TgZ(10, "mat-icon"), s._uU(11, "exit_to_app"), s.qZA(), s.TgZ(12, "span"), s._uU(13, "Logout"), s.qZA()()()()), 2 & fe && (s.xp6(3), s.hij("Hello, ", Te.name, ""), s.xp6(2), s.Q6J("routerLink", s.DdM(4, O)), s.xp6(2), s.Q6J("routerLink", s.DdM(5, De)), s.xp6(2), s.Q6J("routerLink", "/logout"))
                     },
                     dependencies: [S.Hw, C.lW, C.zs, F.yS, F.rH],
                     styles: [".logout[_ngcontent-%COMP%]{margin-left:auto}"]
                 }), be
             })()
         },
         3732: (Ht, $e, v) => {
@@ -113,15 +118,15 @@
                 value: O.MANAGE,
                 title: "Manage"
             }];
             var L = v(4650),
                 be = v(9549),
                 Me = v(4144),
                 fe = v(4859),
-                Oe = v(6895);
+                Te = v(6895);
 
             function ye(J, Ee) {
                 if (1 & J && (L.TgZ(0, "option", 6), L._uU(1), L.qZA()), 2 & J) {
                     const Ie = Ee.$implicit;
                     L.Q6J("value", Ie.value), L.xp6(1), L.Oqu(Ie.title)
                 }
             }
@@ -153,15 +158,15 @@
                         ["mat-button", "", 3, "mat-dialog-close"],
                         ["mat-button", "", "cdkFocusInitial", "", 3, "mat-dialog-close"],
                         [3, "value"]
                     ],
                     template: function(Ie, ze) {
                         1 & Ie && (L.TgZ(0, "h2", 0), L._uU(1), L.qZA(), L.TgZ(2, "mat-dialog-content", 1)(3, "mat-form-field")(4, "mat-label"), L._uU(5, "Permissions"), L.qZA(), L.TgZ(6, "select", 2), L.YNc(7, ye, 2, 2, "option", 3), L.qZA()()(), L.TgZ(8, "mat-dialog-actions")(9, "button", 4), L._uU(10, "Cancel"), L.qZA(), L.TgZ(11, "button", 5), L._uU(12, "Ok"), L.qZA()()), 2 & Ie && (L.xp6(1), L.Oqu(ze.title), L.xp6(1), L.Q6J("formGroup", ze.form), L.xp6(5), L.Q6J("ngForOf", ze.permissions), L.xp6(2), L.Q6J("mat-dialog-close", null), L.xp6(2), L.Q6J("mat-dialog-close", ze.form.value))
                     },
-                    dependencies: [be.KE, be.hX, Me.Nt, fe.lW, C.ZT, C.uh, C.xY, C.H8, Oe.sg, F.YN, F.Kr, F.EJ, F.JJ, F.JL, F.sg, F.u]
+                    dependencies: [be.KE, be.hX, Me.Nt, fe.lW, C.ZT, C.uh, C.xY, C.H8, Te.sg, F.YN, F.Kr, F.EJ, F.JJ, F.JL, F.sg, F.u]
                 }), J
             })();
 
             function xe(J, Ee) {
                 if (1 & J && (L.ynx(0), L.TgZ(1, "option", 9), L._uU(2), L.qZA(), L.BQk()), 2 & J) {
                     const Ie = Ee.$implicit;
                     L.xp6(1), L.s9C("value", Ie), L.xp6(1), L.Oqu(Ie)
@@ -206,15 +211,15 @@
                         ["mat-button", "", 3, "mat-dialog-close"],
                         ["mat-button", "", "cdkFocusInitial", "", 3, "mat-dialog-close", "disabled"],
                         [3, "value"]
                     ],
                     template: function(Ie, ze) {
                         1 & Ie && (L.TgZ(0, "h2", 0), L._uU(1), L.qZA(), L.TgZ(2, "mat-dialog-content", 1)(3, "div", 2)(4, "mat-form-field")(5, "mat-label"), L._uU(6), L.ALo(7, "titlecase"), L.qZA(), L.TgZ(8, "select", 3), L.YNc(9, xe, 3, 2, "ng-container", 4), L.qZA()(), L.TgZ(10, "mat-form-field")(11, "mat-label"), L._uU(12, "Permissions"), L.qZA(), L.TgZ(13, "select", 5), L.YNc(14, pe, 2, 2, "option", 6), L.qZA()()()(), L.TgZ(15, "mat-dialog-actions")(16, "button", 7), L._uU(17, "Cancel"), L.qZA(), L.TgZ(18, "button", 8), L._uU(19, "Ok"), L.qZA()()), 2 & Ie && (L.xp6(1), L.Oqu(ze.title), L.xp6(1), L.Q6J("formGroup", ze.form), L.xp6(4), L.Oqu(L.lcZ(7, 8, ze.data.entityType)), L.xp6(3), L.Q6J("ngForOf", ze.data.entities), L.xp6(5), L.Q6J("ngForOf", ze.permissions), L.xp6(2), L.Q6J("mat-dialog-close", null), L.xp6(2), L.Q6J("mat-dialog-close", ze.form.value)("disabled", ze.form.invalid))
                     },
-                    dependencies: [be.KE, be.hX, Me.Nt, fe.lW, C.ZT, C.uh, C.xY, C.H8, Oe.sg, F.YN, F.Kr, F.EJ, F.JJ, F.JL, F.sg, F.u, Oe.rS]
+                    dependencies: [be.KE, be.hX, Me.Nt, fe.lW, C.ZT, C.uh, C.xY, C.H8, Te.sg, F.YN, F.Kr, F.EJ, F.JJ, F.JL, F.sg, F.u, Te.rS]
                 }), J
             })();
             var Ve = v(7392);
             let We = (() => {
                 class J {
                     constructor(Ie) {
                         this.data = Ie, this.token = ""
@@ -303,15 +308,15 @@
                             ["mat-button", "", 3, "mat-dialog-close"],
                             ["mat-button", "", "cdkFocusInitial", "", 3, "mat-dialog-close", "disabled"],
                             [3, "value"]
                         ],
                         template: function(Ie, ze) {
                             1 & Ie && (L.TgZ(0, "h2", 0), L._uU(1), L.qZA(), L.TgZ(2, "mat-dialog-content", 1)(3, "div", 2)(4, "mat-form-field")(5, "mat-label"), L._uU(6, "Users"), L.qZA(), L.TgZ(7, "select", 3), L.YNc(8, ht, 2, 2, "option", 4), L.qZA()(), L.TgZ(9, "mat-form-field")(10, "mat-label"), L._uU(11, "Permissions"), L.qZA(), L.TgZ(12, "select", 5), L.YNc(13, lt, 2, 2, "option", 4), L.qZA()()()(), L.TgZ(14, "mat-dialog-actions")(15, "button", 6), L._uU(16, "Cancel"), L.qZA(), L.TgZ(17, "button", 7), L._uU(18, "Ok"), L.qZA()()), 2 & Ie && (L.xp6(1), L.Oqu(ze.title), L.xp6(1), L.Q6J("formGroup", ze.form), L.xp6(6), L.Q6J("ngForOf", ze.data.users), L.xp6(5), L.Q6J("ngForOf", ze.permissions), L.xp6(2), L.Q6J("mat-dialog-close", null), L.xp6(2), L.Q6J("mat-dialog-close", ze.form.value)("disabled", ze.form.invalid))
                         },
-                        dependencies: [be.KE, be.hX, Me.Nt, fe.lW, C.ZT, C.uh, C.xY, C.H8, Oe.sg, F.YN, F.Kr, F.EJ, F.JJ, F.JL, F.sg, F.u]
+                        dependencies: [be.KE, be.hX, Me.Nt, fe.lW, C.ZT, C.uh, C.xY, C.H8, Te.sg, F.YN, F.Kr, F.EJ, F.JJ, F.JL, F.sg, F.u]
                     }), J
                 })(),
                 te = (() => {
                     class J {}
                     return J.\u0275fac = function(Ie) {
                         return new(Ie || J)
                     }, J.\u0275cmp = L.Xpm({
@@ -358,15 +363,15 @@
                 if (1 & We && (s.TgZ(0, "td", 11), s._uU(1), s.qZA()), 2 & We) {
                     const lt = ht.$implicit,
                         ae = s.oxw().$implicit;
                     s.xp6(1), s.hij(" ", lt[ae.key], " ")
                 }
             }
 
-            function Oe(We, ht) {
+            function Te(We, ht) {
                 if (1 & We && (s.ynx(0)(1, 5), s.YNc(2, Me, 2, 1, "th", 6), s.YNc(3, fe, 2, 1, "td", 7), s.BQk()()), 2 & We) {
                     const lt = ht.$implicit;
                     s.xp6(1), s.Q6J("matColumnDef", lt.key)
                 }
             }
 
             function ye(We, ht) {
@@ -463,15 +468,15 @@
                         ["mat-menu-item", "", 3, "click"],
                         ["mat-header-row", ""],
                         ["mat-row", ""]
                     ],
                     template: function(lt, ae) {
                         1 & lt && (s.TgZ(0, "div", 0)(1, "mat-form-field")(2, "mat-label"), s._uU(3, "Search"), s.qZA(), s.TgZ(4, "input", 1, 2), s.NdJ("keyup", function(J) {
                             return ae.filter(J)
-                        }), s.qZA()()(), s.TgZ(6, "table", 3), s.YNc(7, Oe, 4, 1, "ng-container", 4), s.ynx(8, 5), s.YNc(9, ye, 2, 0, "th", 6), s.YNc(10, xe, 7, 2, "td", 7), s.BQk(), s.YNc(11, pe, 1, 0, "tr", 8), s.YNc(12, Ge, 1, 0, "tr", 9), s.qZA()), 2 & lt && (s.xp6(6), s.Q6J("dataSource", ae.dataSource), s.xp6(1), s.Q6J("ngForOf", ae.columnConfig), s.xp6(1), s.Q6J("matColumnDef", ae.columnActionName), s.xp6(3), s.Q6J("matHeaderRowDef", ae.columns), s.xp6(1), s.Q6J("matRowDefColumns", ae.columns))
+                        }), s.qZA()()(), s.TgZ(6, "table", 3), s.YNc(7, Te, 4, 1, "ng-container", 4), s.ynx(8, 5), s.YNc(9, ye, 2, 0, "th", 6), s.YNc(10, xe, 7, 2, "td", 7), s.BQk(), s.YNc(11, pe, 1, 0, "tr", 8), s.YNc(12, Ge, 1, 0, "tr", 9), s.qZA()), 2 & lt && (s.xp6(6), s.Q6J("dataSource", ae.dataSource), s.xp6(1), s.Q6J("ngForOf", ae.columnConfig), s.xp6(1), s.Q6J("matColumnDef", ae.columnActionName), s.xp6(3), s.Q6J("matHeaderRowDef", ae.columns), s.xp6(1), s.Q6J("matRowDefColumns", ae.columns))
                     },
                     dependencies: [S.BZ, S.fO, S.as, S.w1, S.Dz, S.nj, S.ge, S.ev, S.XQ, S.Gk, C.KE, C.hX, F.Nt, O.Hw, De.lW, L.VK, L.OP, L.p6, be.sg],
                     styles: [".mat-column-actions{white-space:unset!important;width:90px!important;overflow-wrap:break-word;word-wrap:break-word;word-break:break-word;-webkit-hyphens:auto;hyphens:auto}"]
                 }), We
             })()
         },
         4945: (Ht, $e, v) => {
@@ -591,15 +596,15 @@
         },
         705: (Ht, $e, v) => {
             v.d($e, {
                 e8: () => ye,
                 jR: () => L,
                 $N: () => s.$,
                 PQ: () => be.P,
-                cw: () => Oe,
+                cw: () => Te,
                 Mn: () => S.M
             });
             var s = v(4945),
                 S = v(5419),
                 C = v(4004),
                 F = v(9582),
                 O = v(4650),
@@ -629,15 +634,15 @@
                     factory: g.\u0275fac,
                     providedIn: "root"
                 }), g
             })();
             var be = v(5057),
                 Me = v(2590),
                 fe = v(6046);
-            let Oe = (() => {
+            let Te = (() => {
                     class g {
                         constructor(pe) {
                             this.snackBarService = pe
                         }
                         openSnackBar(pe) {
                             return this.snackBarService.open(pe, "OK", {
                                 duration: Me.i.SNACK_BAR_DURATION
@@ -680,26 +685,26 @@
                 F = v(9549),
                 O = v(4144),
                 De = v(7392),
                 L = v(4859),
                 be = v(3848),
                 Me = v(8255),
                 fe = v(5938),
-                Oe = v(1572),
+                Te = v(1572),
                 ye = v(6046),
                 g = v(4650);
-            const xe = [C.p0, F.lN, O.c, De.Ps, L.ot, be.Nh, Me.Tx, fe.Is, Oe.Cq, ye.ZX];
+            const xe = [C.p0, F.lN, O.c, De.Ps, L.ot, be.Nh, Me.Tx, fe.Is, Te.Cq, ye.ZX];
             let pe = (() => {
                 class a {}
                 return a.\u0275fac = function(r) {
                     return new(r || a)
                 }, a.\u0275mod = g.oAB({
                     type: a
                 }), a.\u0275inj = g.cJS({
-                    imports: [xe, C.p0, F.lN, O.c, De.Ps, L.ot, be.Nh, Me.Tx, fe.Is, Oe.Cq, ye.ZX]
+                    imports: [xe, C.p0, F.lN, O.c, De.Ps, L.ot, be.Nh, Me.Tx, fe.Is, Te.Cq, ye.ZX]
                 }), a
             })();
             var Ge = v(4006),
                 Ve = v(9751),
                 We = v(515),
                 ht = v(9646),
                 lt = v(7579),
@@ -1589,15 +1594,15 @@
             })();
             var De = v(8746),
                 L = v(705),
                 be = v(6895),
                 Me = v(6290),
                 fe = v(1572);
 
-            function Oe(B, h) {
+            function Te(B, h) {
                 if (1 & B && (S.ynx(0), S.TgZ(1, "div", 2), S._UZ(2, "ml-header", 3)(3, "router-outlet"), S.qZA(), S.BQk()), 2 & B) {
                     const p = S.oxw();
                     S.xp6(2), S.Q6J("name", p.user.display_name)
                 }
             }
 
             function ye(B, h) {
@@ -1627,15 +1632,15 @@
                         [4, "ngIf", "ngIfElse"],
                         ["loader", ""],
                         [1, "container"],
                         [3, "name"],
                         [1, "loader", "d-flex", "justify-content-center", "align-items-center"]
                     ],
                     template: function(p, I) {
-                        if (1 & p && (S.YNc(0, Oe, 4, 1, "ng-container", 0), S.YNc(1, ye, 2, 0, "ng-template", null, 1, S.W1O)), 2 & p) {
+                        if (1 & p && (S.YNc(0, Te, 4, 1, "ng-container", 0), S.YNc(1, ye, 2, 0, "ng-template", null, 1, S.W1O)), 2 & p) {
                             const V = S.MAs(2);
                             S.Q6J("ngIf", !I.loading && I.user)("ngIfElse", V)
                         }
                     },
                     dependencies: [be.O5, C.lC, Me.G, fe.Ou],
                     styles: [".loader[_ngcontent-%COMP%]{height:100vh}"]
                 }), B
@@ -1801,15 +1806,15 @@
                     return B.NOOP = new Je, B
                 })();
             const jt = "ng-enter",
                 Zt = "ng-leave",
                 mt = "ng-trigger",
                 Pt = ".ng-trigger",
                 ie = "ng-animating",
-                Te = ".ng-animating";
+                Se = ".ng-animating";
 
             function nt(B) {
                 if ("number" == typeof B) return B;
                 const h = B.match(/^(-?[\.\d]+)(m?s)/);
                 return !h || h.length < 2 ? 0 : xt(parseFloat(h[1]), h[2])
             }
 
@@ -2228,15 +2233,15 @@
                     let q = 0;
                     const Fe = [];
                     let Le = !1,
                         at = !1,
                         Rt = 0;
                     const qt = h.steps.map(w => {
                         const U = this._makeStyleAst(w, p);
-                        let Se = null != U.offset ? U.offset : function ns(B) {
+                        let Oe = null != U.offset ? U.offset : function ns(B) {
                                 if ("string" == typeof B) return null;
                                 let h = null;
                                 if (Array.isArray(B)) B.forEach(p => {
                                     if (p instanceof Map && p.has("offset")) {
                                         const I = p;
                                         h = parseFloat(I.get("offset")), I.delete("offset")
                                     }
@@ -2244,15 +2249,15 @@
                                 else if (B instanceof Map && B.has("offset")) {
                                     const p = B;
                                     h = parseFloat(p.get("offset")), p.delete("offset")
                                 }
                                 return h
                             }(U.styles),
                             dt = 0;
-                        return null != Se && (q++, dt = U.offset = Se), at = at || dt < 0 || dt > 1, Le = Le || dt < Rt, Rt = dt, Fe.push(dt), U
+                        return null != Oe && (q++, dt = U.offset = Oe), at = at || dt < 0 || dt > 1, Le = Le || dt < Rt, Rt = dt, Fe.push(dt), U
                     });
                     at && p.errors.push(function $t() {
                         return new S.vHH(3012, !1)
                     }()), Le && p.errors.push(function Lt() {
                         return new S.vHH(3200, !1)
                     }());
                     const rn = h.steps.length;
@@ -2261,17 +2266,17 @@
                         return new S.vHH(3202, !1)
                     }()) : 0 == q && (Hn = 1 / (rn - 1));
                     const Vn = rn - 1,
                         Cn = p.currentTime,
                         b = p.currentAnimateTimings,
                         P = b.duration;
                     return qt.forEach((w, U) => {
-                        const Se = Hn > 0 ? U == Vn ? 1 : Hn * U : Fe[U],
-                            dt = Se * P;
-                        p.currentTime = Cn + b.delay + dt, b.duration = dt, this._validateStyleAst(w, p), w.offset = Se, I.styles.push(w)
+                        const Oe = Hn > 0 ? U == Vn ? 1 : Hn * U : Fe[U],
+                            dt = Oe * P;
+                        p.currentTime = Cn + b.delay + dt, b.duration = dt, this._validateStyleAst(w, p), w.offset = Oe, I.styles.push(w)
                     }), I
                 }
                 visitReference(h, p) {
                     return {
                         type: 8,
                         animation: Xn(this, Qn(h.animation), p),
                         options: fr(h.options)
@@ -2292,15 +2297,15 @@
                 }
                 visitQuery(h, p) {
                     const I = p.currentQuerySelector,
                         V = h.options || {};
                     p.queryCount++, p.currentQuery = h;
                     const [q, Fe] = function To(B) {
                         const h = !!B.split(/\s*,\s*/).find(p => ":self" == p);
-                        return h && (B = B.replace(ti, "")), B = B.replace(/@\*/g, Pt).replace(/@\w+/g, p => Pt + "-" + p.slice(1)).replace(/:animating/g, Te), [B, h]
+                        return h && (B = B.replace(ti, "")), B = B.replace(/@\*/g, Pt).replace(/@\w+/g, p => Pt + "-" + p.slice(1)).replace(/:animating/g, Se), [B, h]
                     }(h.selector);
                     p.currentQuerySelector = I.length ? I + " " + q : q, Tt(p.collectedStyles, p.currentQuerySelector, new Map);
                     const Le = Xn(this, Qn(h.animation), p);
                     return p.currentQuery = null, p.currentQuerySelector = I, {
                         type: 11,
                         selector: q,
                         limit: V.limit || 0,
@@ -2815,34 +2820,34 @@
                     const rn = [],
                         Hn = this.ast.options && this.ast.options.params || Yr,
                         Cn = this.buildStyles(I, Le && Le.params || Yr, rn),
                         b = at && at.params || Yr,
                         P = this.buildStyles(V, b, rn),
                         w = new Set,
                         U = new Map,
-                        Se = new Map,
+                        Oe = new Map,
                         dt = "void" === V,
                         Ot = {
                             params: Br(b, Hn),
                             delay: this.ast.options?.delay
                         },
                         Jt = qt ? [] : Mr(h, p, this.ast.animation, q, Fe, Cn, P, Ot, Rt, rn);
                     let An = 0;
                     if (Jt.forEach(Gn => {
                             An = Math.max(Gn.duration + Gn.delay, An)
-                        }), rn.length) return Oo(p, this._triggerName, I, V, dt, Cn, P, [], [], U, Se, An, rn);
+                        }), rn.length) return Oo(p, this._triggerName, I, V, dt, Cn, P, [], [], U, Oe, An, rn);
                     Jt.forEach(Gn => {
                         const yn = Gn.element,
                             hi = Tt(U, yn, new Set);
                         Gn.preStyleProps.forEach(ai => hi.add(ai));
-                        const Zn = Tt(Se, yn, new Set);
+                        const Zn = Tt(Oe, yn, new Set);
                         Gn.postStyleProps.forEach(ai => Zn.add(ai)), yn !== p && w.add(yn)
                     });
                     const Ln = Ri(w.values());
-                    return Oo(p, this._triggerName, I, V, dt, Cn, P, Jt, Ln, U, Se, An)
+                    return Oo(p, this._triggerName, I, V, dt, Cn, P, Jt, Ln, U, Oe, An)
                 }
             }
 
             function Br(B, h) {
                 const p = Tn(h);
                 for (const I in B) B.hasOwnProperty(I) && null != B[I] && (p[I] = B[I]);
                 return p
@@ -3362,15 +3367,15 @@
                     return Sr(p) ? this._fetchNamespace(h).listen(p, I, V, q) : () => {}
                 }
                 _buildInstruction(h, p, I, V, q) {
                     return h.transition.build(this.driver, h.element, h.fromState.value, h.toState.value, I, V, h.fromState.options, h.toState.options, p, q)
                 }
                 destroyInnerAnimations(h) {
                     let p = this.driver.query(h, Pt, !0);
-                    p.forEach(I => this.destroyActiveAnimationsForElement(I)), 0 != this.playersByQueriedElement.size && (p = this.driver.query(h, Te, !0), p.forEach(I => this.finishActiveQueriedAnimationOnElement(I)))
+                    p.forEach(I => this.destroyActiveAnimationsForElement(I)), 0 != this.playersByQueriedElement.size && (p = this.driver.query(h, Se, !0), p.forEach(I => this.finishActiveQueriedAnimationOnElement(I)))
                 }
                 destroyActiveAnimationsForElement(h) {
                     const p = this.playersByElement.get(h);
                     p && p.forEach(I => {
                         I.queued ? I.markedForDestroy = !0 : I.destroy()
                     })
                 }
@@ -3450,25 +3455,25 @@
                         w = new Set,
                         U = new Set;
                     for (let Xt = 0; Xt < this.collectedLeaveElements.length; Xt++) {
                         const Kt = this.collectedLeaveElements[Xt],
                             hn = Kt[_i];
                         hn && hn.setForRemoval && (P.push(Kt), w.add(Kt), hn.hasAnimation ? this.driver.query(Kt, ".ng-star-inserted", !0).forEach(Sn => w.add(Sn)) : U.add(Kt))
                     }
-                    const Se = new Map,
+                    const Oe = new Map,
                         dt = $n(Hn, Array.from(w));
                     dt.forEach((Xt, Kt) => {
                         const hn = Zt + b++;
-                        Se.set(Kt, hn), Xt.forEach(Sn => Bi(Sn, hn))
+                        Oe.set(Kt, hn), Xt.forEach(Sn => Bi(Sn, hn))
                     }), h.push(() => {
                         Vn.forEach((Xt, Kt) => {
                             const hn = Cn.get(Kt);
                             Xt.forEach(Sn => tr(Sn, hn))
                         }), dt.forEach((Xt, Kt) => {
-                            const hn = Se.get(Kt);
+                            const hn = Oe.get(Kt);
                             Xt.forEach(Sn => tr(Sn, hn))
                         }), P.forEach(Xt => {
                             this.processLeaveNode(Xt)
                         })
                     });
                     const Ot = [],
                         Jt = [];
@@ -3486,15 +3491,15 @@
                                         Xr.value = qr, ar.set(hn.triggerName, Xr)
                                     }
                                 }
                                 return void Sn.destroy()
                             }
                         }
                         const sr = !rn || !this.driver.containsElement(rn, li),
-                            Ki = Se.get(li),
+                            Ki = Oe.get(li),
                             Rr = Cn.get(li),
                             ci = this._buildInstruction(hn, I, Rr, Ki, sr);
                         if (ci.errors && ci.errors.length) return void Jt.push(ci);
                         if (sr) return Sn.onStart(() => pn(li, ci.fromStyles)), Sn.onDestroy(() => tn(li, ci.toStyles)), void V.push(Sn);
                         if (hn.isFallbackTransition) return Sn.onStart(() => pn(li, ci.fromStyles)), Sn.onDestroy(() => tn(li, ci.toStyles)), void V.push(Sn);
                         const Jr = [];
                         ci.timelines.forEach(Hi => {
@@ -3590,15 +3595,15 @@
                         const Kt = P[Xt],
                             hn = Kt[_i];
                         if (tr(Kt, Zt), hn && hn.hasAnimation) continue;
                         let Sn = [];
                         if (Le.size) {
                             let sr = Le.get(Kt);
                             sr && sr.length && Sn.push(...sr);
-                            let Ki = this.driver.query(Kt, Te, !0);
+                            let Ki = this.driver.query(Kt, Se, !0);
                             for (let Rr = 0; Rr < Ki.length; Rr++) {
                                 let ci = Le.get(Ki[Rr]);
                                 ci && ci.length && Sn.push(...ci)
                             }
                         }
                         const li = Sn.filter(sr => !sr.destroyed);
                         li.length ? vi(this, Kt, li) : this.processLeaveNode(Kt)
@@ -3665,17 +3670,17 @@
                             const P = b[_i];
                             if (P && P.removedBeforeQueried) return new xe.ZN(Cn.duration, Cn.delay);
                             const w = b !== at,
                                 U = function x(B) {
                                     const h = [];
                                     return R(B, h), h
                                 }((I.get(b) || Wo).map(An => An.getRealPlayer())).filter(An => !!An.element && An.element === b),
-                                Se = q.get(b),
+                                Oe = q.get(b),
                                 dt = Fe.get(b),
-                                Ot = j(0, this._normalizer, 0, Cn.keyframes, Se, dt),
+                                Ot = j(0, this._normalizer, 0, Cn.keyframes, Oe, dt),
                                 Jt = this._buildPlayer(Cn, Ot, U);
                             if (Cn.subTimeline && V && rn.add(b), w) {
                                 const An = new Ro(h, Le, b);
                                 An.setRealPlayer(Jt), Rt.push(An)
                             }
                             return Jt
                         });
@@ -4464,15 +4469,15 @@
                         xe && (this._subscribe = xe)
                     }
                     lift(xe) {
                         const pe = new ye;
                         return pe.source = this, pe.operator = xe, pe
                     }
                     subscribe(xe, pe, Ge) {
-                        const Ve = function Oe(ye) {
+                        const Ve = function Te(ye) {
                             return ye && ye instanceof s.Lv || function fe(ye) {
                                 return ye && (0, De.m)(ye.next) && (0, De.m)(ye.error) && (0, De.m)(ye.complete)
                             }(ye) && (0, S.Nn)(ye)
                         }(xe) ? xe : new s.Hp(xe, pe, Ge);
                         return (0, L.x)(() => {
                             const {
                                 operator: We,
@@ -4540,108 +4545,108 @@
             var O = v(8737),
                 De = v(2806);
             let L = (() => {
                 class Me extends s.y {
                     constructor() {
                         super(), this.closed = !1, this.currentObservers = null, this.observers = [], this.isStopped = !1, this.hasError = !1, this.thrownError = null
                     }
-                    lift(Oe) {
+                    lift(Te) {
                         const ye = new be(this, this);
-                        return ye.operator = Oe, ye
+                        return ye.operator = Te, ye
                     }
                     _throwIfClosed() {
                         if (this.closed) throw new F
                     }
-                    next(Oe) {
+                    next(Te) {
                         (0, De.x)(() => {
                             if (this._throwIfClosed(), !this.isStopped) {
                                 this.currentObservers || (this.currentObservers = Array.from(this.observers));
-                                for (const ye of this.currentObservers) ye.next(Oe)
+                                for (const ye of this.currentObservers) ye.next(Te)
                             }
                         })
                     }
-                    error(Oe) {
+                    error(Te) {
                         (0, De.x)(() => {
                             if (this._throwIfClosed(), !this.isStopped) {
-                                this.hasError = this.isStopped = !0, this.thrownError = Oe;
+                                this.hasError = this.isStopped = !0, this.thrownError = Te;
                                 const {
                                     observers: ye
                                 } = this;
-                                for (; ye.length;) ye.shift().error(Oe)
+                                for (; ye.length;) ye.shift().error(Te)
                             }
                         })
                     }
                     complete() {
                         (0, De.x)(() => {
                             if (this._throwIfClosed(), !this.isStopped) {
                                 this.isStopped = !0;
                                 const {
-                                    observers: Oe
+                                    observers: Te
                                 } = this;
-                                for (; Oe.length;) Oe.shift().complete()
+                                for (; Te.length;) Te.shift().complete()
                             }
                         })
                     }
                     unsubscribe() {
                         this.isStopped = this.closed = !0, this.observers = this.currentObservers = null
                     }
                     get observed() {
-                        var Oe;
-                        return (null === (Oe = this.observers) || void 0 === Oe ? void 0 : Oe.length) > 0
+                        var Te;
+                        return (null === (Te = this.observers) || void 0 === Te ? void 0 : Te.length) > 0
                     }
-                    _trySubscribe(Oe) {
-                        return this._throwIfClosed(), super._trySubscribe(Oe)
+                    _trySubscribe(Te) {
+                        return this._throwIfClosed(), super._trySubscribe(Te)
                     }
-                    _subscribe(Oe) {
-                        return this._throwIfClosed(), this._checkFinalizedStatuses(Oe), this._innerSubscribe(Oe)
+                    _subscribe(Te) {
+                        return this._throwIfClosed(), this._checkFinalizedStatuses(Te), this._innerSubscribe(Te)
                     }
-                    _innerSubscribe(Oe) {
+                    _innerSubscribe(Te) {
                         const {
                             hasError: ye,
                             isStopped: g,
                             observers: xe
                         } = this;
-                        return ye || g ? S.Lc : (this.currentObservers = null, xe.push(Oe), new S.w0(() => {
-                            this.currentObservers = null, (0, O.P)(xe, Oe)
+                        return ye || g ? S.Lc : (this.currentObservers = null, xe.push(Te), new S.w0(() => {
+                            this.currentObservers = null, (0, O.P)(xe, Te)
                         }))
                     }
-                    _checkFinalizedStatuses(Oe) {
+                    _checkFinalizedStatuses(Te) {
                         const {
                             hasError: ye,
                             thrownError: g,
                             isStopped: xe
                         } = this;
-                        ye ? Oe.error(g) : xe && Oe.complete()
+                        ye ? Te.error(g) : xe && Te.complete()
                     }
                     asObservable() {
-                        const Oe = new s.y;
-                        return Oe.source = this, Oe
+                        const Te = new s.y;
+                        return Te.source = this, Te
                     }
                 }
-                return Me.create = (fe, Oe) => new be(fe, Oe), Me
+                return Me.create = (fe, Te) => new be(fe, Te), Me
             })();
             class be extends L {
-                constructor(fe, Oe) {
-                    super(), this.destination = fe, this.source = Oe
+                constructor(fe, Te) {
+                    super(), this.destination = fe, this.source = Te
                 }
                 next(fe) {
-                    var Oe, ye;
-                    null === (ye = null === (Oe = this.destination) || void 0 === Oe ? void 0 : Oe.next) || void 0 === ye || ye.call(Oe, fe)
+                    var Te, ye;
+                    null === (ye = null === (Te = this.destination) || void 0 === Te ? void 0 : Te.next) || void 0 === ye || ye.call(Te, fe)
                 }
                 error(fe) {
-                    var Oe, ye;
-                    null === (ye = null === (Oe = this.destination) || void 0 === Oe ? void 0 : Oe.error) || void 0 === ye || ye.call(Oe, fe)
+                    var Te, ye;
+                    null === (ye = null === (Te = this.destination) || void 0 === Te ? void 0 : Te.error) || void 0 === ye || ye.call(Te, fe)
                 }
                 complete() {
-                    var fe, Oe;
-                    null === (Oe = null === (fe = this.destination) || void 0 === fe ? void 0 : fe.complete) || void 0 === Oe || Oe.call(fe)
+                    var fe, Te;
+                    null === (Te = null === (fe = this.destination) || void 0 === fe ? void 0 : fe.complete) || void 0 === Te || Te.call(fe)
                 }
                 _subscribe(fe) {
-                    var Oe, ye;
-                    return null !== (ye = null === (Oe = this.source) || void 0 === Oe ? void 0 : Oe.subscribe(fe)) && void 0 !== ye ? ye : S.Lc
+                    var Te, ye;
+                    return null !== (ye = null === (Te = this.source) || void 0 === Te ? void 0 : Te.subscribe(fe)) && void 0 !== ye ? ye : S.Lc
                 }
             }
         },
         930: (Ht, $e, v) => {
             v.d($e, {
                 Hp: () => Ge,
                 Lv: () => ye
@@ -4657,15 +4662,15 @@
                 return {
                     kind: ae,
                     value: te,
                     error: J
                 }
             }
             var fe = v(3410),
-                Oe = v(2806);
+                Te = v(2806);
             class ye extends S.w0 {
                 constructor(te) {
                     super(), this.isStopped = !1, te ? (this.destination = te, (0, S.Nn)(te) && te.add(this)) : this.destination = lt
                 }
                 static create(te, J, Ee) {
                     return new Ge(te, J, Ee)
                 }
@@ -4760,15 +4765,15 @@
                         }) : Ie = te
                     }
                     this.destination = new pe(Ie)
                 }
             }
 
             function Ve(ae) {
-                C.v.useDeprecatedSynchronousErrorHandling ? (0, Oe.O)(ae) : (0, F.h)(ae)
+                C.v.useDeprecatedSynchronousErrorHandling ? (0, Te.O)(ae) : (0, F.h)(ae)
             }
 
             function ht(ae, te) {
                 const {
                     onStoppedNotification: J
                 } = C.v;
                 J && fe.z.setTimeout(() => J(ae, te))
@@ -4785,33 +4790,33 @@
         727: (Ht, $e, v) => {
             v.d($e, {
                 Lc: () => De,
                 w0: () => O,
                 Nn: () => L
             });
             var s = v(576);
-            const C = (0, v(3888).d)(Me => function(Oe) {
-                Me(this), this.message = Oe ? `${Oe.length} errors occurred during unsubscription:\n${Oe.map((ye,g)=>`${g+1}) ${ye.toString()}`).join("\n  ")}` : "", this.name = "UnsubscriptionError", this.errors = Oe
+            const C = (0, v(3888).d)(Me => function(Te) {
+                Me(this), this.message = Te ? `${Te.length} errors occurred during unsubscription:\n${Te.map((ye,g)=>`${g+1}) ${ye.toString()}`).join("\n  ")}` : "", this.name = "UnsubscriptionError", this.errors = Te
             });
             var F = v(8737);
             class O {
                 constructor(fe) {
                     this.initialTeardown = fe, this.closed = !1, this._parentage = null, this._finalizers = null
                 }
                 unsubscribe() {
                     let fe;
                     if (!this.closed) {
                         this.closed = !0;
                         const {
-                            _parentage: Oe
+                            _parentage: Te
                         } = this;
-                        if (Oe)
-                            if (this._parentage = null, Array.isArray(Oe))
-                                for (const xe of Oe) xe.remove(this);
-                            else Oe.remove(this);
+                        if (Te)
+                            if (this._parentage = null, Array.isArray(Te))
+                                for (const xe of Te) xe.remove(this);
+                            else Te.remove(this);
                         const {
                             initialTeardown: ye
                         } = this;
                         if ((0, s.m)(ye)) try {
                             ye()
                         } catch (xe) {
                             fe = xe instanceof C ? xe.errors : [xe]
@@ -4827,47 +4832,47 @@
                                 fe = fe ?? [], pe instanceof C ? fe = [...fe, ...pe.errors] : fe.push(pe)
                             }
                         }
                         if (fe) throw new C(fe)
                     }
                 }
                 add(fe) {
-                    var Oe;
+                    var Te;
                     if (fe && fe !== this)
                         if (this.closed) be(fe);
                         else {
                             if (fe instanceof O) {
                                 if (fe.closed || fe._hasParent(this)) return;
                                 fe._addParent(this)
-                            }(this._finalizers = null !== (Oe = this._finalizers) && void 0 !== Oe ? Oe : []).push(fe)
+                            }(this._finalizers = null !== (Te = this._finalizers) && void 0 !== Te ? Te : []).push(fe)
                         }
                 }
                 _hasParent(fe) {
                     const {
-                        _parentage: Oe
+                        _parentage: Te
                     } = this;
-                    return Oe === fe || Array.isArray(Oe) && Oe.includes(fe)
+                    return Te === fe || Array.isArray(Te) && Te.includes(fe)
                 }
                 _addParent(fe) {
                     const {
-                        _parentage: Oe
+                        _parentage: Te
                     } = this;
-                    this._parentage = Array.isArray(Oe) ? (Oe.push(fe), Oe) : Oe ? [Oe, fe] : fe
+                    this._parentage = Array.isArray(Te) ? (Te.push(fe), Te) : Te ? [Te, fe] : fe
                 }
                 _removeParent(fe) {
                     const {
-                        _parentage: Oe
+                        _parentage: Te
                     } = this;
-                    Oe === fe ? this._parentage = null : Array.isArray(Oe) && (0, F.P)(Oe, fe)
+                    Te === fe ? this._parentage = null : Array.isArray(Te) && (0, F.P)(Te, fe)
                 }
                 remove(fe) {
                     const {
-                        _finalizers: Oe
+                        _finalizers: Te
                     } = this;
-                    Oe && (0, F.P)(Oe, fe), fe instanceof O && fe._removeParent(this)
+                    Te && (0, F.P)(Te, fe), fe instanceof O && fe._removeParent(this)
                 }
             }
             O.EMPTY = (() => {
                 const Me = new O;
                 return Me.closed = !0, Me
             })();
             const De = O.EMPTY;
@@ -4910,15 +4915,15 @@
                 const xe = (0, De.yG)(g),
                     pe = (0, De.jO)(g),
                     {
                         args: Ge,
                         keys: Ve
                     } = (0, S.D)(g);
                 if (0 === Ge.length) return (0, C.D)([], xe);
-                const We = new s.y(function Oe(g, xe, pe = F.y) {
+                const We = new s.y(function Te(g, xe, pe = F.y) {
                     return Ge => {
                         ye(xe, () => {
                             const {
                                 length: Ve
                             } = g, We = new Array(Ve);
                             let ht = Ve,
                                 lt = Ve;
@@ -4985,28 +4990,28 @@
                 O = v(5403),
                 De = v(3268),
                 L = v(1810);
 
             function be(...Me) {
                 const fe = (0, F.jO)(Me),
                     {
-                        args: Oe,
+                        args: Te,
                         keys: ye
                     } = (0, S.D)(Me),
                     g = new s.y(xe => {
                         const {
                             length: pe
-                        } = Oe;
+                        } = Te;
                         if (!pe) return void xe.complete();
                         const Ge = new Array(pe);
                         let Ve = pe,
                             We = pe;
                         for (let ht = 0; ht < pe; ht++) {
                             let lt = !1;
-                            (0, C.Xf)(Oe[ht]).subscribe((0, O.x)(xe, ae => {
+                            (0, C.Xf)(Te[ht]).subscribe((0, O.x)(xe, ae => {
                                 lt || (lt = !0, We--), Ge[ht] = ae
                             }, () => Ve--, void 0, () => {
                                 (!Ve || !lt) && (We || xe.next(ye ? (0, L.n)(ye, Ge) : Ge), xe.complete())
                             }))
                         }
                     });
                 return fe ? g.pipe((0, De.Z)(fe)) : g
@@ -5029,15 +5034,15 @@
 
             function De(Ie, ze = 0) {
                 return (0, C.e)((vt, Ft) => {
                     Ft.add(Ie.schedule(() => vt.subscribe(Ft), ze))
                 })
             }
             var Me = v(9751),
-                Oe = v(2202),
+                Te = v(2202),
                 ye = v(576);
 
             function xe(Ie, ze) {
                 if (!Ie) throw new Error("Iterable cannot be null");
                 return new Me.y(vt => {
                     (0, S.f)(vt, ze, () => {
                         const Ft = Ie[Symbol.asyncIterator]();
@@ -5075,15 +5080,15 @@
                             return (0, s.Xf)(Ie).pipe(De(ze), O(ze))
                         }(Ie, ze);
                         if ((0, ht.D)(Ie)) return xe(Ie, ze);
                         if ((0, We.T)(Ie)) return function g(Ie, ze) {
                             return new Me.y(vt => {
                                 let Ft;
                                 return (0, S.f)(vt, ze, () => {
-                                    Ft = Ie[Oe.h](), (0, S.f)(vt, ze, () => {
+                                    Ft = Ie[Te.h](), (0, S.f)(vt, ze, () => {
                                         let kt, $t;
                                         try {
                                             ({
                                                 value: kt,
                                                 done: $t
                                             } = Ft.next())
                                         } catch (Lt) {
@@ -5118,26 +5123,26 @@
 
             function fe(pe, Ge, Ve, We) {
                 if ((0, O.m)(Ve) && (We = Ve, Ve = void 0), We) return fe(pe, Ge, Ve).pipe((0, De.Z)(We));
                 const [ht, lt] = function xe(pe) {
                     return (0, O.m)(pe.addEventListener) && (0, O.m)(pe.removeEventListener)
                 }(pe) ? be.map(ae => te => pe[ae](Ge, te, Ve)): function ye(pe) {
                     return (0, O.m)(pe.addListener) && (0, O.m)(pe.removeListener)
-                }(pe) ? L.map(Oe(pe, Ge)) : function g(pe) {
+                }(pe) ? L.map(Te(pe, Ge)) : function g(pe) {
                     return (0, O.m)(pe.on) && (0, O.m)(pe.off)
-                }(pe) ? Me.map(Oe(pe, Ge)) : [];
+                }(pe) ? Me.map(Te(pe, Ge)) : [];
                 if (!ht && (0, F.z)(pe)) return (0, C.z)(ae => fe(ae, Ge, Ve))((0, s.Xf)(pe));
                 if (!ht) throw new TypeError("Invalid event target");
                 return new S.y(ae => {
                     const te = (...J) => ae.next(1 < J.length ? J : J[0]);
                     return ht(te), () => lt(te)
                 })
             }
 
-            function Oe(pe, Ge) {
+            function Te(pe, Ge) {
                 return Ve => We => pe[Ve](Ge, We)
             }
         },
         8421: (Ht, $e, v) => {
             v.d($e, {
                 Xf: () => g
             });
@@ -5147,15 +5152,15 @@
                 F = v(9751),
                 O = v(3670),
                 De = v(2206),
                 L = v(4532),
                 be = v(6495),
                 Me = v(3260),
                 fe = v(576),
-                Oe = v(7849),
+                Te = v(7849),
                 ye = v(8822);
 
             function g(ae) {
                 if (ae instanceof F.y) return ae;
                 if (null != ae) {
                     if ((0, O.c)(ae)) return function xe(ae) {
                         return new F.y(te => {
@@ -5170,15 +5175,15 @@
                             te.complete()
                         })
                     }(ae);
                     if ((0, C.t)(ae)) return function Ge(ae) {
                         return new F.y(te => {
                             ae.then(J => {
                                 te.closed || (te.next(J), te.complete())
-                            }, J => te.error(J)).then(null, Oe.h)
+                            }, J => te.error(J)).then(null, Te.h)
                         })
                     }(ae);
                     if ((0, De.D)(ae)) return We(ae);
                     if ((0, be.T)(ae)) return function Ve(ae) {
                         return new F.y(te => {
                             for (const J of ae)
                                 if (te.next(J), te.closed) return;
@@ -5266,55 +5271,55 @@
             var s = v(9751),
                 S = v(4986),
                 C = v(3532);
 
             function O(De = 0, L, be = S.P) {
                 let Me = -1;
                 return null != L && ((0, C.K)(L) ? be = L : Me = L), new s.y(fe => {
-                    let Oe = function F(De) {
+                    let Te = function F(De) {
                         return De instanceof Date && !isNaN(De)
                     }(De) ? +De - be.now() : De;
-                    Oe < 0 && (Oe = 0);
+                    Te < 0 && (Te = 0);
                     let ye = 0;
                     return be.schedule(function() {
                         fe.closed || (fe.next(ye++), 0 <= Me ? this.schedule(void 0, Me) : fe.complete())
-                    }, Oe)
+                    }, Te)
                 })
             }
         },
         5403: (Ht, $e, v) => {
             v.d($e, {
                 x: () => S
             });
             var s = v(930);
 
             function S(F, O, De, L, be) {
                 return new C(F, O, De, L, be)
             }
             class C extends s.Lv {
                 constructor(O, De, L, be, Me, fe) {
-                    super(O), this.onFinalize = Me, this.shouldUnsubscribe = fe, this._next = De ? function(Oe) {
+                    super(O), this.onFinalize = Me, this.shouldUnsubscribe = fe, this._next = De ? function(Te) {
                         try {
-                            De(Oe)
+                            De(Te)
                         } catch (ye) {
                             O.error(ye)
                         }
-                    } : super._next, this._error = be ? function(Oe) {
+                    } : super._next, this._error = be ? function(Te) {
                         try {
-                            be(Oe)
+                            be(Te)
                         } catch (ye) {
                             O.error(ye)
                         } finally {
                             this.unsubscribe()
                         }
                     } : super._error, this._complete = L ? function() {
                         try {
                             L()
-                        } catch (Oe) {
-                            O.error(Oe)
+                        } catch (Te) {
+                            O.error(Te)
                         } finally {
                             this.unsubscribe()
                         }
                     } : super._complete
                 }
                 unsubscribe() {
                     var O;
@@ -5335,16 +5340,16 @@
                 S = v(5403),
                 C = v(4482);
 
             function F(O) {
                 return (0, C.e)((De, L) => {
                     let fe, be = null,
                         Me = !1;
-                    be = De.subscribe((0, S.x)(L, void 0, void 0, Oe => {
-                        fe = (0, s.Xf)(O(Oe, F(O)(De))), be ? (be.unsubscribe(), be = null, fe.subscribe(L)) : Me = !0
+                    be = De.subscribe((0, S.x)(L, void 0, void 0, Te => {
+                        fe = (0, s.Xf)(O(Te, F(O)(De))), be ? (be.unsubscribe(), be = null, fe.subscribe(L)) : Me = !0
                     })), Me && (be.unsubscribe(), be = null, fe.subscribe(L))
                 })
             }
         },
         4351: (Ht, $e, v) => {
             v.d($e, {
                 b: () => C
@@ -5364,31 +5369,31 @@
                 S = v(4482),
                 C = v(5403);
 
             function F(O, De = s.z) {
                 return (0, S.e)((L, be) => {
                     let Me = null,
                         fe = null,
-                        Oe = null;
+                        Te = null;
                     const ye = () => {
                         if (Me) {
                             Me.unsubscribe(), Me = null;
                             const xe = fe;
                             fe = null, be.next(xe)
                         }
                     };
 
                     function g() {
-                        const xe = Oe + O,
+                        const xe = Te + O,
                             pe = De.now();
                         if (pe < xe) return Me = this.schedule(void 0, xe - pe), void be.add(Me);
                         ye()
                     }
                     L.subscribe((0, C.x)(be, xe => {
-                        fe = xe, Oe = De.now(), Me || (Me = De.schedule(g, O), be.add(Me))
+                        fe = xe, Te = De.now(), Me || (Me = De.schedule(g, O), be.add(Me))
                     }, () => {
                         ye(), be.complete()
                     }, void 0, () => {
                         fe = Me = null
                     }))
                 })
             }
@@ -5409,35 +5414,35 @@
             function fe(g, xe) {
                 return xe ? pe => (0, S.z)(xe.pipe((0, C.q)(1), function L() {
                     return (0, F.e)((g, xe) => {
                         g.subscribe((0, O.x)(xe, De.Z))
                     })
                 }()), pe.pipe(fe(g))) : (0, Me.z)((pe, Ge) => g(pe, Ge).pipe((0, C.q)(1), (0, be.h)(pe)))
             }
-            var Oe = v(5963);
+            var Te = v(5963);
 
             function ye(g, xe = s.z) {
-                const pe = (0, Oe.H)(g, xe);
+                const pe = (0, Te.H)(g, xe);
                 return fe(() => pe)
             }
         },
         1884: (Ht, $e, v) => {
             v.d($e, {
                 x: () => F
             });
             var s = v(4671),
                 S = v(4482),
                 C = v(5403);
 
             function F(De, L = s.y) {
                 return De = De ?? O, (0, S.e)((be, Me) => {
-                    let fe, Oe = !0;
+                    let fe, Te = !0;
                     be.subscribe((0, C.x)(Me, ye => {
                         const g = L(ye);
-                        (Oe || !De(fe, g)) && (Oe = !1, fe = g, Me.next(ye))
+                        (Te || !De(fe, g)) && (Te = !1, fe = g, Me.next(ye))
                     }))
                 })
             }
 
             function O(De, L) {
                 return De === L
             }
@@ -5516,28 +5521,28 @@
             var s = v(4004),
                 S = v(8421),
                 C = v(4482),
                 F = v(9672),
                 O = v(5403),
                 L = v(576);
 
-            function be(Me, fe, Oe = 1 / 0) {
-                return (0, L.m)(fe) ? be((ye, g) => (0, s.U)((xe, pe) => fe(ye, xe, g, pe))((0, S.Xf)(Me(ye, g))), Oe) : ("number" == typeof fe && (Oe = fe), (0, C.e)((ye, g) => function De(Me, fe, Oe, ye, g, xe, pe, Ge) {
+            function be(Me, fe, Te = 1 / 0) {
+                return (0, L.m)(fe) ? be((ye, g) => (0, s.U)((xe, pe) => fe(ye, xe, g, pe))((0, S.Xf)(Me(ye, g))), Te) : ("number" == typeof fe && (Te = fe), (0, C.e)((ye, g) => function De(Me, fe, Te, ye, g, xe, pe, Ge) {
                     const Ve = [];
                     let We = 0,
                         ht = 0,
                         lt = !1;
                     const ae = () => {
                             lt && !Ve.length && !We && fe.complete()
                         },
                         te = Ee => We < ye ? J(Ee) : Ve.push(Ee),
                         J = Ee => {
                             xe && fe.next(Ee), We++;
                             let Ie = !1;
-                            (0, S.Xf)(Oe(Ee, ht++)).subscribe((0, O.x)(fe, ze => {
+                            (0, S.Xf)(Te(Ee, ht++)).subscribe((0, O.x)(fe, ze => {
                                 g?.(ze), xe ? te(ze) : fe.next(ze)
                             }, () => {
                                 Ie = !0
                             }, void 0, () => {
                                 if (Ie) try {
                                     for (We--; Ve.length && We < ye;) {
                                         const ze = Ve.shift();
@@ -5550,15 +5555,15 @@
                             }))
                         };
                     return Me.subscribe((0, O.x)(fe, te, () => {
                         lt = !0, ae()
                     })), () => {
                         Ge?.()
                     }
-                }(ye, g, Me, Oe)))
+                }(ye, g, Me, Te)))
             }
         },
         3099: (Ht, $e, v) => {
             v.d($e, {
                 B: () => O
             });
             var s = v(8421),
@@ -5567,15 +5572,15 @@
                 F = v(4482);
 
             function O(L = {}) {
                 const {
                     connector: be = (() => new S.x),
                     resetOnError: Me = !0,
                     resetOnComplete: fe = !0,
-                    resetOnRefCountZero: Oe = !0
+                    resetOnRefCountZero: Te = !0
                 } = L;
                 return ye => {
                     let g, xe, pe, Ge = 0,
                         Ve = !1,
                         We = !1;
                     const ht = () => {
                             xe?.unsubscribe(), xe = void 0
@@ -5587,15 +5592,15 @@
                             const te = g;
                             lt(), te?.unsubscribe()
                         };
                     return (0, F.e)((te, J) => {
                         Ge++, !We && !Ve && ht();
                         const Ee = pe = pe ?? be();
                         J.add(() => {
-                            Ge--, 0 === Ge && !We && !Ve && (xe = De(ae, Oe))
+                            Ge--, 0 === Ge && !We && !Ve && (xe = De(ae, Te))
                         }), Ee.subscribe(J), !g && Ge > 0 && (g = new C.Hp({
                             next: Ie => Ee.next(Ie),
                             error: Ie => {
                                 We = !0, ht(), xe = De(lt, Me, Ie), Ee.error(Ie)
                             },
                             complete: () => {
                                 Ve = !0, ht(), xe = De(lt, fe), Ee.complete()
@@ -5649,25 +5654,25 @@
                 S = v(4482),
                 C = v(5403);
 
             function F(O, De) {
                 return (0, S.e)((L, be) => {
                     let Me = null,
                         fe = 0,
-                        Oe = !1;
-                    const ye = () => Oe && !Me && be.complete();
+                        Te = !1;
+                    const ye = () => Te && !Me && be.complete();
                     L.subscribe((0, C.x)(be, g => {
                         Me?.unsubscribe();
                         let xe = 0;
                         const pe = fe++;
                         (0, s.Xf)(O(g, pe)).subscribe(Me = (0, C.x)(be, Ge => be.next(De ? De(g, Ge, pe, xe++) : Ge), () => {
                             Me = null, ye()
                         }))
                     }, () => {
-                        Oe = !0, ye()
+                        Te = !0, ye()
                     }))
                 })
             }
         },
         5698: (Ht, $e, v) => {
             v.d($e, {
                 q: () => F
@@ -5711,27 +5716,27 @@
 
             function O(De, L, be) {
                 const Me = (0, s.m)(De) || L || be ? {
                     next: De,
                     error: L,
                     complete: be
                 } : De;
-                return Me ? (0, S.e)((fe, Oe) => {
+                return Me ? (0, S.e)((fe, Te) => {
                     var ye;
                     null === (ye = Me.subscribe) || void 0 === ye || ye.call(Me);
                     let g = !0;
-                    fe.subscribe((0, C.x)(Oe, xe => {
+                    fe.subscribe((0, C.x)(Te, xe => {
                         var pe;
-                        null === (pe = Me.next) || void 0 === pe || pe.call(Me, xe), Oe.next(xe)
+                        null === (pe = Me.next) || void 0 === pe || pe.call(Me, xe), Te.next(xe)
                     }, () => {
                         var xe;
-                        g = !1, null === (xe = Me.complete) || void 0 === xe || xe.call(Me), Oe.complete()
+                        g = !1, null === (xe = Me.complete) || void 0 === xe || xe.call(Me), Te.complete()
                     }, xe => {
                         var pe;
-                        g = !1, null === (pe = Me.error) || void 0 === pe || pe.call(Me, xe), Oe.error(xe)
+                        g = !1, null === (pe = Me.error) || void 0 === pe || pe.call(Me, xe), Te.error(xe)
                     }, () => {
                         var xe, pe;
                         g && (null === (xe = Me.unsubscribe) || void 0 === xe || xe.call(Me)), null === (pe = Me.finalize) || void 0 === pe || pe.call(Me)
                     }))
                 }) : F.y
             }
         },
@@ -5769,16 +5774,16 @@
                     super(L, be), this.scheduler = L, this.work = be, this.pending = !1
                 }
                 schedule(L, be = 0) {
                     var Me;
                     if (this.closed) return this;
                     this.state = L;
                     const fe = this.id,
-                        Oe = this.scheduler;
-                    return null != fe && (this.id = this.recycleAsyncId(Oe, fe, be)), this.pending = !0, this.delay = be, this.id = null !== (Me = this.id) && void 0 !== Me ? Me : this.requestAsyncId(Oe, this.id, be), this
+                        Te = this.scheduler;
+                    return null != fe && (this.id = this.recycleAsyncId(Te, fe, be)), this.pending = !0, this.delay = be, this.id = null !== (Me = this.id) && void 0 !== Me ? Me : this.requestAsyncId(Te, this.id, be), this
                 }
                 requestAsyncId(L, be, Me = 0) {
                     return C.setInterval(L.flush.bind(L, this), Me)
                 }
                 recycleAsyncId(L, be, Me = 0) {
                     if (null != Me && this.delay === Me && !1 === this.pending) return be;
                     null != be && C.clearInterval(be)
@@ -5790,16 +5795,16 @@
                     if (Me) return Me;
                     !1 === this.pending && null != this.id && (this.id = this.recycleAsyncId(this.scheduler, this.id, null))
                 }
                 _execute(L, be) {
                     let fe, Me = !1;
                     try {
                         this.work(L)
-                    } catch (Oe) {
-                        Me = !0, fe = Oe || new Error("Scheduled action threw falsy error")
+                    } catch (Te) {
+                        Me = !0, fe = Te || new Error("Scheduled action threw falsy error")
                     }
                     if (Me) return this.unsubscribe(), fe
                 }
                 unsubscribe() {
                     if (!this.closed) {
                         const {
                             id: L,
@@ -5905,15 +5910,15 @@
                     } while ((Ve = ht[0]) && Ve.id === We && ht.shift());
                     if (this._active = !1, lt) {
                         for (;
                             (Ve = ht[0]) && Ve.id === We && ht.shift();) Ve.unsubscribe();
                         throw lt
                     }
                 }
-            }(class Oe extends s.o {
+            }(class Te extends s.o {
                 constructor(Ve, We) {
                     super(Ve, We), this.scheduler = Ve, this.work = We
                 }
                 requestAsyncId(Ve, We, ht = 0) {
                     return null !== ht && ht > 0 ? super.requestAsyncId(Ve, We, ht) : (Ve.actions.push(this), Ve._scheduled || (Ve._scheduled = fe.setImmediate(Ve.flush.bind(Ve, void 0))))
                 }
                 recycleAsyncId(Ve, We, ht = 0) {
@@ -6294,15 +6299,15 @@
                 IO: () => pe,
                 LC: () => S,
                 SB: () => Me,
                 X$: () => F,
                 ZE: () => ht,
                 ZN: () => We,
                 _j: () => s,
-                eR: () => Oe,
+                eR: () => Te,
                 jt: () => O,
                 k1: () => lt,
                 l3: () => C,
                 oB: () => be,
                 pV: () => g,
                 ru: () => De,
                 vP: () => L
@@ -6357,15 +6362,15 @@
                     type: 0,
                     name: ae,
                     styles: te,
                     options: J
                 }
             }
 
-            function Oe(ae, te, J = null) {
+            function Te(ae, te, J = null) {
                 return {
                     type: 1,
                     expr: ae,
                     animation: te,
                     options: J
                 }
             }
@@ -6541,15 +6546,15 @@
                 F = v(7579),
                 O = v(727),
                 De = v(1135),
                 L = v(9646),
                 be = v(9521),
                 Me = v(8505),
                 fe = v(8372),
-                Oe = v(9300),
+                Te = v(9300),
                 ye = v(4004),
                 g = v(5698),
                 xe = v(5684),
                 pe = v(1884),
                 Ge = v(2722),
                 Ve = v(1281),
                 We = v(9643);
@@ -6574,15 +6579,15 @@
                 withHorizontalOrientation(Ne) {
                     return this._horizontal = Ne, this
                 }
                 withAllowedModifierKeys(Ne) {
                     return this._allowedModifierKeys = Ne, this
                 }
                 withTypeAhead(Ne = 200) {
-                    return this._typeaheadSubscription.unsubscribe(), this._typeaheadSubscription = this._letterKeyStream.pipe((0, Me.b)(ge => this._pressedLetters.push(ge)), (0, fe.b)(Ne), (0, Oe.h)(() => this._pressedLetters.length > 0), (0, ye.U)(() => this._pressedLetters.join(""))).subscribe(ge => {
+                    return this._typeaheadSubscription.unsubscribe(), this._typeaheadSubscription = this._letterKeyStream.pipe((0, Me.b)(ge => this._pressedLetters.push(ge)), (0, fe.b)(Ne), (0, Te.h)(() => this._pressedLetters.length > 0), (0, ye.U)(() => this._pressedLetters.join(""))).subscribe(ge => {
                         const tt = this._getItemsArray();
                         for (let pt = 1; pt < tt.length + 1; pt++) {
                             const jt = (this._activeItemIndex + pt) % tt.length,
                                 Zt = tt[jt];
                             if (!this._skipPredicateFn(Zt) && 0 === Zt.getLabel().toUpperCase().trim().indexOf(ge)) {
                                 this.setActiveItem(jt);
                                 break
@@ -6984,15 +6989,15 @@
                     class Je {
                         constructor(ge, tt, pt, jt, Zt) {
                             this._ngZone = ge, this._platform = tt, this._inputModalityDetector = pt, this._origin = null, this._windowFocused = !1, this._originFromTouchInteraction = !1, this._elementInfo = new Map, this._monitoredElementCount = 0, this._rootNodeFocusListenerCount = new Map, this._windowFocusListener = () => {
                                 this._windowFocused = !0, this._windowFocusTimeoutId = window.setTimeout(() => this._windowFocused = !1)
                             }, this._stopInputModalityDetector = new F.x, this._rootNodeFocusAndBlurListener = mt => {
                                 const Pt = (0, C.sA)(mt),
                                     ie = "focus" === mt.type ? this._onFocus : this._onBlur;
-                                for (let Te = Pt; Te; Te = Te.parentElement) ie.call(this, mt, Te)
+                                for (let Se = Pt; Se; Se = Se.parentElement) ie.call(this, mt, Se)
                             }, this._document = jt, this._detectionMode = Zt?.detectionMode || 0
                         }
                         monitor(ge, tt = !1) {
                             const pt = (0, Ve.fI)(ge);
                             if (!this._platform.isBrowser || 1 !== pt.nodeType) return (0, L.of)(null);
                             const jt = (0, C.kV)(pt) || this._getDocument(),
                                 Zt = this._elementInfo.get(pt);
@@ -7184,16 +7189,16 @@
                 O = /^(ar|ckb|dv|he|iw|fa|nqo|ps|sd|ug|ur|yi|.*[-_](Adlm|Arab|Hebr|Nkoo|Rohg|Thaa))(?!.*[-_](Latn|Cyrl)($|-|_))($|-|_)/i;
             let L = (() => {
                     class fe {
                         constructor(ye) {
                             if (this.value = "ltr", this.change = new s.vpe, ye) {
                                 const xe = ye.documentElement ? ye.documentElement.dir : null;
                                 this.value = function De(fe) {
-                                    const Oe = fe?.toLowerCase() || "";
-                                    return "auto" === Oe && typeof navigator < "u" && navigator?.language ? O.test(navigator.language) ? "rtl" : "ltr" : "rtl" === Oe ? "rtl" : "ltr"
+                                    const Te = fe?.toLowerCase() || "";
+                                    return "auto" === Te && typeof navigator < "u" && navigator?.language ? O.test(navigator.language) ? "rtl" : "ltr" : "rtl" === Te ? "rtl" : "ltr"
                                 }((ye.body ? ye.body.dir : null) || xe || "ltr")
                             }
                         }
                         ngOnDestroy() {
                             this.change.complete()
                         }
                     }
@@ -7261,27 +7266,27 @@
                 Mf: () => C,
                 SV: () => ht,
                 Sd: () => Ge,
                 Vb: () => mn,
                 Z: () => rt,
                 aO: () => wn,
                 b2: () => nn,
-                hY: () => Oe,
+                hY: () => Te,
                 jx: () => L,
                 oh: () => Ve,
                 uR: () => pe,
                 xE: () => Ie,
                 zL: () => be
             });
             const C = 9,
                 O = 13,
                 De = 16,
                 L = 17,
                 be = 18,
-                Oe = 27,
+                Te = 27,
                 ye = 32,
                 pe = 35,
                 Ge = 36,
                 Ve = 37,
                 We = 38,
                 ht = 39,
                 lt = 40,
@@ -7450,15 +7455,15 @@
                 F = v(1281),
                 O = v(3353),
                 De = v(445),
                 L = v(4080),
                 be = v(7579),
                 Me = v(727),
                 fe = v(6451),
-                Oe = v(5698),
+                Te = v(5698),
                 ye = v(2722);
             const g = (0, O.Mq)();
             class xe {
                 constructor(G, $) {
                     this._viewportRuler = G, this._previousHTMLStyles = {
                         top: "",
                         left: ""
@@ -7723,15 +7728,15 @@
                 }
                 get hostElement() {
                     return this._host
                 }
                 attach(G) {
                     !this._host.parentElement && this._previousHostParent && this._previousHostParent.appendChild(this._host);
                     const $ = this._portalOutlet.attach(G);
-                    return this._positionStrategy && this._positionStrategy.attach(this), this._updateStackingOrder(), this._updateElementSize(), this._updateElementDirection(), this._scrollStrategy && this._scrollStrategy.enable(), this._ngZone.onStable.pipe((0, Oe.q)(1)).subscribe(() => {
+                    return this._positionStrategy && this._positionStrategy.attach(this), this._updateStackingOrder(), this._updateElementSize(), this._updateElementDirection(), this._scrollStrategy && this._scrollStrategy.enable(), this._ngZone.onStable.pipe((0, Te.q)(1)).subscribe(() => {
                         this.hasAttached() && this.updatePosition()
                     }), this._togglePointerEvents(!0), this._config.hasBackdrop && this._attachBackdrop(), this._config.panelClass && this._toggleClasses(this._pane, this._config.panelClass, !0), this._attachments.next(), this._keyboardDispatcher.add(this), this._config.disposeOnNavigation && (this._locationChanges = this._location.subscribe(() => this.dispose())), this._outsideClickDispatcher.add(this), $
                 }
                 detach() {
                     if (!this.hasAttached()) return;
                     this.detachBackdrop(), this._togglePointerEvents(!1), this._positionStrategy && this._positionStrategy.detach && this._positionStrategy.detach(), this._scrollStrategy && this._scrollStrategy.disable();
                     const G = this._portalOutlet.detach();
@@ -8361,15 +8366,15 @@
             })()
         },
         3353: (Ht, $e, v) => {
             v.d($e, {
                 Mq: () => xe,
                 Oy: () => ae,
                 ht: () => ht,
-                i$: () => Oe,
+                i$: () => Te,
                 kV: () => We,
                 qK: () => be,
                 sA: () => lt,
                 t4: () => F
             });
             var s = v(4650),
                 S = v(6895);
@@ -8399,15 +8404,15 @@
                 if (De) return De;
                 if ("object" != typeof document || !document) return De = new Set(L), De;
                 let te = document.createElement("input");
                 return De = new Set(L.filter(J => (te.setAttribute("type", J), te.type === J))), De
             }
             let Me, g, Ge;
 
-            function Oe(te) {
+            function Te(te) {
                 return function fe() {
                     if (null == Me && typeof window < "u") try {
                         window.addEventListener("test", null, Object.defineProperty({}, "passive", {
                             get: () => Me = !0
                         }))
                     } finally {
                         Me = Me || !1
@@ -8460,15 +8465,15 @@
                 return typeof __karma__ < "u" && !!__karma__ || typeof jasmine < "u" && !!jasmine || typeof jest < "u" && !!jest || typeof Mocha < "u" && !!Mocha
             }
         },
         4080: (Ht, $e, v) => {
             v.d($e, {
                 C5: () => fe,
                 Pl: () => ht,
-                UE: () => Oe,
+                UE: () => Te,
                 eL: () => ae,
                 en: () => g,
                 u0: () => pe
             });
             var s = v(4650),
                 S = v(6895);
             class Me {
@@ -8487,15 +8492,15 @@
                 }
             }
             class fe extends Me {
                 constructor(Ee, Ie, ze, vt) {
                     super(), this.component = Ee, this.viewContainerRef = Ie, this.injector = ze, this.componentFactoryResolver = vt
                 }
             }
-            class Oe extends Me {
+            class Te extends Me {
                 constructor(Ee, Ie, ze) {
                     super(), this.templateRef = Ee, this.viewContainerRef = Ie, this.context = ze
                 }
                 get origin() {
                     return this.templateRef.elementRef
                 }
                 attach(Ee, Ie = this.context) {
@@ -8514,15 +8519,15 @@
                 constructor() {
                     this._isDisposed = !1, this.attachDomPortal = null
                 }
                 hasAttached() {
                     return !!this._attachedPortal
                 }
                 attach(Ee) {
-                    return Ee instanceof fe ? (this._attachedPortal = Ee, this.attachComponentPortal(Ee)) : Ee instanceof Oe ? (this._attachedPortal = Ee, this.attachTemplatePortal(Ee)) : this.attachDomPortal && Ee instanceof ye ? (this._attachedPortal = Ee, this.attachDomPortal(Ee)) : void 0
+                    return Ee instanceof fe ? (this._attachedPortal = Ee, this.attachComponentPortal(Ee)) : Ee instanceof Te ? (this._attachedPortal = Ee, this.attachTemplatePortal(Ee)) : this.attachDomPortal && Ee instanceof ye ? (this._attachedPortal = Ee, this.attachDomPortal(Ee)) : void 0
                 }
                 detach() {
                     this._attachedPortal && (this._attachedPortal.setAttachedHost(null), this._attachedPortal = null), this._invokeDisposeFn()
                 }
                 dispose() {
                     this.hasAttached() && this.detach(), this._invokeDisposeFn(), this._isDisposed = !0
                 }
@@ -8671,16 +8676,16 @@
                     const {
                         delegate: Q
                     } = Me;
                     return (Q?.cancelAnimationFrame || cancelAnimationFrame)(...ee)
                 },
                 delegate: void 0
             };
-            var Oe = v(640);
-            new class ye extends Oe.v {
+            var Te = v(640);
+            new class ye extends Te.v {
                 flush(Q) {
                     this._active = !0;
                     const X = this._scheduled;
                     this._scheduled = void 0;
                     const {
                         actions: He
                     } = this;
@@ -8959,22 +8964,22 @@
                 }
                 return b.\u0275fac = function(w) {
                     return new(w || b)
                 }, b.\u0275prov = s.Yz7({
                     token: b,
                     factory: function() {
                         return function Me() {
-                            return (0, s.LFG)(Oe)
+                            return (0, s.LFG)(Te)
                         }()
                     },
                     providedIn: "platform"
                 }), b
             })();
             const fe = new s.OlP("Location Initialized");
-            let Oe = (() => {
+            let Te = (() => {
                 class b extends be {
                     constructor(w) {
                         super(), this._doc = w, this._init()
                     }
                     _init() {
                         this.location = window.location, this._history = window.history
                     }
@@ -9009,19 +9014,19 @@
                     }
                     get hash() {
                         return this.location.hash
                     }
                     set pathname(w) {
                         this.location.pathname = w
                     }
-                    pushState(w, U, Se) {
-                        ye() ? this._history.pushState(w, U, Se) : this.location.hash = Se
+                    pushState(w, U, Oe) {
+                        ye() ? this._history.pushState(w, U, Oe) : this.location.hash = Oe
                     }
-                    replaceState(w, U, Se) {
-                        ye() ? this._history.replaceState(w, U, Se) : this.location.hash = Se
+                    replaceState(w, U, Oe) {
+                        ye() ? this._history.replaceState(w, U, Oe) : this.location.hash = Oe
                     }
                     forward() {
                         this._history.forward()
                     }
                     back() {
                         this._history.back()
                     }
@@ -9034,15 +9039,15 @@
                 }
                 return b.\u0275fac = function(w) {
                     return new(w || b)(s.LFG(L))
                 }, b.\u0275prov = s.Yz7({
                     token: b,
                     factory: function() {
                         return function g() {
-                            return new Oe((0, s.LFG)(L))
+                            return new Te((0, s.LFG)(L))
                         }()
                     },
                     providedIn: "platform"
                 }), b
             })();
 
             function ye() {
@@ -9097,23 +9102,23 @@
                             return this._baseHref
                         }
                         prepareExternalUrl(w) {
                             return xe(this._baseHref, w)
                         }
                         path(w = !1) {
                             const U = this._platformLocation.pathname + Ge(this._platformLocation.search),
-                                Se = this._platformLocation.hash;
-                            return Se && w ? `${U}${Se}` : U
+                                Oe = this._platformLocation.hash;
+                            return Oe && w ? `${U}${Oe}` : U
                         }
-                        pushState(w, U, Se, dt) {
-                            const Ot = this.prepareExternalUrl(Se + Ge(dt));
+                        pushState(w, U, Oe, dt) {
+                            const Ot = this.prepareExternalUrl(Oe + Ge(dt));
                             this._platformLocation.pushState(w, U, Ot)
                         }
-                        replaceState(w, U, Se, dt) {
-                            const Ot = this.prepareExternalUrl(Se + Ge(dt));
+                        replaceState(w, U, Oe, dt) {
+                            const Ot = this.prepareExternalUrl(Oe + Ge(dt));
                             this._platformLocation.replaceState(w, U, Ot)
                         }
                         forward() {
                             this._platformLocation.forward()
                         }
                         back() {
                             this._platformLocation.back()
@@ -9151,20 +9156,20 @@
                             let U = this._platformLocation.hash;
                             return null == U && (U = "#"), U.length > 0 ? U.substring(1) : U
                         }
                         prepareExternalUrl(w) {
                             const U = xe(this._baseHref, w);
                             return U.length > 0 ? "#" + U : U
                         }
-                        pushState(w, U, Se, dt) {
-                            let Ot = this.prepareExternalUrl(Se + Ge(dt));
+                        pushState(w, U, Oe, dt) {
+                            let Ot = this.prepareExternalUrl(Oe + Ge(dt));
                             0 == Ot.length && (Ot = this._platformLocation.pathname), this._platformLocation.pushState(w, U, Ot)
                         }
-                        replaceState(w, U, Se, dt) {
-                            let Ot = this.prepareExternalUrl(Se + Ge(dt));
+                        replaceState(w, U, Oe, dt) {
+                            let Ot = this.prepareExternalUrl(Oe + Ge(dt));
                             0 == Ot.length && (Ot = this._platformLocation.pathname), this._platformLocation.replaceState(w, U, Ot)
                         }
                         forward() {
                             this._platformLocation.forward()
                         }
                         back() {
                             this._platformLocation.back()
@@ -9184,20 +9189,20 @@
                     }), b
                 })(),
                 ae = (() => {
                     class b {
                         constructor(w) {
                             this._subject = new s.vpe, this._urlChangeListeners = [], this._urlChangeSubscription = null, this._locationStrategy = w;
                             const U = this._locationStrategy.getBaseHref();
-                            this._baseHref = pe(Ee(U)), this._locationStrategy.onPopState(Se => {
+                            this._baseHref = pe(Ee(U)), this._locationStrategy.onPopState(Oe => {
                                 this._subject.emit({
                                     url: this.path(!0),
                                     pop: !0,
-                                    state: Se.state,
-                                    type: Se.type
+                                    state: Oe.state,
+                                    type: Oe.type
                                 })
                             })
                         }
                         ngOnDestroy() {
                             this._urlChangeSubscription?.unsubscribe(), this._urlChangeListeners = []
                         }
                         path(w = !1) {
@@ -9213,19 +9218,19 @@
                             return b.stripTrailingSlash(function J(b, P) {
                                 return b && P.startsWith(b) ? P.substring(b.length) : P
                             }(this._baseHref, Ee(w)))
                         }
                         prepareExternalUrl(w) {
                             return w && "/" !== w[0] && (w = "/" + w), this._locationStrategy.prepareExternalUrl(w)
                         }
-                        go(w, U = "", Se = null) {
-                            this._locationStrategy.pushState(Se, "", w, U), this._notifyUrlChangeListeners(this.prepareExternalUrl(w + Ge(U)), Se)
+                        go(w, U = "", Oe = null) {
+                            this._locationStrategy.pushState(Oe, "", w, U), this._notifyUrlChangeListeners(this.prepareExternalUrl(w + Ge(U)), Oe)
                         }
-                        replaceState(w, U = "", Se = null) {
-                            this._locationStrategy.replaceState(Se, "", w, U), this._notifyUrlChangeListeners(this.prepareExternalUrl(w + Ge(U)), Se)
+                        replaceState(w, U = "", Oe = null) {
+                            this._locationStrategy.replaceState(Oe, "", w, U), this._notifyUrlChangeListeners(this.prepareExternalUrl(w + Ge(U)), Oe)
                         }
                         forward() {
                             this._locationStrategy.forward()
                         }
                         back() {
                             this._locationStrategy.back()
                         }
@@ -9237,21 +9242,21 @@
                                 this._notifyUrlChangeListeners(U.url, U.state)
                             })), () => {
                                 const U = this._urlChangeListeners.indexOf(w);
                                 this._urlChangeListeners.splice(U, 1), 0 === this._urlChangeListeners.length && (this._urlChangeSubscription?.unsubscribe(), this._urlChangeSubscription = null)
                             }
                         }
                         _notifyUrlChangeListeners(w = "", U) {
-                            this._urlChangeListeners.forEach(Se => Se(w, U))
+                            this._urlChangeListeners.forEach(Oe => Oe(w, U))
                         }
-                        subscribe(w, U, Se) {
+                        subscribe(w, U, Oe) {
                             return this._subject.subscribe({
                                 next: w,
                                 error: U,
-                                complete: Se
+                                complete: Oe
                             })
                         }
                     }
                     return b.normalizeQueryParams = Ge, b.joinWithSlash = xe, b.stripTrailingSlash = pe, b.\u0275fac = function(w) {
                         return new(w || b)(s.LFG(Ve))
                     }, b.\u0275prov = s.Yz7({
                         token: b,
@@ -9268,23 +9273,23 @@
                 return b.replace(/\/index.html$/, "")
             }
 
             function Z(b, P) {
                 P = encodeURIComponent(P);
                 for (const w of b.split(";")) {
                     const U = w.indexOf("="),
-                        [Se, dt] = -1 == U ? [w, ""] : [w.slice(0, U), w.slice(U + 1)];
-                    if (Se.trim() === P) return decodeURIComponent(dt)
+                        [Oe, dt] = -1 == U ? [w, ""] : [w.slice(0, U), w.slice(U + 1)];
+                    if (Oe.trim() === P) return decodeURIComponent(dt)
                 }
                 return null
             }
             let re = (() => {
                 class b {
-                    constructor(w, U, Se, dt) {
-                        this._iterableDiffers = w, this._keyValueDiffers = U, this._ngEl = Se, this._renderer = dt, this._iterableDiffer = null, this._keyValueDiffer = null, this._initialClasses = [], this._rawClass = null
+                    constructor(w, U, Oe, dt) {
+                        this._iterableDiffers = w, this._keyValueDiffers = U, this._ngEl = Oe, this._renderer = dt, this._iterableDiffer = null, this._keyValueDiffer = null, this._initialClasses = [], this._rawClass = null
                     }
                     set klass(w) {
                         this._removeClasses(this._initialClasses), this._initialClasses = "string" == typeof w ? w.split(/\s+/) : [], this._applyClasses(this._initialClasses), this._applyClasses(this._rawClass)
                     }
                     set ngClass(w) {
                         this._removeClasses(this._rawClass), this._applyClasses(this._initialClasses), this._iterableDiffer = null, this._keyValueDiffer = null, this._rawClass = "string" == typeof w ? w.split(/\s+/) : w, this._rawClass && ((0, s.sIi)(this._rawClass) ? this._iterableDiffer = this._iterableDiffers.find(this._rawClass).create() : this._keyValueDiffer = this._keyValueDiffers.find(this._rawClass).create())
                     }
@@ -9311,16 +9316,16 @@
                     _applyClasses(w) {
                         w && (Array.isArray(w) || w instanceof Set ? w.forEach(U => this._toggleClass(U, !0)) : Object.keys(w).forEach(U => this._toggleClass(U, !!w[U])))
                     }
                     _removeClasses(w) {
                         w && (Array.isArray(w) || w instanceof Set ? w.forEach(U => this._toggleClass(U, !1)) : Object.keys(w).forEach(U => this._toggleClass(U, !1)))
                     }
                     _toggleClass(w, U) {
-                        (w = w.trim()) && w.split(/\s+/g).forEach(Se => {
-                            U ? this._renderer.addClass(this._ngEl.nativeElement, Se) : this._renderer.removeClass(this._ngEl.nativeElement, Se)
+                        (w = w.trim()) && w.split(/\s+/g).forEach(Oe => {
+                            U ? this._renderer.addClass(this._ngEl.nativeElement, Oe) : this._renderer.removeClass(this._ngEl.nativeElement, Oe)
                         })
                     }
                 }
                 return b.\u0275fac = function(w) {
                     return new(w || b)(s.Y36(s.ZZ4), s.Y36(s.aQg), s.Y36(s.SBq), s.Y36(s.Qsj))
                 }, b.\u0275dir = s.lG2({
                     type: b,
@@ -9331,16 +9336,16 @@
                         klass: ["class", "klass"],
                         ngClass: "ngClass"
                     },
                     standalone: !0
                 }), b
             })();
             class wt {
-                constructor(P, w, U, Se) {
-                    this.$implicit = P, this.ngForOf = w, this.index = U, this.count = Se
+                constructor(P, w, U, Oe) {
+                    this.$implicit = P, this.ngForOf = w, this.index = U, this.count = Oe
                 }
                 get first() {
                     return 0 === this.index
                 }
                 get last() {
                     return this.index === this.count - 1
                 }
@@ -9349,16 +9354,16 @@
                 }
                 get odd() {
                     return !this.even
                 }
             }
             let Vt = (() => {
                 class b {
-                    constructor(w, U, Se) {
-                        this._viewContainer = w, this._template = U, this._differs = Se, this._ngForOf = null, this._ngForOfDirty = !0, this._differ = null
+                    constructor(w, U, Oe) {
+                        this._viewContainer = w, this._template = U, this._differs = Oe, this._ngForOf = null, this._ngForOfDirty = !0, this._differ = null
                     }
                     set ngForOf(w) {
                         this._ngForOf = w, this._ngForOfDirty = !0
                     }
                     set ngForTrackBy(w) {
                         this._trackByFn = w
                     }
@@ -9377,28 +9382,28 @@
                         if (this._differ) {
                             const w = this._differ.diff(this._ngForOf);
                             w && this._applyChanges(w)
                         }
                     }
                     _applyChanges(w) {
                         const U = this._viewContainer;
-                        w.forEachOperation((Se, dt, Ot) => {
-                            if (null == Se.previousIndex) U.createEmbeddedView(this._template, new wt(Se.item, this._ngForOf, -1, -1), null === Ot ? void 0 : Ot);
+                        w.forEachOperation((Oe, dt, Ot) => {
+                            if (null == Oe.previousIndex) U.createEmbeddedView(this._template, new wt(Oe.item, this._ngForOf, -1, -1), null === Ot ? void 0 : Ot);
                             else if (null == Ot) U.remove(null === dt ? void 0 : dt);
                             else if (null !== dt) {
                                 const Jt = U.get(dt);
-                                U.move(Jt, Ot), nn(Jt, Se)
+                                U.move(Jt, Ot), nn(Jt, Oe)
                             }
                         });
-                        for (let Se = 0, dt = U.length; Se < dt; Se++) {
-                            const Jt = U.get(Se).context;
-                            Jt.index = Se, Jt.count = dt, Jt.ngForOf = this._ngForOf
+                        for (let Oe = 0, dt = U.length; Oe < dt; Oe++) {
+                            const Jt = U.get(Oe).context;
+                            Jt.index = Oe, Jt.count = dt, Jt.ngForOf = this._ngForOf
                         }
-                        w.forEachIdentityChange(Se => {
-                            nn(U.get(Se.currentIndex), Se)
+                        w.forEachIdentityChange(Oe => {
+                            nn(U.get(Oe.currentIndex), Oe)
                         })
                     }
                     static ngTemplateContextGuard(w, U) {
                         return !0
                     }
                 }
                 return b.\u0275fac = function(w) {
@@ -9515,16 +9520,16 @@
                             ngSwitch: "ngSwitch"
                         },
                         standalone: !0
                     }), b
                 })(),
                 cr = (() => {
                     class b {
-                        constructor(w, U, Se) {
-                            this.ngSwitch = Se, Se._addCase(), this._view = new xn(w, U)
+                        constructor(w, U, Oe) {
+                            this.ngSwitch = Oe, Oe._addCase(), this._view = new xn(w, U)
                         }
                         ngDoCheck() {
                             this._view.enforceState(this.ngSwitch._matchCase(this.ngSwitchCase))
                         }
                     }
                     return b.\u0275fac = function(w) {
                         return new(w || b)(s.Y36(s.s_b), s.Y36(s.Rgc), s.Y36(oi, 9))
@@ -9545,19 +9550,19 @@
                             this._viewContainerRef = w, this._viewRef = null, this.ngTemplateOutletContext = null, this.ngTemplateOutlet = null, this.ngTemplateOutletInjector = null
                         }
                         ngOnChanges(w) {
                             if (w.ngTemplateOutlet || w.ngTemplateOutletInjector) {
                                 const U = this._viewContainerRef;
                                 if (this._viewRef && U.remove(U.indexOf(this._viewRef)), this.ngTemplateOutlet) {
                                     const {
-                                        ngTemplateOutlet: Se,
+                                        ngTemplateOutlet: Oe,
                                         ngTemplateOutletContext: dt,
                                         ngTemplateOutletInjector: Ot
                                     } = this;
-                                    this._viewRef = U.createEmbeddedView(Se, dt, Ot ? {
+                                    this._viewRef = U.createEmbeddedView(Oe, dt, Ot ? {
                                         injector: Ot
                                     } : void 0)
                                 } else this._viewRef = null
                             } else this._viewRef && w.ngTemplateOutletContext && this.ngTemplateOutletContext && (this._viewRef.context = this.ngTemplateOutletContext)
                         }
                     }
                     return b.\u0275fac = function(w) {
@@ -9633,22 +9638,22 @@
                 scrollToAnchor(P) {
                     if (!this.supportsScrolling()) return;
                     const w = function xi(b, P) {
                         const w = b.getElementById(P) || b.getElementsByName(P)[0];
                         if (w) return w;
                         if ("function" == typeof b.createTreeWalker && b.body && (b.body.createShadowRoot || b.body.attachShadow)) {
                             const U = b.createTreeWalker(b.body, NodeFilter.SHOW_ELEMENT);
-                            let Se = U.currentNode;
-                            for (; Se;) {
-                                const dt = Se.shadowRoot;
+                            let Oe = U.currentNode;
+                            for (; Oe;) {
+                                const dt = Oe.shadowRoot;
                                 if (dt) {
                                     const Ot = dt.getElementById(P) || dt.querySelector(`[name="${P}"]`);
                                     if (Ot) return Ot
                                 }
-                                Se = U.nextNode()
+                                Oe = U.nextNode()
                             }
                         }
                         return null
                     }(this.document, P);
                     w && (this.scrollToElement(w), w.focus())
                 }
                 setHistoryScrollRestoration(P) {
@@ -9656,17 +9661,17 @@
                         const w = this.window.history;
                         w && w.scrollRestoration && (w.scrollRestoration = P)
                     }
                 }
                 scrollToElement(P) {
                     const w = P.getBoundingClientRect(),
                         U = w.left + this.window.pageXOffset,
-                        Se = w.top + this.window.pageYOffset,
+                        Oe = w.top + this.window.pageYOffset,
                         dt = this.offset();
-                    this.window.scrollTo(U - dt[0], Se - dt[1])
+                    this.window.scrollTo(U - dt[0], Oe - dt[1])
                 }
                 supportScrollRestoration() {
                     try {
                         if (!this.supportsScrolling()) return !1;
                         const P = ur(this.window.history) || ur(Object.getPrototypeOf(this.window.history));
                         return !(!P || !P.writable && !P.set)
                     } catch {
@@ -10435,15 +10440,15 @@
                 F4k: () => Mg,
                 FYo: () => rc,
                 FiY: () => ta,
                 G48: () => MC,
                 Gf: () => D_,
                 GfV: () => oc,
                 GkF: () => Mh,
-                Gpc: () => Oe,
+                Gpc: () => Te,
                 Hsn: () => xg,
                 Ikx: () => kh,
                 JOm: () => Vi,
                 JVY: () => tp,
                 KtG: () => tr,
                 L6k: () => np,
                 LAX: () => ip,
@@ -10584,26 +10589,26 @@
             function Me(e, t) {
                 return null == e || "" === e ? null === t ? "" : t : null == t || "" === t ? e : e + " " + t
             }
             const fe = De({
                 __forward_ref__: De
             });
 
-            function Oe(e) {
-                return e.__forward_ref__ = Oe, e.toString = function() {
+            function Te(e) {
+                return e.__forward_ref__ = Te, e.toString = function() {
                     return be(this())
                 }, e
             }
 
             function ye(e) {
                 return g(e) ? e() : e
             }
 
             function g(e) {
-                return "function" == typeof e && e.hasOwnProperty(fe) && e.__forward_ref__ === Oe
+                return "function" == typeof e && e.hasOwnProperty(fe) && e.__forward_ref__ === Te
             }
             class pe extends Error {
                 constructor(t, n) {
                     super(function Ge(e, t) {
                         return `NG0${Math.abs(e)}${t?": "+t.trim():""}`
                     }(t, n)), this.code = t
                 }
@@ -10752,15 +10757,15 @@
                         l = e.dependencies,
                         d = e.features;
                     return o.inputs = mt(e.inputs, i), o.outputs = mt(e.outputs), d && d.forEach(y => y(o)), o.directiveDefs = l ? () => ("function" == typeof l ? l() : l).map(tt).filter(pt) : null, o.pipeDefs = l ? () => ("function" == typeof l ? l() : l).map(xt).filter(pt) : null, o
                 })
             }
 
             function tt(e) {
-                return Te(e) || nt(e)
+                return Se(e) || nt(e)
             }
 
             function pt(e) {
                 return null !== e
             }
 
             function jt(e) {
@@ -10795,28 +10800,28 @@
                     factory: null,
                     pure: !1 !== e.pure,
                     standalone: !0 === e.standalone,
                     onDestroy: e.type.prototype.ngOnDestroy || null
                 }
             }
 
-            function Te(e) {
+            function Se(e) {
                 return e[Fn] || null
             }
 
             function nt(e) {
                 return e[Mn] || null
             }
 
             function xt(e) {
                 return e[St] || null
             }
 
             function kn(e) {
-                const t = Te(e) || nt(e) || xt(e);
+                const t = Se(e) || nt(e) || xt(e);
                 return null !== t && t.standalone
             }
 
             function In(e, t) {
                 const n = e[ke] || null;
                 if (!n && !0 === t) throw new Error(`Type ${be(e)} does not have '\u0275mod' property.`);
                 return n
@@ -11194,15 +11199,15 @@
                             d = n[++i];
                         dt(l) ? e.setProperty(t, l, d) : e.setAttribute(t, l, d), i++
                     }
                 }
                 return i
             }
 
-            function Se(e) {
+            function Oe(e) {
                 return 3 === e || 4 === e || 6 === e
             }
 
             function dt(e) {
                 return 64 === e.charCodeAt(0)
             }
 
@@ -11513,15 +11518,15 @@
                     if ("style" === t) return e.styles;
                     const n = e.attrs;
                     if (n) {
                         const i = n.length;
                         let o = 0;
                         for (; o < i;) {
                             const l = n[o];
-                            if (Se(l)) break;
+                            if (Oe(l)) break;
                             if (0 === l) o += 2;
                             else if ("number" == typeof l)
                                 for (o++; o < i && "string" == typeof n[o];) o++;
                             else {
                                 if (l === t) return n[o + 1];
                                 o += 2
                             }
@@ -12290,15 +12295,15 @@
                 }
             }
 
             function on(e, t, n, i) {
                 if (!(e = ye(e))) return !1;
                 let o = null,
                     l = ot(e);
-                const d = !l && Te(e);
+                const d = !l && Se(e);
                 if (l || d) {
                     if (d && !d.standalone) return !1;
                     o = e
                 } else {
                     const E = e.ngModule;
                     if (l = ot(E), !l) return !1;
                     o = E
@@ -12665,15 +12670,15 @@
             }
 
             function jv(e, t, n) {
                 let i = 4;
                 const o = e.attrs || [],
                     l = function $v(e) {
                         for (let t = 0; t < e.length; t++)
-                            if (Se(e[t])) return t;
+                            if (Oe(e[t])) return t;
                         return e.length
                     }(o);
                 let d = !1;
                 for (let y = 0; y < t.length; y++) {
                     const E = t[y];
                     if ("number" != typeof E) {
                         if (!d)
@@ -13561,15 +13566,15 @@
                 }
             }
             class _h extends gs {
                 constructor(t) {
                     super(), this.ngModule = t
                 }
                 resolveComponentFactory(t) {
-                    const n = Te(t);
+                    const n = Se(t);
                     return new cc(n, this.ngModule)
                 }
             }
 
             function dg(e) {
                 const t = [];
                 for (let n in e) e.hasOwnProperty(n) && t.push({
@@ -15380,15 +15385,15 @@
                         }(t);
                         let y;
                         if (d) y = n;
                         else {
                             const le = n || {};
                             y = le.index, i = le.injector, o = le.projectableNodes, l = le.environmentInjector || le.ngModuleRef
                         }
-                        const E = d ? t : new cc(Te(t)),
+                        const E = d ? t : new cc(Se(t)),
                             k = i || this.parentInjector;
                         if (!l && null == E.ngModule) {
                             const je = (d ? k : this.parentInjector).get(Ti, null);
                             je && (l = je)
                         }
                         const Y = E.create(k, o, void 0, l);
                         return this.insert(Y.hostView, y), Y
@@ -15821,15 +15826,15 @@
                     }
                     compileModuleAsync(n) {
                         return Promise.resolve(this.compileModuleSync(n))
                     }
                     compileModuleAndAllComponentsSync(n) {
                         const i = this.compileModuleSync(n),
                             l = Gs(In(n).declarations).reduce((d, y) => {
-                                const E = Te(y);
+                                const E = Se(y);
                                 return E && d.push(new cc(E)), d
                             }, []);
                         return new sC(i, l)
                     }
                     compileModuleAndAllComponentsAsync(n) {
                         return Promise.resolve(this.compileModuleAndAllComponentsSync(n))
                     }
@@ -16790,15 +16795,15 @@
             })();
 
             function GC(e) {
                 return "boolean" == typeof e ? e : null != e && "false" !== e
             }
 
             function $C(e, t) {
-                const n = Te(e),
+                const n = Se(e),
                     i = t.elementInjector || pi();
                 return new cc(n).create(i, t.projectableNodes, t.hostElement, t.environmentInjector)
             }
         },
         4006: (Ht, $e, v) => {
             v.d($e, {
                 EJ: () => Tr,
@@ -16855,15 +16860,15 @@
                         }
                     }(), x.\u0275dir = s.lG2({
                         type: x,
                         features: [s.qOj]
                     }), x
                 })();
             const be = new s.OlP("NgValueAccessor"),
-                Oe = {
+                Te = {
                     provide: be,
                     useExisting: (0, s.Gpc)(() => xe),
                     multi: !0
                 },
                 g = new s.OlP("CompositionEventMode");
             let xe = (() => {
                 class x extends De {
@@ -16906,15 +16911,15 @@
                             return K.onTouched()
                         })("compositionstart", function() {
                             return K._compositionStart()
                         })("compositionend", function(ln) {
                             return K._compositionEnd(ln.target.value)
                         })
                     },
-                    features: [s._Bn([Oe]), s.qOj]
+                    features: [s._Bn([Te]), s.qOj]
                 }), x
             })();
 
             function Ge(x) {
                 return null == x || ("string" == typeof x || Array.isArray(x)) && 0 === x.length
             }
 
@@ -17530,15 +17535,15 @@
                 _parentMarkedDirty(R) {
                     return !R && !(!this._parent || !this._parent.dirty) && !this._parent._anyControlsDirty()
                 }
                 _find(R) {
                     return null
                 }
             }
-            class Te extends ie {
+            class Se extends ie {
                 constructor(R, T, K) {
                     super(ge(T), pt(K, T)), this.controls = R, this._initObservables(), this._setUpdateStrategy(T), this._setUpControls(), this.updateValueAndValidity({
                         onlySelf: !0,
                         emitEvent: !!this.asyncValidator
                     })
                 }
                 registerControl(R, T) {
@@ -17629,15 +17634,15 @@
                         if (this.controls[R].enabled) return !1;
                     return Object.keys(this.controls).length > 0 || this.disabled
                 }
                 _find(R) {
                     return this.controls.hasOwnProperty(R) ? this.controls[R] : null
                 }
             }
-            class kn extends Te {}
+            class kn extends Se {}
 
             function Tn(x, R) {
                 return [...R.path, x]
             }
 
             function Ce(x, R) {
                 Ct(x, R), R.valueAccessor.writeValue(x.value), x.disabled && R.valueAccessor.setDisabledState?.(!0),
@@ -17749,15 +17754,15 @@
                     provide: ot,
                     useExisting: (0, s.Gpc)(() => Xe)
                 },
                 he = (() => Promise.resolve())();
             let Xe = (() => {
                 class x extends ot {
                     constructor(T, K) {
-                        super(), this.submitted = !1, this._directives = new Set, this.ngSubmit = new s.vpe, this.form = new Te({}, it(T), et(K))
+                        super(), this.submitted = !1, this._directives = new Set, this.ngSubmit = new s.vpe, this.form = new Se({}, it(T), et(K))
                     }
                     ngAfterViewInit() {
                         this._setUpdateStrategy()
                     }
                     get formDirective() {
                         return this
                     }
@@ -17786,15 +17791,15 @@
                             const K = this._findContainer(T.path);
                             K && K.removeControl(T.name), this._directives.delete(T)
                         })
                     }
                     addFormGroup(T) {
                         he.then(() => {
                             const K = this._findContainer(T.path),
-                                yt = new Te({});
+                                yt = new Se({});
                             gn(yt, T), K.registerControl(T.name, yt), yt.updateValueAndValidity({
                                 emitEvent: !1
                             })
                         })
                     }
                     removeFormGroup(T) {
                         he.then(() => {
@@ -18573,15 +18578,15 @@
                     get nonNullable() {
                         const T = new x;
                         return T.useNonNullable = !0, T
                     }
                     group(T, K = null) {
                         const yt = this._reduceControls(T);
                         let ln = {};
-                        return Nt(K) ? ln = K : null !== K && (ln.validators = K.validator, ln.asyncValidators = K.asyncValidator), new Te(yt, ln)
+                        return Nt(K) ? ln = K : null !== K && (ln.validators = K.validator, ln.asyncValidators = K.asyncValidator), new Se(yt, ln)
                     }
                     record(T, K = null) {
                         const yt = this._reduceControls(T);
                         return new kn(yt, K)
                     }
                     control(T, K, yt) {
                         let ln = {};
@@ -18613,15 +18618,15 @@
                 }), x
             })()
         },
         4859: (Ht, $e, v) => {
             v.d($e, {
                 lW: () => fe,
                 ot: () => ye,
-                zs: () => Oe
+                zs: () => Te
             });
             var s = v(4650),
                 S = v(3238),
                 C = v(2687);
             const F = ["mat-button", ""],
                 O = ["*"],
                 be = ["mat-button", "mat-flat-button", "mat-icon-button", "mat-raised-button", "mat-stroked-button", "mat-mini-fab", "mat-fab"],
@@ -18701,15 +18706,15 @@
                         },
                         dependencies: [S.wG],
                         styles: [".mat-button .mat-button-focus-overlay,.mat-icon-button .mat-button-focus-overlay{opacity:0}.mat-button:hover:not(.mat-button-disabled) .mat-button-focus-overlay,.mat-stroked-button:hover:not(.mat-button-disabled) .mat-button-focus-overlay{opacity:.04}@media(hover: none){.mat-button:hover:not(.mat-button-disabled) .mat-button-focus-overlay,.mat-stroked-button:hover:not(.mat-button-disabled) .mat-button-focus-overlay{opacity:0}}.mat-button,.mat-icon-button,.mat-stroked-button,.mat-flat-button{box-sizing:border-box;position:relative;-webkit-user-select:none;user-select:none;cursor:pointer;outline:none;border:none;-webkit-tap-highlight-color:transparent;display:inline-block;white-space:nowrap;text-decoration:none;vertical-align:baseline;text-align:center;margin:0;min-width:64px;line-height:36px;padding:0 16px;border-radius:4px;overflow:visible}.mat-button::-moz-focus-inner,.mat-icon-button::-moz-focus-inner,.mat-stroked-button::-moz-focus-inner,.mat-flat-button::-moz-focus-inner{border:0}.mat-button.mat-button-disabled,.mat-icon-button.mat-button-disabled,.mat-stroked-button.mat-button-disabled,.mat-flat-button.mat-button-disabled{cursor:default}.mat-button.cdk-keyboard-focused .mat-button-focus-overlay,.mat-button.cdk-program-focused .mat-button-focus-overlay,.mat-icon-button.cdk-keyboard-focused .mat-button-focus-overlay,.mat-icon-button.cdk-program-focused .mat-button-focus-overlay,.mat-stroked-button.cdk-keyboard-focused .mat-button-focus-overlay,.mat-stroked-button.cdk-program-focused .mat-button-focus-overlay,.mat-flat-button.cdk-keyboard-focused .mat-button-focus-overlay,.mat-flat-button.cdk-program-focused .mat-button-focus-overlay{opacity:.12}.mat-button::-moz-focus-inner,.mat-icon-button::-moz-focus-inner,.mat-stroked-button::-moz-focus-inner,.mat-flat-button::-moz-focus-inner{border:0}.mat-raised-button{box-sizing:border-box;position:relative;-webkit-user-select:none;user-select:none;cursor:pointer;outline:none;border:none;-webkit-tap-highlight-color:transparent;display:inline-block;white-space:nowrap;text-decoration:none;vertical-align:baseline;text-align:center;margin:0;min-width:64px;line-height:36px;padding:0 16px;border-radius:4px;overflow:visible;transform:translate3d(0, 0, 0);transition:background 400ms cubic-bezier(0.25, 0.8, 0.25, 1),box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1)}.mat-raised-button::-moz-focus-inner{border:0}.mat-raised-button.mat-button-disabled{cursor:default}.mat-raised-button.cdk-keyboard-focused .mat-button-focus-overlay,.mat-raised-button.cdk-program-focused .mat-button-focus-overlay{opacity:.12}.mat-raised-button::-moz-focus-inner{border:0}._mat-animation-noopable.mat-raised-button{transition:none;animation:none}.mat-stroked-button{border:1px solid currentColor;padding:0 15px;line-height:34px}.mat-stroked-button .mat-button-ripple.mat-ripple,.mat-stroked-button .mat-button-focus-overlay{top:-1px;left:-1px;right:-1px;bottom:-1px}.mat-fab{box-sizing:border-box;position:relative;-webkit-user-select:none;user-select:none;cursor:pointer;outline:none;border:none;-webkit-tap-highlight-color:transparent;display:inline-block;white-space:nowrap;text-decoration:none;vertical-align:baseline;text-align:center;margin:0;min-width:64px;line-height:36px;padding:0 16px;border-radius:4px;overflow:visible;transform:translate3d(0, 0, 0);transition:background 400ms cubic-bezier(0.25, 0.8, 0.25, 1),box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1);min-width:0;border-radius:50%;width:56px;height:56px;padding:0;flex-shrink:0}.mat-fab::-moz-focus-inner{border:0}.mat-fab.mat-button-disabled{cursor:default}.mat-fab.cdk-keyboard-focused .mat-button-focus-overlay,.mat-fab.cdk-program-focused .mat-button-focus-overlay{opacity:.12}.mat-fab::-moz-focus-inner{border:0}._mat-animation-noopable.mat-fab{transition:none;animation:none}.mat-fab .mat-button-wrapper{padding:16px 0;display:inline-block;line-height:24px}.mat-mini-fab{box-sizing:border-box;position:relative;-webkit-user-select:none;user-select:none;cursor:pointer;outline:none;border:none;-webkit-tap-highlight-color:transparent;display:inline-block;white-space:nowrap;text-decoration:none;vertical-align:baseline;text-align:center;margin:0;min-width:64px;line-height:36px;padding:0 16px;border-radius:4px;overflow:visible;transform:translate3d(0, 0, 0);transition:background 400ms cubic-bezier(0.25, 0.8, 0.25, 1),box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1);min-width:0;border-radius:50%;width:40px;height:40px;padding:0;flex-shrink:0}.mat-mini-fab::-moz-focus-inner{border:0}.mat-mini-fab.mat-button-disabled{cursor:default}.mat-mini-fab.cdk-keyboard-focused .mat-button-focus-overlay,.mat-mini-fab.cdk-program-focused .mat-button-focus-overlay{opacity:.12}.mat-mini-fab::-moz-focus-inner{border:0}._mat-animation-noopable.mat-mini-fab{transition:none;animation:none}.mat-mini-fab .mat-button-wrapper{padding:8px 0;display:inline-block;line-height:24px}.mat-icon-button{padding:0;min-width:0;width:40px;height:40px;flex-shrink:0;line-height:40px;border-radius:50%}.mat-icon-button i,.mat-icon-button .mat-icon{line-height:24px}.mat-button-ripple.mat-ripple,.mat-button-focus-overlay{top:0;left:0;right:0;bottom:0;position:absolute;pointer-events:none;border-radius:inherit}.mat-button-ripple.mat-ripple:not(:empty){transform:translateZ(0)}.mat-button-focus-overlay{opacity:0;transition:opacity 200ms cubic-bezier(0.35, 0, 0.25, 1),background-color 200ms cubic-bezier(0.35, 0, 0.25, 1)}._mat-animation-noopable .mat-button-focus-overlay{transition:none}.mat-button-ripple-round{border-radius:50%;z-index:1}.mat-button .mat-button-wrapper>*,.mat-flat-button .mat-button-wrapper>*,.mat-stroked-button .mat-button-wrapper>*,.mat-raised-button .mat-button-wrapper>*,.mat-icon-button .mat-button-wrapper>*,.mat-fab .mat-button-wrapper>*,.mat-mini-fab .mat-button-wrapper>*{vertical-align:middle}.mat-form-field:not(.mat-form-field-appearance-legacy) .mat-form-field-prefix .mat-icon-button,.mat-form-field:not(.mat-form-field-appearance-legacy) .mat-form-field-suffix .mat-icon-button{display:inline-flex;justify-content:center;align-items:center;font-size:inherit;width:2.5em;height:2.5em}.cdk-high-contrast-active .mat-button,.cdk-high-contrast-active .mat-flat-button,.cdk-high-contrast-active .mat-raised-button,.cdk-high-contrast-active .mat-icon-button,.cdk-high-contrast-active .mat-fab,.cdk-high-contrast-active .mat-mini-fab{outline:solid 1px}.cdk-high-contrast-active .mat-button-base.cdk-keyboard-focused,.cdk-high-contrast-active .mat-button-base.cdk-program-focused{outline:solid 3px}\n"],
                         encapsulation: 2,
                         changeDetection: 0
                     }), g
                 })(),
-                Oe = (() => {
+                Te = (() => {
                     class g extends fe {
                         constructor(pe, Ge, Ve, We) {
                             super(Ge, pe, Ve), this._ngZone = We, this._haltDisabledEvents = ht => {
                                 this.disabled && (ht.preventDefault(), ht.stopImmediatePropagation())
                             }
                         }
                         ngAfterViewInit() {
@@ -19117,15 +19122,15 @@
                 F = v(3238),
                 O = v(445),
                 De = v(6895),
                 L = v(7579),
                 be = v(9770),
                 Me = v(9646),
                 fe = v(9300),
-                Oe = v(5698),
+                Te = v(5698),
                 ye = v(8675),
                 g = v(2687),
                 xe = v(3353),
                 pe = v(7340),
                 Ge = v(9521);
 
             function Ve(se, ve) {}
@@ -19302,28 +19307,28 @@
                             animation: [ht.dialogContainer]
                         }
                     }), se
                 })(),
                 J = 0;
             class Ee {
                 constructor(ve, z, ee = "mat-dialog-" + J++) {
-                    this._overlayRef = ve, this._containerInstance = z, this.id = ee, this.disableClose = this._containerInstance._config.disableClose, this._afterOpened = new L.x, this._afterClosed = new L.x, this._beforeClosed = new L.x, this._state = 0, z._id = ee, z._animationStateChanged.pipe((0, fe.h)(Q => "opened" === Q.state), (0, Oe.q)(1)).subscribe(() => {
+                    this._overlayRef = ve, this._containerInstance = z, this.id = ee, this.disableClose = this._containerInstance._config.disableClose, this._afterOpened = new L.x, this._afterClosed = new L.x, this._beforeClosed = new L.x, this._state = 0, z._id = ee, z._animationStateChanged.pipe((0, fe.h)(Q => "opened" === Q.state), (0, Te.q)(1)).subscribe(() => {
                         this._afterOpened.next(), this._afterOpened.complete()
-                    }), z._animationStateChanged.pipe((0, fe.h)(Q => "closed" === Q.state), (0, Oe.q)(1)).subscribe(() => {
+                    }), z._animationStateChanged.pipe((0, fe.h)(Q => "closed" === Q.state), (0, Te.q)(1)).subscribe(() => {
                         clearTimeout(this._closeFallbackTimeout), this._finishDialogClose()
                     }), ve.detachments().subscribe(() => {
                         this._beforeClosed.next(this._result), this._beforeClosed.complete(), this._afterClosed.next(this._result), this._afterClosed.complete(), this.componentInstance = null, this._overlayRef.dispose()
                     }), ve.keydownEvents().pipe((0, fe.h)(Q => Q.keyCode === Ge.hY && !this.disableClose && !(0, Ge.Vb)(Q))).subscribe(Q => {
                         Q.preventDefault(), Ie(this, "keyboard")
                     }), ve.backdropClick().subscribe(() => {
                         this.disableClose ? this._containerInstance._recaptureFocus() : Ie(this, "mouse")
                     })
                 }
                 close(ve) {
-                    this._result = ve, this._containerInstance._animationStateChanged.pipe((0, fe.h)(z => "closing" === z.state), (0, Oe.q)(1)).subscribe(z => {
+                    this._result = ve, this._containerInstance._animationStateChanged.pipe((0, fe.h)(z => "closing" === z.state), (0, Te.q)(1)).subscribe(z => {
                         this._beforeClosed.next(ve), this._beforeClosed.complete(), this._overlayRef.detachBackdrop(), this._closeFallbackTimeout = setTimeout(() => this._finishDialogClose(), z.totalTime + 100)
                     }), this._state = 1, this._containerInstance._startExitAnimation()
                 }
                 afterOpened() {
                     return this._afterOpened
                 }
                 afterClosed() {
@@ -19655,15 +19660,15 @@
                 F = v(3238),
                 O = v(445),
                 De = v(1281),
                 L = v(7579),
                 be = v(6451),
                 Me = v(4968),
                 fe = v(8675),
-                Oe = v(2722),
+                Te = v(2722),
                 ye = v(5698),
                 g = v(7340),
                 xe = v(3353);
             const pe = ["connectionContainer"],
                 Ge = ["inputContainer"],
                 Ve = ["label"];
 
@@ -19885,25 +19890,25 @@
                             return this._connectionContainerRef || this._elementRef
                         }
                         ngAfterContentInit() {
                             this._validateControlChild();
                             const ue = this._control;
                             ue.controlType && this._elementRef.nativeElement.classList.add(`mat-form-field-type-${ue.controlType}`), ue.stateChanges.pipe((0, fe.O)(null)).subscribe(() => {
                                 this._validatePlaceholders(), this._syncDescribedByIds(), this._changeDetectorRef.markForCheck()
-                            }), ue.ngControl && ue.ngControl.valueChanges && ue.ngControl.valueChanges.pipe((0, Oe.R)(this._destroyed)).subscribe(() => this._changeDetectorRef.markForCheck()), this._ngZone.runOutsideAngular(() => {
-                                this._ngZone.onStable.pipe((0, Oe.R)(this._destroyed)).subscribe(() => {
+                            }), ue.ngControl && ue.ngControl.valueChanges && ue.ngControl.valueChanges.pipe((0, Te.R)(this._destroyed)).subscribe(() => this._changeDetectorRef.markForCheck()), this._ngZone.runOutsideAngular(() => {
+                                this._ngZone.onStable.pipe((0, Te.R)(this._destroyed)).subscribe(() => {
                                     this._outlineGapCalculationNeededOnStable && this.updateOutlineGap()
                                 })
                             }), (0, be.T)(this._prefixChildren.changes, this._suffixChildren.changes).subscribe(() => {
                                 this._outlineGapCalculationNeededOnStable = !0, this._changeDetectorRef.markForCheck()
                             }), this._hintChildren.changes.pipe((0, fe.O)(null)).subscribe(() => {
                                 this._processHints(), this._changeDetectorRef.markForCheck()
                             }), this._errorChildren.changes.pipe((0, fe.O)(null)).subscribe(() => {
                                 this._syncDescribedByIds(), this._changeDetectorRef.markForCheck()
-                            }), this._dir && this._dir.change.pipe((0, Oe.R)(this._destroyed)).subscribe(() => {
+                            }), this._dir && this._dir.change.pipe((0, Te.R)(this._destroyed)).subscribe(() => {
                                 "function" == typeof requestAnimationFrame ? this._ngZone.runOutsideAngular(() => {
                                     requestAnimationFrame(() => this.updateOutlineGap())
                                 }) : this.updateOutlineGap()
                             })
                         }
                         ngAfterContentChecked() {
                             this._validateControlChild(), this._outlineGapCalculationNeededImmediately && this.updateOutlineGap()
@@ -20113,15 +20118,15 @@
                 F = v(6895),
                 O = v(9646),
                 De = v(2843),
                 L = v(4128),
                 be = v(727),
                 Me = v(8505),
                 fe = v(4004),
-                Oe = v(262),
+                Te = v(262),
                 ye = v(8746),
                 g = v(3099),
                 xe = v(5698),
                 pe = v(529),
                 Ge = v(1481);
             const Ve = ["*"];
             let We;
@@ -20223,15 +20228,15 @@
                     }
                     _getSvgFromConfig(se) {
                         return se.svgText ? (0, O.of)(kt(this._svgElementFromConfig(se))) : this._loadSvgIconFromConfig(se).pipe((0, fe.U)(ve => kt(ve)))
                     }
                     _getSvgFromIconSetConfigs(se, ve) {
                         const z = this._extractIconWithNameFromAnySet(se, ve);
                         if (z) return (0, O.of)(z);
-                        const ee = ve.filter(Q => !Q.svgText).map(Q => this._loadSvgIconSetFromConfig(Q).pipe((0, Oe.K)(X => {
+                        const ee = ve.filter(Q => !Q.svgText).map(Q => this._loadSvgIconSetFromConfig(Q).pipe((0, Te.K)(X => {
                             const ot = `Loading icon set URL: ${this._sanitizer.sanitize(s.q3G.RESOURCE_URL,Q.url)} failed: ${X.message}`;
                             return this._errorHandler.handleError(new Error(ot)), (0, O.of)(null)
                         })));
                         return (0, L.D)(ee).pipe((0, fe.U)(() => {
                             const Q = this._extractIconWithNameFromAnySet(se, ve);
                             if (!Q) throw ae(se);
                             return Q
@@ -20587,15 +20592,15 @@
                     class ae {}
                     return ae.\u0275fac = function(J) {
                         return new(J || ae)
                     }, ae.\u0275mod = C.oAB({
                         type: ae
                     }), ae.\u0275inj = C.cJS({}), ae
                 })();
-            var Oe = v(4006),
+            var Te = v(4006),
                 ye = v(3238),
                 g = v(9549);
             const pe = new C.OlP("MAT_INPUT_VALUE_ACCESSOR"),
                 Ge = ["button", "checkbox", "file", "hidden", "image", "radio", "range", "reset", "submit"];
             let Ve = 0;
             const We = (0, ye.FD)(class {
                 constructor(ae, te, J, Ee) {
@@ -20624,15 +20629,15 @@
                         get id() {
                             return this._id
                         }
                         set id(J) {
                             this._id = J || this._uid
                         }
                         get required() {
-                            return this._required ?? this.ngControl?.control?.hasValidator(Oe.kI.required) ?? !1
+                            return this._required ?? this.ngControl?.control?.hasValidator(Te.kI.required) ?? !1
                         }
                         set required(J) {
                             this._required = (0, s.Ig)(J)
                         }
                         get type() {
                             return this._type
                         }
@@ -20712,15 +20717,15 @@
                         }
                         _isInlineSelect() {
                             const J = this._elementRef.nativeElement;
                             return this._isNativeSelect && (J.multiple || J.size > 1)
                         }
                     }
                     return ae.\u0275fac = function(J) {
-                        return new(J || ae)(C.Y36(C.SBq), C.Y36(S.t4), C.Y36(Oe.a5, 10), C.Y36(Oe.F, 8), C.Y36(Oe.sg, 8), C.Y36(ye.rD), C.Y36(pe, 10), C.Y36(L), C.Y36(C.R0b), C.Y36(g.G_, 8))
+                        return new(J || ae)(C.Y36(C.SBq), C.Y36(S.t4), C.Y36(Te.a5, 10), C.Y36(Te.F, 8), C.Y36(Te.sg, 8), C.Y36(ye.rD), C.Y36(pe, 10), C.Y36(L), C.Y36(C.R0b), C.Y36(g.G_, 8))
                     }, ae.\u0275dir = C.lG2({
                         type: ae,
                         selectors: [
                             ["input", "matInput", ""],
                             ["textarea", "matInput", ""],
                             ["select", "matNativeControl", ""],
                             ["input", "matNativeControl", ""],
@@ -20783,15 +20788,15 @@
                 F = v(4650),
                 O = v(7579),
                 De = v(727),
                 L = v(6451),
                 be = v(9646),
                 Me = v(3101),
                 fe = v(8675),
-                Oe = v(3900),
+                Te = v(3900),
                 ye = v(5698),
                 g = v(2722),
                 xe = v(9300),
                 pe = v(1005),
                 Ge = v(7340),
                 Ve = v(4080),
                 We = v(6895),
@@ -20987,28 +20992,28 @@
                         set classList(j) {
                             this.panelClass = j
                         }
                         ngOnInit() {
                             this.setPositionClasses()
                         }
                         ngAfterContentInit() {
-                            this._updateDirectDescendants(), this._keyManager = new s.Em(this._directDescendantItems).withWrap().withTypeAhead().withHomeAndEnd(), this._tabSubscription = this._keyManager.tabOut.subscribe(() => this.closed.emit("tab")), this._directDescendantItems.changes.pipe((0, fe.O)(this._directDescendantItems), (0, Oe.w)(j => (0, L.T)(...j.map(ne => ne._focused)))).subscribe(j => this._keyManager.updateActiveItem(j)), this._directDescendantItems.changes.subscribe(j => {
+                            this._updateDirectDescendants(), this._keyManager = new s.Em(this._directDescendantItems).withWrap().withTypeAhead().withHomeAndEnd(), this._tabSubscription = this._keyManager.tabOut.subscribe(() => this.closed.emit("tab")), this._directDescendantItems.changes.pipe((0, fe.O)(this._directDescendantItems), (0, Te.w)(j => (0, L.T)(...j.map(ne => ne._focused)))).subscribe(j => this._keyManager.updateActiveItem(j)), this._directDescendantItems.changes.subscribe(j => {
                                 const ne = this._keyManager;
                                 if ("enter" === this._panelAnimationState && ne.activeItem?._hasFocus()) {
                                     const ue = j.toArray(),
                                         Ze = Math.max(0, Math.min(ue.length - 1, ne.activeItemIndex || 0));
                                     ue[Ze] && !ue[Ze].disabled ? ne.setActiveItem(Ze) : ne.setNextItemActive()
                                 }
                             })
                         }
                         ngOnDestroy() {
                             this._directDescendantItems.destroy(), this._tabSubscription.unsubscribe(), this.closed.complete()
                         }
                         _hovered() {
-                            return this._directDescendantItems.changes.pipe((0, fe.O)(this._directDescendantItems), (0, Oe.w)(ne => (0, L.T)(...ne.map(ue => ue._hovered))))
+                            return this._directDescendantItems.changes.pipe((0, fe.O)(this._directDescendantItems), (0, Te.w)(ne => (0, L.T)(...ne.map(ue => ue._hovered))))
                         }
                         addItem(j) {}
                         removeItem(j) {}
                         _handleKeydown(j) {
                             const ne = j.keyCode,
                                 ue = this._keyManager;
                             switch (ne) {
@@ -21546,15 +21551,15 @@
                 F = v(4650),
                 O = v(3238),
                 De = v(4859),
                 L = v(7579),
                 be = v(3353),
                 Me = v(5698),
                 fe = v(2722),
-                Oe = v(7340),
+                Te = v(7340),
                 ye = v(2687),
                 g = v(1281),
                 xe = v(9841),
                 pe = v(7272),
                 Ge = v(9751),
                 Ve = v(5684),
                 We = v(8372),
@@ -21744,21 +21749,21 @@
                     dependencies: [De.lW, C.O5],
                     styles: [".mat-simple-snackbar{display:flex;justify-content:space-between;align-items:center;line-height:20px;opacity:1}.mat-simple-snackbar-action{flex-shrink:0;margin:-8px -8px -8px 8px}.mat-simple-snackbar-action button{max-height:36px;min-width:0}[dir=rtl] .mat-simple-snackbar-action{margin-left:-8px;margin-right:8px}.mat-simple-snack-bar-content{overflow:hidden;text-overflow:ellipsis}\n"],
                     encapsulation: 2,
                     changeDetection: 0
                 }), z
             })();
             const Ke = {
-                snackBarState: (0, Oe.X$)("state", [(0, Oe.SB)("void, hidden", (0, Oe.oB)({
+                snackBarState: (0, Te.X$)("state", [(0, Te.SB)("void, hidden", (0, Te.oB)({
                     transform: "scale(0.8)",
                     opacity: 0
-                })), (0, Oe.SB)("visible", (0, Oe.oB)({
+                })), (0, Te.SB)("visible", (0, Te.oB)({
                     transform: "scale(1)",
                     opacity: 1
-                })), (0, Oe.eR)("* => visible", (0, Oe.jt)("150ms cubic-bezier(0, 0, 0.2, 1)")), (0, Oe.eR)("* => void, * => hidden", (0, Oe.jt)("75ms cubic-bezier(0.4, 0.0, 1, 1)", (0, Oe.oB)({
+                })), (0, Te.eR)("* => visible", (0, Te.jt)("150ms cubic-bezier(0, 0, 0.2, 1)")), (0, Te.eR)("* => void, * => hidden", (0, Te.jt)("75ms cubic-bezier(0.4, 0.0, 1, 1)", (0, Te.oB)({
                     opacity: 0
                 })))])
             };
             let it = (() => {
                     class z extends S.en {
                         constructor(Q, X, He, ot, bt) {
                             super(), this._ngZone = Q, this._elementRef = X, this._changeDetectorRef = He, this._platform = ot, this.snackBarConfig = bt, this._announceDelay = 150, this._destroyed = !1, this._onAnnounce = new L.x, this._onExit = new L.x, this._onEnter = new L.x, this._animationState = "void", this.attachDomPortal = Ut => (this._assertNotAttached(), this._applySnackBarClasses(), this._portalOutlet.attachDomPortal(Ut)), this._live = "assertive" !== bt.politeness || bt.announcementMessage ? "off" === bt.politeness ? "off" : "polite" : "assertive", this._platform.FIREFOX && ("polite" === this._live && (this._role = "status"), "assertive" === this._live && (this._role = "alert"))
@@ -22995,15 +23000,15 @@
                     ]
                 }), Z
             })();
             var Zt = v(3238),
                 mt = v(6451),
                 Pt = v(9841),
                 ie = v(4004);
-            const Te = [
+            const Se = [
                     [
                         ["caption"]
                     ],
                     [
                         ["colgroup"],
                         ["col"]
                     ]
@@ -23054,15 +23059,15 @@
                         consts: [
                             ["headerRowOutlet", ""],
                             ["rowOutlet", ""],
                             ["noDataRowOutlet", ""],
                             ["footerRowOutlet", ""]
                         ],
                         template: function(H, he) {
-                            1 & H && (s.F$t(Te), s.Hsn(0), s.Hsn(1, 1), s.GkF(2, 0)(3, 1)(4, 2)(5, 3))
+                            1 & H && (s.F$t(Se), s.Hsn(0), s.Hsn(1, 1), s.GkF(2, 0)(3, 1)(4, 2)(5, 3))
                         },
                         dependencies: [St, Mn, Pe, ke],
                         styles: ["mat-table{display:block}mat-header-row{min-height:56px}mat-row,mat-footer-row{min-height:48px}mat-row,mat-header-row,mat-footer-row{display:flex;border-width:0;border-bottom-width:1px;border-style:solid;align-items:center;box-sizing:border-box}mat-cell:first-of-type,mat-header-cell:first-of-type,mat-footer-cell:first-of-type{padding-left:24px}[dir=rtl] mat-cell:first-of-type:not(:only-of-type),[dir=rtl] mat-header-cell:first-of-type:not(:only-of-type),[dir=rtl] mat-footer-cell:first-of-type:not(:only-of-type){padding-left:0;padding-right:24px}mat-cell:last-of-type,mat-header-cell:last-of-type,mat-footer-cell:last-of-type{padding-right:24px}[dir=rtl] mat-cell:last-of-type:not(:only-of-type),[dir=rtl] mat-header-cell:last-of-type:not(:only-of-type),[dir=rtl] mat-footer-cell:last-of-type:not(:only-of-type){padding-right:0;padding-left:24px}mat-cell,mat-header-cell,mat-footer-cell{flex:1;display:flex;align-items:center;overflow:hidden;word-wrap:break-word;min-height:inherit}table.mat-table{border-spacing:0}tr.mat-header-row{height:56px}tr.mat-row,tr.mat-footer-row{height:48px}th.mat-header-cell{text-align:left}[dir=rtl] th.mat-header-cell{text-align:right}th.mat-header-cell,td.mat-cell,td.mat-footer-cell{padding:0;border-bottom-width:1px;border-bottom-style:solid}th.mat-header-cell:first-of-type,td.mat-cell:first-of-type,td.mat-footer-cell:first-of-type{padding-left:24px}[dir=rtl] th.mat-header-cell:first-of-type:not(:only-of-type),[dir=rtl] td.mat-cell:first-of-type:not(:only-of-type),[dir=rtl] td.mat-footer-cell:first-of-type:not(:only-of-type){padding-left:0;padding-right:24px}th.mat-header-cell:last-of-type,td.mat-cell:last-of-type,td.mat-footer-cell:last-of-type{padding-right:24px}[dir=rtl] th.mat-header-cell:last-of-type:not(:only-of-type),[dir=rtl] td.mat-cell:last-of-type:not(:only-of-type),[dir=rtl] td.mat-footer-cell:last-of-type:not(:only-of-type){padding-right:0;padding-left:24px}.mat-table-sticky{position:sticky !important}.mat-table-fixed-layout{table-layout:fixed}\n"],
                         encapsulation: 2
                     }), Z
                 })(),
                 Ce = (() => {
@@ -23388,15 +23393,15 @@
                 F = v(6895),
                 O = v(4650),
                 De = v(3238),
                 L = v(5698),
                 be = v(8675),
                 Me = v(1884),
                 fe = v(2722),
-                Oe = v(3900),
+                Te = v(3900),
                 ye = v(5684),
                 g = v(7579),
                 xe = v(727),
                 pe = v(4968),
                 Ge = v(9646),
                 Ve = v(6451),
                 We = v(515),
@@ -23464,18 +23469,18 @@
                         const kn = O.CHM(ie).index,
                             In = O.oxw();
                         return O.KtG(In._tabFocusChanged(nt, kn))
                     }), O.TgZ(1, "div", 7), O.YNc(2, et, 1, 1, "ng-template", 8), O.YNc(3, ut, 1, 1, "ng-template", null, 9, O.W1O), O.qZA()()
                 }
                 if (2 & mt) {
                     const ie = Pt.$implicit,
-                        Te = Pt.index,
+                        Se = Pt.index,
                         nt = O.MAs(4),
                         xt = O.oxw();
-                    O.ekj("mat-tab-label-active", xt.selectedIndex === Te), O.Q6J("id", xt._getTabLabelId(Te))("ngClass", ie.labelClass)("disabled", ie.disabled)("matRippleDisabled", ie.disabled || xt.disableRipple), O.uIk("tabIndex", xt._getTabIndex(ie, Te))("aria-posinset", Te + 1)("aria-setsize", xt._tabs.length)("aria-controls", xt._getTabContentId(Te))("aria-selected", xt.selectedIndex === Te)("aria-label", ie.ariaLabel || null)("aria-labelledby", !ie.ariaLabel && ie.ariaLabelledby ? ie.ariaLabelledby : null), O.xp6(2), O.Q6J("ngIf", ie.templateLabel)("ngIfElse", nt)
+                    O.ekj("mat-tab-label-active", xt.selectedIndex === Se), O.Q6J("id", xt._getTabLabelId(Se))("ngClass", ie.labelClass)("disabled", ie.disabled)("matRippleDisabled", ie.disabled || xt.disableRipple), O.uIk("tabIndex", xt._getTabIndex(ie, Se))("aria-posinset", Se + 1)("aria-setsize", xt._tabs.length)("aria-controls", xt._getTabContentId(Se))("aria-selected", xt.selectedIndex === Se)("aria-label", ie.ariaLabel || null)("aria-labelledby", !ie.ariaLabel && ie.ariaLabelledby ? ie.ariaLabelledby : null), O.xp6(2), O.Q6J("ngIf", ie.templateLabel)("ngIfElse", nt)
                 }
             }
 
             function ve(mt, Pt) {
                 if (1 & mt) {
                     const ie = O.EpF();
                     O.TgZ(0, "mat-tab-body", 11), O.NdJ("_onCentered", function() {
@@ -23486,38 +23491,38 @@
                         O.CHM(ie);
                         const xt = O.oxw();
                         return O.KtG(xt._setTabBodyWrapperHeight(nt))
                     }), O.qZA()
                 }
                 if (2 & mt) {
                     const ie = Pt.$implicit,
-                        Te = Pt.index,
+                        Se = Pt.index,
                         nt = O.oxw();
-                    O.ekj("mat-tab-body-active", nt.selectedIndex === Te), O.Q6J("id", nt._getTabContentId(Te))("ngClass", ie.bodyClass)("content", ie.content)("position", ie.position)("origin", ie.origin)("animationDuration", nt.animationDuration), O.uIk("tabindex", null != nt.contentTabIndex && nt.selectedIndex === Te ? nt.contentTabIndex : null)("aria-labelledby", nt._getTabLabelId(Te))
+                    O.ekj("mat-tab-body-active", nt.selectedIndex === Se), O.Q6J("id", nt._getTabContentId(Se))("ngClass", ie.bodyClass)("content", ie.content)("position", ie.position)("origin", ie.origin)("animationDuration", nt.animationDuration), O.uIk("tabindex", null != nt.contentTabIndex && nt.selectedIndex === Se ? nt.contentTabIndex : null)("aria-labelledby", nt._getTabLabelId(Se))
                 }
             }
             const ee = new O.OlP("MatInkBarPositioner", {
                 providedIn: "root",
                 factory: function Q() {
                     return Pt => ({
                         left: Pt ? (Pt.offsetLeft || 0) + "px" : "0",
                         width: Pt ? (Pt.offsetWidth || 0) + "px" : "0"
                     })
                 }
             });
             let X = (() => {
                 class mt {
-                    constructor(ie, Te, nt, xt) {
-                        this._elementRef = ie, this._ngZone = Te, this._inkBarPositioner = nt, this._animationMode = xt
+                    constructor(ie, Se, nt, xt) {
+                        this._elementRef = ie, this._ngZone = Se, this._inkBarPositioner = nt, this._animationMode = xt
                     }
                     alignToElement(ie) {
                         this.show(), this._ngZone.onStable.pipe((0, L.q)(1)).subscribe(() => {
-                            const Te = this._inkBarPositioner(ie),
+                            const Se = this._inkBarPositioner(ie),
                                 nt = this._elementRef.nativeElement;
-                            nt.style.left = Te.left, nt.style.width = Te.width
+                            nt.style.left = Se.left, nt.style.width = Se.width
                         })
                     }
                     show() {
                         this._elementRef.nativeElement.style.visibility = "visible"
                     }
                     hide() {
                         this._elementRef.nativeElement.style.visibility = "hidden"
@@ -23528,28 +23533,28 @@
                 }, mt.\u0275dir = O.lG2({
                     type: mt,
                     selectors: [
                         ["mat-ink-bar"]
                     ],
                     hostAttrs: [1, "mat-ink-bar"],
                     hostVars: 2,
-                    hostBindings: function(ie, Te) {
-                        2 & ie && O.ekj("_mat-animation-noopable", "NoopAnimations" === Te._animationMode)
+                    hostBindings: function(ie, Se) {
+                        2 & ie && O.ekj("_mat-animation-noopable", "NoopAnimations" === Se._animationMode)
                     }
                 }), mt
             })();
             const He = new O.OlP("MatTabContent"),
                 bt = new O.OlP("MatTabLabel"),
                 Ut = new O.OlP("MAT_TAB"),
                 G = (0, De.Id)(class {}),
                 $ = new O.OlP("MAT_TAB_GROUP");
             let Re = (() => {
                 class mt extends G {
-                    constructor(ie, Te) {
-                        super(), this._viewContainerRef = ie, this._closestTabGroup = Te, this.textLabel = "", this._contentPortal = null, this._stateChanges = new g.x, this.position = null, this.origin = null, this.isActive = !1
+                    constructor(ie, Se) {
+                        super(), this._viewContainerRef = ie, this._closestTabGroup = Se, this.textLabel = "", this._contentPortal = null, this._stateChanges = new g.x, this.position = null, this.origin = null, this.isActive = !1
                     }
                     get templateLabel() {
                         return this._templateLabel
                     }
                     set templateLabel(ie) {
                         this._setTemplateLabelInput(ie)
                     }
@@ -23572,24 +23577,24 @@
                 return mt.\u0275fac = function(ie) {
                     return new(ie || mt)(O.Y36(O.s_b), O.Y36($, 8))
                 }, mt.\u0275cmp = O.Xpm({
                     type: mt,
                     selectors: [
                         ["mat-tab"]
                     ],
-                    contentQueries: function(ie, Te, nt) {
+                    contentQueries: function(ie, Se, nt) {
                         if (1 & ie && (O.Suo(nt, bt, 5), O.Suo(nt, He, 7, O.Rgc)), 2 & ie) {
                             let xt;
-                            O.iGM(xt = O.CRH()) && (Te.templateLabel = xt.first), O.iGM(xt = O.CRH()) && (Te._explicitContent = xt.first)
+                            O.iGM(xt = O.CRH()) && (Se.templateLabel = xt.first), O.iGM(xt = O.CRH()) && (Se._explicitContent = xt.first)
                         }
                     },
-                    viewQuery: function(ie, Te) {
+                    viewQuery: function(ie, Se) {
                         if (1 & ie && O.Gf(O.Rgc, 7), 2 & ie) {
                             let nt;
-                            O.iGM(nt = O.CRH()) && (Te._implicitContent = nt.first)
+                            O.iGM(nt = O.CRH()) && (Se._implicitContent = nt.first)
                         }
                     },
                     inputs: {
                         disabled: "disabled",
                         textLabel: ["label", "textLabel"],
                         ariaLabel: ["aria-label", "ariaLabel"],
                         ariaLabelledby: ["aria-labelledby", "ariaLabelledby"],
@@ -23600,15 +23605,15 @@
                     features: [O._Bn([{
                         provide: Ut,
                         useExisting: mt
                     }]), O.qOj, O.TTD],
                     ngContentSelectors: Ft,
                     decls: 1,
                     vars: 0,
-                    template: function(ie, Te) {
+                    template: function(ie, Se) {
                         1 & ie && (O.F$t(), O.YNc(0, vt, 1, 0, "ng-template"))
                     },
                     encapsulation: 2
                 }), mt
             })();
             const j = {
                 translateTab: (0, te.X$)("translateTab", [(0, te.SB)("center, void, left-origin-center, right-origin-center", (0, te.oB)({
@@ -23623,16 +23628,16 @@
                     transform: "translate3d(-100%, 0, 0)"
                 }), (0, te.jt)("{{animationDuration}} cubic-bezier(0.35, 0, 0.25, 1)")]), (0, te.eR)("void => right-origin-center", [(0, te.oB)({
                     transform: "translate3d(100%, 0, 0)"
                 }), (0, te.jt)("{{animationDuration}} cubic-bezier(0.35, 0, 0.25, 1)")])])
             };
             let ne = (() => {
                     class mt extends C.Pl {
-                        constructor(ie, Te, nt, xt) {
-                            super(ie, Te, xt), this._host = nt, this._centeringSub = xe.w0.EMPTY, this._leavingSub = xe.w0.EMPTY
+                        constructor(ie, Se, nt, xt) {
+                            super(ie, Se, xt), this._host = nt, this._centeringSub = xe.w0.EMPTY, this._leavingSub = xe.w0.EMPTY
                         }
                         ngOnInit() {
                             super.ngOnInit(), this._centeringSub = this._host._beforeCentering.pipe((0, be.O)(this._host._isCenterPosition(this._host._position))).subscribe(ie => {
                                 ie && !this.hasAttached() && this.attach(this._host._content)
                             }), this._leavingSub = this._host._afterLeavingCenter.subscribe(() => {
                                 this.detach()
                             })
@@ -23649,16 +23654,16 @@
                             ["", "matTabBodyHost", ""]
                         ],
                         features: [O.qOj]
                     }), mt
                 })(),
                 ue = (() => {
                     class mt {
-                        constructor(ie, Te, nt) {
-                            this._elementRef = ie, this._dir = Te, this._dirChangeSubscription = xe.w0.EMPTY, this._translateTabComplete = new g.x, this._onCentering = new O.vpe, this._beforeCentering = new O.vpe, this._afterLeavingCenter = new O.vpe, this._onCentered = new O.vpe(!0), this.animationDuration = "500ms", Te && (this._dirChangeSubscription = Te.change.subscribe(xt => {
+                        constructor(ie, Se, nt) {
+                            this._elementRef = ie, this._dir = Se, this._dirChangeSubscription = xe.w0.EMPTY, this._translateTabComplete = new g.x, this._onCentering = new O.vpe, this._beforeCentering = new O.vpe, this._afterLeavingCenter = new O.vpe, this._onCentered = new O.vpe(!0), this.animationDuration = "500ms", Se && (this._dirChangeSubscription = Se.change.subscribe(xt => {
                                 this._computePositionAnimationState(xt), nt.markForCheck()
                             })), this._translateTabComplete.pipe((0, Me.x)((xt, kn) => xt.fromState === kn.fromState && xt.toState === kn.toState)).subscribe(xt => {
                                 this._isCenterPosition(xt.toState) && this._isCenterPosition(this._position) && this._onCentered.emit(), this._isCenterPosition(xt.fromState) && !this._isCenterPosition(this._position) && this._afterLeavingCenter.emit()
                             })
                         }
                         set position(ie) {
                             this._positionIndex = ie, this._computePositionAnimationState()
@@ -23666,29 +23671,29 @@
                         ngOnInit() {
                             "center" == this._position && null != this.origin && (this._position = this._computePositionFromOrigin(this.origin))
                         }
                         ngOnDestroy() {
                             this._dirChangeSubscription.unsubscribe(), this._translateTabComplete.complete()
                         }
                         _onTranslateTabStarted(ie) {
-                            const Te = this._isCenterPosition(ie.toState);
-                            this._beforeCentering.emit(Te), Te && this._onCentering.emit(this._elementRef.nativeElement.clientHeight)
+                            const Se = this._isCenterPosition(ie.toState);
+                            this._beforeCentering.emit(Se), Se && this._onCentering.emit(this._elementRef.nativeElement.clientHeight)
                         }
                         _getLayoutDirection() {
                             return this._dir && "rtl" === this._dir.value ? "rtl" : "ltr"
                         }
                         _isCenterPosition(ie) {
                             return "center" == ie || "left-origin-center" == ie || "right-origin-center" == ie
                         }
                         _computePositionAnimationState(ie = this._getLayoutDirection()) {
                             this._position = this._positionIndex < 0 ? "ltr" == ie ? "left" : "right" : this._positionIndex > 0 ? "ltr" == ie ? "right" : "left" : "center"
                         }
                         _computePositionFromOrigin(ie) {
-                            const Te = this._getLayoutDirection();
-                            return "ltr" == Te && ie <= 0 || "rtl" == Te && ie > 0 ? "left-origin-center" : "right-origin-center"
+                            const Se = this._getLayoutDirection();
+                            return "ltr" == Se && ie <= 0 || "rtl" == Se && ie > 0 ? "left-origin-center" : "right-origin-center"
                         }
                     }
                     return mt.\u0275fac = function(ie) {
                         return new(ie || mt)(O.Y36(O.SBq), O.Y36(ae.Is, 8), O.Y36(O.sBO))
                     }, mt.\u0275dir = O.lG2({
                         type: mt,
                         inputs: {
@@ -23703,46 +23708,46 @@
                             _afterLeavingCenter: "_afterLeavingCenter",
                             _onCentered: "_onCentered"
                         }
                     }), mt
                 })(),
                 Ze = (() => {
                     class mt extends ue {
-                        constructor(ie, Te, nt) {
-                            super(ie, Te, nt)
+                        constructor(ie, Se, nt) {
+                            super(ie, Se, nt)
                         }
                     }
                     return mt.\u0275fac = function(ie) {
                         return new(ie || mt)(O.Y36(O.SBq), O.Y36(ae.Is, 8), O.Y36(O.sBO))
                     }, mt.\u0275cmp = O.Xpm({
                         type: mt,
                         selectors: [
                             ["mat-tab-body"]
                         ],
-                        viewQuery: function(ie, Te) {
+                        viewQuery: function(ie, Se) {
                             if (1 & ie && O.Gf(C.Pl, 5), 2 & ie) {
                                 let nt;
-                                O.iGM(nt = O.CRH()) && (Te._portalHost = nt.first)
+                                O.iGM(nt = O.CRH()) && (Se._portalHost = nt.first)
                             }
                         },
                         hostAttrs: [1, "mat-tab-body"],
                         features: [O.qOj],
                         decls: 3,
                         vars: 6,
                         consts: [
                             ["cdkScrollable", "", 1, "mat-tab-body-content"],
                             ["content", ""],
                             ["matTabBodyHost", ""]
                         ],
-                        template: function(ie, Te) {
+                        template: function(ie, Se) {
                             1 & ie && (O.TgZ(0, "div", 0, 1), O.NdJ("@translateTab.start", function(xt) {
-                                return Te._onTranslateTabStarted(xt)
+                                return Se._onTranslateTabStarted(xt)
                             })("@translateTab.done", function(xt) {
-                                return Te._translateTabComplete.next(xt)
-                            }), O.YNc(2, kt, 0, 0, "ng-template", 2), O.qZA()), 2 & ie && O.Q6J("@translateTab", O.WLB(3, Lt, Te._position, O.VKq(1, $t, Te.animationDuration)))
+                                return Se._translateTabComplete.next(xt)
+                            }), O.YNc(2, kt, 0, 0, "ng-template", 2), O.qZA()), 2 & ie && O.Q6J("@translateTab", O.WLB(3, Lt, Se._position, O.VKq(1, $t, Se.animationDuration)))
                         },
                         dependencies: [ne],
                         styles: ['.mat-tab-body-content{height:100%;overflow:auto}.mat-tab-group-dynamic-height .mat-tab-body-content{overflow:hidden}.mat-tab-body-content[style*="visibility: hidden"]{display:none}\n'],
                         encapsulation: 2,
                         data: {
                             animation: [j.translateTab]
                         }
@@ -23769,30 +23774,30 @@
                     return new(ie || mt)(O.Y36(O.SBq))
                 }, mt.\u0275dir = O.lG2({
                     type: mt,
                     selectors: [
                         ["", "matTabLabelWrapper", ""]
                     ],
                     hostVars: 3,
-                    hostBindings: function(ie, Te) {
-                        2 & ie && (O.uIk("aria-disabled", !!Te.disabled), O.ekj("mat-tab-disabled", Te.disabled))
+                    hostBindings: function(ie, Se) {
+                        2 & ie && (O.uIk("aria-disabled", !!Se.disabled), O.ekj("mat-tab-disabled", Se.disabled))
                     },
                     inputs: {
                         disabled: "disabled"
                     },
                     features: [O.qOj]
                 }), mt
             })();
             const ce = (0, Ie.i$)({
                 passive: !0
             });
             let sn = (() => {
                     class mt {
-                        constructor(ie, Te, nt, xt, kn, In, Tn) {
-                            this._elementRef = ie, this._changeDetectorRef = Te, this._viewportRuler = nt, this._dir = xt, this._ngZone = kn, this._platform = In, this._animationMode = Tn, this._scrollDistance = 0, this._selectedIndexChanged = !1, this._destroyed = new g.x, this._showPaginationControls = !1, this._disableScrollAfter = !0, this._disableScrollBefore = !0, this._stopScrolling = new g.x, this.disablePagination = !1, this._selectedIndex = 0, this.selectFocusedIndex = new O.vpe, this.indexFocused = new O.vpe, kn.runOutsideAngular(() => {
+                        constructor(ie, Se, nt, xt, kn, In, Tn) {
+                            this._elementRef = ie, this._changeDetectorRef = Se, this._viewportRuler = nt, this._dir = xt, this._ngZone = kn, this._platform = In, this._animationMode = Tn, this._scrollDistance = 0, this._selectedIndexChanged = !1, this._destroyed = new g.x, this._showPaginationControls = !1, this._disableScrollAfter = !0, this._disableScrollBefore = !0, this._stopScrolling = new g.x, this.disablePagination = !1, this._selectedIndex = 0, this.selectFocusedIndex = new O.vpe, this.indexFocused = new O.vpe, kn.runOutsideAngular(() => {
                                 (0, pe.R)(ie.nativeElement, "mouseleave").pipe((0, fe.R)(this._destroyed)).subscribe(() => {
                                     this._stopInterval()
                                 })
                             })
                         }
                         get selectedIndex() {
                             return this._selectedIndex
@@ -23805,32 +23810,32 @@
                                 this._handlePaginatorPress("before")
                             }), (0, pe.R)(this._nextPaginator.nativeElement, "touchstart", ce).pipe((0, fe.R)(this._destroyed)).subscribe(() => {
                                 this._handlePaginatorPress("after")
                             })
                         }
                         ngAfterContentInit() {
                             const ie = this._dir ? this._dir.change : (0, Ge.of)("ltr"),
-                                Te = this._viewportRuler.change(150),
+                                Se = this._viewportRuler.change(150),
                                 nt = () => {
                                     this.updatePagination(), this._alignInkBarToSelectedTab()
                                 };
-                            this._keyManager = new s.Em(this._items).withHorizontalOrientation(this._getLayoutDirection()).withHomeAndEnd().withWrap(), this._keyManager.updateActiveItem(this._selectedIndex), this._ngZone.onStable.pipe((0, L.q)(1)).subscribe(nt), (0, Ve.T)(ie, Te, this._items.changes, this._itemsResized()).pipe((0, fe.R)(this._destroyed)).subscribe(() => {
+                            this._keyManager = new s.Em(this._items).withHorizontalOrientation(this._getLayoutDirection()).withHomeAndEnd().withWrap(), this._keyManager.updateActiveItem(this._selectedIndex), this._ngZone.onStable.pipe((0, L.q)(1)).subscribe(nt), (0, Ve.T)(ie, Se, this._items.changes, this._itemsResized()).pipe((0, fe.R)(this._destroyed)).subscribe(() => {
                                 this._ngZone.run(() => {
                                     Promise.resolve().then(() => {
                                         this._scrollDistance = Math.max(0, Math.min(this._getMaxScrollDistance(), this._scrollDistance)), nt()
                                     })
                                 }), this._keyManager.withHorizontalOrientation(this._getLayoutDirection())
                             }), this._keyManager.change.pipe((0, fe.R)(this._destroyed)).subscribe(xt => {
                                 this.indexFocused.emit(xt), this._setTabFocus(xt)
                             })
                         }
                         _itemsResized() {
-                            return "function" != typeof ResizeObserver ? We.E : this._items.changes.pipe((0, be.O)(this._items), (0, Oe.w)(ie => new ht.y(Te => this._ngZone.runOutsideAngular(() => {
+                            return "function" != typeof ResizeObserver ? We.E : this._items.changes.pipe((0, be.O)(this._items), (0, Te.w)(ie => new ht.y(Se => this._ngZone.runOutsideAngular(() => {
                                 const nt = new ResizeObserver(() => {
-                                    Te.next()
+                                    Se.next()
                                 });
                                 return ie.forEach(xt => {
                                     nt.observe(xt.elementRef.nativeElement)
                                 }), () => {
                                     nt.disconnect()
                                 }
                             }))), (0, ye.T)(1))
@@ -23864,32 +23869,32 @@
                             return this._keyManager ? this._keyManager.activeItemIndex : 0
                         }
                         set focusIndex(ie) {
                             !this._isValidIndex(ie) || this.focusIndex === ie || !this._keyManager || this._keyManager.setActiveItem(ie)
                         }
                         _isValidIndex(ie) {
                             if (!this._items) return !0;
-                            const Te = this._items ? this._items.toArray()[ie] : null;
-                            return !!Te && !Te.disabled
+                            const Se = this._items ? this._items.toArray()[ie] : null;
+                            return !!Se && !Se.disabled
                         }
                         _setTabFocus(ie) {
                             if (this._showPaginationControls && this._scrollToLabel(ie), this._items && this._items.length) {
                                 this._items.toArray()[ie].focus();
-                                const Te = this._tabListContainer.nativeElement;
-                                Te.scrollLeft = "ltr" == this._getLayoutDirection() ? 0 : Te.scrollWidth - Te.offsetWidth
+                                const Se = this._tabListContainer.nativeElement;
+                                Se.scrollLeft = "ltr" == this._getLayoutDirection() ? 0 : Se.scrollWidth - Se.offsetWidth
                             }
                         }
                         _getLayoutDirection() {
                             return this._dir && "rtl" === this._dir.value ? "rtl" : "ltr"
                         }
                         _updateTabScrollPosition() {
                             if (this.disablePagination) return;
                             const ie = this.scrollDistance,
-                                Te = "ltr" === this._getLayoutDirection() ? -ie : ie;
-                            this._tabList.nativeElement.style.transform = `translateX(${Math.round(Te)}px)`, (this._platform.TRIDENT || this._platform.EDGE) && (this._tabListContainer.nativeElement.scrollLeft = 0)
+                                Se = "ltr" === this._getLayoutDirection() ? -ie : ie;
+                            this._tabList.nativeElement.style.transform = `translateX(${Math.round(Se)}px)`, (this._platform.TRIDENT || this._platform.EDGE) && (this._tabListContainer.nativeElement.scrollLeft = 0)
                         }
                         get scrollDistance() {
                             return this._scrollDistance
                         }
                         set scrollDistance(ie) {
                             this._scrollTo(ie)
                         }
@@ -23897,21 +23902,21 @@
                             return this._scrollTo(this._scrollDistance + ("before" == ie ? -1 : 1) * this._tabListContainer.nativeElement.offsetWidth / 3)
                         }
                         _handlePaginatorClick(ie) {
                             this._stopInterval(), this._scrollHeader(ie)
                         }
                         _scrollToLabel(ie) {
                             if (this.disablePagination) return;
-                            const Te = this._items ? this._items.toArray()[ie] : null;
-                            if (!Te) return;
+                            const Se = this._items ? this._items.toArray()[ie] : null;
+                            if (!Se) return;
                             const nt = this._tabListContainer.nativeElement.offsetWidth,
                                 {
                                     offsetLeft: xt,
                                     offsetWidth: kn
-                                } = Te.elementRef.nativeElement;
+                                } = Se.elementRef.nativeElement;
                             let In, Tn;
                             "ltr" == this._getLayoutDirection() ? (In = xt, Tn = In + kn) : (Tn = this._tabListInner.nativeElement.offsetWidth - xt, In = Tn - kn);
                             const Ce = this.scrollDistance,
                                 we = this.scrollDistance + nt;
                             In < Ce ? this.scrollDistance -= Ce - In + 60 : Tn > we && (this.scrollDistance += Tn - we + 60)
                         }
                         _checkPaginationEnabled() {
@@ -23925,37 +23930,37 @@
                             this.disablePagination ? this._disableScrollAfter = this._disableScrollBefore = !0 : (this._disableScrollBefore = 0 == this.scrollDistance, this._disableScrollAfter = this.scrollDistance == this._getMaxScrollDistance(), this._changeDetectorRef.markForCheck())
                         }
                         _getMaxScrollDistance() {
                             return this._tabListInner.nativeElement.scrollWidth - this._tabListContainer.nativeElement.offsetWidth || 0
                         }
                         _alignInkBarToSelectedTab() {
                             const ie = this._items && this._items.length ? this._items.toArray()[this.selectedIndex] : null,
-                                Te = ie ? ie.elementRef.nativeElement : null;
-                            Te ? this._inkBar.alignToElement(Te) : this._inkBar.hide()
+                                Se = ie ? ie.elementRef.nativeElement : null;
+                            Se ? this._inkBar.alignToElement(Se) : this._inkBar.hide()
                         }
                         _stopInterval() {
                             this._stopScrolling.next()
                         }
-                        _handlePaginatorPress(ie, Te) {
-                            Te && null != Te.button && 0 !== Te.button || (this._stopInterval(), (0, lt.H)(650, 100).pipe((0, fe.R)((0, Ve.T)(this._stopScrolling, this._destroyed))).subscribe(() => {
+                        _handlePaginatorPress(ie, Se) {
+                            Se && null != Se.button && 0 !== Se.button || (this._stopInterval(), (0, lt.H)(650, 100).pipe((0, fe.R)((0, Ve.T)(this._stopScrolling, this._destroyed))).subscribe(() => {
                                 const {
                                     maxScrollDistance: nt,
                                     distance: xt
                                 } = this._scrollHeader(ie);
                                 (0 === xt || xt >= nt) && this._stopInterval()
                             }))
                         }
                         _scrollTo(ie) {
                             if (this.disablePagination) return {
                                 maxScrollDistance: 0,
                                 distance: 0
                             };
-                            const Te = this._getMaxScrollDistance();
-                            return this._scrollDistance = Math.max(0, Math.min(Te, ie)), this._scrollDistanceChanged = !0, this._checkScrollingControls(), {
-                                maxScrollDistance: Te,
+                            const Se = this._getMaxScrollDistance();
+                            return this._scrollDistance = Math.max(0, Math.min(Se, ie)), this._scrollDistanceChanged = !0, this._checkScrollingControls(), {
+                                maxScrollDistance: Se,
                                 distance: this._scrollDistance
                             }
                         }
                     }
                     return mt.\u0275fac = function(ie) {
                         return new(ie || mt)(O.Y36(O.SBq), O.Y36(O.sBO), O.Y36(Ee.rL), O.Y36(ae.Is, 8), O.Y36(O.R0b), O.Y36(Ie.t4), O.Y36(O.QbO, 8))
                     }, mt.\u0275dir = O.lG2({
@@ -23963,16 +23968,16 @@
                         inputs: {
                             disablePagination: "disablePagination"
                         }
                     }), mt
                 })(),
                 an = (() => {
                     class mt extends sn {
-                        constructor(ie, Te, nt, xt, kn, In, Tn) {
-                            super(ie, Te, nt, xt, kn, In, Tn), this._disableRipple = !1
+                        constructor(ie, Se, nt, xt, kn, In, Tn) {
+                            super(ie, Se, nt, xt, kn, In, Tn), this._disableRipple = !1
                         }
                         get disableRipple() {
                             return this._disableRipple
                         }
                         set disableRipple(ie) {
                             this._disableRipple = (0, J.Ig)(ie)
                         }
@@ -23988,41 +23993,41 @@
                             disableRipple: "disableRipple"
                         },
                         features: [O.qOj]
                     }), mt
                 })(),
                 Mt = (() => {
                     class mt extends an {
-                        constructor(ie, Te, nt, xt, kn, In, Tn) {
-                            super(ie, Te, nt, xt, kn, In, Tn)
+                        constructor(ie, Se, nt, xt, kn, In, Tn) {
+                            super(ie, Se, nt, xt, kn, In, Tn)
                         }
                     }
                     return mt.\u0275fac = function(ie) {
                         return new(ie || mt)(O.Y36(O.SBq), O.Y36(O.sBO), O.Y36(Ee.rL), O.Y36(ae.Is, 8), O.Y36(O.R0b), O.Y36(Ie.t4), O.Y36(O.QbO, 8))
                     }, mt.\u0275cmp = O.Xpm({
                         type: mt,
                         selectors: [
                             ["mat-tab-header"]
                         ],
-                        contentQueries: function(ie, Te, nt) {
+                        contentQueries: function(ie, Se, nt) {
                             if (1 & ie && O.Suo(nt, de, 4), 2 & ie) {
                                 let xt;
-                                O.iGM(xt = O.CRH()) && (Te._items = xt)
+                                O.iGM(xt = O.CRH()) && (Se._items = xt)
                             }
                         },
-                        viewQuery: function(ie, Te) {
+                        viewQuery: function(ie, Se) {
                             if (1 & ie && (O.Gf(X, 7), O.Gf(bn, 7), O.Gf(dn, 7), O.Gf(wn, 7), O.Gf(Pn, 5), O.Gf(qe, 5)), 2 & ie) {
                                 let nt;
-                                O.iGM(nt = O.CRH()) && (Te._inkBar = nt.first), O.iGM(nt = O.CRH()) && (Te._tabListContainer = nt.first), O.iGM(nt = O.CRH()) && (Te._tabList = nt.first), O.iGM(nt = O.CRH()) && (Te._tabListInner = nt.first), O.iGM(nt = O.CRH()) && (Te._nextPaginator = nt.first), O.iGM(nt = O.CRH()) && (Te._previousPaginator = nt.first)
+                                O.iGM(nt = O.CRH()) && (Se._inkBar = nt.first), O.iGM(nt = O.CRH()) && (Se._tabListContainer = nt.first), O.iGM(nt = O.CRH()) && (Se._tabList = nt.first), O.iGM(nt = O.CRH()) && (Se._tabListInner = nt.first), O.iGM(nt = O.CRH()) && (Se._nextPaginator = nt.first), O.iGM(nt = O.CRH()) && (Se._previousPaginator = nt.first)
                             }
                         },
                         hostAttrs: [1, "mat-tab-header"],
                         hostVars: 4,
-                        hostBindings: function(ie, Te) {
-                            2 & ie && O.ekj("mat-tab-header-pagination-controls-enabled", Te._showPaginationControls)("mat-tab-header-rtl", "rtl" == Te._getLayoutDirection())
+                        hostBindings: function(ie, Se) {
+                            2 & ie && O.ekj("mat-tab-header-pagination-controls-enabled", Se._showPaginationControls)("mat-tab-header-rtl", "rtl" == Se._getLayoutDirection())
                         },
                         inputs: {
                             selectedIndex: "selectedIndex"
                         },
                         outputs: {
                             selectFocusedIndex: "selectFocusedIndex",
                             indexFocused: "indexFocused"
@@ -24040,32 +24045,32 @@
                             ["role", "tablist", 1, "mat-tab-list", 3, "cdkObserveContent"],
                             ["tabList", ""],
                             [1, "mat-tab-labels"],
                             ["tabListInner", ""],
                             ["aria-hidden", "true", "type", "button", "mat-ripple", "", "tabindex", "-1", 1, "mat-tab-header-pagination", "mat-tab-header-pagination-after", "mat-elevation-z4", 3, "matRippleDisabled", "disabled", "mousedown", "click", "touchend"],
                             ["nextPaginator", ""]
                         ],
-                        template: function(ie, Te) {
+                        template: function(ie, Se) {
                             1 & ie && (O.F$t(), O.TgZ(0, "button", 0, 1), O.NdJ("click", function() {
-                                return Te._handlePaginatorClick("before")
+                                return Se._handlePaginatorClick("before")
                             })("mousedown", function(xt) {
-                                return Te._handlePaginatorPress("before", xt)
+                                return Se._handlePaginatorPress("before", xt)
                             })("touchend", function() {
-                                return Te._stopInterval()
+                                return Se._stopInterval()
                             }), O._UZ(2, "div", 2), O.qZA(), O.TgZ(3, "div", 3, 4), O.NdJ("keydown", function(xt) {
-                                return Te._handleKeydown(xt)
+                                return Se._handleKeydown(xt)
                             }), O.TgZ(5, "div", 5, 6), O.NdJ("cdkObserveContent", function() {
-                                return Te._onContentChanges()
+                                return Se._onContentChanges()
                             }), O.TgZ(7, "div", 7, 8), O.Hsn(9), O.qZA(), O._UZ(10, "mat-ink-bar"), O.qZA()(), O.TgZ(11, "button", 9, 10), O.NdJ("mousedown", function(xt) {
-                                return Te._handlePaginatorPress("after", xt)
+                                return Se._handlePaginatorPress("after", xt)
                             })("click", function() {
-                                return Te._handlePaginatorClick("after")
+                                return Se._handlePaginatorClick("after")
                             })("touchend", function() {
-                                return Te._stopInterval()
-                            }), O._UZ(13, "div", 2), O.qZA()), 2 & ie && (O.ekj("mat-tab-header-pagination-disabled", Te._disableScrollBefore), O.Q6J("matRippleDisabled", Te._disableScrollBefore || Te.disableRipple)("disabled", Te._disableScrollBefore || null), O.xp6(5), O.ekj("_mat-animation-noopable", "NoopAnimations" === Te._animationMode), O.xp6(6), O.ekj("mat-tab-header-pagination-disabled", Te._disableScrollAfter), O.Q6J("matRippleDisabled", Te._disableScrollAfter || Te.disableRipple)("disabled", Te._disableScrollAfter || null))
+                                return Se._stopInterval()
+                            }), O._UZ(13, "div", 2), O.qZA()), 2 & ie && (O.ekj("mat-tab-header-pagination-disabled", Se._disableScrollBefore), O.Q6J("matRippleDisabled", Se._disableScrollBefore || Se.disableRipple)("disabled", Se._disableScrollBefore || null), O.xp6(5), O.ekj("_mat-animation-noopable", "NoopAnimations" === Se._animationMode), O.xp6(6), O.ekj("mat-tab-header-pagination-disabled", Se._disableScrollAfter), O.Q6J("matRippleDisabled", Se._disableScrollAfter || Se.disableRipple)("disabled", Se._disableScrollAfter || null))
                         },
                         dependencies: [De.wG, S.wD, X],
                         styles: [".mat-tab-header{display:flex;overflow:hidden;position:relative;flex-shrink:0}.mat-tab-header-pagination{-webkit-user-select:none;user-select:none;position:relative;display:none;justify-content:center;align-items:center;min-width:32px;cursor:pointer;z-index:2;-webkit-tap-highlight-color:transparent;touch-action:none;box-sizing:content-box;background:none;border:none;outline:0;padding:0}.mat-tab-header-pagination::-moz-focus-inner{border:0}.mat-tab-header-pagination-controls-enabled .mat-tab-header-pagination{display:flex}.mat-tab-header-pagination-before,.mat-tab-header-rtl .mat-tab-header-pagination-after{padding-left:4px}.mat-tab-header-pagination-before .mat-tab-header-pagination-chevron,.mat-tab-header-rtl .mat-tab-header-pagination-after .mat-tab-header-pagination-chevron{transform:rotate(-135deg)}.mat-tab-header-rtl .mat-tab-header-pagination-before,.mat-tab-header-pagination-after{padding-right:4px}.mat-tab-header-rtl .mat-tab-header-pagination-before .mat-tab-header-pagination-chevron,.mat-tab-header-pagination-after .mat-tab-header-pagination-chevron{transform:rotate(45deg)}.mat-tab-header-pagination-chevron{border-style:solid;border-width:2px 2px 0 0;height:8px;width:8px}.mat-tab-header-pagination-disabled{box-shadow:none;cursor:default}.mat-tab-list{flex-grow:1;position:relative;transition:transform 500ms cubic-bezier(0.35, 0, 0.25, 1)}.mat-ink-bar{position:absolute;bottom:0;height:2px;transition:500ms cubic-bezier(0.35, 0, 0.25, 1)}._mat-animation-noopable.mat-ink-bar{transition:none;animation:none}.mat-tab-group-inverted-header .mat-ink-bar{bottom:auto;top:0}.cdk-high-contrast-active .mat-ink-bar{outline:solid 2px;height:0}.mat-tab-labels{display:flex}[mat-align-tabs=center]>.mat-tab-header .mat-tab-labels{justify-content:center}[mat-align-tabs=end]>.mat-tab-header .mat-tab-labels{justify-content:flex-end}.mat-tab-label-container{display:flex;flex-grow:1;overflow:hidden;z-index:1}._mat-animation-noopable.mat-tab-list{transition:none;animation:none}.mat-tab-label{height:48px;padding:0 24px;cursor:pointer;box-sizing:border-box;opacity:.6;min-width:160px;text-align:center;display:inline-flex;justify-content:center;align-items:center;white-space:nowrap;position:relative}.mat-tab-label:focus{outline:none}.mat-tab-label:focus:not(.mat-tab-disabled){opacity:1}.cdk-high-contrast-active .mat-tab-label:focus{outline:dotted 2px;outline-offset:-2px}.mat-tab-label.mat-tab-disabled{cursor:default}.cdk-high-contrast-active .mat-tab-label.mat-tab-disabled{opacity:.5}.mat-tab-label .mat-tab-label-content{display:inline-flex;justify-content:center;align-items:center;white-space:nowrap}.cdk-high-contrast-active .mat-tab-label{opacity:1}@media(max-width: 599px){.mat-tab-label{min-width:72px}}\n"],
                         encapsulation: 2
                     }), mt
                 })(),
                 Fn = 0;
@@ -24073,16 +24078,16 @@
             const St = (0, De.pj)((0, De.Kr)(class {
                 constructor(mt) {
                     this._elementRef = mt
                 }
             }), "primary");
             let ke = (() => {
                     class mt extends St {
-                        constructor(ie, Te, nt, xt) {
-                            super(ie), this._changeDetectorRef = Te, this._animationMode = xt, this._tabs = new O.n_E, this._indexToSelect = 0, this._lastFocusedTabIndex = null, this._tabBodyWrapperHeight = 0, this._tabsSubscription = xe.w0.EMPTY, this._tabLabelSubscription = xe.w0.EMPTY, this._selectedIndex = null, this.headerPosition = "above", this.selectedIndexChange = new O.vpe, this.focusChange = new O.vpe, this.animationDone = new O.vpe, this.selectedTabChange = new O.vpe(!0), this._groupId = Fn++, this.animationDuration = nt && nt.animationDuration ? nt.animationDuration : "500ms", this.disablePagination = !(!nt || null == nt.disablePagination) && nt.disablePagination, this.dynamicHeight = !(!nt || null == nt.dynamicHeight) && nt.dynamicHeight, this.contentTabIndex = nt?.contentTabIndex ?? null
+                        constructor(ie, Se, nt, xt) {
+                            super(ie), this._changeDetectorRef = Se, this._animationMode = xt, this._tabs = new O.n_E, this._indexToSelect = 0, this._lastFocusedTabIndex = null, this._tabBodyWrapperHeight = 0, this._tabsSubscription = xe.w0.EMPTY, this._tabLabelSubscription = xe.w0.EMPTY, this._selectedIndex = null, this.headerPosition = "above", this.selectedIndexChange = new O.vpe, this.focusChange = new O.vpe, this.animationDone = new O.vpe, this.selectedTabChange = new O.vpe(!0), this._groupId = Fn++, this.animationDuration = nt && nt.animationDuration ? nt.animationDuration : "500ms", this.disablePagination = !(!nt || null == nt.disablePagination) && nt.disablePagination, this.dynamicHeight = !(!nt || null == nt.dynamicHeight) && nt.dynamicHeight, this.contentTabIndex = nt?.contentTabIndex ?? null
                         }
                         get dynamicHeight() {
                             return this._dynamicHeight
                         }
                         set dynamicHeight(ie) {
                             this._dynamicHeight = (0, J.Ig)(ie)
                         }
@@ -24104,75 +24109,75 @@
                         set contentTabIndex(ie) {
                             this._contentTabIndex = (0, J.su)(ie, null)
                         }
                         get backgroundColor() {
                             return this._backgroundColor
                         }
                         set backgroundColor(ie) {
-                            const Te = this._elementRef.nativeElement;
-                            Te.classList.remove(`mat-background-${this.backgroundColor}`), ie && Te.classList.add(`mat-background-${ie}`), this._backgroundColor = ie
+                            const Se = this._elementRef.nativeElement;
+                            Se.classList.remove(`mat-background-${this.backgroundColor}`), ie && Se.classList.add(`mat-background-${ie}`), this._backgroundColor = ie
                         }
                         ngAfterContentChecked() {
                             const ie = this._indexToSelect = this._clampTabIndex(this._indexToSelect);
                             if (this._selectedIndex != ie) {
-                                const Te = null == this._selectedIndex;
-                                if (!Te) {
+                                const Se = null == this._selectedIndex;
+                                if (!Se) {
                                     this.selectedTabChange.emit(this._createChangeEvent(ie));
                                     const nt = this._tabBodyWrapper.nativeElement;
                                     nt.style.minHeight = nt.clientHeight + "px"
                                 }
                                 Promise.resolve().then(() => {
-                                    this._tabs.forEach((nt, xt) => nt.isActive = xt === ie), Te || (this.selectedIndexChange.emit(ie), this._tabBodyWrapper.nativeElement.style.minHeight = "")
+                                    this._tabs.forEach((nt, xt) => nt.isActive = xt === ie), Se || (this.selectedIndexChange.emit(ie), this._tabBodyWrapper.nativeElement.style.minHeight = "")
                                 })
                             }
-                            this._tabs.forEach((Te, nt) => {
-                                Te.position = nt - ie, null != this._selectedIndex && 0 == Te.position && !Te.origin && (Te.origin = ie - this._selectedIndex)
+                            this._tabs.forEach((Se, nt) => {
+                                Se.position = nt - ie, null != this._selectedIndex && 0 == Se.position && !Se.origin && (Se.origin = ie - this._selectedIndex)
                             }), this._selectedIndex !== ie && (this._selectedIndex = ie, this._lastFocusedTabIndex = null, this._changeDetectorRef.markForCheck())
                         }
                         ngAfterContentInit() {
                             this._subscribeToAllTabChanges(), this._subscribeToTabLabels(), this._tabsSubscription = this._tabs.changes.subscribe(() => {
                                 const ie = this._clampTabIndex(this._indexToSelect);
                                 if (ie === this._selectedIndex) {
-                                    const Te = this._tabs.toArray();
+                                    const Se = this._tabs.toArray();
                                     let nt;
-                                    for (let xt = 0; xt < Te.length; xt++)
-                                        if (Te[xt].isActive) {
-                                            this._indexToSelect = this._selectedIndex = xt, this._lastFocusedTabIndex = null, nt = Te[xt];
+                                    for (let xt = 0; xt < Se.length; xt++)
+                                        if (Se[xt].isActive) {
+                                            this._indexToSelect = this._selectedIndex = xt, this._lastFocusedTabIndex = null, nt = Se[xt];
                                             break
-                                        }! nt && Te[ie] && Promise.resolve().then(() => {
-                                        Te[ie].isActive = !0, this.selectedTabChange.emit(this._createChangeEvent(ie))
+                                        }! nt && Se[ie] && Promise.resolve().then(() => {
+                                        Se[ie].isActive = !0, this.selectedTabChange.emit(this._createChangeEvent(ie))
                                     })
                                 }
                                 this._changeDetectorRef.markForCheck()
                             })
                         }
                         _subscribeToAllTabChanges() {
                             this._allTabs.changes.pipe((0, be.O)(this._allTabs)).subscribe(ie => {
-                                this._tabs.reset(ie.filter(Te => Te._closestTabGroup === this || !Te._closestTabGroup)), this._tabs.notifyOnChanges()
+                                this._tabs.reset(ie.filter(Se => Se._closestTabGroup === this || !Se._closestTabGroup)), this._tabs.notifyOnChanges()
                             })
                         }
                         ngOnDestroy() {
                             this._tabs.destroy(), this._tabsSubscription.unsubscribe(), this._tabLabelSubscription.unsubscribe()
                         }
                         realignInkBar() {
                             this._tabHeader && this._tabHeader._alignInkBarToSelectedTab()
                         }
                         updatePagination() {
                             this._tabHeader && this._tabHeader.updatePagination()
                         }
                         focusTab(ie) {
-                            const Te = this._tabHeader;
-                            Te && (Te.focusIndex = ie)
+                            const Se = this._tabHeader;
+                            Se && (Se.focusIndex = ie)
                         }
                         _focusChanged(ie) {
                             this._lastFocusedTabIndex = ie, this.focusChange.emit(this._createChangeEvent(ie))
                         }
                         _createChangeEvent(ie) {
-                            const Te = new Mn;
-                            return Te.index = ie, this._tabs && this._tabs.length && (Te.tab = this._tabs.toArray()[ie]), Te
+                            const Se = new Mn;
+                            return Se.index = ie, this._tabs && this._tabs.length && (Se.tab = this._tabs.toArray()[ie]), Se
                         }
                         _subscribeToTabLabels() {
                             this._tabLabelSubscription && this._tabLabelSubscription.unsubscribe(), this._tabLabelSubscription = (0, Ve.T)(...this._tabs.map(ie => ie._stateChanges)).subscribe(() => this._changeDetectorRef.markForCheck())
                         }
                         _clampTabIndex(ie) {
                             return Math.min(this._tabs.length - 1, Math.max(ie || 0, 0))
                         }
@@ -24180,29 +24185,29 @@
                             return `mat-tab-label-${this._groupId}-${ie}`
                         }
                         _getTabContentId(ie) {
                             return `mat-tab-content-${this._groupId}-${ie}`
                         }
                         _setTabBodyWrapperHeight(ie) {
                             if (!this._dynamicHeight || !this._tabBodyWrapperHeight) return;
-                            const Te = this._tabBodyWrapper.nativeElement;
-                            Te.style.height = this._tabBodyWrapperHeight + "px", this._tabBodyWrapper.nativeElement.offsetHeight && (Te.style.height = ie + "px")
+                            const Se = this._tabBodyWrapper.nativeElement;
+                            Se.style.height = this._tabBodyWrapperHeight + "px", this._tabBodyWrapper.nativeElement.offsetHeight && (Se.style.height = ie + "px")
                         }
                         _removeTabBodyWrapperHeight() {
                             const ie = this._tabBodyWrapper.nativeElement;
                             this._tabBodyWrapperHeight = ie.clientHeight, ie.style.height = "", this.animationDone.emit()
                         }
-                        _handleClick(ie, Te, nt) {
-                            ie.disabled || (this.selectedIndex = Te.focusIndex = nt)
+                        _handleClick(ie, Se, nt) {
+                            ie.disabled || (this.selectedIndex = Se.focusIndex = nt)
                         }
-                        _getTabIndex(ie, Te) {
-                            return ie.disabled ? null : Te === (this._lastFocusedTabIndex ?? this.selectedIndex) ? 0 : -1
+                        _getTabIndex(ie, Se) {
+                            return ie.disabled ? null : Se === (this._lastFocusedTabIndex ?? this.selectedIndex) ? 0 : -1
                         }
-                        _tabFocusChanged(ie, Te) {
-                            ie && "mouse" !== ie && "touch" !== ie && (this._tabHeader.focusIndex = Te)
+                        _tabFocusChanged(ie, Se) {
+                            ie && "mouse" !== ie && "touch" !== ie && (this._tabHeader.focusIndex = Se)
                         }
                     }
                     return mt.\u0275fac = function(ie) {
                         return new(ie || mt)(O.Y36(O.SBq), O.Y36(O.sBO), O.Y36(Tt, 8), O.Y36(O.QbO, 8))
                     }, mt.\u0275dir = O.lG2({
                         type: mt,
                         inputs: {
@@ -24221,41 +24226,41 @@
                             selectedTabChange: "selectedTabChange"
                         },
                         features: [O.qOj]
                     }), mt
                 })(),
                 Pe = (() => {
                     class mt extends ke {
-                        constructor(ie, Te, nt, xt) {
-                            super(ie, Te, nt, xt)
+                        constructor(ie, Se, nt, xt) {
+                            super(ie, Se, nt, xt)
                         }
                     }
                     return mt.\u0275fac = function(ie) {
                         return new(ie || mt)(O.Y36(O.SBq), O.Y36(O.sBO), O.Y36(Tt, 8), O.Y36(O.QbO, 8))
                     }, mt.\u0275cmp = O.Xpm({
                         type: mt,
                         selectors: [
                             ["mat-tab-group"]
                         ],
-                        contentQueries: function(ie, Te, nt) {
+                        contentQueries: function(ie, Se, nt) {
                             if (1 & ie && O.Suo(nt, Re, 5), 2 & ie) {
                                 let xt;
-                                O.iGM(xt = O.CRH()) && (Te._allTabs = xt)
+                                O.iGM(xt = O.CRH()) && (Se._allTabs = xt)
                             }
                         },
-                        viewQuery: function(ie, Te) {
+                        viewQuery: function(ie, Se) {
                             if (1 & ie && (O.Gf(Ke, 5), O.Gf(it, 5)), 2 & ie) {
                                 let nt;
-                                O.iGM(nt = O.CRH()) && (Te._tabBodyWrapper = nt.first), O.iGM(nt = O.CRH()) && (Te._tabHeader = nt.first)
+                                O.iGM(nt = O.CRH()) && (Se._tabBodyWrapper = nt.first), O.iGM(nt = O.CRH()) && (Se._tabHeader = nt.first)
                             }
                         },
                         hostAttrs: [1, "mat-tab-group"],
                         hostVars: 4,
-                        hostBindings: function(ie, Te) {
-                            2 & ie && O.ekj("mat-tab-group-dynamic-height", Te.dynamicHeight)("mat-tab-group-inverted-header", "below" === Te.headerPosition)
+                        hostBindings: function(ie, Se) {
+                            2 & ie && O.ekj("mat-tab-group-dynamic-height", Se.dynamicHeight)("mat-tab-group-inverted-header", "below" === Se.headerPosition)
                         },
                         inputs: {
                             color: "color",
                             disableRipple: "disableRipple"
                         },
                         exportAs: ["matTabGroup"],
                         features: [O._Bn([{
@@ -24274,20 +24279,20 @@
                             ["role", "tab", "matTabLabelWrapper", "", "mat-ripple", "", "cdkMonitorElementFocus", "", 1, "mat-tab-label", "mat-focus-indicator", 3, "id", "ngClass", "disabled", "matRippleDisabled", "click", "cdkFocusChange"],
                             [1, "mat-tab-label-content"],
                             [3, "ngIf", "ngIfElse"],
                             ["tabTextLabel", ""],
                             [3, "cdkPortalOutlet"],
                             ["role", "tabpanel", 3, "id", "ngClass", "content", "position", "origin", "animationDuration", "_onCentered", "_onCentering"]
                         ],
-                        template: function(ie, Te) {
+                        template: function(ie, Se) {
                             1 & ie && (O.TgZ(0, "mat-tab-header", 0, 1), O.NdJ("indexFocused", function(xt) {
-                                return Te._focusChanged(xt)
+                                return Se._focusChanged(xt)
                             })("selectFocusedIndex", function(xt) {
-                                return Te.selectedIndex = xt
-                            }), O.YNc(2, se, 5, 15, "div", 2), O.qZA(), O.TgZ(3, "div", 3, 4), O.YNc(5, ve, 1, 10, "mat-tab-body", 5), O.qZA()), 2 & ie && (O.Q6J("selectedIndex", Te.selectedIndex || 0)("disableRipple", Te.disableRipple)("disablePagination", Te.disablePagination), O.xp6(2), O.Q6J("ngForOf", Te._tabs), O.xp6(1), O.ekj("_mat-animation-noopable", "NoopAnimations" === Te._animationMode), O.xp6(2), O.Q6J("ngForOf", Te._tabs))
+                                return Se.selectedIndex = xt
+                            }), O.YNc(2, se, 5, 15, "div", 2), O.qZA(), O.TgZ(3, "div", 3, 4), O.YNc(5, ve, 1, 10, "mat-tab-body", 5), O.qZA()), 2 & ie && (O.Q6J("selectedIndex", Se.selectedIndex || 0)("disableRipple", Se.disableRipple)("disablePagination", Se.disablePagination), O.xp6(2), O.Q6J("ngForOf", Se._tabs), O.xp6(1), O.ekj("_mat-animation-noopable", "NoopAnimations" === Se._animationMode), O.xp6(2), O.Q6J("ngForOf", Se._tabs))
                         },
                         dependencies: [Mt, Ze, F.sg, de, De.wG, s.kH, F.mk, F.O5, C.Pl],
                         styles: [".mat-tab-group{display:flex;flex-direction:column;max-width:100%}.mat-tab-group.mat-tab-group-inverted-header{flex-direction:column-reverse}.mat-tab-label{height:48px;padding:0 24px;cursor:pointer;box-sizing:border-box;opacity:.6;min-width:160px;text-align:center;display:inline-flex;justify-content:center;align-items:center;white-space:nowrap;position:relative}.mat-tab-label:focus{outline:none}.mat-tab-label:focus:not(.mat-tab-disabled){opacity:1}.cdk-high-contrast-active .mat-tab-label:focus{outline:dotted 2px;outline-offset:-2px}.mat-tab-label.mat-tab-disabled{cursor:default}.cdk-high-contrast-active .mat-tab-label.mat-tab-disabled{opacity:.5}.mat-tab-label .mat-tab-label-content{display:inline-flex;justify-content:center;align-items:center;white-space:nowrap}.cdk-high-contrast-active .mat-tab-label{opacity:1}@media(max-width: 599px){.mat-tab-label{padding:0 12px}}@media(max-width: 959px){.mat-tab-label{padding:0 12px}}.mat-tab-group[mat-stretch-tabs]>.mat-tab-header .mat-tab-label{flex-basis:0;flex-grow:1}.mat-tab-body-wrapper{position:relative;overflow:hidden;display:flex;transition:height 500ms cubic-bezier(0.35, 0, 0.25, 1)}._mat-animation-noopable.mat-tab-body-wrapper{transition:none;animation:none}.mat-tab-body{top:0;left:0;right:0;bottom:0;position:absolute;display:block;overflow:hidden;outline:0;flex-basis:100%}.mat-tab-body.mat-tab-body-active{position:relative;overflow-x:hidden;overflow-y:auto;z-index:1;flex-grow:1}.mat-tab-group.mat-tab-group-dynamic-height .mat-tab-body.mat-tab-body-active{overflow-y:hidden}\n"],
                         encapsulation: 2
                     }), mt
                 })(),
                 Zt = (() => {
@@ -24369,15 +24374,15 @@
                 }
                 getCookie(we) {
                     return (0, s.Mx)(document.cookie, we)
                 }
             }
             let L, O = null;
             const Me = new S.OlP("TRANSITION_ID"),
-                Oe = [{
+                Te = [{
                     provide: S.ip1,
                     useFactory: function fe(Ce, we, oe) {
                         return () => {
                             oe.get(S.CZH).donePromise.then(() => {
                                 const Qe = (0, s.q)(),
                                     Ct = we.querySelectorAll(`style[ng-transition="${Ce}"]`);
                                 for (let zt = 0; zt < Ct.length; zt++) Qe.remove(Ct[zt])
@@ -24883,15 +24888,15 @@
                                 ngModule: Ce,
                                 providers: [{
                                     provide: S.AFp,
                                     useValue: oe.appId
                                 }, {
                                     provide: Me,
                                     useExisting: S.AFp
-                                }, Oe]
+                                }, Te]
                             }
                         }
                     }
                     return Ce.\u0275fac = function(oe) {
                         return new(oe || Ce)(S.LFG(G, 12))
                     }, Ce.\u0275mod = S.oAB({
                         type: Ce
@@ -25011,15 +25016,15 @@
             const De = (0, v(3888).d)(m => function() {
                 m(this), this.name = "EmptyError", this.message = "no elements in sequence"
             });
             var L = v(9841),
                 be = v(7272),
                 Me = v(9770),
                 fe = v(9635),
-                Oe = v(2843),
+                Te = v(2843),
                 ye = v(9751),
                 g = v(515),
                 xe = v(727),
                 pe = v(4482),
                 Ge = v(5403);
 
             function Ve() {
@@ -25395,15 +25400,15 @@
             }
 
             function Pt(m) {
                 return mt(m.replace(/\+/g, "%20"))
             }
 
             function ie(m) {
-                return `${Zt(m.path)}${function Te(m){return Object.keys(m).map(_=>`;${Zt(_)}=${Zt(m[_])}`).join("")}(m.parameters)}`
+                return `${Zt(m.path)}${function Se(m){return Object.keys(m).map(_=>`;${Zt(_)}=${Zt(m[_])}`).join("")}(m.parameters)}`
             }
             const xt = /^[^\/()?;=#]+/;
 
             function kn(m) {
                 const _ = m.match(xt);
                 return _ ? _[0] : ""
             }
@@ -26581,19 +26586,19 @@
             class us {
                 constructor(_) {
                     this.urlTree = _
                 }
             }
 
             function ko(m) {
-                return (0, Oe._)(new ni(m))
+                return (0, Te._)(new ni(m))
             }
 
             function Os(m) {
-                return (0, Oe._)(new us(m))
+                return (0, Te._)(new us(m))
             }
             class p {
                 constructor(_, f, M, A, W) {
                     this.injector = _, this.configLoader = f, this.urlSerializer = M, this.urlTree = A, this.config = W, this.allowRedirects = !0
                 }
                 apply() {
                     const _ = jr(this.urlTree.root, [], [], this.config).segmentGroup,
@@ -26701,26 +26706,26 @@
                                 return m && vi(m.canLoad)
                             }(Ae) ? Ae.canLoad(_, f) : m.runInContext(() => Ae(_, f)))
                         });
                         return (0, C.of)(W).pipe(Yi(), go())
                     }(_, f, M).pipe((0, ze.z)(A => A ? this.configLoader.loadChildren(_, f).pipe((0, dn.b)(W => {
                         f._loadedRoutes = W.routes, f._loadedInjector = W.injector
                     })) : function B(m) {
-                        return (0, Oe._)(Oi(dr, 3))
+                        return (0, Te._)(Oi(dr, 3))
                     }())) : (0, C.of)({
                         routes: [],
                         injector: _
                     })
                 }
                 lineralizeSegments(_, f) {
                     let M = [],
                         A = f.root;
                     for (;;) {
                         if (M = M.concat(A.segments), 0 === A.numberOfChildren) return (0, C.of)(M);
-                        if (A.numberOfChildren > 1 || !A.children[z]) return (0, Oe._)(new s.vHH(4e3, dr));
+                        if (A.numberOfChildren > 1 || !A.children[z]) return (0, Te._)(new s.vHH(4e3, dr));
                         A = A.children[z]
                     }
                 }
                 applyRedirectCommands(_, f, M) {
                     return this.applyRedirectCreateUrlTree(f, this.urlSerializer.parse(f), _, M)
                 }
                 applyRedirectCreateUrlTree(_, f, M, A) {
@@ -27160,15 +27165,15 @@
                                         urlAfterRedirects: W
                                     }))))
                                 }(this.ngModule.injector, this.configLoader, this.urlSerializer, this.config), (0, dn.b)(cn => {
                                     this.currentNavigation = {
                                         ...this.currentNavigation,
                                         finalUrl: cn.urlAfterRedirects
                                     }, A.urlAfterRedirects = cn.urlAfterRedirects
-                                }), function Se(m, _, f, M, A, W) {
+                                }), function Oe(m, _, f, M, A, W) {
                                     return (0, ze.z)(me => function Le(m, _, f, M, A, W, me = "emptyOnly", Ae = "legacy") {
                                         return new at(m, _, f, M, A, me, Ae, W).recognize().pipe((0, te.w)(Dt => null === Dt ? function Fe(m) {
                                             return new ye.y(_ => _.error(m))
                                         }(new q) : (0, C.of)(Dt)))
                                     }(m, _, f, me.urlAfterRedirects, M.serialize(me.urlAfterRedirects), M, A, W).pipe((0, ae.U)(Ae => ({
                                         ...me,
                                         targetSnapshot: Ae
@@ -27313,15 +27318,15 @@
                                                         const W = {};
                                                         return (0, S.D)(A).pipe((0, ze.z)(me => function Ln(m, _, f, M) {
                                                             const A = Kr(_) ?? M,
                                                                 W = Zr(m, A);
                                                             return j(W.resolve ? W.resolve(_, f) : A.runInContext(() => W(_, f)))
                                                         }(m[me], _, f, M).pipe(Lt(), (0, dn.b)(Ae => {
                                                             W[me] = Ae
-                                                        }))), Ke(1), (0, et.h)(W), (0, wn.K)(me => Or(me) ? g.E : (0, Oe._)(me)))
+                                                        }))), Ke(1), (0, et.h)(W), (0, wn.K)(me => Or(me) ? g.E : (0, Te._)(me)))
                                                     }(W, m, _, M).pipe((0, ae.U)(me => (m._resolvedData = me, m.data = oo(m, f).resolve, A && Gn(A) && (m.data[ee] = A.title), null)))
                                             }(me.route, M, m, _)), (0, dn.b)(() => W++), Ke(1), (0, ze.z)(me => W === A.length ? (0, C.of)(f) : g.E))
                                         })
                                     }(this.paramsInheritanceStrategy, this.ngModule.injector), (0, dn.b)({
                                         next: () => Yt = !0,
                                         complete: () => {
                                             Yt || (this.restoreHistory(Dt), this.cancelNavigationTransition(Dt, "", 2))
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/runtime.5064f1f60b88aea4.js` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/runtime.0cd10aef5e6b1db8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -30,15 +30,15 @@
     }, r.d = (e, i) => {
         for (var t in i) r.o(i, t) && !r.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: i[t]
         })
     }, r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce((i, t) => (r.f[t](e, i), i), [])), r.u = e => e + "." + {
         398: "70c7e628915a6c39",
-        953: "eb8714051ee666a2"
+        953: "94c6a01c085d9731"
     } [e] + ".js", r.miniCssF = e => {}, r.o = (e, i) => Object.prototype.hasOwnProperty.call(e, i), (() => {
         var e = {},
             i = "mlflow-oidc-auth-front:";
         r.l = (t, o, f, n) => {
             if (e[t]) e[t].push(o);
             else {
                 var a, c;
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css`

 * *Files identical despite different names*

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth/views.py` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     BAD_REQUEST,
     ErrorCode,
     INVALID_PARAMETER_VALUE,
     RESOURCE_DOES_NOT_EXIST,
 )
 from mlflow.protos.service_pb2 import (
     CreateExperiment,
+    SearchExperiments,
 )
 from mlflow_oidc_auth.permissions import Permission, get_permission
 from mlflow.server.handlers import (
     catch_mlflow_exception,
     get_endpoints,
 )
 
@@ -43,26 +44,27 @@
 
 # from mlflow_oidc_auth.client import AuthServiceClient
 from mlflow_oidc_auth.config import AppConfig
 from mlflow_oidc_auth.sqlalchemy_store import SqlAlchemyStore
 
 # Create the OAuth2 client
 auth_client = WebApplicationClient(AppConfig.get_property("OIDC_CLIENT_ID"))
-mlflow_client = MlflowClient()
+mlflow_client = MlflowClient(tracking_uri=AppConfig.get_property("MLFLOW_TRACKING_URI"))
 store = SqlAlchemyStore()
 store.init_db((AppConfig.get_property("OIDC_USERS_DB_URI")))
 _logger = logging.getLogger(__name__)
 
 
 def _get_experiment_id(request_data: dict) -> str:
     experiment_id = request_data.get("experiment_id")
     if "experiment_id" not in request_data:
         experiment_id = mlflow_client.get_experiment_by_name(request_data.get("experiment_name")).experiment_id
     return experiment_id
 
+
 def _get_request_param(param: str) -> str:
     if request.method == "GET":
         args = request.args
     elif request.method in ("POST", "PATCH", "DELETE"):
         args = request.json
     else:
         raise MlflowException(
@@ -79,15 +81,22 @@
             "See the API docs for more information about request parameters.",
             INVALID_PARAMETER_VALUE,
         )
     return args[param]
 
 
 def _is_unprotected_route(path: str) -> bool:
-    return path.startswith(("/static", "/favicon.ico", "/health", "/login", "/callback", "/oidc/static", "/oidc/ui"))
+    return path.startswith(
+        (
+            "/health",
+            "/login",
+            "/callback",
+            "/oidc/static",
+        )
+    )
 
 
 def _get_permission_from_store_or_default(store_permission_func: Callable[[], str]) -> Permission:
     """
     Attempts to get permission from store,
     and returns default permission if no record is found.
     """
@@ -101,14 +110,22 @@
     return get_permission(perm)
 
 
 def authenticate_request_basic_auth() -> Union[Authorization, Response]:
     username = request.authorization.username
     password = request.authorization.password
     _logger.debug("Authenticating user %s", username)
+    # check for internal call, if credentials are correct, return True
+    if username == AppConfig.get_property("MLFLOW_TRACKING_USERNAME") and password == AppConfig.get_property(
+        "MLFLOW_TRACKING_PASSWORD"
+    ):
+        _set_username(username)
+        _set_is_admin(True)
+        _logger.debug("User %s authenticated", username)
+        return True
     if store.authenticate_user(username, password):
         _set_username(username)
         _logger.debug("User %s authenticated", username)
         return True
     else:
         _logger.debug("User %s not authenticated", username)
         # let user attempt login again
@@ -228,17 +245,17 @@
     experiment_id = _get_request_param("experiment_id")
     username = _get_username()
     ep = store.get_experiment_permission(experiment_id, username)
     return make_response({"experiment_permission": ep.to_json()})
 
 
 # TODO
-@catch_mlflow_exception
-def search_experiment():
-    return render_template("home.html", username=_get_username())
+# @catch_mlflow_exception
+# def search_experiment():
+#     return render_template("home.html", username=_get_username())
 
 
 def login():
     state = secrets.token_urlsafe(16)
     session["oauth_state"] = state
     # Generate the authorization request URL with the state parameter
     authorization_url = auth_client.prepare_request_uri(
@@ -334,17 +351,17 @@
     if not filename:
         filename = "index.html"
     elif not os.path.exists(os.path.join(ui_directory, filename)):
         filename = "index.html"
     return send_from_directory(ui_directory, filename)
 
 
-# TODO
-def search_model():
-    return render_template("home.html", username=_get_username())
+# # TODO
+# def search_model():
+#     return render_template("home.html", username=_get_username())
 
 
 def create_user():
     try:
         user = store.get_user(_get_username())
         return (
             jsonify({"message": f"User {user.username} (ID: {user.id}) already exists"}),
@@ -401,18 +418,14 @@
 @catch_mlflow_exception
 def get_user():
     username = _get_request_param("username")
     user = store.get_user(username)
     return jsonify({"user": user.to_json()})
 
 
-def oidc_home():
-    return render_template("home.html", username=_get_username())
-
-
 def permissions():
     return redirect(url_for("list_users"))
 
 
 def get_users():
     # check is admin
     # if not _get_is_admin():
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/PKG-INFO` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.1.0
+Version: 1.1.1
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -253,14 +253,17 @@
 | OIDC_AUTHORIZATION_URL | OIDC Auth URL (if discovery URL is not defined) |
 | OIDC_TOKEN_URL         | OIDC Token URL (if discovery URL is not defined) |
 | OIDC_USER_URL          | OIDC User info URL (if discovery URL is not defined) |
 | SECRET_KEY             | Key to perform cookie encryption |
 | OAUTHLIB_INSECURE_TRANSPORT | Development only. Allow to use insecure endpoints for OIDC |
 | LOG_LEVEL                   | Application log level |
 | OIDC_USERS_DB_URI | Database connection string |
+| MLFLOW_TRACKING_USERNAME | Credentials for internal communications via API |
+| MLFLOW_TRACKING_PASSWORD | Credentials for internal communications via API |
+| MLFLOW_TRACKING_URI | URI for internal communications via API |
 
 # Configuration examples
 
 ## Okta
 
 ```bash
 OIDC_DISCOVERY_URL = 'https://<your_domain>.okta.com/.well-known/openid-configuration'
@@ -285,22 +288,27 @@
 OIDC_GROUP_NAME = "mlflow_users_group_name"
 OIDC_ADMIN_GROUP_NAME = "mlflow_admins_group_name"
 ```
 
 > please note, that for getting group membership information, the application should have "GroupMember.Read.All" permission
 
 # Development
+
+Preconditions:
+
+The following tools should be installed for local development:
+
+* git
+* nodejs
+* python
+
 ```shell
 git clone https://github.com/data-platform-hq/mlflow-oidc-auth
 cd mlflow-oidc-auth
-python3 -m venv venv
-source venv/bin/activate
-pip install --editable .
-mlflow server --dev --app-name oidc-auth --host 0.0.0.0 --port 8080
+./scripts/run-dev-server.sh
 ```
 
-
 # License
 Apache 2 Licensed. For more information please see [LICENSE](./LICENSE)
 
 ### Based on MLFlow basic-auth plugin
 https://github.com/mlflow/mlflow/tree/master/mlflow/server/auth
```

### Comparing `mlflow-oidc-auth-1.1.0/mlflow_oidc_auth.egg-info/SOURCES.txt` & `mlflow-oidc-auth-1.1.1/mlflow_oidc_auth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,14 @@
 mlflow_oidc_auth/static/style.css
 mlflow_oidc_auth/templates/_footer.html
 mlflow_oidc_auth/templates/_head.html
 mlflow_oidc_auth/templates/_header.html
 mlflow_oidc_auth/templates/auth.html
 mlflow_oidc_auth/ui/398.70c7e628915a6c39.js
 mlflow_oidc_auth/ui/3rdpartylicenses.txt
-mlflow_oidc_auth/ui/953.eb8714051ee666a2.js
+mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
 mlflow_oidc_auth/ui/favicon.ico
 mlflow_oidc_auth/ui/index.html
-mlflow_oidc_auth/ui/main.ff1acef2e224ca42.js
+mlflow_oidc_auth/ui/main.84383ebc03062e87.js
 mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
-mlflow_oidc_auth/ui/runtime.5064f1f60b88aea4.js
+mlflow_oidc_auth/ui/runtime.0cd10aef5e6b1db8.js
 mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
```

### Comparing `mlflow-oidc-auth-1.1.0/pyproject.toml` & `mlflow-oidc-auth-1.1.1/pyproject.toml`

 * *Files identical despite different names*

