# Comparing `tmp/django_dynamic_admin_forms-2.2.1.tar.gz` & `tmp/django_dynamic_admin_forms-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_admin_forms-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_dynamic_admin_forms-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_dynamic_admin_forms-2.2.1.tar` & `django_dynamic_admin_forms-3.0.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
--rw-r--r--   0        0        0     6688 2023-12-05 12:17:26.230092 django_dynamic_admin_forms-2.2.1/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0      320 2023-12-05 11:23:48.985723 django_dynamic_admin_forms-2.2.1/.coveragerc
--rw-r--r--   0        0        0      288 2023-12-05 11:23:48.985723 django_dynamic_admin_forms-2.2.1/.editorconfig
--rw-r--r--   0        0        0     2225 2023-12-05 12:17:26.230092 django_dynamic_admin_forms-2.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      815 2023-12-18 16:10:12.014812 django_dynamic_admin_forms-2.2.1/.gitignore
--rw-r--r--   0        0        0      668 2023-12-05 12:17:26.230092 django_dynamic_admin_forms-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-10-22 11:06:39.654928 django_dynamic_admin_forms-2.2.1/.python-version
--rw-r--r--   0        0        0      773 2023-12-05 11:23:49.001354 django_dynamic_admin_forms-2.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1057 2023-12-18 16:10:12.007930 django_dynamic_admin_forms-2.2.1/CHANGES.md
--rw-r--r--   0        0        0     1102 2023-12-05 11:23:49.032675 django_dynamic_admin_forms-2.2.1/LICENSE.md
--rw-r--r--   0        0        0      145 2023-12-05 11:23:49.001354 django_dynamic_admin_forms-2.2.1/MANIFEST.in
--rw-r--r--   0        0        0    10481 2023-12-18 16:10:12.011761 django_dynamic_admin_forms-2.2.1/README.md
--rw-r--r--   0        0        0      101 2023-12-18 16:10:12.004915 django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/__init__.py
--rw-r--r--   0        0        0     2770 2023-12-05 11:11:13.944830 django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/admin.py
--rw-r--r--   0        0        0      114 2023-10-22 11:06:39.654928 django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/apps.py
--rw-r--r--   0        0        0     2258 2023-10-22 11:06:39.658928 django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/static/js/dynamic_admin.js
--rw-r--r--   0        0        0     1601 2023-10-22 11:06:39.658928 django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/templates/admin/change_form.html
--rw-r--r--   0        0        0      224 2023-12-18 11:36:35.858088 django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/urls.py
--rw-r--r--   0        0        0      654 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/docs/Makefile
--rw-r--r--   0        0        0     2853 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/docs/conf.py
--rw-r--r--   0        0        0   946599 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/docs/demo.gif
--rw-r--r--   0        0        0       31 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/docs/features/changelog.rst
--rw-r--r--   0        0        0      106 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/docs/make.bat
--rw-r--r--   0        0        0      145 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/e2e/cypress.json
--rw-r--r--   0        0        0     1342 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/e2e/cypress/integration/dynamic-select.spec.js
--rw-r--r--   0        0        0      761 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0      838 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/e2e/cypress/support/commands.js
--rw-r--r--   0        0        0      670 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-2.2.1/e2e/cypress/support/index.js
--rw-r--r--   0        0        0      130 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/e2e/cypress/support/paths.js
--rw-r--r--   0        0        0      266 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/e2e/package.json
--rw-r--r--   0        0        0    48807 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/e2e/yarn.lock
--rw-r--r--   0        0        0     8822 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/fixtures/fixtures-dev.json
--rw-r--r--   0        0        0      655 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/manage.py
--rw-r--r--   0        0        0     5238 2023-12-05 12:17:26.230092 django_dynamic_admin_forms-2.2.1/pyproject.toml
--rw-r--r--   0        0        0       56 2023-12-05 11:23:49.001354 django_dynamic_admin_forms-2.2.1/pytest.init
--rw-r--r--   0        0        0      121 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/scripts/unix/install_requirements.sh
--rw-r--r--   0        0        0       50 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      121 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/scripts/windows/install_requirements.ps1
--rw-r--r--   0        0        0       50 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0     2461 2023-12-18 16:11:01.310970 django_dynamic_admin_forms-2.2.1/settings.py
--rw-r--r--   0        0        0      303 2023-12-05 11:23:49.017049 django_dynamic_admin_forms-2.2.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/testapp/__init__.py
--rw-r--r--   0        0        0     2002 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-2.2.1/testapp/admin.py
--rw-r--r--   0        0        0      146 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/apps.py
--rw-r--r--   0        0        0     2908 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0      569 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/migrations/0002_extend_example.py
--rw-r--r--   0        0        0      571 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/migrations/0003_example_file_field.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     1180 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/models.py
--rw-r--r--   0        0        0      834 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-2.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2387 2023-12-05 11:11:13.944830 django_dynamic_admin_forms-2.2.1/tests/test_admin_generic.py
--rw-r--r--   0        0        0     3120 2023-12-05 11:11:13.944830 django_dynamic_admin_forms-2.2.1/tests/test_admin_unit.py
--rw-r--r--   0        0        0    12484 1970-01-01 00:00:00.000000 django_dynamic_admin_forms-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6681 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0      320 2024-04-11 14:21:47.522749 django_dynamic_admin_forms-3.0.0/.coveragerc
+-rw-r--r--   0        0        0      288 2024-04-11 14:21:47.523759 django_dynamic_admin_forms-3.0.0/.editorconfig
+-rw-r--r--   0        0        0     2213 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      887 2023-12-18 16:13:28.272678 django_dynamic_admin_forms-3.0.0/.gitignore
+-rw-r--r--   0        0        0      668 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-10-22 11:06:39.654928 django_dynamic_admin_forms-3.0.0/.python-version
+-rw-r--r--   0        0        0      773 2024-04-11 14:21:47.526759 django_dynamic_admin_forms-3.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1190 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/CHANGES.md
+-rw-r--r--   0        0        0     1102 2024-04-11 14:21:47.553238 django_dynamic_admin_forms-3.0.0/LICENSE.md
+-rw-r--r--   0        0        0      145 2024-04-11 14:21:47.528043 django_dynamic_admin_forms-3.0.0/MANIFEST.in
+-rw-r--r--   0        0        0    10422 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/README.md
+-rw-r--r--   0        0        0      101 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/__init__.py
+-rw-r--r--   0        0        0     2770 2023-12-05 11:11:13.944830 django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/admin.py
+-rw-r--r--   0        0        0      114 2023-10-22 11:06:39.654928 django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/apps.py
+-rw-r--r--   0        0        0     2258 2023-10-22 11:06:39.658928 django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/static/js/dynamic_admin.js
+-rw-r--r--   0        0        0     1601 2023-10-22 11:06:39.658928 django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/templates/admin/change_form.html
+-rw-r--r--   0        0        0      232 2023-12-18 16:13:28.272678 django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/urls.py
+-rw-r--r--   0        0        0      654 2024-04-11 14:21:47.548008 django_dynamic_admin_forms-3.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2853 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/docs/conf.py
+-rw-r--r--   0        0        0   946599 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/docs/demo.gif
+-rw-r--r--   0        0        0       31 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/docs/features/changelog.rst
+-rw-r--r--   0        0        0      106 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2024-04-11 14:21:47.546885 django_dynamic_admin_forms-3.0.0/docs/make.bat
+-rw-r--r--   0        0        0      145 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/e2e/cypress.json
+-rw-r--r--   0        0        0     1342 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/e2e/cypress/integration/dynamic-select.spec.js
+-rw-r--r--   0        0        0      761 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0      838 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/e2e/cypress/support/commands.js
+-rw-r--r--   0        0        0      670 2023-10-22 11:06:39.662938 django_dynamic_admin_forms-3.0.0/e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      130 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-3.0.0/e2e/cypress/support/paths.js
+-rw-r--r--   0        0        0      266 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-3.0.0/e2e/package.json
+-rw-r--r--   0        0        0    48807 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-3.0.0/e2e/yarn.lock
+-rw-r--r--   0        0        0     8822 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-3.0.0/fixtures/fixtures-dev.json
+-rw-r--r--   0        0        0      679 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/manage.py
+-rw-r--r--   0        0        0     5235 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-11 14:21:47.549240 django_dynamic_admin_forms-3.0.0/scripts/unix/install_requirements.sh
+-rw-r--r--   0        0        0       50 2024-04-11 14:21:47.550238 django_dynamic_admin_forms-3.0.0/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      121 2024-04-11 14:21:47.551238 django_dynamic_admin_forms-3.0.0/scripts/windows/install_requirements.ps1
+-rw-r--r--   0        0        0       50 2024-04-11 14:21:47.552229 django_dynamic_admin_forms-3.0.0/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0     2547 2023-12-18 16:13:28.272678 django_dynamic_admin_forms-3.0.0/settings.py
+-rw-r--r--   0        0        0      303 2024-04-11 14:21:47.540888 django_dynamic_admin_forms-3.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-3.0.0/testapp/__init__.py
+-rw-r--r--   0        0        0     2002 2023-10-22 11:06:39.666928 django_dynamic_admin_forms-3.0.0/testapp/admin.py
+-rw-r--r--   0        0        0      146 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/testapp/apps.py
+-rw-r--r--   0        0        0     2908 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      569 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/testapp/migrations/0002_extend_example.py
+-rw-r--r--   0        0        0      571 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/testapp/migrations/0003_example_file_field.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     1180 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/testapp/models.py
+-rw-r--r--   0        0        0      858 2024-04-11 14:24:12.800647 django_dynamic_admin_forms-3.0.0/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-10-22 11:06:39.670928 django_dynamic_admin_forms-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2387 2023-12-05 11:11:13.944830 django_dynamic_admin_forms-3.0.0/tests/test_admin_generic.py
+-rw-r--r--   0        0        0     3120 2023-12-05 11:11:13.944830 django_dynamic_admin_forms-3.0.0/tests/test_admin_unit.py
+-rw-r--r--   0        0        0    12348 1970-01-01 00:00:00.000000 django_dynamic_admin_forms-3.0.0/PKG-INFO
```

### Comparing `django_dynamic_admin_forms-2.2.1/.ambient-package-update/metadata.py` & `django_dynamic_admin_forms-3.0.0/.ambient-package-update/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 $ source .venv/bin/activate
 $ cd ..
 $ flit install --symlink
 ```
 Now the package should be available in your virtual environment
 and any changes should be directly visible.
 
-Alternatively, simply copy the directory `dynamic_admin_forms`
+Alternatively, copy the directory `dynamic_admin_forms`
 into any normal django project, so that the python interpreter
 finds the local version instead of the installed (old) version.
 
 ## Running E2E tests
 
 To run end-to-end tests locally:
 ```shell
```

### Comparing `django_dynamic_admin_forms-2.2.1/.github/workflows/ci.yml` & `django_dynamic_admin_forms-3.0.0/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

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
@@ -24,15 +24,15 @@
 
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
@@ -41,15 +41,15 @@
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
@@ -63,15 +63,15 @@
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

### Comparing `django_dynamic_admin_forms-2.2.1/.pre-commit-config.yaml` & `django_dynamic_admin_forms-3.0.0/.pre-commit-config.yaml`

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

### Comparing `django_dynamic_admin_forms-2.2.1/.readthedocs.yaml` & `django_dynamic_admin_forms-3.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/CHANGES.md` & `django_dynamic_admin_forms-3.0.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+**3.0.0**
+  * Dropped Django 3.2 & 4.1 support (via `ambient-package-update`)
+  * Internal updates via `ambient-package-update`
+
 **2.2.1**
 
 - Fixed security issue with URL not being wrapped in `admin_view`
 - Improved documentation
 
 **2.2.0**
```

### Comparing `django_dynamic_admin_forms-2.2.1/LICENSE.md` & `django_dynamic_admin_forms-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/README.md` & `django_dynamic_admin_forms-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -296,361 +296,357 @@
 00001270: 7665 6c6f 706d 656e 740d 0a0d 0a46 6f72  velopment....For
 00001280: 206c 6f63 616c 2064 6576 656c 6f70 6d65   local developme
 00001290: 6e74 2c20 6372 6561 7465 2061 2076 6972  nt, create a vir
 000012a0: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
 000012b0: 0d0a 696e 2074 6865 2060 7465 7374 7072  ..in the `testpr
 000012c0: 6f6a 6020 666f 6c64 6572 3a0d 0a60 6060  oj` folder:..```
 000012d0: 7368 656c 6c0d 0a24 2063 6420 7465 7374  shell..$ cd test
-000012e0: 6170 700d 0a24 2070 7974 686f 6e33 202d  app..$ python3 -
-000012f0: 6d20 7665 6e76 202e 7665 6e76 0d0a 2420  m venv .venv..$ 
-00001300: 736f 7572 6365 202e 7665 6e76 2f62 696e  source .venv/bin
-00001310: 2f61 6374 6976 6174 650d 0a24 2063 6420  /activate..$ cd 
-00001320: 2e2e 0d0a 2420 7069 7020 696e 7374 616c  ....$ pip instal
-00001330: 6c20 2d65 202e 0d0a 6060 600d 0a4e 6f77  l -e ...```..Now
-00001340: 2074 6865 2070 6163 6b61 6765 2073 686f   the package sho
-00001350: 756c 6420 6265 2061 7661 696c 6162 6c65  uld be available
-00001360: 2069 6e20 796f 7572 2076 6972 7475 616c   in your virtual
-00001370: 2065 6e76 6972 6f6e 6d65 6e74 0d0a 616e   environment..an
-00001380: 6420 616e 7920 6368 616e 6765 7320 7368  d any changes sh
-00001390: 6f75 6c64 2062 6520 6469 7265 6374 6c79  ould be directly
-000013a0: 2076 6973 6962 6c65 2e20 5275 6e20 7468   visible. Run th
-000013b0: 6520 7072 6f6a 6563 7420 6173 2061 2044  e project as a D
-000013c0: 6a61 6e67 6f20 7365 7276 6572 2061 6e64  jango server and
-000013d0: 206e 6176 6967 6174 6520 746f 2074 6865   navigate to the
-000013e0: 2061 646d 696e 2070 6167 652e 0d0a 0d0a   admin page.....
-000013f0: 416c 7465 726e 6174 6976 656c 792c 2063  Alternatively, c
-00001400: 6f70 7920 7468 6520 6469 7265 6374 6f72  opy the director
-00001410: 7920 6064 796e 616d 6963 5f61 646d 696e  y `dynamic_admin
-00001420: 5f66 6f72 6d73 600d 0a69 6e74 6f20 616e  _forms`..into an
-00001430: 7920 6e6f 726d 616c 2064 6a61 6e67 6f20  y normal django 
-00001440: 7072 6f6a 6563 742c 2073 6f20 7468 6174  project, so that
-00001450: 2074 6865 2070 7974 686f 6e20 696e 7465   the python inte
-00001460: 7270 7265 7465 720d 0a66 696e 6473 2074  rpreter..finds t
-00001470: 6865 206c 6f63 616c 2076 6572 7369 6f6e  he local version
-00001480: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
-00001490: 696e 7374 616c 6c65 6420 286f 6c64 2920  installed (old) 
-000014a0: 7665 7273 696f 6e2e 0d0a 0d0a 2323 2052  version.....## R
-000014b0: 756e 6e69 6e67 2045 3245 2074 6573 7473  unning E2E tests
-000014c0: 0d0a 0d0a 546f 2072 756e 2065 6e64 2d74  ....To run end-t
-000014d0: 6f2d 656e 6420 7465 7374 7320 6c6f 6361  o-end tests loca
-000014e0: 6c6c 793a 0d0a 6060 6073 6865 6c6c 0d0a  lly:..```shell..
-000014f0: 2420 6364 2074 6573 7461 7070 0d0a 2420  $ cd testapp..$ 
-00001500: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
-00001510: 2072 756e 7365 7276 6572 2030 2e30 2e30   runserver 0.0.0
-00001520: 2e30 3a38 3030 3020 2620 2023 2073 7461  .0:8000 &  # sta
-00001530: 7274 2073 6572 7665 720d 0a24 2070 7974  rt server..$ pyt
-00001540: 686f 6e20 6d61 6e61 6765 2e70 7920 6c6f  hon manage.py lo
-00001550: 6164 6461 7461 2066 6978 7475 7265 732f  addata fixtures/
-00001560: 6669 7874 7572 6573 2d64 6576 2e6a 736f  fixtures-dev.jso
-00001570: 6e0d 0a24 2063 6420 2e2e 2f65 3265 0d0a  n..$ cd ../e2e..
-00001580: 2420 7961 726e 2069 6e73 7461 6c6c 2020  $ yarn install  
-00001590: 2320 6f72 206e 706d 2069 6e73 7461 6c6c  # or npm install
-000015a0: 2028 6f6e 6c79 206e 6565 6465 6420 6669   (only needed fi
-000015b0: 7273 7420 7469 6d65 290d 0a24 2079 6172  rst time)..$ yar
-000015c0: 6e20 6379 7072 6573 7320 2023 206f 7220  n cypress  # or 
-000015d0: 6e70 6d20 7275 6e20 6379 7072 6573 730d  npm run cypress.
-000015e0: 0a60 6060 0d0a 0d0a 0d0a 2323 2049 6e73  .```......## Ins
-000015f0: 7461 6c6c 6174 696f 6e0d 0a0d 0a0d 0a0d  tallation.......
-00001600: 0a2d 2049 6e73 7461 6c6c 2074 6865 2070  .- Install the p
-00001610: 6163 6b61 6765 2076 6961 2070 6970 3a0d  ackage via pip:.
-00001620: 0a0d 0a20 2020 2060 6060 7069 7020 696e  ...    ```pip in
-00001630: 7374 616c 6c20 646a 616e 676f 2d64 796e  stall django-dyn
-00001640: 616d 6963 2d61 646d 696e 2d66 6f72 6d73  amic-admin-forms
-00001650: 6060 600d 0a0d 0a20 2020 206f 7220 7669  ```....    or vi
-00001660: 6120 7069 7065 6e76 3a0d 0a0d 0a20 2020  a pipenv:....   
-00001670: 2060 6060 7069 7065 6e76 2069 6e73 7461   ```pipenv insta
-00001680: 6c6c 2064 6a61 6e67 6f2d 6479 6e61 6d69  ll django-dynami
-00001690: 632d 6164 6d69 6e2d 666f 726d 7360 6060  c-admin-forms```
-000016a0: 0d0a 2d20 4164 6420 7468 6520 6d6f 6475  ..- Add the modu
-000016b0: 6c65 2074 6f20 6049 4e53 5441 4c4c 4544  le to `INSTALLED
-000016c0: 5f41 5050 5360 3a0d 0a20 2020 2060 6060  _APPS`:..    ```
-000016d0: 7079 7468 6f6e 0d0a 2020 2020 494e 5354  python..    INST
-000016e0: 414c 4c45 445f 4150 5053 203d 2028 0d0a  ALLED_APPS = (..
-000016f0: 2020 2020 2020 2020 2e2e 2e2c 0d0a 2020          ...,..  
-00001700: 2020 2020 2020 2764 6a61 6e67 6f5f 6479        'django_dy
-00001710: 6e61 6d69 635f 6164 6d69 6e5f 666f 726d  namic_admin_form
-00001720: 7327 2c0d 0a20 2020 2020 2020 2027 646a  s',..        'dj
-00001730: 616e 676f 2e63 6f6e 7472 6962 2e61 646d  ango.contrib.adm
-00001740: 696e 270d 0a20 2020 2020 2020 202e 2e2e  in'..        ...
-00001750: 0d0a 2020 2020 290d 0a20 2020 2060 6060  ..    )..    ```
-00001760: 0d0a 2020 2020 456e 7375 7265 2074 6861  ..    Ensure tha
-00001770: 7420 7468 6520 6064 796e 616d 6963 5f61  t the `dynamic_a
-00001780: 646d 696e 5f66 6f72 6d73 6020 636f 6d65  dmin_forms` come
-00001790: 7320 6265 666f 7265 2074 6865 0d0a 2020  s before the..  
-000017a0: 2020 6465 6661 756c 7420 6064 6a61 6e67    default `djang
-000017b0: 6f2e 636f 6e74 7269 622e 6164 6d69 6e60  o.contrib.admin`
-000017c0: 2069 6e20 7468 6520 6c69 7374 206f 6620   in the list of 
-000017d0: 696e 7374 616c 6c65 6420 6170 7073 2c0d  installed apps,.
-000017e0: 0a20 2020 2062 6563 6175 7365 206f 7468  .    because oth
-000017f0: 6572 7769 7365 2074 6865 2074 656d 706c  erwise the templ
-00001800: 6174 6573 2c20 7768 6963 6820 6172 6520  ates, which are 
-00001810: 6f76 6572 7772 6974 7465 6e20 6279 2060  overwritten by `
-00001820: 6479 6e61 6d69 635f 6164 6d69 6e5f 666f  dynamic_admin_fo
-00001830: 726d 7360 0d0a 2020 2020 776f 6e27 7420  rms`..    won't 
-00001840: 6265 2066 6f75 6e64 2e0d 0a2d 2045 6e73  be found...- Ens
-00001850: 7572 6520 7468 6174 2074 6865 2060 6479  ure that the `dy
-00001860: 6e61 6d69 635f 6164 6d69 6e5f 666f 726d  namic_admin_form
-00001870: 7360 2074 656d 706c 6174 6573 2061 7265  s` templates are
-00001880: 2066 6f75 6e64 2076 6961 2075 7369 6e67   found via using
-00001890: 2060 4150 505f 4449 5253 6020 7365 7474   `APP_DIRS` sett
-000018a0: 696e 673a 0d0a 2020 6060 6070 7974 686f  ing:..  ```pytho
-000018b0: 6e0d 0a20 2054 454d 504c 4154 4553 203d  n..  TEMPLATES =
-000018c0: 205b 0d0a 2020 2020 2020 7b0d 0a20 2020   [..      {..   
-000018d0: 2020 2020 2020 2027 4241 434b 454e 4427         'BACKEND'
-000018e0: 3a20 2764 6a61 6e67 6f2e 7465 6d70 6c61  : 'django.templa
-000018f0: 7465 2e62 6163 6b65 6e64 732e 646a 616e  te.backends.djan
-00001900: 676f 2e44 6a61 6e67 6f54 656d 706c 6174  go.DjangoTemplat
-00001910: 6573 272c 0d0a 2020 2020 2020 2020 2020  es',..          
-00001920: 2741 5050 5f44 4952 5327 3a20 5472 7565  'APP_DIRS': True
-00001930: 2c0d 0a20 2020 2020 2020 2020 202e 2e2e  ,..          ...
-00001940: 0d0a 2020 2020 2020 7d2c 0d0a 2020 5d0d  ..      },..  ].
-00001950: 0a20 2060 6060 0d0a 2d20 5275 6e20 6070  .  ```..- Run `p
-00001960: 7974 686f 6e20 6d61 6e61 6765 2e70 7920  ython manage.py 
-00001970: 636f 6c6c 6563 7473 7461 7469 6360 2074  collectstatic` t
-00001980: 6f20 696e 636c 7564 6520 7468 6973 2061  o include this a
-00001990: 7070 7320 4a61 7661 7363 7269 7074 2063  pps Javascript c
-000019a0: 6f64 6520 696e 2079 6f75 7220 6073 6574  ode in your `set
-000019b0: 7469 6e67 732e 5354 4154 4943 5f52 4f4f  tings.STATIC_ROO
-000019c0: 5460 2064 6972 6563 746f 7279 0d0a 0d0a  T` directory....
-000019d0: 0d0a 0d0a 2323 2043 6f6e 7472 6962 7574  ....## Contribut
-000019e0: 650d 0a0d 0a23 2323 2053 6574 7570 2070  e....### Setup p
-000019f0: 6163 6b61 6765 2066 6f72 2064 6576 656c  ackage for devel
-00001a00: 6f70 6d65 6e74 0d0a 0d0a 2d20 4372 6561  opment....- Crea
-00001a10: 7465 2061 2050 7974 686f 6e20 7669 7274  te a Python virt
-00001a20: 7561 6c65 6e76 2061 6e64 2061 6374 6976  ualenv and activ
-00001a30: 6174 6520 6974 0d0a 2d20 496e 7374 616c  ate it..- Instal
-00001a40: 6c20 2270 6970 2d74 6f6f 6c73 2220 7769  l "pip-tools" wi
-00001a50: 7468 2060 7069 7020 696e 7374 616c 6c20  th `pip install 
-00001a60: 2d55 2070 6970 2d74 6f6f 6c73 600d 0a2d  -U pip-tools`..-
-00001a70: 2043 6f6d 7069 6c65 2074 6865 2072 6571   Compile the req
-00001a80: 7569 7265 6d65 6e74 7320 7769 7468 2060  uirements with `
-00001a90: 7069 702d 636f 6d70 696c 6520 2d2d 6578  pip-compile --ex
-00001aa0: 7472 6120 6465 762c 202d 6f20 7265 7175  tra dev, -o requ
-00001ab0: 6972 656d 656e 7473 2e74 7874 2070 7970  irements.txt pyp
-00001ac0: 726f 6a65 6374 2e74 6f6d 6c20 2d2d 7265  roject.toml --re
-00001ad0: 736f 6c76 6572 3d62 6163 6b74 7261 636b  solver=backtrack
-00001ae0: 696e 6760 0d0a 2d20 5379 6e63 2074 6865  ing`..- Sync the
-00001af0: 2064 6570 656e 6465 6e63 6965 7320 7769   dependencies wi
-00001b00: 7468 2079 6f75 7220 7669 7274 7561 6c65  th your virtuale
-00001b10: 6e76 2077 6974 6820 6070 6970 2d73 796e  nv with `pip-syn
-00001b20: 6360 0d0a 0d0a 2323 2320 4164 6420 6675  c`....### Add fu
-00001b30: 6e63 7469 6f6e 616c 6974 790d 0a0d 0a2d  nctionality....-
-00001b40: 2043 7265 6174 6520 6120 6e65 7720 6272   Create a new br
-00001b50: 616e 6368 2066 6f72 2079 6f75 7220 6665  anch for your fe
-00001b60: 6174 7572 650d 0a2d 2043 6861 6e67 6520  ature..- Change 
-00001b70: 7468 6520 6465 7065 6e64 656e 6379 2069  the dependency i
-00001b80: 6e20 796f 7572 2072 6571 7569 7265 6d65  n your requireme
-00001b90: 6e74 732e 7478 7420 746f 2061 206c 6f63  nts.txt to a loc
-00001ba0: 616c 2028 6564 6974 6162 6c65 2920 6f6e  al (editable) on
-00001bb0: 6520 7468 6174 2070 6f69 6e74 7320 746f  e that points to
-00001bc0: 2079 6f75 7220 6c6f 6361 6c20 6669 6c65   your local file
-00001bd0: 2073 7973 7465 6d3a 0d0a 2020 602d 6520   system:..  `-e 
-00001be0: 2f55 7365 7273 2f77 6f72 6b73 7061 6365  /Users/workspace
-00001bf0: 2f64 6a61 6e67 6f2d 6479 6e61 6d69 632d  /django-dynamic-
-00001c00: 6164 6d69 6e2d 666f 726d 7360 206f 7220  admin-forms` or 
-00001c10: 7669 6120 7069 7020 2060 7069 7020 696e  via pip  `pip in
-00001c20: 7374 616c 6c20 2d65 202f 5573 6572 732f  stall -e /Users/
-00001c30: 776f 726b 7370 6163 652f 646a 616e 676f  workspace/django
-00001c40: 2d64 796e 616d 6963 2d61 646d 696e 2d66  -dynamic-admin-f
-00001c50: 6f72 6d73 600d 0a2d 2045 6e73 7572 6520  orms`..- Ensure 
-00001c60: 7468 6520 636f 6465 2070 6173 7365 7320  the code passes 
-00001c70: 7468 6520 7465 7374 730d 0a2d 2043 7265  the tests..- Cre
-00001c80: 6174 6520 6120 7075 6c6c 2072 6571 7565  ate a pull reque
-00001c90: 7374 0d0a 0d0a 2323 2320 5275 6e20 7465  st....### Run te
-00001ca0: 7374 730d 0a0d 0a2d 2052 756e 2074 6573  sts....- Run tes
-00001cb0: 7473 0d0a 2020 6060 6060 0d0a 2020 7079  ts..  ````..  py
-00001cc0: 7465 7374 202d 2d64 7320 7365 7474 696e  test --ds settin
-00001cd0: 6773 2074 6573 7473 0d0a 2020 6060 6060  gs tests..  ````
-00001ce0: 0d0a 0d0a 2d20 4368 6563 6b20 636f 7665  ....- Check cove
-00001cf0: 7261 6765 0d0a 2020 6060 6060 0d0a 2020  rage..  ````..  
-00001d00: 636f 7665 7261 6765 2072 756e 202d 6d20  coverage run -m 
-00001d10: 7079 7465 7374 202d 2d64 7320 7365 7474  pytest --ds sett
-00001d20: 696e 6773 2074 6573 7473 0d0a 2020 636f  ings tests..  co
-00001d30: 7665 7261 6765 2072 6570 6f72 7420 2d6d  verage report -m
-00001d40: 0d0a 2020 6060 6060 0d0a 0d0a 2323 2320  ..  ````....### 
-00001d50: 4769 7420 686f 6f6b 7320 2876 6961 2070  Git hooks (via p
-00001d60: 7265 2d63 6f6d 6d69 7429 0d0a 0d0a 5765  re-commit)....We
-00001d70: 2075 7365 2070 7265 2d70 7573 6820 686f   use pre-push ho
-00001d80: 6f6b 7320 746f 2065 6e73 7572 6520 7468  oks to ensure th
-00001d90: 6174 206f 6e6c 7920 6c69 6e74 6564 2063  at only linted c
-00001da0: 6f64 6520 7265 6163 6865 7320 6f75 7220  ode reaches our 
-00001db0: 7265 6d6f 7465 2072 6570 6f73 6974 6f72  remote repositor
-00001dc0: 7920 616e 6420 7069 7065 6c69 6e65 7320  y and pipelines 
-00001dd0: 6172 656e 2774 2074 7269 6767 6572 6564  aren't triggered
-00001de0: 2069 6e0d 0a76 6169 6e2e 0d0a 0d0a 546f   in..vain.....To
-00001df0: 2065 6e61 626c 6520 7468 6520 636f 6e66   enable the conf
-00001e00: 6967 7572 6564 2070 7265 2d70 7573 6820  igured pre-push 
-00001e10: 686f 6f6b 732c 2079 6f75 206e 6565 6420  hooks, you need 
-00001e20: 746f 205b 696e 7374 616c 6c5d 2868 7474  to [install](htt
-00001e30: 7073 3a2f 2f70 7265 2d63 6f6d 6d69 742e  ps://pre-commit.
-00001e40: 636f 6d2f 2920 7072 652d 636f 6d6d 6974  com/) pre-commit
-00001e50: 2061 6e64 2072 756e 206f 6e63 653a 0d0a   and run once:..
-00001e60: 0d0a 2020 2020 7072 652d 636f 6d6d 6974  ..    pre-commit
-00001e70: 2069 6e73 7461 6c6c 202d 7420 7072 652d   install -t pre-
-00001e80: 7075 7368 202d 7420 7072 652d 636f 6d6d  push -t pre-comm
-00001e90: 6974 202d 2d69 6e73 7461 6c6c 2d68 6f6f  it --install-hoo
-00001ea0: 6b73 0d0a 0d0a 5468 6973 2077 696c 6c20  ks....This will 
-00001eb0: 7065 726d 616e 656e 746c 7920 696e 7374  permanently inst
-00001ec0: 616c 6c20 7468 6520 6769 7420 686f 6f6b  all the git hook
-00001ed0: 7320 666f 7220 626f 7468 2c20 6672 6f6e  s for both, fron
-00001ee0: 7465 6e64 2061 6e64 2062 6163 6b65 6e64  tend and backend
-00001ef0: 2c20 696e 2079 6f75 7220 6c6f 6361 6c0d  , in your local.
-00001f00: 0a5b 602e 6769 742f 686f 6f6b 7360 5d28  .[`.git/hooks`](
-00001f10: 2e2f 2e67 6974 2f68 6f6f 6b73 2920 666f  ./.git/hooks) fo
-00001f20: 6c64 6572 2e0d 0a54 6865 2068 6f6f 6b73  lder...The hooks
-00001f30: 2061 7265 2063 6f6e 6669 6775 7265 6420   are configured 
-00001f40: 696e 2074 6865 205b 602e 7072 652d 636f  in the [`.pre-co
-00001f50: 6d6d 6974 2d63 6f6e 6669 672e 7961 6d6c  mmit-config.yaml
-00001f60: 605d 2874 656d 706c 6174 6573 2f2e 7072  `](templates/.pr
-00001f70: 652d 636f 6d6d 6974 2d63 6f6e 6669 672e  e-commit-config.
-00001f80: 7961 6d6c 2e74 706c 292e 0d0a 0d0a 596f  yaml.tpl).....Yo
-00001f90: 7520 6361 6e20 6368 6563 6b20 7768 6574  u can check whet
-00001fa0: 6865 7220 686f 6f6b 7320 776f 726b 2061  her hooks work a
-00001fb0: 7320 696e 7465 6e64 6564 2075 7369 6e67  s intended using
-00001fc0: 2074 6865 205b 7275 6e5d 2868 7474 7073   the [run](https
-00001fd0: 3a2f 2f70 7265 2d63 6f6d 6d69 742e 636f  ://pre-commit.co
-00001fe0: 6d2f 2370 7265 2d63 6f6d 6d69 742d 7275  m/#pre-commit-ru
-00001ff0: 6e29 2063 6f6d 6d61 6e64 3a0d 0a0d 0a20  n) command:.... 
-00002000: 2020 2070 7265 2d63 6f6d 6d69 7420 7275     pre-commit ru
-00002010: 6e20 5b68 6f6f 6b2d 6964 5d20 5b6f 7074  n [hook-id] [opt
-00002020: 696f 6e73 5d0d 0a0d 0a45 7861 6d70 6c65  ions]....Example
-00002030: 3a20 7275 6e20 7369 6e67 6c65 2068 6f6f  : run single hoo
-00002040: 6b0d 0a0d 0a20 2020 2070 7265 2d63 6f6d  k....    pre-com
-00002050: 6d69 7420 7275 6e20 7275 6666 202d 2d61  mit run ruff --a
-00002060: 6c6c 2d66 696c 6573 202d 2d68 6f6f 6b2d  ll-files --hook-
-00002070: 7374 6167 6520 7075 7368 0d0a 0d0a 4578  stage push....Ex
-00002080: 616d 706c 653a 2072 756e 2061 6c6c 2068  ample: run all h
-00002090: 6f6f 6b73 206f 6620 7072 652d 7075 7368  ooks of pre-push
-000020a0: 2073 7461 6765 0d0a 0d0a 2020 2020 7072   stage....    pr
-000020b0: 652d 636f 6d6d 6974 2072 756e 202d 2d61  e-commit run --a
-000020c0: 6c6c 2d66 696c 6573 202d 2d68 6f6f 6b2d  ll-files --hook-
-000020d0: 7374 6167 6520 7075 7368 0d0a 0d0a 2323  stage push....##
-000020e0: 2320 5570 6461 7465 2064 6f63 756d 656e  # Update documen
-000020f0: 7461 7469 6f6e 0d0a 0d0a 2d20 546f 2062  tation....- To b
-00002100: 7569 6c64 2074 6865 2064 6f63 756d 656e  uild the documen
-00002110: 7461 7469 6f6e 2072 756e 3a20 6073 7068  tation run: `sph
-00002120: 696e 782d 6275 696c 6420 646f 6373 2f20  inx-build docs/ 
-00002130: 646f 6373 2f5f 6275 696c 642f 6874 6d6c  docs/_build/html
-00002140: 2f60 2e0d 0a2d 204f 7065 6e20 6064 6f63  /`...- Open `doc
-00002150: 732f 5f62 7569 6c64 2f68 746d 6c2f 696e  s/_build/html/in
-00002160: 6465 782e 6874 6d6c 6020 746f 2073 6565  dex.html` to see
-00002170: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00002180: 6f6e 2e0d 0a0d 0a23 2323 2054 7261 6e73  on.....### Trans
-00002190: 6c61 7469 6f6e 2066 696c 6573 0d0a 0d0a  lation files....
-000021a0: 4966 2079 6f75 2068 6176 6520 6164 6465  If you have adde
-000021b0: 6420 6375 7374 6f6d 2074 6578 742c 206d  d custom text, m
-000021c0: 616b 6520 7375 7265 2074 6f20 7772 6170  ake sure to wrap
-000021d0: 2069 7420 696e 2060 5f28 2960 2077 6865   it in `_()` whe
-000021e0: 7265 2060 5f60 2069 730d 0a67 6574 7465  re `_` is..gette
-000021f0: 7874 5f6c 617a 7920 2860 6672 6f6d 2064  xt_lazy (`from d
-00002200: 6a61 6e67 6f2e 7574 696c 732e 7472 616e  jango.utils.tran
-00002210: 736c 6174 696f 6e20 696d 706f 7274 2067  slation import g
-00002220: 6574 7465 7874 5f6c 617a 7920 6173 205f  ettext_lazy as _
-00002230: 6029 2e0d 0a0d 0a48 6f77 2074 6f20 6372  `).....How to cr
-00002240: 6561 7465 2074 7261 6e73 6c61 7469 6f6e  eate translation
-00002250: 2066 696c 653a 0d0a 0d0a 2a20 4e61 7669   file:....* Navi
-00002260: 6761 7465 2074 6f20 6064 6a61 6e67 6f2d  gate to `django-
-00002270: 6479 6e61 6d69 632d 6164 6d69 6e2d 666f  dynamic-admin-fo
-00002280: 726d 7360 0d0a 2a20 6070 7974 686f 6e20  rms`..* `python 
-00002290: 6d61 6e61 6765 2e70 7920 6d61 6b65 6d65  manage.py makeme
-000022a0: 7373 6167 6573 202d 6c20 6465 600d 0a2a  ssages -l de`..*
-000022b0: 2048 6176 6520 6120 6c6f 6f6b 2061 7420   Have a look at 
-000022c0: 7468 6520 6e65 772f 6368 616e 6765 6420  the new/changed 
-000022d0: 6669 6c65 7320 7769 7468 696e 2060 646a  files within `dj
-000022e0: 616e 676f 5f64 796e 616d 6963 5f61 646d  ango_dynamic_adm
-000022f0: 696e 5f66 6f72 6d73 2f6c 6f63 616c 6560  in_forms/locale`
-00002300: 0d0a 0d0a 486f 7720 746f 2063 6f6d 7069  ....How to compi
-00002310: 6c65 2074 7261 6e73 6c61 7469 6f6e 2066  le translation f
-00002320: 696c 6573 3a0d 0a0d 0a2a 204e 6176 6967  iles:....* Navig
-00002330: 6174 6520 746f 2060 646a 616e 676f 2d64  ate to `django-d
-00002340: 796e 616d 6963 2d61 646d 696e 2d66 6f72  ynamic-admin-for
-00002350: 6d73 600d 0a2a 2060 7079 7468 6f6e 206d  ms`..* `python m
-00002360: 616e 6167 652e 7079 2063 6f6d 7069 6c65  anage.py compile
-00002370: 6d65 7373 6167 6573 600d 0a2a 2048 6176  messages`..* Hav
-00002380: 6520 6120 6c6f 6f6b 2061 7420 7468 6520  e a look at the 
-00002390: 6e65 772f 6368 616e 6765 6420 6669 6c65  new/changed file
-000023a0: 7320 7769 7468 696e 2060 646a 616e 676f  s within `django
-000023b0: 5f64 796e 616d 6963 5f61 646d 696e 5f66  _dynamic_admin_f
-000023c0: 6f72 6d73 2f6c 6f63 616c 6560 0d0a 0d0a  orms/locale`....
-000023d0: 2323 2320 5075 626c 6973 6820 746f 2052  ### Publish to R
-000023e0: 6561 6454 6865 446f 6373 2e69 6f0d 0a0d  eadTheDocs.io...
-000023f0: 0a2d 2046 6574 6368 2074 6865 206c 6174  .- Fetch the lat
-00002400: 6573 7420 6368 616e 6765 7320 696e 2047  est changes in G
-00002410: 6974 4875 6220 6d69 7272 6f72 2061 6e64  itHub mirror and
-00002420: 2070 7573 6820 7468 656d 0d0a 2d20 5472   push them..- Tr
-00002430: 6967 6765 7220 6e65 7720 6275 696c 6420  igger new build 
-00002440: 6174 2052 6561 6454 6865 446f 6373 2e69  at ReadTheDocs.i
-00002450: 6f20 2866 6f6c 6c6f 7720 696e 7374 7275  o (follow instru
-00002460: 6374 696f 6e73 2069 6e20 6164 6d69 6e20  ctions in admin 
-00002470: 7061 6e65 6c20 6174 2052 5444 2920 6966  panel at RTD) if
-00002480: 2074 6865 2047 6974 4875 6220 7765 6268   the GitHub webh
-00002490: 6f6f 6b20 6973 206e 6f74 2079 6574 2073  ook is not yet s
-000024a0: 6574 0d0a 2020 7570 2e0d 0a0d 0a23 2323  et..  up.....###
-000024b0: 2050 7562 6c69 7368 2074 6f20 5079 5069   Publish to PyPi
-000024c0: 0d0a 0d0a 2d20 5570 6461 7465 2064 6f63  ....- Update doc
-000024d0: 756d 656e 7461 7469 6f6e 2061 626f 7574  umentation about
-000024e0: 206e 6577 2f63 6861 6e67 6564 2066 756e   new/changed fun
-000024f0: 6374 696f 6e61 6c69 7479 0d0a 0d0a 2d20  ctionality....- 
-00002500: 5570 6461 7465 2074 6865 2060 4368 616e  Update the `Chan
-00002510: 6765 6c6f 6760 0d0a 0d0a 2d20 496e 6372  gelog`....- Incr
-00002520: 656d 656e 7420 7665 7273 696f 6e20 696e  ement version in
-00002530: 206d 6169 6e20 605f 5f69 6e69 745f 5f2e   main `__init__.
-00002540: 7079 600d 0a0d 0a2d 2043 7265 6174 6520  py`....- Create 
-00002550: 7075 6c6c 2072 6571 7565 7374 202f 206d  pull request / m
-00002560: 6572 6765 2074 6f20 6d61 7374 6572 0d0a  erge to master..
-00002570: 0d0a 2d20 5468 6973 2070 726f 6a65 6374  ..- This project
-00002580: 2075 7365 7320 7468 6520 666c 6974 2070   uses the flit p
-00002590: 6163 6b61 6765 2074 6f20 7075 626c 6973  ackage to publis
-000025a0: 6820 746f 2050 7950 492e 2054 6875 7320  h to PyPI. Thus 
-000025b0: 7075 626c 6973 6869 6e67 2073 686f 756c  publishing shoul
-000025c0: 6420 6265 2061 7320 6561 7379 2061 7320  d be as easy as 
-000025d0: 7275 6e6e 696e 673a 0d0a 2020 6060 600d  running:..  ```.
-000025e0: 0a20 2066 6c69 7420 7075 626c 6973 680d  .  flit publish.
-000025f0: 0a20 2060 6060 0d0a 0d0a 2020 546f 2070  .  ```....  To p
-00002600: 7562 6c69 7368 2074 6f20 5465 7374 5079  ublish to TestPy
-00002610: 5049 2075 7365 2074 6865 2066 6f6c 6c6f  PI use the follo
-00002620: 7769 6e67 2065 6e73 7572 6520 7468 6174  wing ensure that
-00002630: 2079 6f75 2068 6176 6520 7365 7420 7570   you have set up
-00002640: 2079 6f75 7220 2e70 7970 6972 6320 6173   your .pypirc as
-00002650: 0d0a 2020 7368 6f77 6e20 5b68 6572 655d  ..  shown [here]
-00002660: 2868 7474 7073 3a2f 2f66 6c69 742e 7265  (https://flit.re
-00002670: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00002680: 6c61 7465 7374 2f75 706c 6f61 642e 6874  latest/upload.ht
-00002690: 6d6c 2375 7369 6e67 2d70 7970 6972 6329  ml#using-pypirc)
-000026a0: 2061 6e64 2075 7365 2074 6865 2066 6f6c   and use the fol
-000026b0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0d  lowing command:.
-000026c0: 0a0d 0a20 2060 6060 0d0a 2020 666c 6974  ...  ```..  flit
-000026d0: 2070 7562 6c69 7368 202d 2d72 6570 6f73   publish --repos
-000026e0: 6974 6f72 7920 7465 7374 7079 7069 0d0a  itory testpypi..
-000026f0: 2020 6060 600d 0a0d 0a23 2323 204d 6169    ```....### Mai
-00002700: 6e74 656e 616e 6365 0d0a 0d0a 506c 6561  ntenance....Plea
-00002710: 7365 206e 6f74 6520 7468 6174 2074 6869  se note that thi
-00002720: 7320 7061 636b 6167 6520 7375 7070 6f72  s package suppor
-00002730: 7473 2074 6865 205b 616d 6269 656e 742d  ts the [ambient-
-00002740: 7061 636b 6167 652d 7570 6461 7465 5d28  package-update](
-00002750: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00002760: 2f70 726f 6a65 6374 2f61 6d62 6965 6e74  /project/ambient
-00002770: 2d70 6163 6b61 6765 2d75 7064 6174 652f  -package-update/
-00002780: 292e 0d0a 536f 2079 6f75 2064 6f6e 2774  )...So you don't
-00002790: 2068 6176 6520 746f 2077 6f72 7279 2061   have to worry a
-000027a0: 626f 7574 2074 6865 206d 6169 6e74 656e  bout the mainten
-000027b0: 616e 6365 206f 6620 7468 6973 2070 6163  ance of this pac
-000027c0: 6b61 6765 2e20 416c 6c20 696d 706f 7274  kage. All import
-000027d0: 616e 7420 636f 6e66 6967 7572 6174 696f  ant configuratio
-000027e0: 6e20 616e 6420 7365 7475 7020 6669 6c65  n and setup file
-000027f0: 7320 6172 650d 0a62 6569 6e67 2072 656e  s are..being ren
-00002800: 6465 7265 6420 6279 2074 6869 7320 7570  dered by this up
-00002810: 6461 7465 722e 2049 7420 776f 726b 7320  dater. It works 
-00002820: 7369 6d69 6c61 7220 746f 2077 656c 6c2d  similar to well-
-00002830: 6b6e 6f77 6e20 7570 6461 7465 7273 206c  known updaters l
-00002840: 696b 6520 6070 7975 7067 7261 6465 6020  ike `pyupgrade` 
-00002850: 6f72 2060 646a 616e 676f 2d75 7067 7261  or `django-upgra
-00002860: 6465 602e 0d0a 0d0a 546f 2072 756e 2061  de`.....To run a
-00002870: 6e20 7570 6461 7465 2c20 7265 6665 7220  n update, refer 
-00002880: 746f 2074 6865 205b 646f 6375 6d65 6e74  to the [document
-00002890: 6174 696f 6e20 7061 6765 5d28 6874 7470  ation page](http
-000028a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000028b0: 6a65 6374 2f61 6d62 6965 6e74 2d70 6163  ject/ambient-pac
-000028c0: 6b61 6765 2d75 7064 6174 652f 290d 0a6f  kage-update/)..o
-000028d0: 6620 7468 6520 2261 6d62 6965 6e74 2d70  f the "ambient-p
-000028e0: 6163 6b61 6765 2d75 7064 6174 6522 2e0d  ackage-update"..
-000028f0: 0a                                       .
+000012e0: 7072 6f6a 0d0a 2420 7079 7468 6f6e 3320  proj..$ python3 
+000012f0: 2d6d 2076 656e 7620 2e76 656e 760d 0a24  -m venv .venv..$
+00001300: 2073 6f75 7263 6520 2e76 656e 762f 6269   source .venv/bi
+00001310: 6e2f 6163 7469 7661 7465 0d0a 2420 6364  n/activate..$ cd
+00001320: 202e 2e0d 0a24 2066 6c69 7420 696e 7374   ....$ flit inst
+00001330: 616c 6c20 2d2d 7379 6d6c 696e 6b0d 0a60  all --symlink..`
+00001340: 6060 0d0a 4e6f 7720 7468 6520 7061 636b  ``..Now the pack
+00001350: 6167 6520 7368 6f75 6c64 2062 6520 6176  age should be av
+00001360: 6169 6c61 626c 6520 696e 2079 6f75 7220  ailable in your 
+00001370: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00001380: 656e 740d 0a61 6e64 2061 6e79 2063 6861  ent..and any cha
+00001390: 6e67 6573 2073 686f 756c 6420 6265 2064  nges should be d
+000013a0: 6972 6563 746c 7920 7669 7369 626c 652e  irectly visible.
+000013b0: 0d0a 0d0a 416c 7465 726e 6174 6976 656c  ....Alternativel
+000013c0: 792c 2063 6f70 7920 7468 6520 6469 7265  y, copy the dire
+000013d0: 6374 6f72 7920 6064 796e 616d 6963 5f61  ctory `dynamic_a
+000013e0: 646d 696e 5f66 6f72 6d73 600d 0a69 6e74  dmin_forms`..int
+000013f0: 6f20 616e 7920 6e6f 726d 616c 2064 6a61  o any normal dja
+00001400: 6e67 6f20 7072 6f6a 6563 742c 2073 6f20  ngo project, so 
+00001410: 7468 6174 2074 6865 2070 7974 686f 6e20  that the python 
+00001420: 696e 7465 7270 7265 7465 720d 0a66 696e  interpreter..fin
+00001430: 6473 2074 6865 206c 6f63 616c 2076 6572  ds the local ver
+00001440: 7369 6f6e 2069 6e73 7465 6164 206f 6620  sion instead of 
+00001450: 7468 6520 696e 7374 616c 6c65 6420 286f  the installed (o
+00001460: 6c64 2920 7665 7273 696f 6e2e 0d0a 0d0a  ld) version.....
+00001470: 2323 2052 756e 6e69 6e67 2045 3245 2074  ## Running E2E t
+00001480: 6573 7473 0d0a 0d0a 546f 2072 756e 2065  ests....To run e
+00001490: 6e64 2d74 6f2d 656e 6420 7465 7374 7320  nd-to-end tests 
+000014a0: 6c6f 6361 6c6c 793a 0d0a 6060 6073 6865  locally:..```she
+000014b0: 6c6c 0d0a 2420 6364 2074 6573 7470 726f  ll..$ cd testpro
+000014c0: 6a0d 0a24 2070 7974 686f 6e20 6d61 6e61  j..$ python mana
+000014d0: 6765 2e70 7920 7275 6e73 6572 7665 7220  ge.py runserver 
+000014e0: 302e 302e 302e 303a 3830 3030 2026 2020  0.0.0.0:8000 &  
+000014f0: 2320 7374 6172 7420 7365 7276 6572 0d0a  # start server..
+00001500: 2420 7079 7468 6f6e 206d 616e 6167 652e  $ python manage.
+00001510: 7079 206c 6f61 6464 6174 6120 6669 7874  py loaddata fixt
+00001520: 7572 6573 2f66 6978 7475 7265 732d 6465  ures/fixtures-de
+00001530: 762e 6a73 6f6e 0d0a 2420 6364 202e 2e2f  v.json..$ cd ../
+00001540: 6532 650d 0a24 2079 6172 6e20 696e 7374  e2e..$ yarn inst
+00001550: 616c 6c20 2023 206f 7220 6e70 6d20 696e  all  # or npm in
+00001560: 7374 616c 6c20 286f 6e6c 7920 6e65 6564  stall (only need
+00001570: 6564 2066 6972 7374 2074 696d 6529 0d0a  ed first time)..
+00001580: 2420 7961 726e 2063 7970 7265 7373 2020  $ yarn cypress  
+00001590: 2320 6f72 206e 706d 2072 756e 2063 7970  # or npm run cyp
+000015a0: 7265 7373 0d0a 6060 600d 0a0d 0a0d 0a23  ress..```......#
+000015b0: 2320 496e 7374 616c 6c61 7469 6f6e 0d0a  # Installation..
+000015c0: 0d0a 0d0a 0d0a 2d20 496e 7374 616c 6c20  ......- Install 
+000015d0: 7468 6520 7061 636b 6167 6520 7669 6120  the package via 
+000015e0: 7069 703a 0d0a 0d0a 2020 2020 6060 6070  pip:....    ```p
+000015f0: 6970 2069 6e73 7461 6c6c 2064 6a61 6e67  ip install djang
+00001600: 6f2d 6479 6e61 6d69 632d 6164 6d69 6e2d  o-dynamic-admin-
+00001610: 666f 726d 7360 6060 0d0a 0d0a 2020 2020  forms```....    
+00001620: 6f72 2076 6961 2070 6970 656e 763a 0d0a  or via pipenv:..
+00001630: 0d0a 2020 2020 6060 6070 6970 656e 7620  ..    ```pipenv 
+00001640: 696e 7374 616c 6c20 646a 616e 676f 2d64  install django-d
+00001650: 796e 616d 6963 2d61 646d 696e 2d66 6f72  ynamic-admin-for
+00001660: 6d73 6060 600d 0a2d 2041 6464 2074 6865  ms```..- Add the
+00001670: 206d 6f64 756c 6520 746f 2060 494e 5354   module to `INST
+00001680: 414c 4c45 445f 4150 5053 603a 0d0a 2020  ALLED_APPS`:..  
+00001690: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
+000016a0: 2049 4e53 5441 4c4c 4544 5f41 5050 5320   INSTALLED_APPS 
+000016b0: 3d20 280d 0a20 2020 2020 2020 202e 2e2e  = (..        ...
+000016c0: 2c0d 0a20 2020 2020 2020 2027 646a 616e  ,..        'djan
+000016d0: 676f 5f64 796e 616d 6963 5f61 646d 696e  go_dynamic_admin
+000016e0: 5f66 6f72 6d73 272c 0d0a 2020 2020 2020  _forms',..      
+000016f0: 2020 2764 6a61 6e67 6f2e 636f 6e74 7269    'django.contri
+00001700: 622e 6164 6d69 6e27 0d0a 2020 2020 2020  b.admin'..      
+00001710: 2020 2e2e 2e0d 0a20 2020 2029 0d0a 2020    .....    )..  
+00001720: 2020 6060 600d 0a20 2020 2045 6e73 7572    ```..    Ensur
+00001730: 6520 7468 6174 2074 6865 2060 6479 6e61  e that the `dyna
+00001740: 6d69 635f 6164 6d69 6e5f 666f 726d 7360  mic_admin_forms`
+00001750: 2063 6f6d 6573 2062 6566 6f72 6520 7468   comes before th
+00001760: 650d 0a20 2020 2064 6566 6175 6c74 2060  e..    default `
+00001770: 646a 616e 676f 2e63 6f6e 7472 6962 2e61  django.contrib.a
+00001780: 646d 696e 6020 696e 2074 6865 206c 6973  dmin` in the lis
+00001790: 7420 6f66 2069 6e73 7461 6c6c 6564 2061  t of installed a
+000017a0: 7070 732c 0d0a 2020 2020 6265 6361 7573  pps,..    becaus
+000017b0: 6520 6f74 6865 7277 6973 6520 7468 6520  e otherwise the 
+000017c0: 7465 6d70 6c61 7465 732c 2077 6869 6368  templates, which
+000017d0: 2061 7265 206f 7665 7277 7269 7474 656e   are overwritten
+000017e0: 2062 7920 6064 796e 616d 6963 5f61 646d   by `dynamic_adm
+000017f0: 696e 5f66 6f72 6d73 600d 0a20 2020 2077  in_forms`..    w
+00001800: 6f6e 2774 2062 6520 666f 756e 642e 0d0a  on't be found...
+00001810: 2d20 456e 7375 7265 2074 6861 7420 7468  - Ensure that th
+00001820: 6520 6064 796e 616d 6963 5f61 646d 696e  e `dynamic_admin
+00001830: 5f66 6f72 6d73 6020 7465 6d70 6c61 7465  _forms` template
+00001840: 7320 6172 6520 666f 756e 6420 7669 6120  s are found via 
+00001850: 7573 696e 6720 6041 5050 5f44 4952 5360  using `APP_DIRS`
+00001860: 2073 6574 7469 6e67 3a0d 0a20 2060 6060   setting:..  ```
+00001870: 7079 7468 6f6e 0d0a 2020 5445 4d50 4c41  python..  TEMPLA
+00001880: 5445 5320 3d20 5b0d 0a20 2020 2020 207b  TES = [..      {
+00001890: 0d0a 2020 2020 2020 2020 2020 2742 4143  ..          'BAC
+000018a0: 4b45 4e44 273a 2027 646a 616e 676f 2e74  KEND': 'django.t
+000018b0: 656d 706c 6174 652e 6261 636b 656e 6473  emplate.backends
+000018c0: 2e64 6a61 6e67 6f2e 446a 616e 676f 5465  .django.DjangoTe
+000018d0: 6d70 6c61 7465 7327 2c0d 0a20 2020 2020  mplates',..     
+000018e0: 2020 2020 2027 4150 505f 4449 5253 273a       'APP_DIRS':
+000018f0: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
+00001900: 2020 2e2e 2e0d 0a20 2020 2020 207d 2c0d    .....      },.
+00001910: 0a20 205d 0d0a 2020 6060 600d 0a2d 2052  .  ]..  ```..- R
+00001920: 756e 2060 7079 7468 6f6e 206d 616e 6167  un `python manag
+00001930: 652e 7079 2063 6f6c 6c65 6374 7374 6174  e.py collectstat
+00001940: 6963 6020 746f 2069 6e63 6c75 6465 2074  ic` to include t
+00001950: 6869 7320 6170 7073 204a 6176 6173 6372  his apps Javascr
+00001960: 6970 7420 636f 6465 2069 6e20 796f 7572  ipt code in your
+00001970: 2060 7365 7474 696e 6773 2e53 5441 5449   `settings.STATI
+00001980: 435f 524f 4f54 6020 6469 7265 6374 6f72  C_ROOT` director
+00001990: 790d 0a0d 0a0d 0a0d 0a23 2320 436f 6e74  y........## Cont
+000019a0: 7269 6275 7465 0d0a 0d0a 2323 2320 5365  ribute....### Se
+000019b0: 7475 7020 7061 636b 6167 6520 666f 7220  tup package for 
+000019c0: 6465 7665 6c6f 706d 656e 740d 0a0d 0a2d  development....-
+000019d0: 2043 7265 6174 6520 6120 5079 7468 6f6e   Create a Python
+000019e0: 2076 6972 7475 616c 656e 7620 616e 6420   virtualenv and 
+000019f0: 6163 7469 7661 7465 2069 740d 0a2d 2049  activate it..- I
+00001a00: 6e73 7461 6c6c 2022 7069 702d 746f 6f6c  nstall "pip-tool
+00001a10: 7322 2077 6974 6820 6070 6970 2069 6e73  s" with `pip ins
+00001a20: 7461 6c6c 202d 5520 7069 702d 746f 6f6c  tall -U pip-tool
+00001a30: 7360 0d0a 2d20 436f 6d70 696c 6520 7468  s`..- Compile th
+00001a40: 6520 7265 7175 6972 656d 656e 7473 2077  e requirements w
+00001a50: 6974 6820 6070 6970 2d63 6f6d 7069 6c65  ith `pip-compile
+00001a60: 202d 2d65 7874 7261 2064 6576 2c20 2d6f   --extra dev, -o
+00001a70: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+00001a80: 7420 7079 7072 6f6a 6563 742e 746f 6d6c  t pyproject.toml
+00001a90: 202d 2d72 6573 6f6c 7665 723d 6261 636b   --resolver=back
+00001aa0: 7472 6163 6b69 6e67 600d 0a2d 2053 796e  tracking`..- Syn
+00001ab0: 6320 7468 6520 6465 7065 6e64 656e 6369  c the dependenci
+00001ac0: 6573 2077 6974 6820 796f 7572 2076 6972  es with your vir
+00001ad0: 7475 616c 656e 7620 7769 7468 2060 7069  tualenv with `pi
+00001ae0: 702d 7379 6e63 600d 0a0d 0a23 2323 2041  p-sync`....### A
+00001af0: 6464 2066 756e 6374 696f 6e61 6c69 7479  dd functionality
+00001b00: 0d0a 0d0a 2d20 4372 6561 7465 2061 206e  ....- Create a n
+00001b10: 6577 2062 7261 6e63 6820 666f 7220 796f  ew branch for yo
+00001b20: 7572 2066 6561 7475 7265 0d0a 2d20 4368  ur feature..- Ch
+00001b30: 616e 6765 2074 6865 2064 6570 656e 6465  ange the depende
+00001b40: 6e63 7920 696e 2079 6f75 7220 7265 7175  ncy in your requ
+00001b50: 6972 656d 656e 7473 2e74 7874 2074 6f20  irements.txt to 
+00001b60: 6120 6c6f 6361 6c20 2865 6469 7461 626c  a local (editabl
+00001b70: 6529 206f 6e65 2074 6861 7420 706f 696e  e) one that poin
+00001b80: 7473 2074 6f20 796f 7572 206c 6f63 616c  ts to your local
+00001b90: 2066 696c 6520 7379 7374 656d 3a0d 0a20   file system:.. 
+00001ba0: 2060 2d65 202f 5573 6572 732f 776f 726b   `-e /Users/work
+00001bb0: 7370 6163 652f 646a 616e 676f 2d64 796e  space/django-dyn
+00001bc0: 616d 6963 2d61 646d 696e 2d66 6f72 6d73  amic-admin-forms
+00001bd0: 6020 6f72 2076 6961 2070 6970 2020 6070  ` or via pip  `p
+00001be0: 6970 2069 6e73 7461 6c6c 202d 6520 2f55  ip install -e /U
+00001bf0: 7365 7273 2f77 6f72 6b73 7061 6365 2f64  sers/workspace/d
+00001c00: 6a61 6e67 6f2d 6479 6e61 6d69 632d 6164  jango-dynamic-ad
+00001c10: 6d69 6e2d 666f 726d 7360 0d0a 2d20 456e  min-forms`..- En
+00001c20: 7375 7265 2074 6865 2063 6f64 6520 7061  sure the code pa
+00001c30: 7373 6573 2074 6865 2074 6573 7473 0d0a  sses the tests..
+00001c40: 2d20 4372 6561 7465 2061 2070 756c 6c20  - Create a pull 
+00001c50: 7265 7175 6573 740d 0a0d 0a23 2323 2052  request....### R
+00001c60: 756e 2074 6573 7473 0d0a 0d0a 2d20 5275  un tests....- Ru
+00001c70: 6e20 7465 7374 730d 0a20 2060 6060 600d  n tests..  ````.
+00001c80: 0a20 2070 7974 6573 7420 2d2d 6473 2073  .  pytest --ds s
+00001c90: 6574 7469 6e67 7320 7465 7374 730d 0a20  ettings tests.. 
+00001ca0: 2060 6060 600d 0a0d 0a2d 2043 6865 636b   ````....- Check
+00001cb0: 2063 6f76 6572 6167 650d 0a20 2060 6060   coverage..  ```
+00001cc0: 600d 0a20 2063 6f76 6572 6167 6520 7275  `..  coverage ru
+00001cd0: 6e20 2d6d 2070 7974 6573 7420 2d2d 6473  n -m pytest --ds
+00001ce0: 2073 6574 7469 6e67 7320 7465 7374 730d   settings tests.
+00001cf0: 0a20 2063 6f76 6572 6167 6520 7265 706f  .  coverage repo
+00001d00: 7274 202d 6d0d 0a20 2060 6060 600d 0a0d  rt -m..  ````...
+00001d10: 0a23 2323 2047 6974 2068 6f6f 6b73 2028  .### Git hooks (
+00001d20: 7669 6120 7072 652d 636f 6d6d 6974 290d  via pre-commit).
+00001d30: 0a0d 0a57 6520 7573 6520 7072 652d 7075  ...We use pre-pu
+00001d40: 7368 2068 6f6f 6b73 2074 6f20 656e 7375  sh hooks to ensu
+00001d50: 7265 2074 6861 7420 6f6e 6c79 206c 696e  re that only lin
+00001d60: 7465 6420 636f 6465 2072 6561 6368 6573  ted code reaches
+00001d70: 206f 7572 2072 656d 6f74 6520 7265 706f   our remote repo
+00001d80: 7369 746f 7279 2061 6e64 2070 6970 656c  sitory and pipel
+00001d90: 696e 6573 2061 7265 6e27 7420 7472 6967  ines aren't trig
+00001da0: 6765 7265 6420 696e 0d0a 7661 696e 2e0d  gered in..vain..
+00001db0: 0a0d 0a54 6f20 656e 6162 6c65 2074 6865  ...To enable the
+00001dc0: 2063 6f6e 6669 6775 7265 6420 7072 652d   configured pre-
+00001dd0: 7075 7368 2068 6f6f 6b73 2c20 796f 7520  push hooks, you 
+00001de0: 6e65 6564 2074 6f20 5b69 6e73 7461 6c6c  need to [install
+00001df0: 5d28 6874 7470 733a 2f2f 7072 652d 636f  ](https://pre-co
+00001e00: 6d6d 6974 2e63 6f6d 2f29 2070 7265 2d63  mmit.com/) pre-c
+00001e10: 6f6d 6d69 7420 616e 6420 7275 6e20 6f6e  ommit and run on
+00001e20: 6365 3a0d 0a0d 0a20 2020 2070 7265 2d63  ce:....    pre-c
+00001e30: 6f6d 6d69 7420 696e 7374 616c 6c20 2d74  ommit install -t
+00001e40: 2070 7265 2d70 7573 6820 2d74 2070 7265   pre-push -t pre
+00001e50: 2d63 6f6d 6d69 7420 2d2d 696e 7374 616c  -commit --instal
+00001e60: 6c2d 686f 6f6b 730d 0a0d 0a54 6869 7320  l-hooks....This 
+00001e70: 7769 6c6c 2070 6572 6d61 6e65 6e74 6c79  will permanently
+00001e80: 2069 6e73 7461 6c6c 2074 6865 2067 6974   install the git
+00001e90: 2068 6f6f 6b73 2066 6f72 2062 6f74 682c   hooks for both,
+00001ea0: 2066 726f 6e74 656e 6420 616e 6420 6261   frontend and ba
+00001eb0: 636b 656e 642c 2069 6e20 796f 7572 206c  ckend, in your l
+00001ec0: 6f63 616c 0d0a 5b60 2e67 6974 2f68 6f6f  ocal..[`.git/hoo
+00001ed0: 6b73 605d 282e 2f2e 6769 742f 686f 6f6b  ks`](./.git/hook
+00001ee0: 7329 2066 6f6c 6465 722e 0d0a 5468 6520  s) folder...The 
+00001ef0: 686f 6f6b 7320 6172 6520 636f 6e66 6967  hooks are config
+00001f00: 7572 6564 2069 6e20 7468 6520 5b60 2e70  ured in the [`.p
+00001f10: 7265 2d63 6f6d 6d69 742d 636f 6e66 6967  re-commit-config
+00001f20: 2e79 616d 6c60 5d28 7465 6d70 6c61 7465  .yaml`](template
+00001f30: 732f 2e70 7265 2d63 6f6d 6d69 742d 636f  s/.pre-commit-co
+00001f40: 6e66 6967 2e79 616d 6c2e 7470 6c29 2e0d  nfig.yaml.tpl)..
+00001f50: 0a0d 0a59 6f75 2063 616e 2063 6865 636b  ...You can check
+00001f60: 2077 6865 7468 6572 2068 6f6f 6b73 2077   whether hooks w
+00001f70: 6f72 6b20 6173 2069 6e74 656e 6465 6420  ork as intended 
+00001f80: 7573 696e 6720 7468 6520 5b72 756e 5d28  using the [run](
+00001f90: 6874 7470 733a 2f2f 7072 652d 636f 6d6d  https://pre-comm
+00001fa0: 6974 2e63 6f6d 2f23 7072 652d 636f 6d6d  it.com/#pre-comm
+00001fb0: 6974 2d72 756e 2920 636f 6d6d 616e 643a  it-run) command:
+00001fc0: 0d0a 0d0a 2020 2020 7072 652d 636f 6d6d  ....    pre-comm
+00001fd0: 6974 2072 756e 205b 686f 6f6b 2d69 645d  it run [hook-id]
+00001fe0: 205b 6f70 7469 6f6e 735d 0d0a 0d0a 4578   [options]....Ex
+00001ff0: 616d 706c 653a 2072 756e 2073 696e 676c  ample: run singl
+00002000: 6520 686f 6f6b 0d0a 0d0a 2020 2020 7072  e hook....    pr
+00002010: 652d 636f 6d6d 6974 2072 756e 2072 7566  e-commit run ruf
+00002020: 6620 2d2d 616c 6c2d 6669 6c65 7320 2d2d  f --all-files --
+00002030: 686f 6f6b 2d73 7461 6765 2070 7573 680d  hook-stage push.
+00002040: 0a0d 0a45 7861 6d70 6c65 3a20 7275 6e20  ...Example: run 
+00002050: 616c 6c20 686f 6f6b 7320 6f66 2070 7265  all hooks of pre
+00002060: 2d70 7573 6820 7374 6167 650d 0a0d 0a20  -push stage.... 
+00002070: 2020 2070 7265 2d63 6f6d 6d69 7420 7275     pre-commit ru
+00002080: 6e20 2d2d 616c 6c2d 6669 6c65 7320 2d2d  n --all-files --
+00002090: 686f 6f6b 2d73 7461 6765 2070 7573 680d  hook-stage push.
+000020a0: 0a0d 0a23 2323 2055 7064 6174 6520 646f  ...### Update do
+000020b0: 6375 6d65 6e74 6174 696f 6e0d 0a0d 0a2d  cumentation....-
+000020c0: 2054 6f20 6275 696c 6420 7468 6520 646f   To build the do
+000020d0: 6375 6d65 6e74 6174 696f 6e20 7275 6e3a  cumentation run:
+000020e0: 2060 7370 6869 6e78 2d62 7569 6c64 2064   `sphinx-build d
+000020f0: 6f63 732f 2064 6f63 732f 5f62 7569 6c64  ocs/ docs/_build
+00002100: 2f68 746d 6c2f 602e 0d0a 2d20 4f70 656e  /html/`...- Open
+00002110: 2060 646f 6373 2f5f 6275 696c 642f 6874   `docs/_build/ht
+00002120: 6d6c 2f69 6e64 6578 2e68 746d 6c60 2074  ml/index.html` t
+00002130: 6f20 7365 6520 7468 6520 646f 6375 6d65  o see the docume
+00002140: 6e74 6174 696f 6e2e 0d0a 0d0a 2323 2320  ntation.....### 
+00002150: 5472 616e 736c 6174 696f 6e20 6669 6c65  Translation file
+00002160: 730d 0a0d 0a49 6620 796f 7520 6861 7665  s....If you have
+00002170: 2061 6464 6564 2063 7573 746f 6d20 7465   added custom te
+00002180: 7874 2c20 6d61 6b65 2073 7572 6520 746f  xt, make sure to
+00002190: 2077 7261 7020 6974 2069 6e20 605f 2829   wrap it in `_()
+000021a0: 6020 7768 6572 6520 605f 6020 6973 0d0a  ` where `_` is..
+000021b0: 6765 7474 6578 745f 6c61 7a79 2028 6066  gettext_lazy (`f
+000021c0: 726f 6d20 646a 616e 676f 2e75 7469 6c73  rom django.utils
+000021d0: 2e74 7261 6e73 6c61 7469 6f6e 2069 6d70  .translation imp
+000021e0: 6f72 7420 6765 7474 6578 745f 6c61 7a79  ort gettext_lazy
+000021f0: 2061 7320 5f60 292e 0d0a 0d0a 486f 7720   as _`).....How 
+00002200: 746f 2063 7265 6174 6520 7472 616e 736c  to create transl
+00002210: 6174 696f 6e20 6669 6c65 3a0d 0a0d 0a2a  ation file:....*
+00002220: 204e 6176 6967 6174 6520 746f 2060 646a   Navigate to `dj
+00002230: 616e 676f 2d64 796e 616d 6963 2d61 646d  ango-dynamic-adm
+00002240: 696e 2d66 6f72 6d73 600d 0a2a 2060 7079  in-forms`..* `py
+00002250: 7468 6f6e 206d 616e 6167 652e 7079 206d  thon manage.py m
+00002260: 616b 656d 6573 7361 6765 7320 2d6c 2064  akemessages -l d
+00002270: 6560 0d0a 2a20 4861 7665 2061 206c 6f6f  e`..* Have a loo
+00002280: 6b20 6174 2074 6865 206e 6577 2f63 6861  k at the new/cha
+00002290: 6e67 6564 2066 696c 6573 2077 6974 6869  nged files withi
+000022a0: 6e20 6064 6a61 6e67 6f5f 6479 6e61 6d69  n `django_dynami
+000022b0: 635f 6164 6d69 6e5f 666f 726d 732f 6c6f  c_admin_forms/lo
+000022c0: 6361 6c65 600d 0a0d 0a48 6f77 2074 6f20  cale`....How to 
+000022d0: 636f 6d70 696c 6520 7472 616e 736c 6174  compile translat
+000022e0: 696f 6e20 6669 6c65 733a 0d0a 0d0a 2a20  ion files:....* 
+000022f0: 4e61 7669 6761 7465 2074 6f20 6064 6a61  Navigate to `dja
+00002300: 6e67 6f2d 6479 6e61 6d69 632d 6164 6d69  ngo-dynamic-admi
+00002310: 6e2d 666f 726d 7360 0d0a 2a20 6070 7974  n-forms`..* `pyt
+00002320: 686f 6e20 6d61 6e61 6765 2e70 7920 636f  hon manage.py co
+00002330: 6d70 696c 656d 6573 7361 6765 7360 0d0a  mpilemessages`..
+00002340: 2a20 4861 7665 2061 206c 6f6f 6b20 6174  * Have a look at
+00002350: 2074 6865 206e 6577 2f63 6861 6e67 6564   the new/changed
+00002360: 2066 696c 6573 2077 6974 6869 6e20 6064   files within `d
+00002370: 6a61 6e67 6f5f 6479 6e61 6d69 635f 6164  jango_dynamic_ad
+00002380: 6d69 6e5f 666f 726d 732f 6c6f 6361 6c65  min_forms/locale
+00002390: 600d 0a0d 0a23 2323 2050 7562 6c69 7368  `....### Publish
+000023a0: 2074 6f20 5265 6164 5468 6544 6f63 732e   to ReadTheDocs.
+000023b0: 696f 0d0a 0d0a 2d20 4665 7463 6820 7468  io....- Fetch th
+000023c0: 6520 6c61 7465 7374 2063 6861 6e67 6573  e latest changes
+000023d0: 2069 6e20 4769 7448 7562 206d 6972 726f   in GitHub mirro
+000023e0: 7220 616e 6420 7075 7368 2074 6865 6d0d  r and push them.
+000023f0: 0a2d 2054 7269 6767 6572 206e 6577 2062  .- Trigger new b
+00002400: 7569 6c64 2061 7420 5265 6164 5468 6544  uild at ReadTheD
+00002410: 6f63 732e 696f 2028 666f 6c6c 6f77 2069  ocs.io (follow i
+00002420: 6e73 7472 7563 7469 6f6e 7320 696e 2061  nstructions in a
+00002430: 646d 696e 2070 616e 656c 2061 7420 5254  dmin panel at RT
+00002440: 4429 2069 6620 7468 6520 4769 7448 7562  D) if the GitHub
+00002450: 2077 6562 686f 6f6b 2069 7320 6e6f 7420   webhook is not 
+00002460: 7965 7420 7365 740d 0a20 2075 702e 0d0a  yet set..  up...
+00002470: 0d0a 2323 2320 5075 626c 6973 6820 746f  ..### Publish to
+00002480: 2050 7950 690d 0a0d 0a2d 2055 7064 6174   PyPi....- Updat
+00002490: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+000024a0: 6162 6f75 7420 6e65 772f 6368 616e 6765  about new/change
+000024b0: 6420 6675 6e63 7469 6f6e 616c 6974 790d  d functionality.
+000024c0: 0a0d 0a2d 2055 7064 6174 6520 7468 6520  ...- Update the 
+000024d0: 6043 6861 6e67 656c 6f67 600d 0a0d 0a2d  `Changelog`....-
+000024e0: 2049 6e63 7265 6d65 6e74 2076 6572 7369   Increment versi
+000024f0: 6f6e 2069 6e20 6d61 696e 2060 5f5f 696e  on in main `__in
+00002500: 6974 5f5f 2e70 7960 0d0a 0d0a 2d20 4372  it__.py`....- Cr
+00002510: 6561 7465 2070 756c 6c20 7265 7175 6573  eate pull reques
+00002520: 7420 2f20 6d65 7267 6520 746f 206d 6173  t / merge to mas
+00002530: 7465 720d 0a0d 0a2d 2054 6869 7320 7072  ter....- This pr
+00002540: 6f6a 6563 7420 7573 6573 2074 6865 2066  oject uses the f
+00002550: 6c69 7420 7061 636b 6167 6520 746f 2070  lit package to p
+00002560: 7562 6c69 7368 2074 6f20 5079 5049 2e20  ublish to PyPI. 
+00002570: 5468 7573 2070 7562 6c69 7368 696e 6720  Thus publishing 
+00002580: 7368 6f75 6c64 2062 6520 6173 2065 6173  should be as eas
+00002590: 7920 6173 2072 756e 6e69 6e67 3a0d 0a20  y as running:.. 
+000025a0: 2060 6060 0d0a 2020 666c 6974 2070 7562   ```..  flit pub
+000025b0: 6c69 7368 0d0a 2020 6060 600d 0a0d 0a20  lish..  ```.... 
+000025c0: 2054 6f20 7075 626c 6973 6820 746f 2054   To publish to T
+000025d0: 6573 7450 7950 4920 7573 6520 7468 6520  estPyPI use the 
+000025e0: 666f 6c6c 6f77 696e 6720 656e 7375 7265  following ensure
+000025f0: 2074 6861 7420 796f 7520 6861 7665 2073   that you have s
+00002600: 6574 2075 7020 796f 7572 202e 7079 7069  et up your .pypi
+00002610: 7263 2061 730d 0a20 2073 686f 776e 205b  rc as..  shown [
+00002620: 6865 7265 5d28 6874 7470 733a 2f2f 666c  here](https://fl
+00002630: 6974 2e72 6561 6474 6865 646f 6373 2e69  it.readthedocs.i
+00002640: 6f2f 656e 2f6c 6174 6573 742f 7570 6c6f  o/en/latest/uplo
+00002650: 6164 2e68 746d 6c23 7573 696e 672d 7079  ad.html#using-py
+00002660: 7069 7263 2920 616e 6420 7573 6520 7468  pirc) and use th
+00002670: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00002680: 616e 643a 0d0a 0d0a 2020 6060 600d 0a20  and:....  ```.. 
+00002690: 2066 6c69 7420 7075 626c 6973 6820 2d2d   flit publish --
+000026a0: 7265 706f 7369 746f 7279 2074 6573 7470  repository testp
+000026b0: 7970 690d 0a20 2060 6060 0d0a 0d0a 2323  ypi..  ```....##
+000026c0: 2320 4d61 696e 7465 6e61 6e63 650d 0a0d  # Maintenance...
+000026d0: 0a50 6c65 6173 6520 6e6f 7465 2074 6861  .Please note tha
+000026e0: 7420 7468 6973 2070 6163 6b61 6765 2073  t this package s
+000026f0: 7570 706f 7274 7320 7468 6520 5b61 6d62  upports the [amb
+00002700: 6965 6e74 2d70 6163 6b61 6765 2d75 7064  ient-package-upd
+00002710: 6174 655d 2868 7474 7073 3a2f 2f70 7970  ate](https://pyp
+00002720: 692e 6f72 672f 7072 6f6a 6563 742f 616d  i.org/project/am
+00002730: 6269 656e 742d 7061 636b 6167 652d 7570  bient-package-up
+00002740: 6461 7465 2f29 2e0d 0a53 6f20 796f 7520  date/)...So you 
+00002750: 646f 6e27 7420 6861 7665 2074 6f20 776f  don't have to wo
+00002760: 7272 7920 6162 6f75 7420 7468 6520 6d61  rry about the ma
+00002770: 696e 7465 6e61 6e63 6520 6f66 2074 6869  intenance of thi
+00002780: 7320 7061 636b 6167 652e 2041 6c6c 2069  s package. All i
+00002790: 6d70 6f72 7461 6e74 2063 6f6e 6669 6775  mportant configu
+000027a0: 7261 7469 6f6e 2061 6e64 2073 6574 7570  ration and setup
+000027b0: 2066 696c 6573 2061 7265 0d0a 6265 696e   files are..bein
+000027c0: 6720 7265 6e64 6572 6564 2062 7920 7468  g rendered by th
+000027d0: 6973 2075 7064 6174 6572 2e20 4974 2077  is updater. It w
+000027e0: 6f72 6b73 2073 696d 696c 6172 2074 6f20  orks similar to 
+000027f0: 7765 6c6c 2d6b 6e6f 776e 2075 7064 6174  well-known updat
+00002800: 6572 7320 6c69 6b65 2060 7079 7570 6772  ers like `pyupgr
+00002810: 6164 6560 206f 7220 6064 6a61 6e67 6f2d  ade` or `django-
+00002820: 7570 6772 6164 6560 2e0d 0a0d 0a54 6f20  upgrade`.....To 
+00002830: 7275 6e20 616e 2075 7064 6174 652c 2072  run an update, r
+00002840: 6566 6572 2074 6f20 7468 6520 5b64 6f63  efer to the [doc
+00002850: 756d 656e 7461 7469 6f6e 2070 6167 655d  umentation page]
+00002860: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00002870: 672f 7072 6f6a 6563 742f 616d 6269 656e  g/project/ambien
+00002880: 742d 7061 636b 6167 652d 7570 6461 7465  t-package-update
+00002890: 2f29 0d0a 6f66 2074 6865 2022 616d 6269  /)..of the "ambi
+000028a0: 656e 742d 7061 636b 6167 652d 7570 6461  ent-package-upda
+000028b0: 7465 222e 0d0a                           te"...
```

### Comparing `django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/admin.py` & `django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/admin.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/static/js/dynamic_admin.js` & `django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/static/js/dynamic_admin.js`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/django_dynamic_admin_forms/templates/admin/change_form.html` & `django_dynamic_admin_forms-3.0.0/django_dynamic_admin_forms/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/docs/Makefile` & `django_dynamic_admin_forms-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/docs/conf.py` & `django_dynamic_admin_forms-3.0.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django.setup()
 
 from django_dynamic_admin_forms import __version__  # noqa: E402
 
 # -- Project information -----------------------------------------------------
 
 project = "django-dynamic-admin-forms"
-copyright = "2023, Ambient Innovation: GmbH"  # noqa: A001
+copyright = "2024, Ambient Innovation: GmbH"  # noqa: A001
 author = "Ambient Innovation: GmbH <hello@ambient.digital>"
 version = __version__
 release = __version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `django_dynamic_admin_forms-2.2.1/docs/demo.gif` & `django_dynamic_admin_forms-3.0.0/docs/demo.gif`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/docs/make.bat` & `django_dynamic_admin_forms-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/e2e/cypress/integration/dynamic-select.spec.js` & `django_dynamic_admin_forms-3.0.0/e2e/cypress/integration/dynamic-select.spec.js`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/e2e/cypress/plugins/index.js` & `django_dynamic_admin_forms-3.0.0/e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/e2e/cypress/support/commands.js` & `django_dynamic_admin_forms-3.0.0/e2e/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/e2e/cypress/support/index.js` & `django_dynamic_admin_forms-3.0.0/e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/e2e/yarn.lock` & `django_dynamic_admin_forms-3.0.0/e2e/yarn.lock`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/fixtures/fixtures-dev.json` & `django_dynamic_admin_forms-3.0.0/fixtures/fixtures-dev.json`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/pyproject.toml` & `django_dynamic_admin_forms-3.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     {'name' = 'Fabian Binz', 'email' = 'fabian.binz@ambient.digital'},
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
@@ -42,35 +40,35 @@
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
    'flit~=3.9',
-   'ambient-package-update~=23.12.4',
+   'ambient-package-update~=24.4.4',
    'unittest-parametrize~=1.4',
 ]
 
 [tool.flit.module]
 name = "django_dynamic_admin_forms"
 
 [project.urls]
 'Homepage' = 'https://github.com/ambient-innovation/django-dynamic-admin/'
 'Documentation' = 'https://django-dynamic-admin-forms.readthedocs.io/en/latest/index.html'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/django-dynamic-admin/issues'
 'Changelog' = 'https://django-dynamic-admin-forms.readthedocs.io/en/latest/features/changelog.html'
 
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
@@ -84,19 +82,19 @@
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
@@ -110,15 +108,15 @@
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
@@ -167,23 +165,28 @@
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

### Comparing `django_dynamic_admin_forms-2.2.1/testapp/admin.py` & `django_dynamic_admin_forms-3.0.0/testapp/admin.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/testapp/migrations/0001_initial.py` & `django_dynamic_admin_forms-3.0.0/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/testapp/migrations/0002_extend_example.py` & `django_dynamic_admin_forms-3.0.0/testapp/migrations/0002_extend_example.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/testapp/migrations/0003_example_file_field.py` & `django_dynamic_admin_forms-3.0.0/testapp/migrations/0003_example_file_field.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/testapp/models.py` & `django_dynamic_admin_forms-3.0.0/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/testapp/urls.py` & `django_dynamic_admin_forms-3.0.0/testapp/urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""config URL Configuration
-
-The `urlpatterns` list routes URLs to views. For more information please see:
-    https://docs.djangoproject.com/en/3.1/topics/http/urls/
-Examples:
-Function views
-    1. Add an import:  from my_app import views
-    2. Add a URL to urlpatterns:  path('', views.home, name='home')
-Class-based views
-    1. Add an import:  from other_app.views import Home
-    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
-Including another URLconf
-    1. Import the include() function: from django.urls import include, path
-    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
-"""
-from django.contrib import admin
-from django.urls import include, path
-
-urlpatterns = [
-    path("admin/", admin.site.urls),
-    path("dynamic-admin-form/", include("django_dynamic_admin_forms.urls")),
-]
+"""config URL Configuration
+
+The `urlpatterns` list routes URLs to views. For more information please see:
+    https://docs.djangoproject.com/en/3.1/topics/http/urls/
+Examples:
+Function views
+    1. Add an import:  from my_app import views
+    2. Add a URL to urlpatterns:  path('', views.home, name='home')
+Class-based views
+    1. Add an import:  from other_app.views import Home
+    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
+Including another URLconf
+    1. Import the include() function: from django.urls import include, path
+    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
+"""
+
+from django.contrib import admin
+from django.urls import include, path
+
+urlpatterns = [
+    path("admin/", admin.site.urls),
+    path("dynamic-admin-form/", include("django_dynamic_admin_forms.urls")),
+]
```

### Comparing `django_dynamic_admin_forms-2.2.1/tests/test_admin_generic.py` & `django_dynamic_admin_forms-3.0.0/tests/test_admin_generic.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/tests/test_admin_unit.py` & `django_dynamic_admin_forms-3.0.0/tests/test_admin_unit.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_admin_forms-2.2.1/PKG-INFO` & `django_dynamic_admin_forms-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: django-dynamic-admin-forms
-Version: 2.2.1
+Version: 3.0.0
 Summary: Add simple dynamic interaction to the otherwise static django admin.
 Author-email: Ambient Digital <hello@ambient.digital>, Fabian Binz <fabian.binz@ambient.digital>
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
@@ -27,20 +25,20 @@
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
 Requires-Dist: flit~=3.9 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.12.4 ; extra == "dev"
+Requires-Dist: ambient-package-update~=24.4.4 ; extra == "dev"
 Requires-Dist: unittest-parametrize~=1.4 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/django-dynamic-admin/issues
 Project-URL: Changelog, https://django-dynamic-admin-forms.readthedocs.io/en/latest/features/changelog.html
 Project-URL: Documentation, https://django-dynamic-admin-forms.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/ambient-innovation/django-dynamic-admin/
 Project-URL: Maintained by, https://ambient.digital/
 Provides-Extra: dev
@@ -159,32 +157,32 @@
 - only tested with Django 3.2
 
 ## Development
 
 For local development, create a virtual environment
 in the `testproj` folder:
 ```shell
-$ cd testapp
+$ cd testproj
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ cd ..
-$ pip install -e .
+$ flit install --symlink
 ```
 Now the package should be available in your virtual environment
-and any changes should be directly visible. Run the project as a Django server and navigate to the admin page.
+and any changes should be directly visible.
 
 Alternatively, copy the directory `dynamic_admin_forms`
 into any normal django project, so that the python interpreter
 finds the local version instead of the installed (old) version.
 
 ## Running E2E tests
 
 To run end-to-end tests locally:
 ```shell
-$ cd testapp
+$ cd testproj
 $ python manage.py runserver 0.0.0.0:8000 &  # start server
 $ python manage.py loaddata fixtures/fixtures-dev.json
 $ cd ../e2e
 $ yarn install  # or npm install (only needed first time)
 $ yarn cypress  # or npm run cypress
 ```
```

