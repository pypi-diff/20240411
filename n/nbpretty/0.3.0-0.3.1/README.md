# Comparing `tmp/nbpretty-0.3.0.tar.gz` & `tmp/nbpretty-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbpretty-0.3.0.tar", max compression
+gzip compressed data, was "nbpretty-0.3.1.tar", max compression
```

## Comparing `nbpretty-0.3.0.tar` & `nbpretty-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-01-08 13:46:29.513400 nbpretty-0.3.0/LICENSE
--rw-r--r--   0        0        0      167 2024-01-08 13:46:29.513400 nbpretty-0.3.0/README.rst
--rw-r--r--   0        0        0     4580 2024-01-08 13:46:29.513400 nbpretty-0.3.0/nbpretty/__init__.py
--rw-r--r--   0        0        0    10806 2024-01-08 13:46:29.514400 nbpretty-0.3.0/nbpretty/preprocessors.py
--rw-r--r--   0        0        0       33 2024-01-08 13:46:29.514400 nbpretty-0.3.0/nbpretty/templates/nbpretty/conf.json
--rw-r--r--   0        0        0     2157 2024-01-08 13:46:29.514400 nbpretty-0.3.0/nbpretty/templates/nbpretty/index.html.j2
--rw-r--r--   0        0        0     2045 2024-01-08 13:46:29.514400 nbpretty-0.3.0/nbpretty/templates/nbpretty/static/custom.css
--rw-r--r--   0        0        0     4132 2024-01-08 13:46:29.514400 nbpretty-0.3.0/nbpretty/toc.py
--rw-r--r--   0        0        0      616 2024-01-08 13:46:29.514400 nbpretty-0.3.0/nbpretty/utils.py
--rw-r--r--   0        0        0      936 2024-01-08 13:46:29.514400 nbpretty-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 nbpretty-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-11 08:05:40.618852 nbpretty-0.3.1/LICENSE
+-rw-r--r--   0        0        0      167 2024-04-11 08:05:40.618852 nbpretty-0.3.1/README.rst
+-rw-r--r--   0        0        0     4580 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/__init__.py
+-rw-r--r--   0        0        0    10806 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/preprocessors.py
+-rw-r--r--   0        0        0       33 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/templates/nbpretty/conf.json
+-rw-r--r--   0        0        0     2157 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/templates/nbpretty/index.html.j2
+-rw-r--r--   0        0        0     2045 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/templates/nbpretty/static/custom.css
+-rw-r--r--   0        0        0     4132 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/toc.py
+-rw-r--r--   0        0        0      616 2024-04-11 08:05:40.619852 nbpretty-0.3.1/nbpretty/utils.py
+-rw-r--r--   0        0        0      929 2024-04-11 08:05:40.619852 nbpretty-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 nbpretty-0.3.1/PKG-INFO
```

### Comparing `nbpretty-0.3.0/LICENSE` & `nbpretty-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/nbpretty/__init__.py` & `nbpretty-0.3.1/nbpretty/__init__.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/nbpretty/preprocessors.py` & `nbpretty-0.3.1/nbpretty/preprocessors.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/nbpretty/templates/nbpretty/index.html.j2` & `nbpretty-0.3.1/nbpretty/templates/nbpretty/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/nbpretty/templates/nbpretty/static/custom.css` & `nbpretty-0.3.1/nbpretty/templates/nbpretty/static/custom.css`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/nbpretty/toc.py` & `nbpretty-0.3.1/nbpretty/toc.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/nbpretty/utils.py` & `nbpretty-0.3.1/nbpretty/utils.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.0/pyproject.toml` & `nbpretty-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "nbpretty"
-version = "0.3.0"
+version = "0.3.1"
 description = "A tool to convert sets of Jupyter notebook files into a single, cohesive set of linked pages"
 authors = ["Matt Williams <matt@milliams.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://gitlab.com/milliams/nbpretty"
 documentation = "https://nbpretty.readthedocs.io"
 
 [tool.poetry.scripts]
 nbpretty = "nbpretty:main"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 PyYAML = "^6.0"
-nbconvert = "^6.4.0"
+nbconvert = "^7.0"
 click = "^8.0"
-rich = "^12.0.0"
-livereload = "^2.0.0"
-ipython = "^8.0.0"
-jinja2 = "<3.1"
+rich = "^13.0"
+livereload = "^2.0"
+ipython = "^8.0"
+jinja2 = "^3.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.0"
+pytest = "^8.0.0"
 beautifulsoup4 = "^4.0.0"
-mypy = "^0.950"
+mypy = "^1.0"
 types-PyYAML = "^6.0"
 sphinx = "^4.0.0"
 sphinx-autobuild = "^2021.3.0"
-coverage = "^6.0"
-sphinx-book-theme = "^0.3.2"
-nbclient = "^0.6.6"
-ipykernel = "^6.15.1"
-interactive-system-magic = "^0.2.0"
+coverage = "^7.0"
+sphinx-book-theme = "^1.0"
+nbclient = "^0.6"
+ipykernel = "^6.15"
+interactive-system-magic = "^0.2"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nbpretty-0.3.0/PKG-INFO` & `nbpretty-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: nbpretty
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to convert sets of Jupyter notebook files into a single, cohesive set of linked pages
 Home-page: https://gitlab.com/milliams/nbpretty
 License: MIT
 Author: Matt Williams
 Author-email: matt@milliams.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0,<9.0)
-Requires-Dist: ipython (>=8.0.0,<9.0.0)
-Requires-Dist: jinja2 (<3.1)
-Requires-Dist: livereload (>=2.0.0,<3.0.0)
-Requires-Dist: nbconvert (>=6.4.0,<7.0.0)
-Requires-Dist: rich (>=12.0.0,<13.0.0)
+Requires-Dist: ipython (>=8.0,<9.0)
+Requires-Dist: jinja2 (>=3.1,<4.0)
+Requires-Dist: livereload (>=2.0,<3.0)
+Requires-Dist: nbconvert (>=7.0,<8.0)
+Requires-Dist: rich (>=13.0,<14.0)
 Project-URL: Documentation, https://nbpretty.readthedocs.io
 Project-URL: Repository, https://gitlab.com/milliams/nbpretty
 Description-Content-Type: text/x-rst
 
 nbpretty
 ========
```

