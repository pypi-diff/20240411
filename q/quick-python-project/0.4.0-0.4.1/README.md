# Comparing `tmp/quick_python_project-0.4.0.tar.gz` & `tmp/quick_python_project-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_python_project-0.4.0.tar", last modified: Tue Mar 26 21:05:38 2024, max compression
+gzip compressed data, was "quick_python_project-0.4.1.tar", last modified: Thu Apr 11 18:42:12 2024, max compression
```

## Comparing `quick_python_project-0.4.0.tar` & `quick_python_project-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.452676 quick_python_project-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.444676 quick_python_project-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.444676 quick_python_project-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-26 21:05:38.452676 quick_python_project-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 21:05:38.452676 quick_python_project-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.444676 quick_python_project-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.448676 quick_python_project-0.4.0/src/quick_python_project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/project_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.448676 quick_python_project-0.4.0/src/quick_python_project/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template___init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_hatchling_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_poetry_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/src/quick_python_project/templates/template_setuptools_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.448676 quick_python_project-0.4.0/src/quick_python_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-26 21:05:38.000000 quick_python_project-0.4.0/src/quick_python_project.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:38.448676 quick_python_project-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/tests/test_project_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-26 21:05:33.000000 quick_python_project-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.719890 quick_python_project-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.711890 quick_python_project-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.715890 quick_python_project-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-11 18:42:12.719890 quick_python_project-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:42:12.719890 quick_python_project-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.711890 quick_python_project-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.715890 quick_python_project-0.4.1/src/quick_python_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/project_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.719890 quick_python_project-0.4.1/src/quick_python_project/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template___init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_hatchling_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_poetry_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/src/quick_python_project/templates/template_setuptools_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.719890 quick_python_project-0.4.1/src/quick_python_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 18:42:12.000000 quick_python_project-0.4.1/src/quick_python_project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:12.719890 quick_python_project-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/tests/test_project_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-11 18:42:08.000000 quick_python_project-0.4.1/tox.ini
```

### Comparing `quick_python_project-0.4.0/.coveragerc` & `quick_python_project-0.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/.github/workflows/cd.yml` & `quick_python_project-0.4.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/.github/workflows/ci.yml` & `quick_python_project-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/.gitignore` & `quick_python_project-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/PKG-INFO` & `quick_python_project-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: quick_python_project
-Version: 0.4.0
+Version: 0.4.1
 Summary: A CLI tool to create empty Python projects
 Author-email: James Berkheimer <james.berkheimer@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/james-berkheimer/quick_python_project
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: colorlog
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: covdefaults; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `quick_python_project-0.4.0/README.md` & `quick_python_project-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/pyproject.toml` & `quick_python_project-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/src/quick_python_project/cli.py` & `quick_python_project-0.4.1/src/quick_python_project/cli.py`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/src/quick_python_project/project_generation.py` & `quick_python_project-0.4.1/src/quick_python_project/project_generation.py`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/src/quick_python_project/templates/template_.gitignore` & `quick_python_project-0.4.1/src/quick_python_project/templates/template_.gitignore`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/src/quick_python_project/templates/template_LICENSE` & `quick_python_project-0.4.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2024 James Berkheimer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `quick_python_project-0.4.0/src/quick_python_project/templates/template_hatchling_pyproject.toml` & `quick_python_project-0.4.1/src/quick_python_project/templates/template_hatchling_pyproject.toml`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/src/quick_python_project/templates/template_setuptools_pyproject.toml` & `quick_python_project-0.4.1/src/quick_python_project/templates/template_setuptools_pyproject.toml`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/src/quick_python_project.egg-info/PKG-INFO` & `quick_python_project-0.4.1/src/quick_python_project.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: quick_python_project
-Version: 0.4.0
+Version: 0.4.1
 Summary: A CLI tool to create empty Python projects
 Author-email: James Berkheimer <james.berkheimer@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/james-berkheimer/quick_python_project
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: colorlog
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: covdefaults; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `quick_python_project-0.4.0/src/quick_python_project.egg-info/SOURCES.txt` & `quick_python_project-0.4.1/src/quick_python_project.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .gitignore
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 tox.ini
 .github/workflows/cd.yml
 .github/workflows/ci.yml
 src/quick_python_project/__init__.py
@@ -13,15 +14,14 @@
 src/quick_python_project.egg-info/PKG-INFO
 src/quick_python_project.egg-info/SOURCES.txt
 src/quick_python_project.egg-info/dependency_links.txt
 src/quick_python_project.egg-info/entry_points.txt
 src/quick_python_project.egg-info/requires.txt
 src/quick_python_project.egg-info/top_level.txt
 src/quick_python_project/templates/template_.gitignore
-src/quick_python_project/templates/template_LICENSE
 src/quick_python_project/templates/template_README.md
 src/quick_python_project/templates/template___init__.py
 src/quick_python_project/templates/template_config.json
 src/quick_python_project/templates/template_hatchling_pyproject.toml
 src/quick_python_project/templates/template_main.py
 src/quick_python_project/templates/template_poetry_pyproject.toml
 src/quick_python_project/templates/template_setuptools_pyproject.toml
```

### Comparing `quick_python_project-0.4.0/tests/test_cli.py` & `quick_python_project-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quick_python_project-0.4.0/tests/test_project_generation.py` & `quick_python_project-0.4.1/tests/test_project_generation.py`

 * *Files identical despite different names*

