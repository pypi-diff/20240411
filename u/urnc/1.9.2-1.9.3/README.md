# Comparing `tmp/urnc-1.9.2.tar.gz` & `tmp/urnc-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urnc-1.9.2.tar", last modified: Fri Dec 29 11:37:27 2023, max compression
+gzip compressed data, was "urnc-1.9.3.tar", last modified: Thu Jan  4 17:49:42 2024, max compression
```

## Comparing `urnc-1.9.2.tar` & `urnc-1.9.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:27.540639 urnc-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-29 11:37:15.000000 urnc-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-12-29 11:37:27.540639 urnc-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-12-29 11:37:15.000000 urnc-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-12-29 11:37:15.000000 urnc-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 11:37:27.540639 urnc-1.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:27.540639 urnc-1.9.2/urnc/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:27.540639 urnc-1.9.2/urnc/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/preprocessor/add_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/preprocessor/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/preprocessor/remove_solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/preprocessor/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-12-29 11:37:15.000000 urnc-1.9.2/urnc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:27.540639 urnc-1.9.2/urnc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-12-29 11:37:27.000000 urnc-1.9.2/urnc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-29 11:37:27.000000 urnc-1.9.2/urnc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 11:37:27.000000 urnc-1.9.2/urnc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-29 11:37:27.000000 urnc-1.9.2/urnc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-29 11:37:27.000000 urnc-1.9.2/urnc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-29 11:37:27.000000 urnc-1.9.2/urnc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:42.722367 urnc-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-04 17:49:33.000000 urnc-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-01-04 17:49:42.722367 urnc-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-01-04 17:49:33.000000 urnc-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-04 17:49:33.000000 urnc-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 17:49:42.722367 urnc-1.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:42.722367 urnc-1.9.3/urnc/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:42.722367 urnc-1.9.3/urnc/preprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/preprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/preprocessor/add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/preprocessor/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/preprocessor/remove_solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/preprocessor/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-01-04 17:49:33.000000 urnc-1.9.3/urnc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:42.722367 urnc-1.9.3/urnc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-01-04 17:49:42.000000 urnc-1.9.3/urnc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-04 17:49:42.000000 urnc-1.9.3/urnc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 17:49:42.000000 urnc-1.9.3/urnc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-04 17:49:42.000000 urnc-1.9.3/urnc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-04 17:49:42.000000 urnc-1.9.3/urnc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-04 17:49:42.000000 urnc-1.9.3/urnc.egg-info/top_level.txt
```

### Comparing `urnc-1.9.2/LICENSE` & `urnc-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/PKG-INFO` & `urnc-1.9.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urnc
-Version: 1.9.2
+Version: 1.9.3
 Summary: A package to convert UR FIDS jupyter notebooks
 Author-email: Michael Huttner <michael@mhuttner.com>, Tobias Schmidt <tobias.schmidt331@gmail.com>
 Project-URL: Homepage, https://spang-lab.github.io/urnc
 Project-URL: Source, https://github.com/spang-lab/urnc
 Project-URL: Bug Tracker, https://github.com/spang-lab/urnc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,19 @@
 Requires-Dist: python-dateutil>=2
 Requires-Dist: GitPython>=3.1.31
 Requires-Dist: nbconvert>=7.8.0
 Requires-Dist: semver>=3.0.1
 Requires-Dist: tomli_w>=1.0.0
 Requires-Dist: ruamel.yaml>=0.18.4
 Requires-Dist: requests>=2.31.0
-Requires-Dist: freezegun
+
+[![PyTest](https://github.com/spang-lab/urnc/actions/workflows/test.yaml/badge.svg)](https://github.com/spang-lab/urnc/actions)
+[![Codecov](https://codecov.io/gh/spang-lab/urnc/branch/main/graph/badge.svg)](https://app.codecov.io/gh/spang-lab/urnc?branch=main)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/urnc.svg?label=PyPI%20downloads)](
+https://pypi.org/project/urnc/)
 
 # URNC
 
 Uni Regensburg Notebook Converter
 
 ## Installation
```

### Comparing `urnc-1.9.2/README.md` & `urnc-1.9.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![PyTest](https://github.com/spang-lab/urnc/actions/workflows/test.yaml/badge.svg)](https://github.com/spang-lab/urnc/actions)
+[![Codecov](https://codecov.io/gh/spang-lab/urnc/branch/main/graph/badge.svg)](https://app.codecov.io/gh/spang-lab/urnc?branch=main)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/urnc.svg?label=PyPI%20downloads)](
+https://pypi.org/project/urnc/)
+
 # URNC
 
 Uni Regensburg Notebook Converter
 
 ## Installation
 
 ```sh
```

### Comparing `urnc-1.9.2/urnc/ci.py` & `urnc-1.9.3/urnc/ci.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 def write_gitignore(repo, student_repo, config):
     main_gitignore = join(repo.working_dir, ".gitignore")
     student_gitignore = join(student_repo.working_dir, ".gitignore")
     if (exists(main_gitignore)):
         shutil.copy(main_gitignore, student_gitignore)
     exclude = get_config_value(config, "git", "exclude", default=[])
     now = datetime.now()
-    with open(student_gitignore, "a") as gitignore:
+    with open(student_gitignore, "a", newline = "\n") as gitignore:
         for value in exclude:
             if isinstance(value, str):
                 gitignore.write(f"{value}\n")
             else:
                 if "after" in value:
                     if now < dateutil.parser.parse(value["after"]):
                         continue
```

### Comparing `urnc-1.9.2/urnc/convert.py` & `urnc-1.9.3/urnc/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,9 +76,9 @@
         notebook = nbformat.read(file, as_version=4)
         resources = {}
         resources["path"] = file
         (output_text, _) = converter.from_notebook_node(notebook, resources)
 
         if (out_file is None or dry_run):
             continue
-        with open(out_file, "w") as f:
+        with open(out_file, "w", newline='\n') as f:
             f.write(output_text)
```

### Comparing `urnc-1.9.2/urnc/logger.py` & `urnc-1.9.3/urnc/logger.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/main.py` & `urnc-1.9.3/urnc/main.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/preprocessor/add_tags.py` & `urnc-1.9.3/urnc/preprocessor/add_tags.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/preprocessor/lint.py` & `urnc-1.9.3/urnc/preprocessor/lint.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/preprocessor/remove_solutions.py` & `urnc-1.9.3/urnc/preprocessor/remove_solutions.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/preprocessor/util.py` & `urnc-1.9.3/urnc/preprocessor/util.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/pull.py` & `urnc-1.9.3/urnc/pull.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc/util.py` & `urnc-1.9.3/urnc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 def write_config(data):
     filename = "config.yaml"
     base_path = get_git_root()
 
     path = os.path.join(base_path, filename)
     try:
-        with open(path, "w") as f:
+        with open(path, "w", newline = "\n") as f:
             yaml.dump(data, f)
             return path
     except Exception as e:
         raise click.FileError(path, str(e))
 
 
 def read_pyproject():
```

### Comparing `urnc-1.9.2/urnc/version.py` & `urnc-1.9.3/urnc/version.py`

 * *Files identical despite different names*

### Comparing `urnc-1.9.2/urnc.egg-info/PKG-INFO` & `urnc-1.9.3/urnc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urnc
-Version: 1.9.2
+Version: 1.9.3
 Summary: A package to convert UR FIDS jupyter notebooks
 Author-email: Michael Huttner <michael@mhuttner.com>, Tobias Schmidt <tobias.schmidt331@gmail.com>
 Project-URL: Homepage, https://spang-lab.github.io/urnc
 Project-URL: Source, https://github.com/spang-lab/urnc
 Project-URL: Bug Tracker, https://github.com/spang-lab/urnc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,19 @@
 Requires-Dist: python-dateutil>=2
 Requires-Dist: GitPython>=3.1.31
 Requires-Dist: nbconvert>=7.8.0
 Requires-Dist: semver>=3.0.1
 Requires-Dist: tomli_w>=1.0.0
 Requires-Dist: ruamel.yaml>=0.18.4
 Requires-Dist: requests>=2.31.0
-Requires-Dist: freezegun
+
+[![PyTest](https://github.com/spang-lab/urnc/actions/workflows/test.yaml/badge.svg)](https://github.com/spang-lab/urnc/actions)
+[![Codecov](https://codecov.io/gh/spang-lab/urnc/branch/main/graph/badge.svg)](https://app.codecov.io/gh/spang-lab/urnc?branch=main)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/urnc.svg?label=PyPI%20downloads)](
+https://pypi.org/project/urnc/)
 
 # URNC
 
 Uni Regensburg Notebook Converter
 
 ## Installation
```

