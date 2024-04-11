# Comparing `tmp/django_pony_express-1.3.0.tar.gz` & `tmp/django_pony_express-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pony_express-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pony_express-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pony_express-1.3.0.tar` & `django_pony_express-2.0.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     2602 2023-12-04 15:24:45.657869 django_pony_express-1.3.0/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0      320 2023-12-04 16:19:53.569813 django_pony_express-1.3.0/.coveragerc
--rw-r--r--   0        0        0      288 2023-12-04 16:19:53.569813 django_pony_express-1.3.0/.editorconfig
--rw-r--r--   0        0        0     2225 2023-12-04 16:23:08.928198 django_pony_express-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3137 2023-12-04 15:24:45.661871 django_pony_express-1.3.0/.gitignore
--rw-r--r--   0        0        0      668 2023-12-04 16:23:08.928198 django_pony_express-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      773 2023-12-04 16:19:53.569813 django_pony_express-1.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1506 2023-12-04 16:23:08.928198 django_pony_express-1.3.0/CHANGES.md
--rw-r--r--   0        0        0    71412 2023-12-04 16:19:53.601453 django_pony_express-1.3.0/LICENSE.md
--rw-r--r--   0        0        0      138 2023-12-04 16:19:53.569813 django_pony_express-1.3.0/MANIFEST.in
--rw-r--r--   0        0        0     6287 2023-12-04 16:23:08.928198 django_pony_express-1.3.0/README.md
--rw-r--r--   0        0        0       85 2023-12-04 16:23:08.928198 django_pony_express-1.3.0/django_pony_express/__init__.py
--rw-r--r--   0        0        0      114 2023-12-04 15:24:45.663888 django_pony_express-1.3.0/django_pony_express/errors.py
--rw-r--r--   0        0        0     1564 2023-12-04 15:24:45.663888 django_pony_express-1.3.0/django_pony_express/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.663888 django_pony_express-1.3.0/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0    11100 2023-12-04 15:24:45.663888 django_pony_express-1.3.0/django_pony_express/services/base.py
--rw-r--r--   0        0        0     9771 2023-12-04 15:24:45.663888 django_pony_express-1.3.0/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      654 2023-12-04 16:19:53.589443 django_pony_express-1.3.0/docs/Makefile
--rw-r--r--   0        0        0     2825 2023-12-04 16:19:53.589443 django_pony_express-1.3.0/docs/conf.py
--rw-r--r--   0        0        0       32 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/docs/features/changelog.rst
--rw-r--r--   0        0        0     9438 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/docs/features/mail.md
--rw-r--r--   0        0        0     4912 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/docs/features/tests.md
--rw-r--r--   0        0        0      264 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-12-04 16:19:53.589443 django_pony_express-1.3.0/docs/make.bat
--rw-r--r--   0        0        0      655 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/manage.py
--rw-r--r--   0        0        0     5386 2023-12-04 16:23:08.928198 django_pony_express-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-12-04 16:19:53.585431 django_pony_express-1.3.0/pytest.init
--rw-r--r--   0        0        0      121 2023-12-04 16:19:53.601453 django_pony_express-1.3.0/scripts/unix/install_requirements.sh
--rw-r--r--   0        0        0       50 2023-12-04 16:19:53.601453 django_pony_express-1.3.0/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      121 2023-12-04 16:19:53.601453 django_pony_express-1.3.0/scripts/windows/install_requirements.ps1
--rw-r--r--   0        0        0       50 2023-12-04 16:19:53.601453 django_pony_express-1.3.0/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0     1620 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/settings.py
--rw-r--r--   0        0        0      289 2023-12-04 16:19:53.589443 django_pony_express-1.3.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/testapp/__init__.py
--rw-r--r--   0        0        0      134 2023-12-04 15:24:45.665922 django_pony_express-1.3.0/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      145 2023-12-04 15:24:45.670166 django_pony_express-1.3.0/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      137 2023-12-04 15:24:45.670166 django_pony_express-1.3.0/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.670166 django_pony_express-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0       27 2023-12-04 15:24:45.670166 django_pony_express-1.3.0/tests/files/testfile.txt
--rw-r--r--   0        0        0     9340 2023-12-04 15:24:45.670166 django_pony_express-1.3.0/tests/test_email_test_service.py
--rw-r--r--   0        0        0    15224 2023-12-04 15:24:45.670166 django_pony_express-1.3.0/tests/test_mail_services.py
--rw-r--r--   0        0        0     8281 1970-01-01 00:00:00.000000 django_pony_express-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2602 2023-12-04 15:24:45.657869 django_pony_express-2.0.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0      320 2024-04-11 14:12:18.255023 django_pony_express-2.0.0/.coveragerc
+-rw-r--r--   0        0        0      288 2024-04-11 14:12:18.256031 django_pony_express-2.0.0/.editorconfig
+-rw-r--r--   0        0        0     2213 2024-04-11 14:16:18.950523 django_pony_express-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3137 2023-12-04 15:24:45.661871 django_pony_express-2.0.0/.gitignore
+-rw-r--r--   0        0        0      668 2024-04-11 14:16:18.950523 django_pony_express-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      773 2024-04-11 14:12:18.259031 django_pony_express-2.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1652 2024-04-11 14:16:18.951515 django_pony_express-2.0.0/CHANGES.md
+-rw-r--r--   0        0        0    71412 2024-04-11 14:12:18.291569 django_pony_express-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0      138 2024-04-11 14:12:18.260033 django_pony_express-2.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     6287 2024-04-11 14:12:18.272133 django_pony_express-2.0.0/README.md
+-rw-r--r--   0        0        0       85 2024-04-11 14:16:18.951515 django_pony_express-2.0.0/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/errors.py
+-rw-r--r--   0        0        0     1564 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0    11100 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/services/base.py
+-rw-r--r--   0        0        0     9771 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      654 2024-04-11 14:12:18.279570 django_pony_express-2.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2825 2024-04-11 14:16:18.951515 django_pony_express-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0       32 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/features/changelog.rst
+-rw-r--r--   0        0        0     9438 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/features/mail.md
+-rw-r--r--   0        0        0     4912 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/features/tests.md
+-rw-r--r--   0        0        0      264 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2024-04-11 14:12:18.278560 django_pony_express-2.0.0/docs/make.bat
+-rw-r--r--   0        0        0      679 2024-04-11 14:16:18.952522 django_pony_express-2.0.0/manage.py
+-rw-r--r--   0        0        0     5402 2024-04-11 14:16:18.952522 django_pony_express-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-11 14:12:18.281561 django_pony_express-2.0.0/scripts/unix/install_requirements.sh
+-rw-r--r--   0        0        0       50 2024-04-11 14:12:18.282568 django_pony_express-2.0.0/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      121 2024-04-11 14:12:18.284573 django_pony_express-2.0.0/scripts/windows/install_requirements.ps1
+-rw-r--r--   0        0        0       50 2024-04-11 14:12:18.285570 django_pony_express-2.0.0/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0     1620 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/settings.py
+-rw-r--r--   0        0        0      289 2024-04-11 14:12:18.273137 django_pony_express-2.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/testapp/__init__.py
+-rw-r--r--   0        0        0      134 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      145 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      137 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       27 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/files/testfile.txt
+-rw-r--r--   0        0        0     9340 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/test_email_test_service.py
+-rw-r--r--   0        0        0    15224 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/test_mail_services.py
+-rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 django_pony_express-2.0.0/PKG-INFO
```

### Comparing `django_pony_express-1.3.0/.ambient-package-update/metadata.py` & `django_pony_express-2.0.0/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/.github/workflows/ci.yml` & `django_pony_express-2.0.0/.github/workflows/ci.yml`

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

### Comparing `django_pony_express-1.3.0/.gitignore` & `django_pony_express-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/.pre-commit-config.yaml` & `django_pony_express-2.0.0/.pre-commit-config.yaml`

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

### Comparing `django_pony_express-1.3.0/.readthedocs.yaml` & `django_pony_express-2.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/CHANGES.md` & `django_pony_express-2.0.0/CHANGES.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+* *2.0.0* (2024-04-11)
+  * Dropped Django 3.2 & 4.1 support (via `ambient-package-update`)
+  * Internal updates via `ambient-package-update`
+
 * *1.3.0** (2023-12-04)
   * Added Django 5.0 support
 
 * *1.2.5** (2023-11-13)
   * Fixed wrong import path in docs
 
 * *1.2.4** (2023-11-03)
```

### Comparing `django_pony_express-1.3.0/LICENSE.md` & `django_pony_express-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/README.md` & `django_pony_express-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/django_pony_express/locale/de/LC_MESSAGES/django.po` & `django_pony_express-2.0.0/django_pony_express/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/django_pony_express/services/base.py` & `django_pony_express-2.0.0/django_pony_express/services/base.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/django_pony_express/services/tests.py` & `django_pony_express-2.0.0/django_pony_express/services/tests.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/docs/Makefile` & `django_pony_express-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/docs/conf.py` & `django_pony_express-2.0.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django.setup()
 
 from django_pony_express import __version__  # noqa: E402
 
 # -- Project information -----------------------------------------------------
 
 project = "django-pony-express"
-copyright = "2023, Ambient Innovation: GmbH"  # noqa: A001
+copyright = "2024, Ambient Innovation: GmbH"  # noqa: A001
 author = "Ambient Innovation: GmbH <hello@ambient.digital>"
 version = __version__
 release = __version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `django_pony_express-1.3.0/docs/features/mail.md` & `django_pony_express-2.0.0/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/docs/features/tests.md` & `django_pony_express-2.0.0/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/docs/make.bat` & `django_pony_express-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/pyproject.toml` & `django_pony_express-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

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
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -36,39 +34,40 @@
     'html2text>=2020.1.16',
 ]
 
 
 [project.optional-dependencies]
 dev = [
    'typer~=0.9',
-   'freezegun~=1.2',
-   'pytest-django~=4.5',
-   'pytest-mock~=3.10',
+   'freezegun~=1.3',
+   'pytest-django~=4.7',
+   'pytest-mock~=3.12',
    'coverage~=7.3',
    'pre-commit~=3.5',
-   'ruff~=0.1',
-   'sphinx==4.2.0',
-   'sphinx-rtd-theme==1.0.0',
-   'm2r2==0.3.1',
+   'ruff~=0.1.7',
+   'sphinx~=7.1',
+   'sphinx-rtd-theme~=2.0',
+   'm2r2==0.3.3.post2',
    'mistune<2.0.0',
-   'ambient-package-update~=23.12.2',
+   'flit~=3.9',
+   'ambient-package-update~=24.4.4',
 ]
 
 [tool.flit.module]
 name = "django_pony_express"
 
 [project.urls]
 'Homepage' = 'https://github.com/ambient-innovation/django-pony-express/'
 'Documentation' = 'https://django-pony-express.readthedocs.io/en/latest/index.html'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/django-pony-express/issues'
 'Changelog' = 'https://django-pony-express.readthedocs.io/en/latest/features/changelog.html'
 
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
@@ -82,23 +81,23 @@
     "PIE",     # Bunch of useful rules
     # "SIM",     # Simplifies your code
     "INT",     # Validates your gettext translation strings
     "PERF",    # PerfLint
     "PGH",     # No all-purpose "# noqa" and eval validation
     "PL",      # PyLint
 ]
-ignore = [
+lint.ignore = [
     'N999', # Project name contains underscore, not fixable
     'A003', # Django attributes shadow python builtins
     'DJ001', # Django model text-based fields shouldn't be nullable
     'B905', # Can be enabled when Python <=3.9 support is dropped
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
@@ -112,15 +111,15 @@
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
@@ -169,23 +168,28 @@
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

### Comparing `django_pony_express-1.3.0/settings.py` & `django_pony_express-2.0.0/settings.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/tests/test_email_test_service.py` & `django_pony_express-2.0.0/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/tests/test_mail_services.py` & `django_pony_express-2.0.0/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-1.3.0/PKG-INFO` & `django_pony_express-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 1.3.0
+Version: 2.0.0
 Summary: Class-based emails including a test suite for Django
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
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -22,25 +20,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: Django>=3.2
 Requires-Dist: html2text>=2020.1.16
 Requires-Dist: typer~=0.9 ; extra == "dev"
-Requires-Dist: freezegun~=1.2 ; extra == "dev"
-Requires-Dist: pytest-django~=4.5 ; extra == "dev"
-Requires-Dist: pytest-mock~=3.10 ; extra == "dev"
+Requires-Dist: freezegun~=1.3 ; extra == "dev"
+Requires-Dist: pytest-django~=4.7 ; extra == "dev"
+Requires-Dist: pytest-mock~=3.12 ; extra == "dev"
 Requires-Dist: coverage~=7.3 ; extra == "dev"
 Requires-Dist: pre-commit~=3.5 ; extra == "dev"
-Requires-Dist: ruff~=0.1 ; extra == "dev"
-Requires-Dist: sphinx==4.2.0 ; extra == "dev"
-Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
-Requires-Dist: m2r2==0.3.1 ; extra == "dev"
+Requires-Dist: ruff~=0.1.7 ; extra == "dev"
+Requires-Dist: sphinx~=7.1 ; extra == "dev"
+Requires-Dist: sphinx-rtd-theme~=2.0 ; extra == "dev"
+Requires-Dist: m2r2==0.3.3.post2 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.12.2 ; extra == "dev"
+Requires-Dist: flit~=3.9 ; extra == "dev"
+Requires-Dist: ambient-package-update~=24.4.4 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/django-pony-express/issues
 Project-URL: Changelog, https://django-pony-express.readthedocs.io/en/latest/features/changelog.html
 Project-URL: Documentation, https://django-pony-express.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/ambient-innovation/django-pony-express/
 Project-URL: Maintained by, https://ambient.digital/
 Provides-Extra: dev
```

