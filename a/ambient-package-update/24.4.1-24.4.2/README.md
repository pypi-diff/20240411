# Comparing `tmp/ambient_package_update-24.4.1.tar.gz` & `tmp/ambient_package_update-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_package_update-24.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ambient_package_update-24.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient_package_update-24.4.1.tar` & `ambient_package_update-24.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      432 2024-03-28 09:26:53.193919 ambient_package_update-24.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3122 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/.gitignore
--rw-r--r--   0        0        0      642 2024-04-11 13:38:59.651610 ambient_package_update-24.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4001 2023-12-05 11:25:02.798121 ambient_package_update-24.4.1/CHANGES.md
--rw-r--r--   0        0        0     1064 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/LICENSE.md
--rw-r--r--   0        0        0     4719 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/README.md
--rw-r--r--   0        0        0       90 2024-04-11 13:40:04.722334 ambient_package_update-24.4.1/ambient_package_update/__init__.py
--rw-r--r--   0        0        0     3681 2023-12-05 11:19:03.483109 ambient_package_update-24.4.1/ambient_package_update/cli.py
--rw-r--r--   0        0        0    70069 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/ambient_package_update/licenses/GPL.md
--rw-r--r--   0        0        0     1084 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/ambient_package_update/licenses/MIT.md
--rw-r--r--   0        0        0        0 2023-12-04 15:03:51.349480 ambient_package_update-24.4.1/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0       94 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      689 2024-04-11 13:41:03.522281 ambient_package_update-24.4.1/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      918 2023-12-05 11:16:09.487698 ambient_package_update-24.4.1/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      240 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      103 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0      303 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      270 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     2987 2024-03-28 09:40:18.641481 ambient_package_update-24.4.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      720 2024-04-11 13:37:12.286993 ambient_package_update-24.4.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      742 2023-12-04 15:03:51.353492 ambient_package_update-24.4.1/ambient_package_update/templates/.readthedocs.yaml.tpl
--rw-r--r--   0        0        0      133 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     5881 2023-12-05 11:23:35.552515 ambient_package_update-24.4.1/ambient_package_update/templates/README.md.tpl
--rw-r--r--   0        0        0      634 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2769 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      760 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     5281 2024-04-11 13:49:19.793561 ambient_package_update-24.4.1/ambient_package_update/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0      201 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/unix/install_requirements.sh.tpl
--rw-r--r--   0        0        0       49 2023-12-04 15:03:51.356000 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/unix/publish_to_pypi.sh.tpl
--rw-r--r--   0        0        0      201 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/windows/install_requirements.ps1.tpl
--rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/ambient_package_update/templates/scripts/windows/publish_to_pypi.ps1.tpl
--rw-r--r--   0        0        0      269 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/ambient_package_update/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     4143 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/pyproject.toml
--rw-r--r--   0        0        0     1482 2023-12-04 15:06:50.299033 ambient_package_update-24.4.1/requirements.txt
--rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      548 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/unix/setup_venv_unix.sh
--rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0      446 2023-12-04 15:03:51.358527 ambient_package_update-24.4.1/scripts/windows/setup_venv.ps1
--rw-r--r--   0        0        0     6119 1970-01-01 00:00:00.000000 ambient_package_update-24.4.1/PKG-INFO
+-rw-r--r--   0        0        0      432 2024-03-28 09:26:53.193919 ambient_package_update-24.4.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3122 2023-12-04 15:03:51.349480 ambient_package_update-24.4.2/.gitignore
+-rw-r--r--   0        0        0      642 2024-04-11 13:38:59.651610 ambient_package_update-24.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4189 2024-04-11 13:51:54.170705 ambient_package_update-24.4.2/CHANGES.md
+-rw-r--r--   0        0        0     1064 2023-12-04 15:03:51.349480 ambient_package_update-24.4.2/LICENSE.md
+-rw-r--r--   0        0        0     4719 2023-12-04 15:03:51.349480 ambient_package_update-24.4.2/README.md
+-rw-r--r--   0        0        0       90 2024-04-11 13:51:54.170705 ambient_package_update-24.4.2/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0     3681 2023-12-05 11:19:03.483109 ambient_package_update-24.4.2/ambient_package_update/cli.py
+-rw-r--r--   0        0        0    70069 2023-12-04 15:03:51.349480 ambient_package_update-24.4.2/ambient_package_update/licenses/GPL.md
+-rw-r--r--   0        0        0     1084 2023-12-04 15:03:51.349480 ambient_package_update-24.4.2/ambient_package_update/licenses/MIT.md
+-rw-r--r--   0        0        0        0 2023-12-04 15:03:51.349480 ambient_package_update-24.4.2/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0       94 2023-12-04 15:03:51.353492 ambient_package_update-24.4.2/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      689 2024-04-11 13:41:03.522281 ambient_package_update-24.4.2/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      918 2023-12-05 11:16:09.487698 ambient_package_update-24.4.2/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      240 2023-12-04 15:03:51.353492 ambient_package_update-24.4.2/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      103 2023-12-04 15:03:51.353492 ambient_package_update-24.4.2/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0      303 2023-12-04 15:03:51.353492 ambient_package_update-24.4.2/ambient_package_update/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      270 2023-12-04 15:03:51.353492 ambient_package_update-24.4.2/ambient_package_update/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     2987 2024-03-28 09:40:18.641481 ambient_package_update-24.4.2/ambient_package_update/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      720 2024-04-11 13:37:12.286993 ambient_package_update-24.4.2/ambient_package_update/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      742 2023-12-04 15:03:51.353492 ambient_package_update-24.4.2/ambient_package_update/templates/.readthedocs.yaml.tpl
+-rw-r--r--   0        0        0      133 2023-12-04 15:03:51.356000 ambient_package_update-24.4.2/ambient_package_update/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5881 2023-12-05 11:23:35.552515 ambient_package_update-24.4.2/ambient_package_update/templates/README.md.tpl
+-rw-r--r--   0        0        0      634 2023-12-04 15:03:51.356000 ambient_package_update-24.4.2/ambient_package_update/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2769 2023-12-04 15:03:51.356000 ambient_package_update-24.4.2/ambient_package_update/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      760 2023-12-04 15:03:51.356000 ambient_package_update-24.4.2/ambient_package_update/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     5281 2024-04-11 13:49:19.793561 ambient_package_update-24.4.2/ambient_package_update/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0      201 2023-12-04 15:03:51.356000 ambient_package_update-24.4.2/ambient_package_update/templates/scripts/unix/install_requirements.sh.tpl
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.356000 ambient_package_update-24.4.2/ambient_package_update/templates/scripts/unix/publish_to_pypi.sh.tpl
+-rw-r--r--   0        0        0      201 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/ambient_package_update/templates/scripts/windows/install_requirements.ps1.tpl
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/ambient_package_update/templates/scripts/windows/publish_to_pypi.ps1.tpl
+-rw-r--r--   0        0        0      269 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/ambient_package_update/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     4143 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1482 2023-12-04 15:06:50.299033 ambient_package_update-24.4.2/requirements.txt
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      548 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/scripts/unix/setup_venv_unix.sh
+-rw-r--r--   0        0        0       49 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0      446 2023-12-04 15:03:51.358527 ambient_package_update-24.4.2/scripts/windows/setup_venv.ps1
+-rw-r--r--   0        0        0     6119 1970-01-01 00:00:00.000000 ambient_package_update-24.4.2/PKG-INFO
```

### Comparing `ambient_package_update-24.4.1/.gitignore` & `ambient_package_update-24.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/.pre-commit-config.yaml` & `ambient_package_update-24.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/CHANGES.md` & `ambient_package_update-24.4.2/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+**24.4.2 (2024-04-11)**
+* Updated Changelog.md
+
+**24.4.1 (2024-04-11)**
+* Dropped Django 3.2 & 4.1
+* Updated linters
+* Updated some GitHub actions
+* Moved pytest config to pyproject.toml
+
 **23.12.4 (2023-12-05)**
 * Added optional GitHub package name
 * Added "flit" to package dev dependencies
 
 **23.12.3 (2023-12-05)**
 * Dependency-Constants updated
```

### Comparing `ambient_package_update-24.4.1/LICENSE.md` & `ambient_package_update-24.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/README.md` & `ambient_package_update-24.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/cli.py` & `ambient_package_update-24.4.2/ambient_package_update/cli.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/licenses/GPL.md` & `ambient_package_update-24.4.2/ambient_package_update/licenses/GPL.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/licenses/MIT.md` & `ambient_package_update-24.4.2/ambient_package_update/licenses/MIT.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/metadata/constants.py` & `ambient_package_update-24.4.2/ambient_package_update/metadata/constants.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/metadata/package.py` & `ambient_package_update-24.4.2/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/.readthedocs.yaml.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/.readthedocs.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/README.md.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/README.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/docs/Makefile.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/docs/conf.py.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/docs/make.bat.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/ambient_package_update/templates/pyproject.toml.tpl` & `ambient_package_update-24.4.2/ambient_package_update/templates/pyproject.toml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/pyproject.toml` & `ambient_package_update-24.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/requirements.txt` & `ambient_package_update-24.4.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/scripts/unix/setup_venv_unix.sh` & `ambient_package_update-24.4.2/scripts/unix/setup_venv_unix.sh`

 * *Files identical despite different names*

### Comparing `ambient_package_update-24.4.1/PKG-INFO` & `ambient_package_update-24.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 24.4.1
+Version: 24.4.2
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```
