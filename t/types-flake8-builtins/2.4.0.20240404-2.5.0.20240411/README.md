# Comparing `tmp/types-flake8-builtins-2.4.0.20240404.tar.gz` & `tmp/types-flake8-builtins-2.5.0.20240411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-builtins-2.4.0.20240404.tar", last modified: Thu Apr  4 02:16:32 2024, max compression
+gzip compressed data, was "types-flake8-builtins-2.5.0.20240411.tar", last modified: Thu Apr 11 02:17:26 2024, max compression
```

## Comparing `types-flake8-builtins-2.4.0.20240404.tar` & `types-flake8-builtins-2.5.0.20240411.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:26.797950 types-flake8-builtins-2.5.0.20240411/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-11 02:17:24.000000 types-flake8-builtins-2.5.0.20240411/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 02:17:24.000000 types-flake8-builtins-2.5.0.20240411/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-11 02:17:26.797950 types-flake8-builtins-2.5.0.20240411/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:26.793950 types-flake8-builtins-2.5.0.20240411/flake8_builtins-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-11 02:17:24.000000 types-flake8-builtins-2.5.0.20240411/flake8_builtins-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-11 02:17:24.000000 types-flake8-builtins-2.5.0.20240411/flake8_builtins-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 02:17:24.000000 types-flake8-builtins-2.5.0.20240411/flake8_builtins-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:17:26.797950 types-flake8-builtins-2.5.0.20240411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 02:17:24.000000 types-flake8-builtins-2.5.0.20240411/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:26.797950 types-flake8-builtins-2.5.0.20240411/types_flake8_builtins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-11 02:17:26.000000 types-flake8-builtins-2.5.0.20240411/types_flake8_builtins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 02:17:26.000000 types-flake8-builtins-2.5.0.20240411/types_flake8_builtins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:17:26.000000 types-flake8-builtins-2.5.0.20240411/types_flake8_builtins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 02:17:26.000000 types-flake8-builtins-2.5.0.20240411/types_flake8_builtins.egg-info/top_level.txt
```

### Comparing `types-flake8-builtins-2.4.0.20240404/CHANGELOG.md` & `types-flake8-builtins-2.5.0.20240411/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+## 2.5.0.20240411 (2024-04-11)
+
+[stubsabot] Bump flake8-builtins to 2.5.* (#11739)
+
+Release: https://pypi.org/pypi/flake8-builtins/2.5.0
+Homepage: https://github.com/gforcada/flake8-builtins
+Repository: https://github.com/gforcada/flake8-builtins
+Changelog: https://github.com/gforcada/flake8-builtins/blob/main/CHANGES.rst
+Diff: https://github.com/gforcada/flake8-builtins/compare/2.4.0...2.5.0
+
+Stubsabot analysis of the diff between the two releases:
+ - 0 public Python files have been added.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 1 file included in typeshed's stubs has been modified or renamed: `flake8_builtins.py`.
+ - Total lines of Python code added: 5.
+ - Total lines of Python code deleted: 1.
+
 ## 2.4.0.20240404 (2024-04-04)
 
 [stubsabot] Bump flake8-builtins to 2.4.* (#11697)
 
 Co-authored-by: stubsabot <>
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
```

### Comparing `types-flake8-builtins-2.4.0.20240404/PKG-INFO` & `types-flake8-builtins-2.5.0.20240411/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-builtins
-Version: 2.4.0.20240404
+Version: 2.5.0.20240411
 Summary: Typing stubs for flake8-builtins
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-builtins.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-builtins`.
 
 This version of `types-flake8-builtins` aims to provide accurate annotations
-for `flake8-builtins==2.4.*`.
+for `flake8-builtins==2.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-builtins. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0685754ab3b9c8c242d064c7b5d78d39d3ab0b57` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
+This package was generated from typeshed commit `fe02cba606d1329afd8b1e28451b390d678305e8` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
 pytype 2024.3.19.
```

### Comparing `types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/__init__.pyi` & `types-flake8-builtins-2.5.0.20240411/flake8_builtins-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-builtins-2.4.0.20240404/setup.py` & `types-flake8-builtins-2.5.0.20240411/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-builtins`.
 
 This version of `types-flake8-builtins` aims to provide accurate annotations
-for `flake8-builtins==2.4.*`.
+for `flake8-builtins==2.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-builtins. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0685754ab3b9c8c242d064c7b5d78d39d3ab0b57` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
+This package was generated from typeshed commit `fe02cba606d1329afd8b1e28451b390d678305e8` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
 pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="2.4.0.20240404",
+      version="2.5.0.20240411",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-builtins.md",
```

### Comparing `types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/PKG-INFO` & `types-flake8-builtins-2.5.0.20240411/types_flake8_builtins.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-builtins
-Version: 2.4.0.20240404
+Version: 2.5.0.20240411
 Summary: Typing stubs for flake8-builtins
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-builtins.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-builtins`.
 
 This version of `types-flake8-builtins` aims to provide accurate annotations
-for `flake8-builtins==2.4.*`.
+for `flake8-builtins==2.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-builtins. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0685754ab3b9c8c242d064c7b5d78d39d3ab0b57` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
+This package was generated from typeshed commit `fe02cba606d1329afd8b1e28451b390d678305e8` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
 pytype 2024.3.19.
```

