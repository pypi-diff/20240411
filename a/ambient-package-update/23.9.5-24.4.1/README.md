# Comparing `tmp/ambient_package_update-23.9.5.tar.gz` & `tmp/ambient_package_update-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_package_update-23.9.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ambient_package_update-24.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient_package_update-23.9.5.tar` & `ambient_package_update-24.4.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient_package_update-23.9.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient_package_update-23.9.5/.gitignore
--rw-r--r--   0        0        0      922 2023-09-08 08:06:23.073413 ambient_package_update-23.9.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2568 2023-09-08 08:17:49.501980 ambient_package_update-23.9.5/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient_package_update-23.9.5/LICENSE.md
--rw-r--r--   0        0        0     4630 2023-08-31 12:01:38.656482 ambient_package_update-23.9.5/README.md
--rw-r--r--   0        0        0       93 2023-09-08 08:17:49.489970 ambient_package_update-23.9.5/ambient_package_update/__init__.py
--rw-r--r--   0        0        0     3502 2023-09-08 07:58:08.974543 ambient_package_update-23.9.5/ambient_package_update/cli.py
--rw-r--r--   0        0        0    71415 2023-08-28 09:00:47.218002 ambient_package_update-23.9.5/ambient_package_update/licenses/GPL.md
--rw-r--r--   0        0        0     1105 2023-08-28 09:00:47.218002 ambient_package_update-23.9.5/ambient_package_update/licenses/MIT.md
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient_package_update-23.9.5/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient_package_update-23.9.5/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      498 2023-08-28 09:00:47.218002 ambient_package_update-23.9.5/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      764 2023-08-28 09:00:47.233628 ambient_package_update-23.9.5/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      192 2023-08-28 08:58:02.426643 ambient_package_update-23.9.5/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient_package_update-23.9.5/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0       82 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1292 2023-09-08 08:13:02.748229 ambient_package_update-23.9.5/ambient_package_update/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      922 2023-09-08 08:06:23.073413 ambient_package_update-23.9.5/ambient_package_update/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0      137 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     5354 2023-08-31 12:01:38.651973 ambient_package_update-23.9.5/ambient_package_update/templates/README.md.tpl
--rw-r--r--   0        0        0      654 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2853 2023-08-14 09:13:14.022655 ambient_package_update-23.9.5/ambient_package_update/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     5084 2023-09-08 07:57:02.432415 ambient_package_update-23.9.5/ambient_package_update/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-22 13:32:26.216194 ambient_package_update-23.9.5/ambient_package_update/templates/pytest.init.tpl
--rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.9.5/ambient_package_update/templates/scripts/unix/publish_to_pypi.sh.tpl
--rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.9.5/ambient_package_update/templates/scripts/windows/publish_to_pypi.ps1.tpl
--rw-r--r--   0        0        0       69 2023-05-22 13:32:26.231832 ambient_package_update-23.9.5/ambient_package_update/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     3891 2023-08-28 09:00:47.233628 ambient_package_update-23.9.5/pyproject.toml
--rw-r--r--   0        0        0     1741 2023-08-14 08:58:21.387582 ambient_package_update-23.9.5/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.9.5/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient_package_update-23.9.5/scripts/unix/setup_venv_unix.sh
--rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.9.5/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient_package_update-23.9.5/scripts/windows/setup_venv.ps1
--rw-r--r--   0        0        0     5777 1970-01-01 00:00:00.000000 ambient_package_update-23.9.5/PKG-INFO
+-rw-r--r--   0        0        0      432 2024-03-28 09:26:53.193919 ambient_package_update-24.4.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3122 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/.gitignore
+-rw-r--r--   0        0        0      642 2024-04-11 13:38:59.651610 ambient_package_update-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4001 2023-12-05 11:25:02.798121 ambient_package_update-24.4.1/CHANGES.md
+-rw-r--r--   0        0        0     1064 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/LICENSE.md
+-rw-r--r--   0        0        0     4719 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/README.md
+-rw-r--r--   0        0        0       90 2024-04-11 13:40:04.722334 ambient_package_update-24.4.1/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0     3681 2023-12-05 11:19:03.483109 ambient_package_update-24.4.1/ambient_package_update/cli.py
+-rw-r--r--   0        0        0    70069 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/ambient_package_update/licenses/GPL.md
+-rw-r--r--   0        0        0     1084 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/ambient_package_update/licenses/MIT.md
+-rw-r--r--   0        0        0        0 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0       94 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      689 2024-04-11 13:41:03.522281 ambient_package_update-24.4.1/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      918 2023-12-05 11:16:09.487698 ambient_package_update-24.4.1/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      240 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      103 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0      303 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      270 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     2987 2024-03-28 09:40:18.641481 ambient_package_update-24.4.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      720 2024-04-11 13:37:12.286993 ambient_package_update-24.4.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      742 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/templates/.readthedocs.yaml.tpl
+-rw-r--r--   0        0        0      133 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5881 2023-12-05 11:23:35.552515 ambient_package_update-24.4.1/ambient_package_update/templates/README.md.tpl
+-rw-r--r--   0        0        0      634 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2769 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      760 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     5281 2024-04-11 13:49:19.793561 ambient_package_update-24.4.1/ambient_package_update/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0      201 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/unix/install_requirements.sh.tpl
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/unix/publish_to_pypi.sh.tpl
+-rw-r--r--   0        0        0      201 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/windows/install_requirements.ps1.tpl
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/windows/publish_to_pypi.ps1.tpl
+-rw-r--r--   0        0        0      269 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/ambient_package_update/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     4143 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1482 2023-12-04 15:06:50.299033 ambient_package_update-24.4.1/requirements.txt
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      548 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/unix/setup_venv_unix.sh
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0      446 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/windows/setup_venv.ps1
+-rw-r--r--   0        0        0     6119 1970-01-01 00:00:00.000000 ambient_package_update-24.4.1/PKG-INFO
```

### Comparing `ambient_package_update-23.9.5/.gitignore` & `ambient_package_update-24.4.1/.gitignore`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-.idea/
-
-# PyCharm
-.idea/
-
-# Test databases
-*.sqlite
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+.idea/
+
+# PyCharm
+.idea/
+
+# Test databases
+*.sqlite
```

### Comparing `ambient_package_update-23.9.5/.pre-commit-config.yaml` & `ambient_package_update-24.4.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-# you find the full pre-commit-tools docu under:
-# https://pre-commit.com/
-
-repos:
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.7.0
-    hooks:
-      - id: black
-        args: [ --check, --diff, --config, ./pyproject.toml ]
-        language_version: python3.11
-        stages: [ push ]
-
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    # Ruff version.
-    rev: 'v0.0.285'
-    hooks:
-      - id: ruff
-        args: [ --fix, --exit-non-zero-on-fix ]
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.10.1
-    hooks:
-      - id: pyupgrade
-        args: [ --py38-plus ]
-        language_version: python3.11
-        stages: [ push ]
-
-  - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.14.0
-    hooks:
-      - id: django-upgrade
-        args: [--target-version, "3.2"]
-        language_version: python3.11
-        stages: [ push ]
+# you find the full pre-commit-tools docu under:
+# https://pre-commit.com/
+
+repos:
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.5
+    hooks:
+      # Run the Ruff linter.
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
+      # Run the Ruff formatter.
+      - id: ruff-format
+
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.15.2
+    hooks:
+      - id: pyupgrade
+        args: [ --py{{ supported_python_versions.0|replace(".", "") }}-plus ]
+        stages: [ push ]
+
+  - repo: https://github.com/adamchainz/django-upgrade
+    rev: 1.16.0
+    hooks:
+      - id: django-upgrade
+        args: [--target-version, "{{ supported_django_versions.0 }}"]
+        stages: [ push ]
```

### Comparing `ambient_package_update-23.9.5/LICENSE.md` & `ambient_package_update-24.4.1/ambient_package_update/licenses/MIT.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ambient
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) {{ license_year }} {{ company }}
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ambient_package_update-23.9.5/README.md` & `ambient_package_update-24.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,134 @@
-[![PyPI release](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.org/project/ambient-package-update/)
-[![Downloads](https://static.pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
-[![Coding Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-
-# Ambient Package Update
-
-This repository will help keep all Python packages following a certain basic structure tidy and up-to-date. It's being 
-maintained by [Ambient Digital](https://ambient.digital). 
-
-This package will render all required configuration and installation files for your target package.
-
-Typical use-cases:
-
-- A new Python or Django version was released
-- A Python or Django version was deprecated
-- You want to update the Sphinx documentation builder
-- You want to update the linter versions
-- You want to add the third-party dependencies
-
-## Versioning
-
-This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
-
-## How to update a package
-
-These steps will tell you how to update a package which was created by using this updater.
-
-- Navigate to the main directory of **your** package
-- Activate your virtualenv
-- Run `python -m ambient_package_update.cli render-templates`
-- Validate the changes and increment the version accordingly
-- Release a new version of your target package
-
-## How to create a new package
-
-Just follow these steps if you want to create a new package and maintain it using this updater.
-
-- Create a new repo at GitHub
-- Check out the new repository in the same directory this updater lives in (not inside the updater!)
-- Create a directory ".ambient-package-update" and create a file "metadata.py" inside.
-
-```python
-from ambient_package_update.metadata.author import PackageAuthor
-from ambient_package_update.metadata.constants import DEV_DEPENDENCIES
-from ambient_package_update.metadata.package import PackageMetadata
-from ambient_package_update.metadata.readme import ReadmeContent
-from ambient_package_update.metadata.ruff_ignored_inspection import RuffIgnoredInspection
-
-METADATA = PackageMetadata(
-    package_name='my_package_name',
-    authors=[
-        PackageAuthor(
-            name='Ambient Digital',
-            email='hello@ambient.digital',
-        ),
-    ],
-    development_status='5 - Production/Stable',
-    readme_content=ReadmeContent(
-        tagline='A fancy tagline for your new package',
-        content="""A multiline string containing specific things you want to have in your package readme.
-""",
-    ),
-    dependencies=[
-        'my_dependency>=1.0',
-    ],
-    optional_dependencies={
-        'dev': [
-            *DEV_DEPENDENCIES,
-        ],
-        # you might add further extras here
-    },
-    ruff_ignore_list=[
-        RuffIgnoredInspection(key='XYZ', comment="Reason why we need this exception"),
-
-    ],
-)
-```
-
-- Install the `ambient_package_update` package
-  ```
-  # ideally in a virtual environment
-  pip install ambient-package-update
-  ```
-- Add `docs/index.rst` and link your readme and changelog to have a basic documentation (surely, you can add or write
-  more custom docs if you want!)
-- Enable the readthedocs hook in your GitHub repo to update your documentation on a commit basis
-- Finally, follow the steps of the section above (`How to update a package`).
-
-## Contribution
-
-### Dependency updates
-
-The dependencies of this package are being maintained with `pip-tools`. 
-
-> pip install -U pip-tools
-
-To add/update/remove a package, please do so in the main `pyproject.toml`. Afterward, call the following command to
-reflect your changes in the `requirements.txt`.
-
-> pip-compile --upgrade
-
-To install the packages, run:
-
-> pip-sync
-
-### Publish to PyPi
-
-- Update documentation about new/changed functionality
-
-- Update the `Changelog`
-
-- Increment version in main `__init__.py`
-
-- Increment version of this package in dependencies in `ambient_package_update/metadata/constants.py`
-
-- Create pull request / merge to master
-
-- This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
-
-  ```
-  flit publish
-  ```
-
-  To publish to TestPyPI use the following ensure that you have set up your .pypirc as
-  shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
-
-  ```
-  flit publish --repository testpypi
-  ```
-
-## Changelog
-
-Can be found at [GitHub](https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md).
+[![PyPI release](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.org/project/ambient-package-update/)
+[![Downloads](https://static.pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
+[![Linting](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Coding Style](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://github.com/astral-sh/ruff)
+
+# Ambient Package Update
+
+This repository will help keep all Python packages following a certain basic structure tidy and up-to-date. It's being 
+maintained by [Ambient Digital](https://ambient.digital). 
+
+This package will render all required configuration and installation files for your target package.
+
+Typical use-cases:
+
+- A new Python or Django version was released
+- A Python or Django version was deprecated
+- You want to update the Sphinx documentation builder
+- You want to update the linter versions
+- You want to add the third-party dependencies
+
+## Versioning
+
+This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
+
+## How to update a package
+
+These steps will tell you how to update a package which was created by using this updater.
+
+- Navigate to the main directory of **your** package
+- Activate your virtualenv
+- Run `python -m ambient_package_update.cli render-templates`
+- Validate the changes and increment the version accordingly
+- Release a new version of your target package
+
+## How to create a new package
+
+Just follow these steps if you want to create a new package and maintain it using this updater.
+
+- Create a new repo at GitHub
+- Check out the new repository in the same directory this updater lives in (not inside the updater!)
+- Create a directory ".ambient-package-update" and create a file "metadata.py" inside.
+
+```python
+from ambient_package_update.metadata.author import PackageAuthor
+from ambient_package_update.metadata.constants import DEV_DEPENDENCIES
+from ambient_package_update.metadata.package import PackageMetadata
+from ambient_package_update.metadata.readme import ReadmeContent
+from ambient_package_update.metadata.ruff_ignored_inspection import RuffIgnoredInspection
+
+METADATA = PackageMetadata(
+    package_name='my_package_name',
+    authors=[
+        PackageAuthor(
+            name='Ambient Digital',
+            email='hello@ambient.digital',
+        ),
+    ],
+    development_status='5 - Production/Stable',
+    readme_content=ReadmeContent(
+        tagline='A fancy tagline for your new package',
+        content="""A multiline string containing specific things you want to have in your package readme.
+""",
+    ),
+    dependencies=[
+        'my_dependency>=1.0',
+    ],
+    optional_dependencies={
+        'dev': [
+            *DEV_DEPENDENCIES,
+        ],
+        # you might add further extras here
+    },
+    ruff_ignore_list=[
+        RuffIgnoredInspection(key='XYZ', comment="Reason why we need this exception"),
+
+    ],
+)
+```
+
+- Install the `ambient_package_update` package
+  ```
+  # ideally in a virtual environment
+  pip install ambient-package-update
+  ```
+- Add `docs/index.rst` and link your readme and changelog to have a basic documentation (surely, you can add or write
+  more custom docs if you want!)
+- Enable the readthedocs hook in your GitHub repo to update your documentation on a commit basis
+- Finally, follow the steps of the section above (`How to update a package`).
+
+## Contribution
+
+### Dependency updates
+
+The dependencies of this package are being maintained with `pip-tools`. 
+
+> pip install -U pip-tools
+
+To add/update/remove a package, please do so in the main `pyproject.toml`. Afterward, call the following command to
+reflect your changes in the `requirements.txt`.
+
+> pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking
+
+To install the packages, run:
+
+> pip-sync
+
+### Publish to PyPi
+
+- Update documentation about new/changed functionality
+
+- Update the `Changelog`
+
+- Increment version in main `__init__.py`
+
+- Increment version of this package in dependencies in `ambient_package_update/metadata/constants.py`
+
+- Create pull request / merge to master
+
+- This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
+
+  ```
+  flit publish
+  ```
+
+  To publish to TestPyPI use the following ensure that you have set up your .pypirc as
+  shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
+
+  ```
+  flit publish --repository testpypi
+  ```
+
+## Changelog
+
+Can be found at [GitHub](https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md).
```

### Comparing `ambient_package_update-23.9.5/ambient_package_update/cli.py` & `ambient_package_update-24.4.1/ambient_package_update/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,116 @@
-import os
-import subprocess
-import sys
-from datetime import UTC, datetime
-from importlib import import_module
-from pathlib import Path
-
-import typer
-from jinja2 import Template
-
-from ambient_package_update.metadata.constants import LICENSE_GPL
-from ambient_package_update.metadata.package import PackageMetadata
-
-BASE_PATH = Path(__file__).parent
-
-app = typer.Typer()
-
-
-@app.command()
-def get_metadata() -> PackageMetadata:
-    sys.path.append("./.ambient-package-update")
-    try:
-        m = import_module('metadata')
-    except ModuleNotFoundError as e:
-        raise RuntimeError('Please create a directory ".ambient-package-update" and add a "metadata.py".') from e
-    sys.path.pop()
-
-    return m.METADATA
-
-
-def get_template_path() -> Path:
-    return BASE_PATH / "templates"
-
-
-def create_rendered_file(*, template: Path, relative_target_path: Path | str) -> None:
-    """
-    Takes a template Path object and renders a template in the target package.
-    """
-    metadata_dict = get_metadata().__dict__
-
-    j2_template = Template(template.read_text(), keep_trailing_newline=True)
-    j2_template.globals['current_year'] = datetime.now(tz=UTC).date().year
-    j2_template.globals['license_label'] = (
-        "GNU General Public License (GPL)" if metadata_dict['license'] == LICENSE_GPL else "MIT License"
-    )
-
-    rendered_string = j2_template.render(metadata_dict)
-
-    # Create missing directories
-    print(relative_target_path)
-    relative_target_dir = os.path.dirname(relative_target_path)
-    if relative_target_dir:
-        os.makedirs(os.path.dirname(relative_target_path), exist_ok=True)
-
-    with open(relative_target_path, 'w') as f:
-        f.write(rendered_string)
-
-    abs_path = Path(relative_target_path).resolve()
-    print(f'> Successfully rendered template "{abs_path}".')
-
-
-@app.command()
-def render_templates():
-    template_list = []
-    # Collect all template files and add them to "template_list"
-    for path, subdirs, files in os.walk(get_template_path()):
-        print(path, subdirs, files)
-        for file in files:
-            template_list.append(Path(f"{path}/{file}"))
-
-    print('Start rending distribution templates.')
-
-    for template in template_list:
-        create_rendered_file(
-            template=template, relative_target_path=str(Path(template).relative_to(get_template_path()))[:-4]
-        )
-
-    # License file is conditional so we have to render it separately
-    metadata_dict = get_metadata().__dict__
-    create_rendered_file(
-        template=BASE_PATH / f"licenses/{metadata_dict['license']}.md", relative_target_path='LICENSE.md'
-    )
-
-    print('Rendering finished.')
-
-
-@app.command()
-def build_docs(package_name: str):
-    print(f'Building docs for package "{package_name}"')
-    subprocess.call(f"cd ../{package_name} && sphinx-build docs/ docs/_build/html/", shell=True)
-
-
-@app.command()
-def run_tests():
-    print('Running tests')
-
-    package_data = get_metadata()
-    dependency_list = package_data.dependencies
-
-    if package_data.optional_dependencies:
-        for _, opt_dependency in package_data.optional_dependencies.items():
-            dependency_list += opt_dependency
-
-    dependency_list = ' '.join(f'"{d}"' for d in dependency_list)
-    subprocess.call(f"pip install {dependency_list}", shell=True)
-
-    subprocess.call("pytest --ds settings tests", shell=True)
-
-
-if __name__ == "__main__":
-    app()
+import os
+import subprocess
+import sys
+from datetime import UTC, datetime
+from importlib import import_module
+from os.path import basename
+from pathlib import Path
+
+import typer
+from jinja2 import Template
+
+from ambient_package_update.metadata.constants import LICENSE_GPL
+from ambient_package_update.metadata.package import PackageMetadata
+
+BASE_PATH = Path(__file__).parent
+
+app = typer.Typer()
+
+
+@app.command()
+def get_metadata() -> PackageMetadata:
+    sys.path.append("./.ambient-package-update")
+    try:
+        m = import_module("metadata")
+    except ModuleNotFoundError as e:
+        raise RuntimeError('Please create a directory ".ambient-package-update" and add a "metadata.py".') from e
+    sys.path.pop()
+
+    return m.METADATA
+
+
+def get_template_path() -> Path:
+    return BASE_PATH / "templates"
+
+
+def create_rendered_file(*, template: Path, relative_target_path: Path | str) -> None:
+    """
+    Takes a template Path object and renders a template in the target package.
+    """
+    metadata_dict = get_metadata().__dict__
+
+    # Special case: We might want to set an explicit GitHub package name
+    metadata_dict["github_package_name"] = (
+        metadata_dict["github_package_name"] if metadata_dict["github_package_name"] else metadata_dict["package_name"]
+    )
+
+    j2_template = Template(template.read_text(), keep_trailing_newline=True)
+    j2_template.globals["current_year"] = datetime.now(tz=UTC).date().year
+    j2_template.globals["license_label"] = (
+        "GNU General Public License (GPL)" if metadata_dict["license"] == LICENSE_GPL else "MIT License"
+    )
+
+    print(f"> Rendering template {basename(template)!r}...")
+    rendered_string = j2_template.render(metadata_dict)
+
+    # Create missing directories
+    relative_target_dir = os.path.dirname(relative_target_path)
+    if relative_target_dir:
+        os.makedirs(os.path.dirname(relative_target_path), exist_ok=True)
+
+    with open(relative_target_path, "w") as f:
+        f.write(rendered_string)
+
+    abs_path = Path(relative_target_path).resolve()
+    print(f'> Successfully rendered template "{abs_path}".')
+
+
+@app.command()
+def render_templates():
+    template_list = []
+    # Collect all template files and add them to "template_list"
+    for path, subdirs, files in os.walk(get_template_path()):
+        print(path, subdirs, files)
+        [template_list.append(Path(f"{path}/{file}")) for file in files]
+
+    print("Start rending distribution templates.")
+
+    for template in template_list:
+        create_rendered_file(
+            template=template, relative_target_path=str(Path(template).relative_to(get_template_path()))[:-4]
+        )
+
+    # License file is conditional so we have to render it separately
+    metadata_dict = get_metadata().__dict__
+    create_rendered_file(
+        template=BASE_PATH / f"licenses/{metadata_dict['license']}.md", relative_target_path="LICENSE.md"
+    )
+
+    print("Rendering finished.")
+
+
+@app.command()
+def build_docs(package_name: str):
+    print(f'Building docs for package "{package_name}"')
+    subprocess.call(f"cd ../{package_name} && sphinx-build docs/ docs/_build/html/", shell=True)
+
+
+@app.command()
+def run_tests():
+    print("Running tests")
+
+    package_data = get_metadata()
+    dependency_list = package_data.dependencies
+
+    if package_data.optional_dependencies:
+        for opt_dependency in package_data.optional_dependencies.values():
+            dependency_list += opt_dependency
+
+    dependency_list = " ".join(f'"{d}"' for d in dependency_list)
+    subprocess.call(f"pip install {dependency_list}", shell=True)
+
+    subprocess.call("pytest --ds settings tests", shell=True)
+
+
+if __name__ == "__main__":
+    app()
```

### Comparing `ambient_package_update-23.9.5/ambient_package_update/licenses/GPL.md` & `ambient_package_update-24.4.1/ambient_package_update/licenses/GPL.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1347 +1,1347 @@
-GNU GENERAL PUBLIC LICENSE
-Version 3, 29 June 2007
-
- Copyright (C) {{ license_year }} {{ company }}
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-# Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-# GNU GENERAL PUBLIC LICENSE
-## Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-# Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-# TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-# END OF TERMS AND CONDITIONS
-
-## How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
+
+ Copyright (C) {{ license_year }} {{ company }}
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+# Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+# GNU GENERAL PUBLIC LICENSE
+## Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+# Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+# TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+# END OF TERMS AND CONDITIONS
+
+## How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ambient_package_update-23.9.5/ambient_package_update/metadata/package.py` & `ambient_package_update-24.4.1/ambient_package_update/metadata/package.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-import dataclasses
-import datetime
-
-from ambient_package_update.metadata.author import PackageAuthor
-from ambient_package_update.metadata.constants import LICENSE_MIT
-from ambient_package_update.metadata.readme import ReadmeContent
-from ambient_package_update.metadata.ruff_ignored_inspection import RuffIgnoredInspection
-
-
-@dataclasses.dataclass
-class PackageMetadata:
-    package_name: str
-    company: str
-    authors: list[PackageAuthor]
-    development_status: str
-    readme_content: ReadmeContent
-    dependencies: list[str]
-    license: str = LICENSE_MIT
-    license_year: int = datetime.datetime.now(tz=datetime.UTC).year
-    optional_dependencies: dict[str, list[str]] = None
-    ruff_ignore_list: list[RuffIgnoredInspection] = None
+import dataclasses
+import datetime
+
+from ambient_package_update.metadata.author import PackageAuthor
+from ambient_package_update.metadata.constants import LICENSE_MIT
+from ambient_package_update.metadata.readme import ReadmeContent
+from ambient_package_update.metadata.ruff_ignored_inspection import RuffIgnoredInspection
+
+
+@dataclasses.dataclass
+class PackageMetadata:
+    package_name: str
+    company: str
+    authors: list[PackageAuthor]
+    development_status: str
+    readme_content: ReadmeContent
+    has_migrations: bool
+    dependencies: list[str]
+    supported_django_versions: list[str]
+    supported_python_versions: list[str]
+    min_coverage: float = 100.0
+    license: str = LICENSE_MIT
+    license_year: int = datetime.datetime.now(tz=datetime.UTC).year
+    github_package_name: str = None
+    optional_dependencies: dict[str, list[str]] = None
+    ruff_ignore_list: list[RuffIgnoredInspection] = None
```

### Comparing `ambient_package_update-23.9.5/ambient_package_update/templates/README.md.tpl` & `ambient_package_update-24.4.1/ambient_package_update/templates/README.md.tpl`

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,160 @@
-[![PyPI release](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)](https://pypi.org/project/{{ package_name|replace("_", "-") }}/)
-[![Downloads](https://static.pepy.tech/badge/{{ package_name|replace("_", "-") }})](https://pepy.tech/project/{{ package_name|replace("_", "-") }})
-[![Coding Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![Documentation Status](https://readthedocs.org/projects/{{ package_name|replace("_", "-") }}/badge/?version=latest)](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/?badge=latest)
-
-{{ readme_content.tagline }}
-
-* [PyPI](https://pypi.org/project/{{ package_name|replace("_", "-") }}/)
-* [GitHub](https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }})
-* [Full documentation](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html)
-* Creator & Maintainer: [Ambient Digital](https://ambient.digital)
-
-{{ readme_content.content }}
-
-## Installation
-
-{% if readme_content.installation %}
-  {{ readme_content.installation }}
-{% else %}
-- Install the package via pip:
-
-  `pip install {{ package_name|replace("_", "-") }}`
-
-  or via pipenv:
-
-  `pipenv install {{ package_name|replace("_", "-") }}`
-
-- Add module to `INSTALLED_APPS` within the main django `settings.py`:
-
-    ````
-    INSTALLED_APPS = (
-        ...
-        '{{ package_name }}',
-    )
-     ````
-{% endif %}
-
-## Contribute
-
-### Setup package for development
-
-- Create a Python virtualenv and activate it
-- Install "pip-tools" with `pip install pip-tools`
-- Compile the requirements with `pip-compile --extra {% for area, dependency_list in optional_dependencies.items() %}{{ area }},{% endfor %} -o requirements.txt pyproject.toml --resolver=backtracking`
-- Sync the dependencies with your virtualenv with `pip-sync`
-
-### Add functionality
-
-- Create a new branch for your feature
-- Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
-  `-e /Users/workspace/{{ package_name|replace("_", "-") }}` or via pip  `pip install -e /Users/workspace/{{ package_name|replace("_", "-") }}`
-- Ensure the code passes the tests
-- Create a pull request
-
-### Run tests
-
-- Run tests
-  ````
-  pytest --ds settings tests
-  ````
-
-### Git hooks (via pre-commit)
-
-We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
-vain.
-
-To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
-
-    pre-commit install -t pre-push -t pre-commit --install-hooks
-
-This will permanently install the git hooks for both, frontend and backend, in your local
-[`.git/hooks`](./.git/hooks) folder.
-The hooks are configured in the [`.pre-commit-config.yaml`](templates/.pre-commit-config.yaml.tpl).
-
-You can check whether hooks work as intended using the [run](https://pre-commit.com/#pre-commit-run) command:
-
-    pre-commit run [hook-id] [options]
-
-Example: run single hook
-
-    pre-commit run ruff --all-files --hook-stage push
-
-Example: run all hooks of pre-push stage
-
-    pre-commit run --all-files --hook-stage push
-
-### Update documentation
-
-- To build the documentation run: `sphinx-build docs/ docs/_build/html/`.
-- Open `docs/_build/html/index.html` to see the documentation.
-
-### Translation files
-
-If you have added custom text, make sure to wrap it in `_()` where `_` is
-gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
-
-How to create translation file:
-
-* Navigate to `{{ package_name|replace("_", "-") }}`
-* `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `{{ package_name }}/locale`
-
-How to compile translation files:
-
-* Navigate to `{{ package_name|replace("_", "-") }}`
-* `python manage.py compilemessages`
-* Have a look at the new/changed files within `{{ package_name }}/locale`
-
-### Publish to ReadTheDocs.io
-
-- Fetch the latest changes in GitHub mirror and push them
-- Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
-  up.
-
-### Publish to PyPi
-
-- Update documentation about new/changed functionality
-
-- Update the `Changelog`
-
-- Increment version in main `__init__.py`
-
-- Create pull request / merge to master
-
-- This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
-  ```
-  flit publish
-  ```
-
-  To publish to TestPyPI use the following ensure that you have set up your .pypirc as
-  shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
-
-  ```
-  flit publish --repository testpypi
-  ```
-
-### Maintenance
-
-Please note that this package supports the [ambient-package-update](https://pypi.org/project/ambient-package-update/).
-So you don't have to worry about the maintenance of this package. All important configuration and setup files are
-being rendered by this updater. It works similar to well-known updaters like `pyupgrade` or `django-upgrade`.
-
-To run an update, refer to the [documentation page](https://pypi.org/project/ambient-package-update/)
-of the "ambient-package-update".
+[![PyPI release](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)](https://pypi.org/project/{{ package_name|replace("_", "-") }}/)
+[![Downloads](https://static.pepy.tech/badge/{{ package_name|replace("_", "-") }})](https://pepy.tech/project/{{ package_name|replace("_", "-") }})
+[![Coverage](https://img.shields.io/badge/Coverage-{{ min_coverage }}%25-success)](https://github.com/ambient-innovation/{{ github_package_name|replace("_", "-") }}/actions?workflow=CI)
+[![Linting](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Coding Style](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://github.com/astral-sh/ruff)
+[![Documentation Status](https://readthedocs.org/projects/{{ package_name|replace("_", "-") }}/badge/?version=latest)](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/?badge=latest)
+
+{{ readme_content.tagline }}
+
+* [PyPI](https://pypi.org/project/{{ package_name|replace("_", "-") }}/)
+* [GitHub](https://github.com/ambient-innovation/{{ github_package_name|replace("_", "-") }})
+* [Full documentation](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html)
+* Creator & Maintainer: [Ambient Digital](https://ambient.digital)
+
+{{ readme_content.content }}
+
+## Installation
+
+{% if readme_content.custom_installation %}
+{{ readme_content.custom_installation }}
+{% else %}
+- Install the package via pip:
+
+  `pip install {{ package_name|replace("_", "-") }}`
+
+  or via pipenv:
+
+  `pipenv install {{ package_name|replace("_", "-") }}`
+
+- Add module to `INSTALLED_APPS` within the main django `settings.py`:
+
+    ````
+    INSTALLED_APPS = (
+        ...
+        '{{ package_name }}',
+    )
+     ````
+
+{% if has_migrations %}
+- Apply migrations by running:
+
+  `python ./manage.py migrate`
+{% endif %}
+
+{% if readme_content.additional_installation %}{{ readme_content.additional_installation }}{% endif %}
+{% endif %}
+
+## Contribute
+
+### Setup package for development
+
+- Create a Python virtualenv and activate it
+- Install "pip-tools" with `pip install -U pip-tools`
+- Compile the requirements with `pip-compile --extra {% for area, dependency_list in optional_dependencies.items() %}{{ area }},{% endfor %} -o requirements.txt pyproject.toml --resolver=backtracking`
+- Sync the dependencies with your virtualenv with `pip-sync`
+
+### Add functionality
+
+- Create a new branch for your feature
+- Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
+  `-e /Users/workspace/{{ package_name|replace("_", "-") }}` or via pip  `pip install -e /Users/workspace/{{ package_name|replace("_", "-") }}`
+- Ensure the code passes the tests
+- Create a pull request
+
+### Run tests
+
+- Run tests
+  ````
+  pytest --ds settings tests
+  ````
+
+- Check coverage
+  ````
+  coverage run -m pytest --ds settings tests
+  coverage report -m
+  ````
+
+### Git hooks (via pre-commit)
+
+We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
+vain.
+
+To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
+
+    pre-commit install -t pre-push -t pre-commit --install-hooks
+
+This will permanently install the git hooks for both, frontend and backend, in your local
+[`.git/hooks`](./.git/hooks) folder.
+The hooks are configured in the [`.pre-commit-config.yaml`](templates/.pre-commit-config.yaml.tpl).
+
+You can check whether hooks work as intended using the [run](https://pre-commit.com/#pre-commit-run) command:
+
+    pre-commit run [hook-id] [options]
+
+Example: run single hook
+
+    pre-commit run ruff --all-files --hook-stage push
+
+Example: run all hooks of pre-push stage
+
+    pre-commit run --all-files --hook-stage push
+
+### Update documentation
+
+- To build the documentation run: `sphinx-build docs/ docs/_build/html/`.
+- Open `docs/_build/html/index.html` to see the documentation.
+
+### Translation files
+
+If you have added custom text, make sure to wrap it in `_()` where `_` is
+gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
+
+How to create translation file:
+
+* Navigate to `{{ package_name|replace("_", "-") }}`
+* `python manage.py makemessages -l de`
+* Have a look at the new/changed files within `{{ package_name }}/locale`
+
+How to compile translation files:
+
+* Navigate to `{{ package_name|replace("_", "-") }}`
+* `python manage.py compilemessages`
+* Have a look at the new/changed files within `{{ package_name }}/locale`
+
+### Publish to ReadTheDocs.io
+
+- Fetch the latest changes in GitHub mirror and push them
+- Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
+  up.
+
+### Publish to PyPi
+
+- Update documentation about new/changed functionality
+
+- Update the `Changelog`
+
+- Increment version in main `__init__.py`
+
+- Create pull request / merge to master
+
+- This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
+  ```
+  flit publish
+  ```
+
+  To publish to TestPyPI use the following ensure that you have set up your .pypirc as
+  shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
+
+  ```
+  flit publish --repository testpypi
+  ```
+
+### Maintenance
+
+Please note that this package supports the [ambient-package-update](https://pypi.org/project/ambient-package-update/).
+So you don't have to worry about the maintenance of this package. All important configuration and setup files are
+being rendered by this updater. It works similar to well-known updaters like `pyupgrade` or `django-upgrade`.
+
+To run an update, refer to the [documentation page](https://pypi.org/project/ambient-package-update/)
+of the "ambient-package-update".
```

### Comparing `ambient_package_update-23.9.5/ambient_package_update/templates/docs/Makefile.tpl` & `ambient_package_update-24.4.1/ambient_package_update/templates/docs/Makefile.tpl`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `ambient_package_update-23.9.5/ambient_package_update/templates/pyproject.toml.tpl` & `ambient_package_update-24.4.1/ambient_package_update/templates/pyproject.toml.tpl`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,169 @@
-[build-system]
-requires = ["flit_core>=3.4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "{{ package_name|replace("_", "-") }}"
-authors = [{% for author in authors %}
-    {'name' = '{{ author.name }}', 'email' = '{{ author.email }}'},{% endfor %}
-]
-readme = "README.md"
-classifiers = [
-    "Development Status :: {{ development_status }}",
-    "Environment :: Web Environment",
-    "Framework :: Django",
-    "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.1",
-    "Framework :: Django :: 4.2",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: {{ license_label }}",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Utilities",
-]
-dynamic = ["version", "description"]
-license = {"file" = "LICENSE.md"}
-dependencies = [{% for dependency in dependencies %}
-    '{{ dependency }}',{% endfor %}
-]
-
-{% if optional_dependencies %}
-[project.optional-dependencies]{% for area, dependency_list in optional_dependencies.items() %}
-{{ area }} = [{% for dependency in dependency_list %}
-   '{{ dependency }}',{% endfor %}
-]{% endfor %}{% endif %}
-
-[tool.flit.module]
-name = "{{ package_name }}"
-
-[project.urls]
-'Homepage' = 'https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }}/'
-'Documentation' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html'
-'Maintained by' = 'https://ambient.digital/'
-'Bugtracker' = 'https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }}/issues'
-'Changelog' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/features/changelog.html'
-
-
-[tool.black]
-# use force-exclude, so that black also applies exclude when run using pre-commit: https://github.com/psf/black/issues/395
-force-exclude = '''.*/migrations/.*'''
-line-length = 120
-multi_line_output = 3
-skip-string-normalization = true
-include_trailing_comma = true
-
-[tool.ruff]
-select = [
-    "E",       # pycodestyle errors
-    "W",       # pycodestyle warnings
-    "F",       # Pyflakes
-    "N",       # pep8-naming
-    "I",       # isort
-    "B",       # flake8-bugbear
-    "A",       # flake8-builtins
-    "DTZ",     # flake8-datetimez
-    "DJ",      # flake8-django
-    "RUF100",  # Removes unnecessary "#noqa" comments
-    "YTT",     # Avoid non-future-prove usages of "sys"
-    # "FBT",     # Protects you from the "boolean trap bug"
-    "C4",      # Checks for unnecessary conversions
-    "PIE",     # Bunch of useful rules
-    # "SIM",     # Simplifies your code
-    "INT",     # Validates your gettext translation strings
-    "PGH",     # No all-purpose "# noqa" and eval validation
-    # "UP",      # PyUpgrade
-]
-ignore = [{% for ruff_ignore in ruff_ignore_list %}
-    '{{ ruff_ignore.key }}', # {{ ruff_ignore.comment }}{% endfor %}
-]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = [
-    "E",       # pycodestyle errors
-    "W",       # pycodestyle warnings
-    "F",       # Pyflakes
-    "N",       # pep8-naming
-    "I",       # isort
-    "B",       # flake8-bugbear
-    "A",       # flake8-builtins
-    "DTZ",     # flake8-datetimez
-    "DJ",      # flake8-django
-    "RUF100",  # Removes unnecessary "#noqa" comments
-    "YTT",     # Avoid non-future-prove usages of "sys"
-    # "FBT",     # Protects you from the "boolean trap bug"
-    "C4",      # Checks for unnecessary conversions
-    "PIE",     # Bunch of useful rules
-    # "SIM",     # Simplifies your code
-    "INT",     # Validates your gettext translation strings
-    "PGH",     # No all-purpose "# noqa" and eval validation
-    # "UP",      # PyUpgrade
-]
-unfixable = []
-
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".pytype",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-    "*/migrations/*"
-]
-
-# Same as Black.
-line-length = 120
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-# Assume Python 3.11
-target-version = "py311"
-
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-envlist = py{38,39,310,311}-django{32,41,42}
-isolated_build = True
-
-[testenv]
-# Django deprecation overview: https://www.djangoproject.com/download/
-deps =
-    django32: Django>=3.2,<3.3
-    django41: Django>=4.1,<4.2
-    django42: Django>=4.2,<4.3
-extras = {% for area, dependency_list in optional_dependencies.items() %}{{ area }},{% endfor %}
-commands =
-    pytest --ds settings tests
-
-[gh-actions]
-python =
-    3.8: py38
-    3.9: py39
-    3.10: py310
-    3.11: py311
-"""
+[build-system]
+requires = ["flit_core>=3.4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "{{ package_name|replace("_", "-") }}"
+authors = [{% for author in authors %}
+    {'name' = '{{ author.name }}', 'email' = '{{ author.email }}'},{% endfor %}
+]
+readme = "README.md"
+classifiers = [
+    "Development Status :: {{ development_status }}",
+    "Environment :: Web Environment",
+    "Framework :: Django",{% for django_version in supported_django_versions %}
+    "Framework :: Django :: {{ django_version }}",{% endfor %}
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: {{ license_label }}",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",{% for python_version in supported_python_versions %}
+    "Programming Language :: Python :: {{ python_version }}",{% endfor %}
+    "Topic :: Utilities",
+]
+dynamic = ["version", "description"]
+license = {"file" = "LICENSE.md"}
+dependencies = [{% for dependency in dependencies %}
+    '{{ dependency }}',{% endfor %}
+]
+
+{% if optional_dependencies %}
+[project.optional-dependencies]{% for area, dependency_list in optional_dependencies.items() %}
+{{ area }} = [{% for dependency in dependency_list %}
+   '{{ dependency }}',{% endfor %}
+]{% endfor %}{% endif %}
+
+[tool.flit.module]
+name = "{{ package_name }}"
+
+[project.urls]
+'Homepage' = 'https://github.com/ambient-innovation/{{ github_package_name|replace("_", "-") }}/'
+'Documentation' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html'
+'Maintained by' = 'https://ambient.digital/'
+'Bugtracker' = 'https://github.com/ambient-innovation/{{ github_package_name|replace("_", "-") }}/issues'
+'Changelog' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/features/changelog.html'
+
+[tool.ruff]
+select = [
+    "E",       # pycodestyle errors
+    "W",       # pycodestyle warnings
+    "F",       # Pyflakes
+    "N",       # pep8-naming
+    "I",       # isort
+    "B",       # flake8-bugbear
+    "A",       # flake8-builtins
+    "DTZ",     # flake8-datetimez
+    "DJ",      # flake8-django
+    "TD",      # flake8-to-do
+    "RUF100",  # Removes unnecessary "#noqa" comments
+    "YTT",     # Avoid non-future-prove usages of "sys"
+    # "FBT",     # Protects you from the "boolean trap bug"
+    "C4",      # Checks for unnecessary conversions
+    "PIE",     # Bunch of useful rules
+    # "SIM",     # Simplifies your code
+    "INT",     # Validates your gettext translation strings
+    "PERF",    # PerfLint
+    "PGH",     # No all-purpose "# noqa" and eval validation
+    "PL",      # PyLint
+]
+ignore = [{% for ruff_ignore in ruff_ignore_list %}
+    '{{ ruff_ignore.key }}', # {{ ruff_ignore.comment }}{% endfor %}
+]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = [
+    "E",       # pycodestyle errors
+    "W",       # pycodestyle warnings
+    "F",       # Pyflakes
+    "N",       # pep8-naming
+    "I",       # isort
+    "B",       # flake8-bugbear
+    "A",       # flake8-builtins
+    "DTZ",     # flake8-datetimez
+    "DJ",      # flake8-django
+    "TD",      # flake8-to-do
+    "RUF100",  # Removes unnecessary "#noqa" comments
+    "YTT",     # Avoid non-future-prove usages of "sys"
+    # "FBT",     # Protects you from the "boolean trap bug"
+    "C4",      # Checks for unnecessary conversions
+    "PIE",     # Bunch of useful rules
+    # "SIM",     # Simplifies your code
+    "INT",     # Validates your gettext translation strings
+    "PERF",    # PerfLint
+    "PGH",     # No all-purpose "# noqa" and eval validation
+    "PL",      # PyLint
+]
+unfixable = []
+
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "*/migrations/*"
+]
+
+# Same as Black.
+line-length = 120
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.12
+target-version = "py312"
+
+[tool.ruff.format]
+# Like Black, use double quotes for strings.
+quote-style = "double"
+
+# Like Black, indent with spaces, rather than tabs.
+indent-style = "space"
+
+# Like Black, respect magic trailing commas.
+skip-magic-trailing-comma = false
+
+# Like Black, automatically detect the appropriate line ending.
+line-ending = "auto"
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+envlist = py{38,39,310,311}-django{32,41,42}
+isolated_build = True
+
+[testenv]
+# Django deprecation overview: https://www.djangoproject.com/download/
+deps ={% for django_version in supported_django_versions %}
+    django{{ django_version|replace(".", "") }}: Django=={{ django_version }}.*{% endfor %}
+extras = {% for area, dependency_list in optional_dependencies.items() %}{{ area }},{% endfor %}
+commands =
+    coverage run -m pytest --ds settings tests
+
+[gh-actions]
+python ={% for python_version in supported_python_versions %}
+    {{ python_version }}: py{{ python_version|replace(".", "") }}{% endfor %}
+"""
+
+[tool.pytest.ini_options]
+python_files = [
+    "tests.py",
+    "test_*.py",
+    "*_tests.py",
+]
```

### Comparing `ambient_package_update-23.9.5/scripts/unix/setup_venv_unix.sh` & `ambient_package_update-24.4.1/scripts/unix/setup_venv_unix.sh`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#!/bin/bash
-
-echo "Create virtualenv"
-python -m venv venv
-echo "Activate virtualenv"
-source "./venv/bin/activate"
-echo "Update pip"
-python -m pip install --upgrade pip
-echo "Install pip-tools"
-pip install pip-tools
-echo "Render requirements file"
-pip-compile --extra=dev -o requirements.txt pyproject.toml --resolver=backtracking
-echo "Install python dependencies"
-pip-sync
-echo "Install dependencies from requirements"
-python -m pip install -r requirements.txt
-echo "Install git hooks"
-pre-commit install -t pre-push -t pre-commit --install-hooks
+#!/bin/bash
+
+echo "Create virtualenv"
+python -m venv venv
+echo "Activate virtualenv"
+source "./venv/bin/activate"
+echo "Update pip"
+python -m pip install --upgrade pip
+echo "Install pip-tools"
+pip install pip-tools
+echo "Render requirements file"
+pip-compile --extra=dev -o requirements.txt pyproject.toml --resolver=backtracking
+echo "Install python dependencies"
+pip-sync
+echo "Install dependencies from requirements"
+python -m pip install -r requirements.txt
+echo "Install git hooks"
+pre-commit install -t pre-push -t pre-commit --install-hooks
```

### Comparing `ambient_package_update-23.9.5/PKG-INFO` & `ambient_package_update-24.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.9.5
+Version: 24.4.1
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Dist: typer~=0.9
-Requires-Dist: Jinja2~=3.1
-Requires-Dist: flit~=3.9
-Requires-Dist: keyring~=24.2
-Requires-Dist: pre-commit~=3.3
-Requires-Dist: black~=23.7
+Requires-Dist: typer~=0.9 ; extra == "dev"
+Requires-Dist: Jinja2~=3.1 ; extra == "dev"
+Requires-Dist: flit~=3.9 ; extra == "dev"
+Requires-Dist: keyring~=24.2 ; extra == "dev"
+Requires-Dist: pre-commit~=3.5 ; extra == "dev"
+Requires-Dist: ruff~=0.1 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-package-update/issues
 Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md
 Project-URL: Documentation, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md
 Project-URL: Homepage, https://github.com/ambient-innovation/ambient-package-update/
 Project-URL: Maintained by, https://ambient.digital/
+Provides-Extra: dev
 
 [![PyPI release](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.org/project/ambient-package-update/)
 [![Downloads](https://static.pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
-[![Coding Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Linting](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Coding Style](https://img.shields.io/badge/code%20style-Ruff-000000.svg)](https://github.com/astral-sh/ruff)
 
 # Ambient Package Update
 
 This repository will help keep all Python packages following a certain basic structure tidy and up-to-date. It's being 
 maintained by [Ambient Digital](https://ambient.digital). 
 
 This package will render all required configuration and installation files for your target package.
@@ -121,15 +123,15 @@
 The dependencies of this package are being maintained with `pip-tools`. 
 
 > pip install -U pip-tools
 
 To add/update/remove a package, please do so in the main `pyproject.toml`. Afterward, call the following command to
 reflect your changes in the `requirements.txt`.
 
-> pip-compile --upgrade
+> pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking
 
 To install the packages, run:
 
 > pip-sync
 
 ### Publish to PyPi
```

