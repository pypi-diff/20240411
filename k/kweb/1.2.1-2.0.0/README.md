# Comparing `tmp/kweb-1.2.1.tar.gz` & `tmp/kweb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kweb-1.2.1.tar", last modified: Tue Dec 19 01:45:09 2023, max compression
+gzip compressed data, was "kweb-2.0.0.tar", last modified: Thu Apr 11 17:14:55 2024, max compression
```

## Comparing `kweb-1.2.1.tar` & `kweb-2.0.0.tar`

### file list

```diff
@@ -1,70 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.245047 kweb-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-19 01:44:52.000000 kweb-1.2.1/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-19 01:44:52.000000 kweb-1.2.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-19 01:44:52.000000 kweb-1.2.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-19 01:44:52.000000 kweb-1.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-19 01:44:52.000000 kweb-1.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-19 01:44:52.000000 kweb-1.2.1/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-19 01:44:52.000000 kweb-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-12-19 01:44:52.000000 kweb-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-12-19 01:44:52.000000 kweb-1.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-19 01:44:52.000000 kweb-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2023-12-19 01:45:09.245047 kweb-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-19 01:44:52.000000 kweb-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-19 01:44:52.000000 kweb-1.2.1/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.233047 kweb-1.2.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    84467 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/_static/kweb.png
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/markdown.md
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-19 01:44:52.000000 kweb-1.2.1/docs/rst.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2023-12-19 01:44:52.000000 kweb-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 01:45:09.245047 kweb-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.229047 kweb-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.237047 kweb-1.2.1/src/kweb/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.237047 kweb-1.2.1/src/kweb/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/api/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/api/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/default.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16213 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/layout_server.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/server_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.237047 kweb-1.2.1/src/kweb/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.241047 kweb-1.2.1/src/kweb/static/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)    80668 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/bootstrap/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   331827 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/bootstrap/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   232855 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/bootstrap/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   588931 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/bootstrap/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    60582 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/bootstrap/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220293 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/bootstrap/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/client.css
--rw-r--r--   0 runner    (1001) docker     (127)   271141 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.241047 kweb-1.2.1/src/kweb/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/img/kweb.png
--rw-r--r--   0 runner    (1001) docker     (127)    19244 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/static/viewer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.241047 kweb-1.2.1/src/kweb/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/templates/browser.html
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/templates/viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-12-19 01:44:52.000000 kweb-1.2.1/src/kweb/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.241047 kweb-1.2.1/src/kweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2023-12-19 01:45:09.000000 kweb-1.2.1/src/kweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-12-19 01:45:09.000000 kweb-1.2.1/src/kweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 01:45:09.000000 kweb-1.2.1/src/kweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-19 01:45:09.000000 kweb-1.2.1/src/kweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-19 01:45:09.000000 kweb-1.2.1/src/kweb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:45:09.241047 kweb-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-19 01:44:52.000000 kweb-1.2.1/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:55.325864 kweb-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 17:14:41.000000 kweb-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-11 17:14:55.325864 kweb-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-11 17:14:41.000000 kweb-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-11 17:14:41.000000 kweb-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:14:55.325864 kweb-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:55.321864 kweb-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:55.321864 kweb-2.0.0/src/kweb/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:55.321864 kweb-2.0.0/src/kweb/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/api/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/api/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25463 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/layout_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/server_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-11 17:14:41.000000 kweb-2.0.0/src/kweb/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:55.325864 kweb-2.0.0/src/kweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-11 17:14:55.000000 kweb-2.0.0/src/kweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-11 17:14:55.000000 kweb-2.0.0/src/kweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:14:55.000000 kweb-2.0.0/src/kweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-11 17:14:55.000000 kweb-2.0.0/src/kweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 17:14:55.000000 kweb-2.0.0/src/kweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:14:55.325864 kweb-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 17:14:41.000000 kweb-2.0.0/tests/test_sample.py
```

### Comparing `kweb-1.2.1/LICENSE` & `kweb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kweb-1.2.1/PKG-INFO` & `kweb-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: kweb
-Version: 1.2.1
+Version: 2.0.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: klayout>=0.28.11
+Requires-Dist: klayout>=0.28.17
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: jinja2
+Requires-Dist: pydantic_extra_types>=2.6.0
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: pylsp-mypy; extra == "dev"
 Requires-Dist: types-cachetools; extra == "dev"
 Requires-Dist: towncrier; extra == "dev"
 Requires-Dist: tbump; extra == "dev"
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: docutils==0.17.1; extra == "docs"
+Requires-Dist: docutils==0.21.1; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinxcontrib-video; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx-book-theme==0.3.3; extra == "docs"
+Requires-Dist: sphinx-book-theme==1.1.2; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-markdown-tables==0.0.17; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: autodoc_pydantic; extra == "docs"
 Provides-Extra: ipy
 Requires-Dist: ipython; extra == "ipy"
 Requires-Dist: ipywidgets; extra == "ipy"
 Requires-Dist: ipyevents; extra == "ipy"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 
-# kweb 1.2.1
+# kweb 2.0.0
 
 KLayout Web Viewer ![demo](docs/_static/kweb.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Install & Run
 
@@ -64,15 +65,15 @@
 #### Advanced Usage
 
 KWeb offers two basic apps:
 
 - Browser:
 
   A version that provides a version with a file browser for a folder and the kweb viewer for viewing the gds file in that folder.
-  This can be used by importing the funciton `kweb.browser.get_app` and settings the `KWEB_FILESLOCATION` env variable of passing
+  This can be used by importing the function `kweb.browser.get_app` and settings the `KWEB_FILESLOCATION` env variable of passing
   `fileslocation=<Path object for target folder>` to the function. Alternatively there is a default one in `kweb.default.app` that
   will only look for the env variable.
 
 - Viewer:
 
   Only enables the `/gds/<filename>` endpoints, no root path, i.e. no file browser. Available at `kweb.viewer.get_app`. This version
   doesn't provide a listener for the env variable. Use the `fileslocation` parameter in the function instead.
@@ -81,15 +82,15 @@
 
 #### Clone & Installl
 
 
 ```bash
 # Clone the repository to your local
 git clone https://github.com/gdsfactory/kweb.git
-# Install the necessary dependecies
+# Install the necessary dependencies
 cd /kweb
 python -m pip install -e .[dev]
 ```
 
 #### Set a folder for kweb to use when looking for gds files
 
 ```bash
@@ -104,13 +105,13 @@
 ```
 
 Copy the link http://127.0.0.1:8000/gds/file.gds (or http://localhost:8000/gds/file.gds also works) to your browser to open the waveguide example
 
 
 #### Contributing
 
-Pleas make sure you have also installed pre-commit before committing:
+Please make sure you have also installed pre-commit before committing:
 
 ```bash
 python -m pip install pre-commit
 pre-commit install
 ```
```

### Comparing `kweb-1.2.1/README.md` & `kweb-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# kweb 1.2.1
+# kweb 2.0.0
 
 KLayout Web Viewer ![demo](docs/_static/kweb.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Install & Run
 
@@ -19,15 +19,15 @@
 #### Advanced Usage
 
 KWeb offers two basic apps:
 
 - Browser:
 
   A version that provides a version with a file browser for a folder and the kweb viewer for viewing the gds file in that folder.
-  This can be used by importing the funciton `kweb.browser.get_app` and settings the `KWEB_FILESLOCATION` env variable of passing
+  This can be used by importing the function `kweb.browser.get_app` and settings the `KWEB_FILESLOCATION` env variable of passing
   `fileslocation=<Path object for target folder>` to the function. Alternatively there is a default one in `kweb.default.app` that
   will only look for the env variable.
 
 - Viewer:
 
   Only enables the `/gds/<filename>` endpoints, no root path, i.e. no file browser. Available at `kweb.viewer.get_app`. This version
   doesn't provide a listener for the env variable. Use the `fileslocation` parameter in the function instead.
@@ -36,15 +36,15 @@
 
 #### Clone & Installl
 
 
 ```bash
 # Clone the repository to your local
 git clone https://github.com/gdsfactory/kweb.git
-# Install the necessary dependecies
+# Install the necessary dependencies
 cd /kweb
 python -m pip install -e .[dev]
 ```
 
 #### Set a folder for kweb to use when looking for gds files
 
 ```bash
@@ -59,13 +59,13 @@
 ```
 
 Copy the link http://127.0.0.1:8000/gds/file.gds (or http://localhost:8000/gds/file.gds also works) to your browser to open the waveguide example
 
 
 #### Contributing
 
-Pleas make sure you have also installed pre-commit before committing:
+Please make sure you have also installed pre-commit before committing:
 
 ```bash
 python -m pip install pre-commit
 pre-commit install
 ```
```

### Comparing `kweb-1.2.1/src/kweb/api/browser.py` & `kweb-2.0.0/src/kweb/api/browser.py`

 * *Files identical despite different names*

### Comparing `kweb-1.2.1/src/kweb/api/viewer.py` & `kweb-2.0.0/src/kweb/api/viewer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,52 @@
 from pathlib import Path
+from typing import Annotated
 
-from fastapi import APIRouter, Request
+from fastapi import APIRouter, Depends, Request
 from fastapi.exceptions import HTTPException
 from fastapi.responses import HTMLResponse
 from fastapi.templating import Jinja2Templates
+from pydantic import BaseModel
 from starlette.templating import _TemplateResponse
 
-# from . import __version__ as version
+from .. import __version__ as version
 
 router = APIRouter()
 templates = Jinja2Templates(
     directory=(Path(__file__).parent.parent / "templates").resolve()
 )
 
 
-@router.get("/gds/{gds_name:path}", response_class=HTMLResponse)
-async def gds_view_static(
-    request: Request,
-    gds_name: str,
-    layer_props: str | None = None,
-    cell: str | None = None,
-) -> _TemplateResponse:
-    settings = router.dependencies[0].dependency()  # type: ignore[misc]
-    gds_file = (settings.fileslocation / f"{gds_name}").with_suffix(".gds")
+class FileView(BaseModel):
+    file: Path
+    cell: str | None = None
+    layer_props: str | None = None
+    rdb: str | None = None
 
-    exists = (
-        gds_file.exists()
-        and gds_file.is_file()
-        and gds_file.stat().st_mode  # type: ignore[misc, operator]
-    )
 
-    if not exists:
-        raise HTTPException(
-            status_code=404,
-            detail=f'No gds found with name "{gds_name}".'
-            " It doesn't exist or is not accessible",
-        )
-
-    return await show_file(request, gds_file, layer_props, cell)
-
-
-@router.get("/file/{file_name:path}", response_class=HTMLResponse)
+@router.get("/view", response_class=HTMLResponse)
 async def file_view_static(
-    request: Request,
-    file_name: str,
-    layer_props: str | None = None,
-    cell: str | None = None,
+    request: Request, params: Annotated[FileView, Depends()]
 ) -> _TemplateResponse:
     settings = router.dependencies[0].dependency()  # type: ignore[misc]
-    file = settings.fileslocation / f"{file_name}"
+    _file = settings.fileslocation / f"{params.file}"
 
-    exists = (
-        file.exists()
-        and file.is_file()
-        and file.stat().st_mode  # type: ignore[misc, operator]
-    )
+    exists = _file.is_file() and _file.stat().st_mode
 
     if not exists:
         raise HTTPException(
             status_code=404,
-            detail=f'No file found with name "{file_name}".'
+            detail=f'No file found with name "{_file}".'
             " It doesn't exist or is not accessible",
         )
 
-    return await show_file(request, file, layer_props, cell)
+    return await show_file(request, layout_params=params)
 
 
-async def show_file(
-    request: Request,
-    file: Path,
-    layer_props: str | None = None,
-    cell: str | None = None,
-) -> _TemplateResponse:
+async def show_file(request: Request, layout_params: FileView) -> _TemplateResponse:
     root_path = request.scope["root_path"]
 
     match request.url.scheme:
         case "https":
             ws_scheme = "wss://"
         case "http":
             ws_scheme = "ws://"
@@ -92,23 +63,20 @@
         )
     else:
         url = ws_scheme + (request.url.hostname or "localhost") + root_path
 
     template_params = {
         "request": request,
         "url": url,
-        "file": file,
-        "layer_props": layer_props,
     }
 
-    if cell is not None:
-        template_params["cell"] = cell
+    template_params["params"] = layout_params.model_dump(mode="json", exclude_none=True)
 
     return templates.TemplateResponse(
         "viewer.html",
         template_params,
     )
 
 
-# @router.get("/status")
-# async def status() -> dict[str, Any]:
-#     return {"server": "kweb", "version": version}
+@router.get("/status")
+async def kweb_status() -> dict[str, str | int]:
+    return {"server": "kweb", "version": version}
```

### Comparing `kweb-1.2.1/src/kweb/browser.py` & `kweb-2.0.0/src/kweb/browser.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,46 +3,53 @@
 from fastapi import Depends, FastAPI
 from fastapi.staticfiles import StaticFiles
 from pydantic import ValidationError
 
 from . import config
 from .api.browser import router as browser_router
 from .api.viewer import router as viewer_router
-from .layout_server import EditableLayoutViewServerEndpoint, LayoutViewServerEndpoint
+from .layout_server import LayoutViewServerEndpoint
 
 
 def get_app(fileslocation: Path | str | None = None, editable: bool = False) -> FastAPI:
     if fileslocation is None:
-
-        def settings() -> config.Config:
-            try:
-                return config.Config()
-            except ValidationError:
-                raise ValueError(
-                    "To start the Kweb please set the environment "
-                    "variable KWEB_FILESLOCATION to a path in your filesystem."
-                    " Alternatively, you can set the filepath in the get_app function."
-                )
+        try:
+            _settings = config.Config()
+        except ValidationError:
+            raise ValueError(
+                "To start the Kweb please set the environment "
+                "variable KWEB_FILESLOCATION to a path in your filesystem."
+                " Alternatively, you can set the filepath in the get_app function."
+            )
 
     else:
+        _settings = config.Config(fileslocation=fileslocation, editable=editable)
 
-        def settings() -> config.Config:
-            return config.Config(fileslocation=fileslocation)
+    def settings() -> config.Config:
+        return _settings
 
     staticfiles = StaticFiles(directory=Path(__file__).parent / "static")
 
     # app = FastAPI(routes=[WebSocketRoute("/ws", endpoint=LayoutViewServerEndpoint)])
 
     app = FastAPI()
     viewer_router.dependencies.insert(0, Depends(settings))
     browser_router.dependencies.insert(0, Depends(settings))
 
-    if editable:
-        app.add_websocket_route("/ws", EditableLayoutViewServerEndpoint)
-    else:
-        app.add_websocket_route("/ws", LayoutViewServerEndpoint)
+    _settings = settings()
+
+    class BrowserLayoutViewServerEndpoint(
+        LayoutViewServerEndpoint,
+        root=_settings.fileslocation,
+        editable=editable,
+        add_missing_layers=_settings.add_missing_layers,
+        meta_splitter=_settings.meta_splitter,
+    ):
+        pass
+
+    app.add_websocket_route("/ws", BrowserLayoutViewServerEndpoint)
     viewer_router.dependencies.insert(0, Depends(settings))
     app.include_router(viewer_router)
     app.include_router(browser_router)
     app.mount("/static", staticfiles, name="kweb_static")
 
     return app
```

### Comparing `kweb-1.2.1/src/kweb/server_jupyter.py` & `kweb-2.0.0/src/kweb/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `kweb-1.2.1/src/kweb/viewer.py` & `kweb-2.0.0/src/kweb/viewer.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,30 +4,38 @@
 from fastapi.staticfiles import StaticFiles
 from starlette.routing import WebSocketRoute
 
 from . import config
 from .api.viewer import router
 
 # from .layout_server import EditableLayoutViewServerEndpoint
-from .layout_server import EditableLayoutViewServerEndpoint, LayoutViewServerEndpoint
+from .layout_server import LayoutViewServerEndpoint
 
 
 def get_app(fileslocation: Path | str, editable: bool = False) -> FastAPI:
     # config.settings.fileslocation = Path(fileslocation)
+    _settings = config.Config(fileslocation=fileslocation, editable=editable)
+
     def settings() -> config.Config:
-        return config.Config(fileslocation=fileslocation)
+        return _settings
 
     staticfiles = StaticFiles(directory=Path(__file__).parent / "static")
 
-    if editable:
-        app = FastAPI(
-            routes=[WebSocketRoute("/ws", endpoint=EditableLayoutViewServerEndpoint)]
-        )
-    else:
-        app = FastAPI(routes=[WebSocketRoute("/ws", endpoint=LayoutViewServerEndpoint)])
+    class BrowserLayoutViewServerEndpoint(
+        LayoutViewServerEndpoint,
+        root=_settings.fileslocation,
+        editable=editable,
+        add_missing_layers=_settings.add_missing_layers,
+        meta_splitter=_settings.meta_splitter,
+    ):
+        pass
+
+    app = FastAPI(
+        routes=[WebSocketRoute("/ws", endpoint=BrowserLayoutViewServerEndpoint)]
+    )
 
     # insert the settings as the first dependency
     router.dependencies.insert(0, Depends(settings))
     app.include_router(router)
     app.mount("/static", staticfiles, name="kweb_static")
 
     return app
```

### Comparing `kweb-1.2.1/src/kweb.egg-info/PKG-INFO` & `kweb-2.0.0/src/kweb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: kweb
-Version: 1.2.1
+Version: 2.0.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: klayout>=0.28.11
+Requires-Dist: klayout>=0.28.17
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: jinja2
+Requires-Dist: pydantic_extra_types>=2.6.0
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: pylsp-mypy; extra == "dev"
 Requires-Dist: types-cachetools; extra == "dev"
 Requires-Dist: towncrier; extra == "dev"
 Requires-Dist: tbump; extra == "dev"
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: docutils==0.17.1; extra == "docs"
+Requires-Dist: docutils==0.21.1; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinxcontrib-video; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx-book-theme==0.3.3; extra == "docs"
+Requires-Dist: sphinx-book-theme==1.1.2; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-markdown-tables==0.0.17; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: autodoc_pydantic; extra == "docs"
 Provides-Extra: ipy
 Requires-Dist: ipython; extra == "ipy"
 Requires-Dist: ipywidgets; extra == "ipy"
 Requires-Dist: ipyevents; extra == "ipy"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 
-# kweb 1.2.1
+# kweb 2.0.0
 
 KLayout Web Viewer ![demo](docs/_static/kweb.png)
 
 Based on https://github.com/klayoutmatthias/canvas2canvas
 
 ## Install & Run
 
@@ -64,15 +65,15 @@
 #### Advanced Usage
 
 KWeb offers two basic apps:
 
 - Browser:
 
   A version that provides a version with a file browser for a folder and the kweb viewer for viewing the gds file in that folder.
-  This can be used by importing the funciton `kweb.browser.get_app` and settings the `KWEB_FILESLOCATION` env variable of passing
+  This can be used by importing the function `kweb.browser.get_app` and settings the `KWEB_FILESLOCATION` env variable of passing
   `fileslocation=<Path object for target folder>` to the function. Alternatively there is a default one in `kweb.default.app` that
   will only look for the env variable.
 
 - Viewer:
 
   Only enables the `/gds/<filename>` endpoints, no root path, i.e. no file browser. Available at `kweb.viewer.get_app`. This version
   doesn't provide a listener for the env variable. Use the `fileslocation` parameter in the function instead.
@@ -81,15 +82,15 @@
 
 #### Clone & Installl
 
 
 ```bash
 # Clone the repository to your local
 git clone https://github.com/gdsfactory/kweb.git
-# Install the necessary dependecies
+# Install the necessary dependencies
 cd /kweb
 python -m pip install -e .[dev]
 ```
 
 #### Set a folder for kweb to use when looking for gds files
 
 ```bash
@@ -104,13 +105,13 @@
 ```
 
 Copy the link http://127.0.0.1:8000/gds/file.gds (or http://localhost:8000/gds/file.gds also works) to your browser to open the waveguide example
 
 
 #### Contributing
 
-Pleas make sure you have also installed pre-commit before committing:
+Please make sure you have also installed pre-commit before committing:
 
 ```bash
 python -m pip install pre-commit
 pre-commit install
 ```
```

