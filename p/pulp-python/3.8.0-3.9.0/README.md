# Comparing `tmp/pulp-python-3.8.0.tar.gz` & `tmp/pulp-python-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-python-3.8.0.tar", last modified: Mon Dec 19 18:31:27 2022, max compression
+gzip compressed data, was "pulp-python-3.9.0.tar", last modified: Fri Mar 17 19:08:53 2023, max compression
```

## Comparing `pulp-python-3.8.0.tar` & `pulp-python-3.9.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.699937 pulp-python-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2022-12-19 18:31:26.000000 pulp-python-3.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2022-12-19 18:31:13.000000 pulp-python-3.8.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (123)      540 2022-12-19 18:31:13.000000 pulp-python-3.8.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2022-12-19 18:31:13.000000 pulp-python-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-19 18:31:13.000000 pulp-python-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-19 18:31:27.699937 pulp-python-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2022-12-19 18:31:13.000000 pulp-python-3.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-19 18:31:13.000000 pulp-python-3.8.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.687937 pulp-python-3.8.0/pulp_python/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.691937 pulp-python-3.8.0/pulp_python/app/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-19 18:31:26.000000 pulp-python-3.8.0/pulp_python/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.691937 pulp-python-3.8.0/pulp_python/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0002_pythonpackagecontent_python_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0003_new_sync_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0004_DATA_swap_distribution_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0005_pythonpackagecontent_sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0006_pythonrepository_autopublish.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0007_pythonpackagecontent_mv-2-1.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0008_pythonpackagecontent_unique_sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0009_pythondistribution_allow_uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/0010_update_json_field.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.691937 pulp-python-3.8.0/pulp_python/app/pypi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/pypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/pypi/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/pypi/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    14879 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.691937 pulp-python-3.8.0/pulp_python/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/tasks/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/tasks/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/tasks/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.695937 pulp-python-3.8.0/pulp_python/app/webserver_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/webserver_snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/webserver_snippets/apache.conf
--rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/app/webserver_snippets/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.695937 pulp-python-3.8.0/pulp_python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.695937 pulp-python-3.8.0/pulp_python/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.695937 pulp-python-3.8.0/pulp_python/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_auto_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_consume_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_crud_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_full_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_pypi_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    22745 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14366 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.699937 pulp-python-3.8.0/pulp_python/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.699937 pulp-python-3.8.0/pulp_python/tests/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.699937 pulp-python-3.8.0/pulp_python/tests/upgrade/post/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/upgrade/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/upgrade/post/test_publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.699937 pulp-python-3.8.0/pulp_python/tests/upgrade/pre/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/upgrade/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pulp_python/tests/upgrade/pre/test_publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 18:31:27.691937 pulp-python-3.8.0/pulp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-19 18:31:27.000000 pulp-python-3.8.0/pulp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2022-12-19 18:31:27.000000 pulp-python-3.8.0/pulp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 18:31:27.000000 pulp-python-3.8.0/pulp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-19 18:31:27.000000 pulp-python-3.8.0/pulp_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-19 18:31:27.000000 pulp-python-3.8.0/pulp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-19 18:31:27.000000 pulp-python-3.8.0/pulp_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-19 18:31:13.000000 pulp-python-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-19 18:31:13.000000 pulp-python-3.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 18:31:27.699937 pulp-python-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-19 18:31:26.000000 pulp-python-3.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-19 18:31:13.000000 pulp-python-3.8.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-19 18:31:13.000000 pulp-python-3.8.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-03-17 19:08:51.000000 pulp-python-3.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-17 19:08:42.000000 pulp-python-3.9.0/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-17 19:08:42.000000 pulp-python-3.9.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-03-17 19:08:42.000000 pulp-python-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-17 19:08:42.000000 pulp-python-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-17 19:08:53.397604 pulp-python-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-17 19:08:42.000000 pulp-python-3.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-17 19:08:42.000000 pulp-python-3.9.0/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.385604 pulp-python-3.9.0/pulp_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.389604 pulp-python-3.9.0/pulp_python/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-17 19:08:52.000000 pulp-python-3.9.0/pulp_python/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.393604 pulp-python-3.9.0/pulp_python/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0002_pythonpackagecontent_python_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0003_new_sync_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0004_DATA_swap_distribution_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0005_pythonpackagecontent_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0006_pythonrepository_autopublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0007_pythonpackagecontent_mv-2-1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0008_pythonpackagecontent_unique_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0009_pythondistribution_allow_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/0010_update_json_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.393604 pulp-python-3.9.0/pulp_python/app/pypi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/pypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/pypi/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/pypi/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/tasks/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/tasks/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/tasks/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/app/webserver_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/webserver_snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/webserver_snippets/apache.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/app/webserver_snippets/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_auto_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_consume_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_crud_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_full_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_pypi_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24098 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/upgrade/post/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/upgrade/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/upgrade/post/test_publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.397604 pulp-python-3.9.0/pulp_python/tests/upgrade/pre/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/upgrade/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pulp_python/tests/upgrade/pre/test_publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:08:53.389604 pulp-python-3.9.0/pulp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-17 19:08:53.000000 pulp-python-3.9.0/pulp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-17 19:08:53.000000 pulp-python-3.9.0/pulp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:08:53.000000 pulp-python-3.9.0/pulp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-17 19:08:53.000000 pulp-python-3.9.0/pulp_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-17 19:08:53.000000 pulp-python-3.9.0/pulp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 19:08:53.000000 pulp-python-3.9.0/pulp_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-17 19:08:42.000000 pulp-python-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-17 19:08:42.000000 pulp-python-3.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:08:53.397604 pulp-python-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-17 19:08:52.000000 pulp-python-3.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-17 19:08:42.000000 pulp-python-3.9.0/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 19:08:42.000000 pulp-python-3.9.0/unittest_requirements.txt
```

### Comparing `pulp-python-3.8.0/CHANGES.rst` & `pulp-python-3.9.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,43 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+3.9.0 (2023-03-17)
+==================
+
+
+Features
+--------
+
+- Added version filter to package list endpoint.
+  `#577 <https://github.com/pulp/pulp_python/issues/577>`__
+- Allow duplicate uploads to return existing packages instead of erring.
+  `#590 <https://github.com/pulp/pulp_python/issues/590>`__
+
+
+Bugfixes
+--------
+
+- Fixed pull-through caching ignoring remote proxy settings.
+  `#553 <https://github.com/pulp/pulp_python/issues/553>`__
+- Changed includes and excludes openapi schema to report as array of strings instead of object.
+  `#576 <https://github.com/pulp/pulp_python/issues/576>`__
+- Fixed syncing ignoring remote proxy.
+  `#581 <https://github.com/pulp/pulp_python/issues/581>`__
+- Fixed duplicate operationID for generated PyPI simple endpoints schema.
+  `#594 <https://github.com/pulp/pulp_python/issues/594>`__
+
+
+----
+
+
 3.8.0 (2022-12-19)
 ==================
 
 
 Bugfixes
 --------
```

### Comparing `pulp-python-3.8.0/COMMITMENT` & `pulp-python-3.9.0/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/COPYRIGHT` & `pulp-python-3.9.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/LICENSE` & `pulp-python-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/PKG-INFO` & `pulp-python-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-python
-Version: 3.8.0
+Version: 3.9.0
 Summary: pulp-python plugin for the Pulp Project
 Home-page: https://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: # pulp_python
```

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0001_initial.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0003_new_sync_filters.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0003_new_sync_filters.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0004_DATA_swap_distribution_model.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0004_DATA_swap_distribution_model.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0005_pythonpackagecontent_sha256.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0005_pythonpackagecontent_sha256.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0007_pythonpackagecontent_mv-2-1.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0007_pythonpackagecontent_mv-2-1.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0008_pythonpackagecontent_unique_sha256.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0008_pythonpackagecontent_unique_sha256.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/migrations/0010_update_json_field.py` & `pulp-python-3.9.0/pulp_python/app/migrations/0010_update_json_field.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/models.py` & `pulp-python-3.9.0/pulp_python/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/pypi/serializers.py` & `pulp-python-3.9.0/pulp_python/app/pypi/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/pypi/views.py` & `pulp-python-3.9.0/pulp_python/app/pypi/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,20 +197,28 @@
             digest, _, value = parsed.fragment.partition('=')
             stripped_url = urlunsplit(chain(parsed[:3], ("", "")))
             redirect = f'{path}/{link.text}?redirect={stripped_url}'
             d_url = urljoin(BASE_CONTENT_URL, redirect)
             return link.text, d_url, value if digest == 'sha256' else ''
 
         url = remote.get_remote_artifact_url(f'simple/{package}/')
-        response = requests.get(url, stream=True)
+        kwargs = {}
+        if proxy_url := remote.proxy_url:
+            if remote.proxy_username or remote.proxy_password:
+                parsed_proxy = urlparse(proxy_url)
+                netloc = f"{remote.proxy_username}:{remote.proxy_password}@{parsed_proxy.netloc}"
+                proxy_url = urlunsplit((parsed_proxy.scheme, netloc, "", "", ""))
+            kwargs["proxies"] = {"http": proxy_url, "https": proxy_url}
+
+        response = requests.get(url, stream=True, **kwargs)
         links = parse_links_stream_response(response)
         packages = (parse_url(link) for link in links)
         return StreamingHttpResponse(write_simple_detail(package, packages, streamed=True))
 
-    @extend_schema(summary="Get package simple page")
+    @extend_schema(operation_id="pypi_simple_package_read", summary="Get package simple page")
     def retrieve(self, request, path, package):
         """Retrieves the simple api html page for a package."""
         distro, repo_ver, content = self.get_drvc(path)
         # Should I redirect if the normalized name is different?
         normalized = canonicalize_name(package)
         if distro.remote:
             if not repo_ver or not content.filter(name__normalize=normalized).exists():
```

### Comparing `pulp-python-3.8.0/pulp_python/app/serializers.py` & `pulp-python-3.9.0/pulp_python/app/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,28 +222,29 @@
 
         if data.get("sha256") and data["sha256"] != artifact.sha256:
             raise serializers.ValidationError(
                 detail={"sha256": _(
                     "The uploaded artifact's sha256 checksum does not match the one provided"
                 )}
             )
-        sha256 = artifact.sha256
-        if sha256 and python_models.PythonPackageContent.objects.filter(sha256=sha256).exists():
-            raise serializers.ValidationError(detail={"sha256": _('This field must be unique')})
 
         _data = parse_project_metadata(vars(metadata))
         _data['packagetype'] = metadata.packagetype
         _data['version'] = metadata.version
         _data['filename'] = filename
-        _data['sha256'] = sha256
+        _data['sha256'] = artifact.sha256
 
         data.update(_data)
 
         return data
 
+    def retrieve(self, validated_data):
+        content = python_models.PythonPackageContent.objects.filter(sha256=validated_data["sha256"])
+        return content.first()
+
     class Meta:
         fields = core_serializers.SingleArtifactContentUploadSerializer.Meta.fields + (
             'filename', 'packagetype', 'name', 'version', 'sha256', 'metadata_version', 'summary',
             'description', 'description_content_type', 'keywords', 'home_page', 'download_url',
             'author', 'author_email', 'maintainer', 'maintainer_email', 'license',
             'requires_python', 'project_url', 'project_urls', 'platform', 'supported_platform',
             'requires_dist', 'provides_dist', 'obsoletes_dist', 'requires_external', 'classifiers'
@@ -274,28 +275,29 @@
 
 
 class PythonRemoteSerializer(core_serializers.RemoteSerializer):
     """
     A Serializer for PythonRemote.
     """
 
-    includes = serializers.JSONField(
+    includes = serializers.ListField(
+        child=serializers.CharField(allow_blank=False),
         required=False,
-        default=list,
+        allow_empty=True,
         help_text=_(
-            "A JSON list containing project specifiers for Python packages to include."
+            "A list containing project specifiers for Python packages to include."
         ),
     )
-    excludes = serializers.JSONField(
+    excludes = serializers.ListField(
+        child=serializers.CharField(allow_blank=False),
         required=False,
-        default=list,
+        allow_empty=True,
         help_text=_(
-            "A JSON list containing project specifiers for Python packages to exclude."
+            "A list containing project specifiers for Python packages to exclude."
         ),
-
     )
     prereleases = serializers.BooleanField(
         required=False,
         help_text=_('Whether or not to include pre-release packages in the sync.')
     )
     policy = serializers.ChoiceField(
         help_text=_("The policy to use when downloading content. The possible values include: "
```

### Comparing `pulp-python-3.8.0/pulp_python/app/tasks/publish.py` & `pulp-python-3.9.0/pulp_python/app/tasks/publish.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/tasks/sync.py` & `pulp-python-3.9.0/pulp_python/app/tasks/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from aiohttp import ClientResponseError, ClientError
 from lxml.etree import LxmlError
 from gettext import gettext as _
-from os import environ
+from os import environ, path
 
 from rest_framework import serializers
 
 from pulpcore.plugin.models import Artifact, ProgressReport, Remote, Repository
 from pulpcore.plugin.stages import (
     DeclarativeArtifact,
     DeclarativeContent,
@@ -22,15 +22,15 @@
 from pulp_python.app.utils import parse_metadata, PYPI_LAST_SERIAL
 from pypi_simple import parse_repo_index_page
 
 from bandersnatch.mirror import Mirror
 from bandersnatch.master import Master
 from bandersnatch.configuration import BandersnatchConfig
 from packaging.requirements import Requirement
-from urllib.parse import urljoin
+from urllib.parse import urljoin, urlsplit, urlunsplit
 
 logger = logging.getLogger(__name__)
 
 
 def sync(remote_pk, repository_pk, mirror):
     """
     Sync content from the remote repository.
@@ -107,22 +107,30 @@
         self.remote = remote
         create_bandersnatch_config(remote)
 
     async def run(self):
         """
         If includes is specified, then only sync those,else try to sync all other packages
         """
+        # Prevent bandersnatch from reading actual .netrc file, set to nonexistent file
+        # See discussion on https://github.com/pulp/pulp_python/issues/581
+        environ["NETRC"] = f"{path.curdir}/.fake-netrc"
         # TODO Change Bandersnatch internal API to take proxy settings in from config parameters
-        if self.remote.proxy_url:
-            environ['http_proxy'] = self.remote.proxy_url
-            environ['https_proxy'] = self.remote.proxy_url
+        if proxy_url := self.remote.proxy_url:
+            if self.remote.proxy_username or self.remote.proxy_password:
+                parsed_proxy = urlsplit(proxy_url)
+                creds = f"{self.remote.proxy_username}:{self.remote.proxy_password}"
+                netloc = f"{creds}@{parsed_proxy.netloc}"
+                proxy_url = urlunsplit((parsed_proxy.scheme, netloc, "", "", ""))
+            environ['http_proxy'] = proxy_url
+            environ['https_proxy'] = proxy_url
         # Bandersnatch includes leading slash when forming API urls
         url = self.remote.url.rstrip("/")
         # local & global timeouts defaults to 10secs and 5 hours
-        async with PulpMaster(url) as master:
+        async with Master(url) as master:
             deferred_download = self.remote.policy != Remote.IMMEDIATE
             workers = self.remote.download_concurrency or self.remote.DEFAULT_DOWNLOAD_CONCURRENCY
             async with ProgressReport(
                 message="Fetching Project Metadata", code="sync.fetching.project"
             ) as p:
                 pmirror = PulpMirror(
                     serial=0,  # Serial currently isn't supported by Pulp
@@ -136,26 +144,14 @@
                 if self.remote.includes:
                     packages_to_sync = [
                         Requirement(pkg).name for pkg in self.remote.includes
                     ]
                 await pmirror.synchronize(packages_to_sync)
 
 
-class PulpMaster(Master):
-    """
-    Temporary subclass of bandersnatch.Master until features are in bandersnatch.
-    """
-
-    async def __aenter__(self) -> "Master":
-        """Ensure Pulp does not try to read the .netrc file."""
-        await super().__aenter__()
-        self.session._trust_env = False
-        return self
-
-
 class PulpMirror(Mirror):
     """
     Pulp Mirror Class to perform syncing using Bandersnatch
     """
 
     def __init__(
         self, serial, master, workers, deferred_download, python_stage, progress_report
```

### Comparing `pulp-python-3.8.0/pulp_python/app/tasks/upload.py` & `pulp-python-3.9.0/pulp_python/app/tasks/upload.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/urls.py` & `pulp-python-3.9.0/pulp_python/app/urls.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/utils.py` & `pulp-python-3.9.0/pulp_python/app/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/app/viewsets.py` & `pulp-python-3.9.0/pulp_python/app/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             'name': ['exact', 'in'],
             'author': ['exact', 'in'],
             'packagetype': ['exact', 'in'],
             'requires_python': ['exact', 'in', "contains"],
             'filename': ['exact', 'in', 'contains'],
             'keywords': ['in', 'contains'],
             'sha256': ['exact', 'in'],
+            'version': ['exact', 'gt', 'lt', 'gte', 'lte']
         }
 
 
 class PythonPackageSingleArtifactContentUploadViewSet(
         core_viewsets.SingleArtifactContentUploadViewSet):
     """
     <!-- User-facing documentation, rendered as html-->
```

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_auto_publish.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_auto_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_consume_content.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_consume_content.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_crud_content_unit.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_crud_content_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,28 +142,24 @@
         self.assertEqual(content_unit.pulp_href, content_list_search.pulp_href)
         self.check_package_data(content_unit.to_dict())
 
     def test_07_upload_duplicate_file_without_repo(self):
         """
         1) upload file
         2) upload the same file again
-        3) this should fail/send an error
+        3) this should return first unit
         """
         delete_orphans()
         response = self.do_upload()
         created_resources = monitor_task(response.task).created_resources
         content_unit = self.content_api.read(created_resources[0])
         self.check_package_data(content_unit.to_dict())
 
-        with self.assertRaises(PulpTaskError) as cm:
-            monitor_task(self.do_upload().task)
-        task_report = cm.exception.task.to_dict()
-        msg = "This field must be unique"
-        self.assertTrue("sha256" in task_report["error"]["description"])
-        self.assertTrue(msg in task_report["error"]["description"])
+        created_resources = monitor_task(self.do_upload().task).created_resources
+        self.assertEqual(content_unit.pulp_href, created_resources[0])
 
     def test_08_upload_same_filename_different_artifact(self):
         """
         1) upload PYTHON_EGG file with PYTHON_EGG filename
         2) upload aiohttp-3.3.0.tar.gz with PYTHON_EGG filename
         3) assert that two content units where created
         """
```

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_crud_publications.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_crud_publications.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_crud_remotes.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_download_content.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_download_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,32 +120,32 @@
         self.assertEqual(get_content_summary(repo3.to_dict()), PYTHON_LG_FIXTURE_SUMMARY)
 
     def test_full_fixtures_to_pulp_sync(self):
         """
         This test checks that Pulp can fully sync another Python Package repository that is not
         PyPI. This reads the repository's simple page if XMLRPC isn't supported.
         """
-        remote = self._create_remote(includes="", prereleases=True)
+        remote = self._create_remote(includes=[], prereleases=True)
         repo = self._create_repo_and_sync_with_remote(remote)
         self.assertEqual(get_content_summary(repo.to_dict()), PYTHON_LG_FIXTURE_SUMMARY)
 
     def test_full_pulp_to_pulp_sync(self):
         """
         This test checks that Pulp can fully sync all packages from another Pulp instance
         without having to specify the includes field.
         """
         remote = self._create_remote(includes=PYTHON_MD_PROJECT_SPECIFIER)
         repo = self._create_repo_and_sync_with_remote(remote)
         # Test using live generated simple pages
         distro = self._create_distribution_from_repo(repo)
 
-        remote = self._create_remote(includes="", url=distro.base_url)
+        remote = self._create_remote(includes=[], url=distro.base_url)
         repo2 = self._create_repo_and_sync_with_remote(remote)
         self.assertEqual(get_content_summary(repo2.to_dict()), PYTHON_MD_FIXTURE_SUMMARY)
 
         # Now test using publication simple pages
         pub = self._create_publication(repo)
         distro2 = self._create_distribution_from_publication(pub)
-        remote = self._create_remote(includes="", url=distro2.base_url, prereleases=True)
+        remote = self._create_remote(includes=[], url=distro2.base_url, prereleases=True)
 
         repo3 = self._create_repo_and_sync_with_remote(remote)
         self.assertEqual(get_content_summary(repo3.to_dict()), PYTHON_MD_FIXTURE_SUMMARY)
```

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_full_mirror.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_full_mirror.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_pypi_apis.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_pypi_apis.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/api/test_sync.py` & `pulp-python-3.9.0/pulp_python/tests/functional/api/test_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding=utf-8
 """Tests that sync python plugin repositories."""
+import pytest
 import unittest
 
 from pulp_smash import config
-from pulp_smash.pulp3.bindings import monitor_task, PulpTaskError, delete_orphans
+from pulp_smash.pulp3.bindings import monitor_task, PulpTaskError
 from pulp_smash.pulp3.utils import (
     gen_repo,
     get_added_content_summary,
     get_removed_content_summary,
     get_content_summary,
 )
 
@@ -578,17 +579,14 @@
         cls.remote = None
 
     @classmethod
     def tearDown(cls):
         """Destroy class-wide variables per test"""
         cls.remote_api.delete(cls.remote.pulp_href)
         cls.repo_api.delete(cls.repo.pulp_href)
-        # This is the last test case to be ran, delete orphans
-        # TODO: Move this to pytest hook when converting to pytest style
-        delete_orphans()
 
     def test_no_windows_sync(self):
         """Tests that no windows packages are synced"""
         body = gen_python_remote(
             includes=["scipy"],
             exclude_platforms=["windows"],
             prereleases=True,
@@ -639,14 +637,60 @@
 
         self.assertEqual(
             get_content_summary(self.repo.to_dict())[PYTHON_CONTENT_NAME],
             SCIPY_COUNTS["no_os"]
         )
 
 
+@pytest.mark.parallel
+def test_proxy_sync(
+    python_repo,
+    python_repo_api_client,
+    python_remote_factory,
+    python_content_api_client,
+    http_proxy,
+):
+    """Test syncing with a proxy."""
+    body = gen_python_remote(proxy_url=http_proxy.proxy_url)
+    remote = python_remote_factory(**body)
+    sync_resp = python_repo_api_client.sync(python_repo.pulp_href, {"remote": remote.pulp_href})
+    monitor_task(sync_resp.task)
+
+    repo = python_repo_api_client.read(python_repo.pulp_href)
+    assert repo.latest_version_href[-2] == "1"
+
+    content_resp = python_content_api_client.list(repository_version=repo.latest_version_href)
+    assert content_resp.count == 2
+
+
+@pytest.mark.parallel
+def test_proxy_auth_sync(
+    python_repo,
+    python_repo_api_client,
+    python_remote_factory,
+    python_content_api_client,
+    http_proxy_with_auth,
+):
+    """Test syncing with a proxy with auth."""
+    body = gen_python_remote(
+        proxy_url=http_proxy_with_auth.proxy_url,
+        proxy_username=http_proxy_with_auth.username,
+        proxy_password=http_proxy_with_auth.password,
+    )
+    remote = python_remote_factory(**body)
+    sync_resp = python_repo_api_client.sync(python_repo.pulp_href, {"remote": remote.pulp_href})
+    monitor_task(sync_resp.task)
+
+    repo = python_repo_api_client.read(python_repo.pulp_href)
+    assert repo.latest_version_href[-2] == "1"
+
+    content_resp = python_content_api_client.list(repository_version=repo.latest_version_href)
+    assert content_resp.count == 2
+
+
 def sync_to_remote(self, body, create=False, mirror=False):
     """Takes a body and creates/updates a remote object, then it performs a sync"""
     if create:
         type(self).remote = self.remote_api.create(body)
     else:
         remote_task = self.remote_api.partial_update(self.remote.pulp_href, body)
         monitor_task(remote_task.task)
```

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/conftest.py` & `pulp-python-3.9.0/pulp_python/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/constants.py` & `pulp-python-3.9.0/pulp_python/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/functional/utils.py` & `pulp-python-3.9.0/pulp_python/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/upgrade/post/test_publish.py` & `pulp-python-3.9.0/pulp_python/tests/upgrade/post/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python/tests/upgrade/pre/test_publish.py` & `pulp-python-3.9.0/pulp_python/tests/upgrade/pre/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pulp_python.egg-info/PKG-INFO` & `pulp-python-3.9.0/pulp_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-python
-Version: 3.8.0
+Version: 3.9.0
 Summary: pulp-python plugin for the Pulp Project
 Home-page: https://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: # pulp_python
```

### Comparing `pulp-python-3.8.0/pulp_python.egg-info/SOURCES.txt` & `pulp-python-3.9.0/pulp_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/pyproject.toml` & `pulp-python-3.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-python-3.8.0/setup.py` & `pulp-python-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="pulp-python",
-    version="3.8.0",
+    version="3.9.0",
     description="pulp-python plugin for the Pulp Project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv2+",
     python_requires=">=3.8",
     author="Pulp Project Developers",
     author_email="pulp-list@redhat.com",
```

