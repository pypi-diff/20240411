# Comparing `tmp/django_migration_zero-1.1.2.tar.gz` & `tmp/django_migration_zero-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_migration_zero-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_migration_zero-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_migration_zero-1.1.2.tar` & `django_migration_zero-2.0.0.tar`

### file list

```diff
@@ -1,70 +1,69 @@
--rw-r--r--   0        0        0     3695 2023-12-05 10:06:01.264839 django_migration_zero-1.1.2/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0      320 2023-12-05 10:06:38.653921 django_migration_zero-1.1.2/.coveragerc
--rw-r--r--   0        0        0      288 2023-12-05 10:06:38.653921 django_migration_zero-1.1.2/.editorconfig
--rw-r--r--   0        0        0     2740 2023-12-05 10:18:19.323936 django_migration_zero-1.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3282 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/.gitignore
--rw-r--r--   0        0        0      668 2023-12-05 10:18:19.323936 django_migration_zero-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      773 2023-12-05 10:06:38.669428 django_migration_zero-1.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1435 2023-12-15 12:53:18.183135 django_migration_zero-1.1.2/CHANGES.md
--rw-r--r--   0        0        0     1102 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/LICENSE.md
--rw-r--r--   0        0        0      140 2023-12-05 10:06:38.669428 django_migration_zero-1.1.2/MANIFEST.in
--rw-r--r--   0        0        0     7915 2023-12-05 10:18:19.323936 django_migration_zero-1.1.2/README.md
--rw-r--r--   0        0        0      182 2023-12-15 12:53:30.906344 django_migration_zero-1.1.2/django_migration_zero/__init__.py
--rw-r--r--   0        0        0      455 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/admin.py
--rw-r--r--   0        0        0      279 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/apps.py
--rw-r--r--   0        0        0      199 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/helpers/__init__.py
--rw-r--r--   0        0        0     2991 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/helpers/file_system.py
--rw-r--r--   0        0        0      193 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/helpers/logger.py
--rw-r--r--   0        0        0      921 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1396 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/management/commands/__init__.py
--rw-r--r--   0        0        0      370 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/management/commands/handle_migration_zero_reset.py
--rw-r--r--   0        0        0      917 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/management/commands/reset_local_migration_files.py
--rw-r--r--   0        0        0     1320 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/managers.py
--rw-r--r--   0        0        0     1465 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/migrations/__init__.py
--rw-r--r--   0        0        0     1413 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/models.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/services/__init__.py
--rw-r--r--   0        0        0     2307 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/services/deployment.py
--rw-r--r--   0        0        0     1401 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/services/local.py
--rw-r--r--   0        0        0      612 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/django_migration_zero/settings.py
--rw-r--r--   0        0        0      654 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/docs/Makefile
--rw-r--r--   0        0        0     2833 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/docs/conf.py
--rw-r--r--   0        0        0     2758 2023-12-06 15:24:37.072384 django_migration_zero-1.1.2/docs/features/01_introduction.md
--rw-r--r--   0        0        0      850 2023-12-15 12:52:50.776456 django_migration_zero-1.1.2/docs/features/02_configuration.md
--rw-r--r--   0        0        0     8678 2023-12-06 15:22:32.234863 django_migration_zero-1.1.2/docs/features/03_workflow.md
--rw-r--r--   0        0        0     1720 2023-12-15 12:52:50.767843 django_migration_zero-1.1.2/docs/features/04_common_issues_and_solutions.md
--rw-r--r--   0        0        0     1490 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/docs/features/05_architecture.md
--rw-r--r--   0        0        0     1602 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/docs/features/06_management_commands.md
--rw-r--r--   0        0        0       33 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/docs/features/07_changelog.rst
--rw-r--r--   0        0        0      455 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/docs/make.bat
--rw-r--r--   0        0        0      699 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/manage.py
--rw-r--r--   0        0        0     5130 2023-12-05 10:18:19.323936 django_migration_zero-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       56 2023-12-05 10:06:38.669428 django_migration_zero-1.1.2/pytest.init
--rw-r--r--   0        0        0      121 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/scripts/unix/install_requirements.sh
--rw-r--r--   0        0        0       50 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      121 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/scripts/windows/install_requirements.ps1
--rw-r--r--   0        0        0       50 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0     3541 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/settings.py
--rw-r--r--   0        0        0      293 2023-12-05 10:06:38.685082 django_migration_zero-1.1.2/setup.cfg
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/testapp/__init__.py
--rw-r--r--   0        0        0      144 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/helpers/__init__.py
--rw-r--r--   0        0        0     2144 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/helpers/test_file_system.py
--rw-r--r--   0        0        0      259 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/helpers/test_logger.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/management/commands/__init__.py
--rw-r--r--   0        0        0      589 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/management/commands/test_handle_migration_zero_reset.py
--rw-r--r--   0        0        0     1725 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/management/commands/test_reset_local_migration_files.py
--rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/services/__init__.py
--rw-r--r--   0        0        0     3006 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/services/test_deployment.py
--rw-r--r--   0        0        0     2584 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/services/test_local.py
--rw-r--r--   0        0        0     2387 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/test_admin.py
--rw-r--r--   0        0        0     2007 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/test_managers.py
--rw-r--r--   0        0        0     1244 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/test_models.py
--rw-r--r--   0        0        0      788 2023-12-05 10:06:01.280467 django_migration_zero-1.1.2/tests/test_settings.py
--rw-r--r--   0        0        0     9972 1970-01-01 00:00:00.000000 django_migration_zero-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3695 2023-12-05 10:06:01.264839 django_migration_zero-2.0.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0      320 2024-04-11 14:07:17.462200 django_migration_zero-2.0.0/.coveragerc
+-rw-r--r--   0        0        0      288 2024-04-11 14:07:17.463212 django_migration_zero-2.0.0/.editorconfig
+-rw-r--r--   0        0        0     2728 2024-04-11 14:13:19.069151 django_migration_zero-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3282 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/.gitignore
+-rw-r--r--   0        0        0      668 2024-04-11 14:13:19.070152 django_migration_zero-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      773 2024-04-11 14:07:17.468214 django_migration_zero-2.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1581 2024-04-11 14:13:19.070152 django_migration_zero-2.0.0/CHANGES.md
+-rw-r--r--   0        0        0     1102 2024-04-11 14:07:17.494583 django_migration_zero-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0      140 2024-04-11 14:07:17.469211 django_migration_zero-2.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     7915 2024-04-11 14:07:17.481592 django_migration_zero-2.0.0/README.md
+-rw-r--r--   0        0        0      182 2024-04-11 14:13:19.071152 django_migration_zero-2.0.0/django_migration_zero/__init__.py
+-rw-r--r--   0        0        0      455 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/admin.py
+-rw-r--r--   0        0        0      279 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/apps.py
+-rw-r--r--   0        0        0      199 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/exceptions.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/helpers/__init__.py
+-rw-r--r--   0        0        0     2991 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/helpers/file_system.py
+-rw-r--r--   0        0        0      193 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/helpers/logger.py
+-rw-r--r--   0        0        0      921 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1396 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/management/commands/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-11 14:13:19.071152 django_migration_zero-2.0.0/django_migration_zero/management/commands/handle_migration_zero_reset.py
+-rw-r--r--   0        0        0      917 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/management/commands/reset_local_migration_files.py
+-rw-r--r--   0        0        0     1320 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/managers.py
+-rw-r--r--   0        0        0     1465 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/migrations/__init__.py
+-rw-r--r--   0        0        0     1413 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/models.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/services/__init__.py
+-rw-r--r--   0        0        0     2307 2024-01-04 13:56:50.223239 django_migration_zero-2.0.0/django_migration_zero/services/deployment.py
+-rw-r--r--   0        0        0     1387 2024-04-11 14:13:19.071152 django_migration_zero-2.0.0/django_migration_zero/services/local.py
+-rw-r--r--   0        0        0      612 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/django_migration_zero/settings.py
+-rw-r--r--   0        0        0      654 2024-04-11 14:07:17.489582 django_migration_zero-2.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2833 2024-04-11 14:13:19.072152 django_migration_zero-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0     2758 2023-12-06 15:24:37.072384 django_migration_zero-2.0.0/docs/features/01_introduction.md
+-rw-r--r--   0        0        0      850 2023-12-15 12:52:50.776456 django_migration_zero-2.0.0/docs/features/02_configuration.md
+-rw-r--r--   0        0        0     8678 2023-12-06 15:22:32.234863 django_migration_zero-2.0.0/docs/features/03_workflow.md
+-rw-r--r--   0        0        0     1720 2023-12-15 12:52:50.767843 django_migration_zero-2.0.0/docs/features/04_common_issues_and_solutions.md
+-rw-r--r--   0        0        0     1490 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/docs/features/05_architecture.md
+-rw-r--r--   0        0        0     1602 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/docs/features/06_management_commands.md
+-rw-r--r--   0        0        0       33 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/docs/features/07_changelog.rst
+-rw-r--r--   0        0        0      455 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2024-04-11 14:07:17.488362 django_migration_zero-2.0.0/docs/make.bat
+-rw-r--r--   0        0        0      701 2024-04-11 14:13:19.072152 django_migration_zero-2.0.0/manage.py
+-rw-r--r--   0        0        0     5144 2024-04-11 14:13:19.073152 django_migration_zero-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-11 14:07:17.490594 django_migration_zero-2.0.0/scripts/unix/install_requirements.sh
+-rw-r--r--   0        0        0       50 2024-04-11 14:07:17.491592 django_migration_zero-2.0.0/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      121 2024-04-11 14:07:17.492591 django_migration_zero-2.0.0/scripts/windows/install_requirements.ps1
+-rw-r--r--   0        0        0       50 2024-04-11 14:07:17.493591 django_migration_zero-2.0.0/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0     3541 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/settings.py
+-rw-r--r--   0        0        0      293 2024-04-11 14:07:17.482607 django_migration_zero-2.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/testapp/__init__.py
+-rw-r--r--   0        0        0      144 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     2144 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/helpers/test_file_system.py
+-rw-r--r--   0        0        0      259 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/helpers/test_logger.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/management/commands/__init__.py
+-rw-r--r--   0        0        0      589 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/management/commands/test_handle_migration_zero_reset.py
+-rw-r--r--   0        0        0     1725 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/management/commands/test_reset_local_migration_files.py
+-rw-r--r--   0        0        0        0 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/services/__init__.py
+-rw-r--r--   0        0        0     3006 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/services/test_deployment.py
+-rw-r--r--   0        0        0     2584 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/services/test_local.py
+-rw-r--r--   0        0        0     2387 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/test_admin.py
+-rw-r--r--   0        0        0     2007 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/test_managers.py
+-rw-r--r--   0        0        0     1244 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/test_models.py
+-rw-r--r--   0        0        0      788 2023-12-05 10:06:01.280467 django_migration_zero-2.0.0/tests/test_settings.py
+-rw-r--r--   0        0        0     9937 1970-01-01 00:00:00.000000 django_migration_zero-2.0.0/PKG-INFO
```

### Comparing `django_migration_zero-1.1.2/.ambient-package-update/metadata.py` & `django_migration_zero-2.0.0/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/.github/workflows/ci.yml` & `django_migration_zero-2.0.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   linting:
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - name: Install required packages
         run: pip install pre-commit
 
       - name: Run pre-commit hooks
@@ -23,15 +23,15 @@
   
   validate_migrations:
     name: Validate migrations
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
 
       - name: Install dependencies
         run: python -m pip install -U pip-tools && pip-compile --extra dev, -o requirements.txt pyproject.toml --resolver=backtracking && pip-sync
 
       - name: Validate migration integrity
@@ -39,15 +39,15 @@
 
   tests:
     name: Python ${{ matrix.python-version }}, django ${{ matrix.django-version }}
     runs-on: ubuntu-22.04
     strategy:
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12', ]
-        django-version: ['32', '41', '42', '50', ]
+        django-version: ['42', '50', ]
 
         exclude:
           - python-version: '3.12'
             django-version: 32
           - python-version: '3.11'
             django-version: 32
           - python-version: '3.10'
@@ -56,15 +56,15 @@
             django-version: 50
           - python-version: '3.9'
             django-version: 50
 
     steps:
       - uses: actions/checkout@v4
       - name: setup python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: pip install tox
       - name: Run Tests
         env:
           TOXENV: django${{ matrix.django-version }}
@@ -78,15 +78,15 @@
   coverage:
     name: Coverage
     runs-on: ubuntu-22.04
     needs: tests
     steps:
       - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
 
       - name: Install dependencies
         run: python -m pip install --upgrade coverage[toml]
 
       - name: Download data
```

### Comparing `django_migration_zero-1.1.2/.gitignore` & `django_migration_zero-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/.pre-commit-config.yaml` & `django_migration_zero-2.0.0/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # you find the full pre-commit-tools docu under:
 # https://pre-commit.com/
 
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.6
+    rev: v0.3.5
     hooks:
       # Run the Ruff linter.
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       # Run the Ruff formatter.
       - id: ruff-format
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [ --py38-plus ]
         stages: [ push ]
 
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.15.0
+    rev: 1.16.0
     hooks:
       - id: django-upgrade
-        args: [--target-version, "3.2"]
+        args: [--target-version, "4.2"]
         stages: [ push ]
```

### Comparing `django_migration_zero-1.1.2/.readthedocs.yaml` & `django_migration_zero-2.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/CHANGES.md` & `django_migration_zero-2.0.0/CHANGES.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+* *2.0.0* (2024-04-11)
+  * Dropped Django 3.2 & 4.1 support (via `ambient-package-update`)
+  * Internal updates via `ambient-package-update`
+
 * *1.1.2* (2023-12-15)
   * Improved documentation
 
 * *1.1.1* (2023-12-06)
   * Improved documentation
 
 * *1.1.0* (2023-12-05)
```

### Comparing `django_migration_zero-1.1.2/LICENSE.md` & `django_migration_zero-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/README.md` & `django_migration_zero-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/helpers/file_system.py` & `django_migration_zero-2.0.0/django_migration_zero/helpers/file_system.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/locale/de/LC_MESSAGES/django.mo` & `django_migration_zero-2.0.0/django_migration_zero/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/locale/de/LC_MESSAGES/django.po` & `django_migration_zero-2.0.0/django_migration_zero/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/management/commands/reset_local_migration_files.py` & `django_migration_zero-2.0.0/django_migration_zero/management/commands/reset_local_migration_files.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/managers.py` & `django_migration_zero-2.0.0/django_migration_zero/managers.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/migrations/0001_initial.py` & `django_migration_zero-2.0.0/django_migration_zero/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/models.py` & `django_migration_zero-2.0.0/django_migration_zero/models.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/services/deployment.py` & `django_migration_zero-2.0.0/django_migration_zero/services/deployment.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/django_migration_zero/services/local.py` & `django_migration_zero-2.0.0/django_migration_zero/services/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     get_migration_files,
     has_migration_directory,
 )
 from django_migration_zero.helpers.logger import get_logger
 
 
 class ResetMigrationFiles:
-    help = "Remove all local migrations files and create new initial ones."  # noqa: A003
+    help = "Remove all local migrations files and create new initial ones."
 
     dry_run: bool
     exclude_initials: bool
 
     def __init__(self, dry_run: bool = False, exclude_initials: bool = False):
         super().__init__()
```

### Comparing `django_migration_zero-1.1.2/django_migration_zero/settings.py` & `django_migration_zero-2.0.0/django_migration_zero/settings.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/Makefile` & `django_migration_zero-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/conf.py` & `django_migration_zero-2.0.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django.setup()
 
 from django_migration_zero import __version__  # noqa: E402
 
 # -- Project information -----------------------------------------------------
 
 project = "django-migration-zero"
-copyright = "2023, Ambient Innovation: GmbH"  # noqa: A001
+copyright = "2024, Ambient Innovation: GmbH"  # noqa: A001
 author = "Ambient Innovation: GmbH <hello@ambient.digital>"
 version = __version__
 release = __version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `django_migration_zero-1.1.2/docs/features/01_introduction.md` & `django_migration_zero-2.0.0/docs/features/01_introduction.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/features/02_configuration.md` & `django_migration_zero-2.0.0/docs/features/02_configuration.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/features/03_workflow.md` & `django_migration_zero-2.0.0/docs/features/03_workflow.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/features/04_common_issues_and_solutions.md` & `django_migration_zero-2.0.0/docs/features/04_common_issues_and_solutions.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/features/05_architecture.md` & `django_migration_zero-2.0.0/docs/features/05_architecture.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/features/06_management_commands.md` & `django_migration_zero-2.0.0/docs/features/06_management_commands.md`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/docs/make.bat` & `django_migration_zero-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/manage.py` & `django_migration_zero-2.0.0/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 """Django's command-line utility for administrative tasks."""
+
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
     os.environ.setdefault("DJANGO_SETTINGS_MODULE", "django_migration_zero.settings")
```

### Comparing `django_migration_zero-1.1.2/pyproject.toml` & `django_migration_zero-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     {'name' = 'Ambient Digital', 'email' = 'hello@ambient.digital'},
 ]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -41,34 +39,35 @@
    'typer~=0.9',
    'freezegun~=1.3',
    'pytest-django~=4.7',
    'pytest-mock~=3.12',
    'coverage~=7.3',
    'pre-commit~=3.5',
    'ruff~=0.1.7',
-   'sphinx==4.2.0',
-   'sphinx-rtd-theme==1.0.0',
-   'm2r2==0.3.1',
+   'sphinx~=7.1',
+   'sphinx-rtd-theme~=2.0',
+   'm2r2==0.3.3.post2',
    'mistune<2.0.0',
-   'ambient-package-update~=23.12.3',
+   'flit~=3.9',
+   'ambient-package-update~=24.4.4',
    'unittest-parametrize~=1.3',
 ]
 
 [tool.flit.module]
 name = "django_migration_zero"
 
 [project.urls]
 'Homepage' = 'https://github.com/ambient-innovation/django-migration-zero/'
 'Documentation' = 'https://django-migration-zero.readthedocs.io/en/latest/index.html'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/django-migration-zero/issues'
 'Changelog' = 'https://django-migration-zero.readthedocs.io/en/latest/features/changelog.html'
 
 [tool.ruff]
-select = [
+lint.select = [
     "E",       # pycodestyle errors
     "W",       # pycodestyle warnings
     "F",       # Pyflakes
     "N",       # pep8-naming
     "I",       # isort
     "B",       # flake8-bugbear
     "A",       # flake8-builtins
@@ -82,19 +81,19 @@
     "PIE",     # Bunch of useful rules
     # "SIM",     # Simplifies your code
     "INT",     # Validates your gettext translation strings
     "PERF",    # PerfLint
     "PGH",     # No all-purpose "# noqa" and eval validation
     "PL",      # PyLint
 ]
-ignore = [
+lint.ignore = [
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = [
+lint.fixable = [
     "E",       # pycodestyle errors
     "W",       # pycodestyle warnings
     "F",       # Pyflakes
     "N",       # pep8-naming
     "I",       # isort
     "B",       # flake8-bugbear
     "A",       # flake8-builtins
@@ -108,15 +107,15 @@
     "PIE",     # Bunch of useful rules
     # "SIM",     # Simplifies your code
     "INT",     # Validates your gettext translation strings
     "PERF",    # PerfLint
     "PGH",     # No all-purpose "# noqa" and eval validation
     "PL",      # PyLint
 ]
-unfixable = []
+lint.unfixable = []
 
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
@@ -165,23 +164,28 @@
 [tox]
 envlist = py{38,39,310,311}-django{32,41,42}
 isolated_build = True
 
 [testenv]
 # Django deprecation overview: https://www.djangoproject.com/download/
 deps =
-    django32: Django==3.2.*
-    django41: Django==4.1.*
     django42: Django==4.2.*
     django50: Django==5.0.*
 extras = dev,
 commands =
     coverage run -m pytest --ds settings tests
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
     3.12: py312
 """
+
+[tool.pytest.ini_options]
+python_files = [
+    "tests.py",
+    "test_*.py",
+    "*_tests.py",
+]
```

### Comparing `django_migration_zero-1.1.2/settings.py` & `django_migration_zero-2.0.0/settings.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/helpers/test_file_system.py` & `django_migration_zero-2.0.0/tests/helpers/test_file_system.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/management/commands/test_handle_migration_zero_reset.py` & `django_migration_zero-2.0.0/tests/management/commands/test_handle_migration_zero_reset.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/management/commands/test_reset_local_migration_files.py` & `django_migration_zero-2.0.0/tests/management/commands/test_reset_local_migration_files.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/services/test_deployment.py` & `django_migration_zero-2.0.0/tests/services/test_deployment.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/services/test_local.py` & `django_migration_zero-2.0.0/tests/services/test_local.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/test_admin.py` & `django_migration_zero-2.0.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/test_managers.py` & `django_migration_zero-2.0.0/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/test_models.py` & `django_migration_zero-2.0.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/tests/test_settings.py` & `django_migration_zero-2.0.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_migration_zero-1.1.2/PKG-INFO` & `django_migration_zero-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: django-migration-zero
-Version: 1.1.2
+Version: 2.0.0
 Summary: Holistic implementation of "migration zero" pattern for Django covering local changes and in-production database adjustments.
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -27,19 +25,20 @@
 Requires-Dist: typer~=0.9 ; extra == "dev"
 Requires-Dist: freezegun~=1.3 ; extra == "dev"
 Requires-Dist: pytest-django~=4.7 ; extra == "dev"
 Requires-Dist: pytest-mock~=3.12 ; extra == "dev"
 Requires-Dist: coverage~=7.3 ; extra == "dev"
 Requires-Dist: pre-commit~=3.5 ; extra == "dev"
 Requires-Dist: ruff~=0.1.7 ; extra == "dev"
-Requires-Dist: sphinx==4.2.0 ; extra == "dev"
-Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
-Requires-Dist: m2r2==0.3.1 ; extra == "dev"
+Requires-Dist: sphinx~=7.1 ; extra == "dev"
+Requires-Dist: sphinx-rtd-theme~=2.0 ; extra == "dev"
+Requires-Dist: m2r2==0.3.3.post2 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.12.3 ; extra == "dev"
+Requires-Dist: flit~=3.9 ; extra == "dev"
+Requires-Dist: ambient-package-update~=24.4.4 ; extra == "dev"
 Requires-Dist: unittest-parametrize~=1.3 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/django-migration-zero/issues
 Project-URL: Changelog, https://django-migration-zero.readthedocs.io/en/latest/features/changelog.html
 Project-URL: Documentation, https://django-migration-zero.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/ambient-innovation/django-migration-zero/
 Project-URL: Maintained by, https://ambient.digital/
 Provides-Extra: dev
```

