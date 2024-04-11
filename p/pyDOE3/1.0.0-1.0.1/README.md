# Comparing `tmp/pydoe3-1.0.0.tar.gz` & `tmp/pydoe3-1.0.1.tar.gz`

## Comparing `pydoe3-1.0.0.tar` & `pydoe3-1.0.1.tar`

### file list

```diff
@@ -1,86 +1,52 @@
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydoe3-1.0.0/.github/workflows/release-pypi.yml
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/Makefile
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/conf.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/factorial.rst
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/index.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/index_TOC.rst
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/randomized.rst
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/rsm.rst
--rw-r--r--   0        0        0    18144 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0    41544 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/doctrees/factorial.doctree
--rw-r--r--   0        0        0    42788 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/doctrees/index_TOC.doctree
--rw-r--r--   0        0        0    26749 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/doctrees/randomized.doctree
--rw-r--r--   0        0        0    30411 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/doctrees/rsm.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/.buildinfo
--rw-r--r--   0        0        0    21494 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/factorial.html
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/genindex.html
--rw-r--r--   0        0        0    17070 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/index.html
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/index_TOC.html
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/objects.inv
--rw-r--r--   0        0        0    16952 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/randomized.html
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/rsm.html
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/search.html
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/searchindex.js
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_images/lhs.png
--rw-r--r--   0        0        0    22705 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_images/lhs_custom_distribution.png
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_sources/factorial.txt
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_sources/index.txt
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_sources/index_TOC.txt
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_sources/randomized.txt
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_sources/rsm.txt
--rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/_default.css
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/ajax-loader.gif
--rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/basic.css
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/comment-bright.png
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/comment-close.png
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/comment.png
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/contents.png
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/down-pressed.png
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/down.png
--rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/drawing.svg
--rw-r--r--   0        0        0    51262 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/favicon.ico
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/file.png
--rw-r--r--   0        0        0   262283 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/jquery.js
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/lhs.png
--rw-r--r--   0        0        0    22705 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/lhs_custom_distribution.png
--rw-r--r--   0        0        0    44563 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/lhs_custom_distribution.svg
--rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/logo.png
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/logo.svg
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/minus.png
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/navigation.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/plus.png
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18479 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/sphinxdoc.css
--rw-r--r--   0        0        0    42643 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/underscore.js
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/up-pressed.png
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/up.png
--rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_build/html/_static/websupport.js
--rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/_default.css
--rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/drawing.svg
--rw-r--r--   0        0        0    51262 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/favicon.ico
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/lhs.png
--rw-r--r--   0        0        0    22705 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/lhs_custom_distribution.png
--rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/logo.png
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_static/logo.svg
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 pydoe3-1.0.0/doc/_templates/layout.html
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/__init__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/build_regression_matrix.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_box_behnken.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_composite.py
--rw-r--r--   0        0        0    18136 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_factorial.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_fold.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_gsd.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_lhs.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_plackett_burman.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_repeat_center.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_star.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/doe_union.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyDOE3/var_regression_matrix.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pydoe3-1.0.0/.gitignore
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pydoe3-1.0.0/LICENSE
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pydoe3-1.0.0/README.md
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pydoe3-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 pydoe3-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pydoe3-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pydoe3-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pydoe3-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydoe3-1.0.1/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 pydoe3-1.0.1/.github/workflows/release-pypi.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pydoe3-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/Makefile
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/conf.py
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/factorial.rst
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/index.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/index_TOC.rst
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/make.bat
+-rw-r--r--   0        0        0     5593 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/randomized.rst
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/requirements.txt
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/rsm.rst
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/_default.css
+-rw-r--r--   0        0        0    13959 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/drawing.svg
+-rw-r--r--   0        0        0    51262 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/lhs.png
+-rw-r--r--   0        0        0    22705 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/lhs_custom_distribution.png
+-rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/logo.png
+-rw-r--r--   0        0        0    14579 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/logo.svg
+-rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_static/logo_pydoe3.png
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 pydoe3-1.0.1/doc/_templates/layout.html
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/_version.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/build_regression_matrix.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_box_behnken.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_composite.py
+-rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_factorial.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_fold.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_gsd.py
+-rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_lhs.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_plackett_burman.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_repeat_center.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_star.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/doe_union.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyDOE3/var_regression_matrix.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_box_behnken.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_composite.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_factorial.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_gsd.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_lhs.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_plackett_burman.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_repeat_center.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_star.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pydoe3-1.0.1/tests/test_union.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pydoe3-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pydoe3-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 pydoe3-1.0.1/README.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 pydoe3-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 pydoe3-1.0.1/PKG-INFO
```

### Comparing `pydoe3-1.0.0/.github/workflows/release-pypi.yml` & `pydoe3-1.0.1/.github/workflows/release-pypi.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-name: Release to PyPI
-
-on:
-  release:
-    types: [published]
-
-concurrency:
-  group: ${{ github.workflow }}-${{ github.ref }}
-  cancel-in-progress: true
-
-permissions:
-  contents: read
-
-jobs:
-  release:
-    runs-on: ubuntu-latest
-    environment: pypi
-    permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
-      id-token: write
-    steps:
-    - uses: actions/checkout@v4
-      with:
-        # Include all history to get tags for versioning
-        fetch-depth: 0
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: '3.x'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install hatch
-    - name: Build package
-      run: hatch build
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@release/v1
+name: Release to PyPI
+
+on:
+  release:
+    types: [published]
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
+permissions:
+  contents: read
+
+jobs:
+  release:
+    runs-on: ubuntu-latest
+    environment: pypi
+    permissions:
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
+    steps:
+
+    - name: Checkout sources
+      uses: actions/checkout@v4
+      with:
+        # Include all history to get tags for versioning
+        fetch-depth: 0
+
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install hatch
+
+    - name: Build package
+      run: hatch build
+
+    - name: Publish package
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `pydoe3-1.0.0/doc/Makefile` & `pydoe3-1.0.1/doc/Makefile`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# Makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = sphinx-build
-PAPER         =
-
-# Internal variables.
-PAPEROPT_a4     = -D latex_paper_size=a4
-PAPEROPT_letter = -D latex_paper_size=letter
-ALLSPHINXOPTS   = -d _build/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) .
-
-.PHONY: help clean html dirhtml pickle json htmlhelp qthelp changes linkcheck doctest # latex 
-
-help:
-	@echo "Please use \`make <target>' where <target> is one of"
-	@echo "  html      to make standalone HTML files"
-	@echo "  dirhtml   to make HTML files named index.html in directories"
-	@echo "  pickle    to make pickle files"
-	@echo "  json      to make JSON files"
-	@echo "  htmlhelp  to make HTML files and a HTML help project"
-	@echo "  qthelp    to make HTML files and a qthelp project"
-# 	@echo "  latex     to make LaTeX files, you can set PAPER=a4 or PAPER=letter"
-	@echo "  changes   to make an overview of all changed/added/deprecated items"
-	@echo "  linkcheck to check all external links for integrity"
-	@echo "  doctest   to run all doctests embedded in the documentation (if enabled)"
-
-clean:
-	-rm -rf _build/*
-
-# The HTML needs latex because the PDF version is linked to:
-html: # latex
-# 	(cd _build/latex; make all-pdf)
-	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) _build/html
-	@echo
-	@echo "Build finished. The HTML pages are in _build/html."
-
-dirhtml:
-	$(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) _build/dirhtml
-	@echo
-	@echo "Build finished. The HTML pages are in _build/dirhtml."
-
-pickle:
-	$(SPHINXBUILD) -b pickle $(ALLSPHINXOPTS) _build/pickle
-	@echo
-	@echo "Build finished; now you can process the pickle files."
-
-json:
-	$(SPHINXBUILD) -b json $(ALLSPHINXOPTS) _build/json
-	@echo
-	@echo "Build finished; now you can process the JSON files."
-
-htmlhelp:
-	$(SPHINXBUILD) -b htmlhelp $(ALLSPHINXOPTS) _build/htmlhelp
-	@echo
-	@echo "Build finished; now you can run HTML Help Workshop with the" \
-	      ".hhp project file in _build/htmlhelp."
-
-qthelp:
-	$(SPHINXBUILD) -b qthelp $(ALLSPHINXOPTS) _build/qthelp
-	@echo
-	@echo "Build finished; now you can run "qcollectiongenerator" with the" \
-	      ".qhcp project file in _build/qthelp, like this:"
-	@echo "# qcollectiongenerator _build/qthelp/uncertaintiesPythonpackage.qhcp"
-	@echo "To view the help file:"
-	@echo "# assistant -collectionFile _build/qthelp/uncertaintiesPythonpackage.qhc"
-
-# latex:
-# 	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) _build/latex
-# 	@echo
-# 	@echo "Build finished; the LaTeX files are in _build/latex."
-# 	@echo "Run \`make all-pdf' or \`make all-ps' in that directory to" \
-# 	      "run these through (pdf)latex."
-
-changes:
-	$(SPHINXBUILD) -b changes $(ALLSPHINXOPTS) _build/changes
-	@echo
-	@echo "The overview file is in _build/changes."
-
-linkcheck:
-	$(SPHINXBUILD) -b linkcheck $(ALLSPHINXOPTS) _build/linkcheck
-	@echo
-	@echo "Link check complete; look for any errors in the above output " \
-	      "or in _build/linkcheck/output.txt."
-
-doctest:
-	$(SPHINXBUILD) -b doctest $(ALLSPHINXOPTS) _build/doctest
-	@echo "Testing of doctests in the sources finished, look at the " \
-	      "results in _build/doctest/output.txt."
+# Makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = sphinx-build
+PAPER         =
+
+# Internal variables.
+PAPEROPT_a4     = -D latex_paper_size=a4
+PAPEROPT_letter = -D latex_paper_size=letter
+ALLSPHINXOPTS   = -d _build/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) .
+
+.PHONY: help clean html dirhtml pickle json htmlhelp qthelp changes linkcheck doctest # latex 
+
+help:
+	@echo "Please use \`make <target>' where <target> is one of"
+	@echo "  html      to make standalone HTML files"
+	@echo "  dirhtml   to make HTML files named index.html in directories"
+	@echo "  pickle    to make pickle files"
+	@echo "  json      to make JSON files"
+	@echo "  htmlhelp  to make HTML files and a HTML help project"
+	@echo "  qthelp    to make HTML files and a qthelp project"
+# 	@echo "  latex     to make LaTeX files, you can set PAPER=a4 or PAPER=letter"
+	@echo "  changes   to make an overview of all changed/added/deprecated items"
+	@echo "  linkcheck to check all external links for integrity"
+	@echo "  doctest   to run all doctests embedded in the documentation (if enabled)"
+
+clean:
+	-rm -rf _build/*
+
+# The HTML needs latex because the PDF version is linked to:
+html: # latex
+# 	(cd _build/latex; make all-pdf)
+	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) _build/html
+	@echo
+	@echo "Build finished. The HTML pages are in _build/html."
+
+dirhtml:
+	$(SPHINXBUILD) -b dirhtml $(ALLSPHINXOPTS) _build/dirhtml
+	@echo
+	@echo "Build finished. The HTML pages are in _build/dirhtml."
+
+pickle:
+	$(SPHINXBUILD) -b pickle $(ALLSPHINXOPTS) _build/pickle
+	@echo
+	@echo "Build finished; now you can process the pickle files."
+
+json:
+	$(SPHINXBUILD) -b json $(ALLSPHINXOPTS) _build/json
+	@echo
+	@echo "Build finished; now you can process the JSON files."
+
+htmlhelp:
+	$(SPHINXBUILD) -b htmlhelp $(ALLSPHINXOPTS) _build/htmlhelp
+	@echo
+	@echo "Build finished; now you can run HTML Help Workshop with the" \
+	      ".hhp project file in _build/htmlhelp."
+
+qthelp:
+	$(SPHINXBUILD) -b qthelp $(ALLSPHINXOPTS) _build/qthelp
+	@echo
+	@echo "Build finished; now you can run "qcollectiongenerator" with the" \
+	      ".qhcp project file in _build/qthelp, like this:"
+	@echo "# qcollectiongenerator _build/qthelp/uncertaintiesPythonpackage.qhcp"
+	@echo "To view the help file:"
+	@echo "# assistant -collectionFile _build/qthelp/uncertaintiesPythonpackage.qhc"
+
+# latex:
+# 	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) _build/latex
+# 	@echo
+# 	@echo "Build finished; the LaTeX files are in _build/latex."
+# 	@echo "Run \`make all-pdf' or \`make all-ps' in that directory to" \
+# 	      "run these through (pdf)latex."
+
+changes:
+	$(SPHINXBUILD) -b changes $(ALLSPHINXOPTS) _build/changes
+	@echo
+	@echo "The overview file is in _build/changes."
+
+linkcheck:
+	$(SPHINXBUILD) -b linkcheck $(ALLSPHINXOPTS) _build/linkcheck
+	@echo
+	@echo "Link check complete; look for any errors in the above output " \
+	      "or in _build/linkcheck/output.txt."
+
+doctest:
+	$(SPHINXBUILD) -b doctest $(ALLSPHINXOPTS) _build/doctest
+	@echo "Testing of doctests in the sources finished, look at the " \
+	      "results in _build/doctest/output.txt."
```

### Comparing `pydoe3-1.0.0/doc/conf.py` & `pydoe3-1.0.1/doc/conf.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-# -*- coding: utf-8 -*-
-#
-# ad Python package documentation build configuration file, created by
-# sphinx-quickstart on Tue Jun  8 18:32:22 2010.
-#
-# This file is execfile()d with the current directory set to its containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-from datetime import date
-
-import sys, os
-
-sys.path.insert(0, os.path.abspath('..'))
-
-import pyDOE3
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.append(os.path.abspath('.'))
-
-# -- General configuration -----------------------------------------------------
-
-# Add any Sphinx extension module names here, as strings. They can be extensions
-# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = []
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix of source filenames.
-source_suffix = '.rst'
-
-# The encoding of source files.
-#source_encoding = 'utf-8'
-
-# The master toctree document.
-master_doc = 'index_TOC'
-
-# General information about the project.
-project = u'pyDOE3'
-if date.today().year!=2013:
-    copyright = u'2013–%d, Abraham Lee' % date.today().year
-else:
-    copyright = u'2013, Abraham Lee'
-
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-#
-# The short X.Y version.
-version = '1'
-# The full version, including alpha/beta/rc tags.
-release = pyDOE3.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#language = None
-
-# There are two options for replacing |today|: either, you set today to some
-# non-false value, then it is used:
-#today = ''
-# Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
-
-# List of documents that shouldn't be included in the build.
-#unused_docs = []
-
-# List of directories, relative to source directory, that shouldn't be searched
-# for source files.
-exclude_trees = ['_build']
-
-# The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
-
-# If true, the current module name will be prepended to all description
-# unit titles (such as .. function::).
-#add_module_names = True
-
-# If true, sectionauthor and moduleauthor directives will be shown in the
-# output. They are ignored by default.
-#show_authors = False
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
-
-
-# -- Options for HTML output ---------------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  Major themes that come with
-# Sphinx are currently 'default' and 'sphinxdoc'.
-html_theme = 'sphinxdoc'
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
-# documentation.
-# html_theme_options = {}
-
-# Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
-
-# The name for this set of Sphinx documents.  If None, it defaults to
-# "<project> v<release> documentation".
-#html_title = None
-
-# A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
-
-# The name of an image file (relative to this directory) to place at the top
-# of the sidebar.
-#html_logo = None
-
-# The name of an image file (within the static path) to use as favicon of the
-# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
-# pixels large.
-html_favicon = 'favicon.ico'
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
-# using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
-
-# If true, SmartyPants will be used to convert quotes and dashes to
-# typographically correct entities.
-#html_use_smartypants = True
-
-# Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
-
-# Additional templates that should be rendered to pages, maps page names to
-# template names.
-#html_additional_pages = {}
-
-# If false, no module index is generated.
-#html_use_modindex = True
-
-# If false, no index is generated.
-#html_use_index = True
-
-# If true, the index is split into individual pages for each letter.
-#html_split_index = False
-
-# If true, links to the reST sources are added to the pages.
-html_show_sourcelink = False
-
-# If true, an OpenSearch description file will be output, and all pages will
-# contain a <link> tag referring to it.  The value of this option must be the
-# base URL from which the finished HTML is served.
-#html_use_opensearch = ''
-
-# If nonempty, this is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = ''
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'pyDOEPythonPackagedoc'
-
-
-# -- Options for LaTeX output --------------------------------------------------
-
-# The paper size ('letter' or 'a4').
-#latex_paper_size = 'letter'
-
-# The font size ('10pt', '11pt' or '12pt').
-#latex_font_size = '10pt'
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass [howto/manual]).
-# latex_documents = [
-#   ('index_TOC', 'adPythonPackage.tex', u'ad Python package Documentation',
-#   u'Abraham Lee', 'manual'),
-# ]
-
-# The name of an image file (relative to this directory) to place at the top of
-# the title page.
-#latex_logo = None
-
-# For "manual" documents, if this is true, then toplevel headings are parts,
-# not chapters.
-#latex_use_parts = False
-
-# Additional stuff for the LaTeX preamble.
-#latex_preamble = ''
-
-# Documents to append as an appendix to all manuals.
-#latex_appendices = []
-
-# If false, no module index is generated.
-#latex_use_modindex = True
+# -*- coding: utf-8 -*-
+#
+# ad Python package documentation build configuration file, created by
+# sphinx-quickstart on Tue Jun  8 18:32:22 2010.
+#
+# This file is execfile()d with the current directory set to its containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+from datetime import date
+
+import sys, os
+
+sys.path.insert(0, os.path.abspath('..'))
+
+import pyDOE3
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+#sys.path.append(os.path.abspath('.'))
+
+# -- General configuration -----------------------------------------------------
+
+# Add any Sphinx extension module names here, as strings. They can be extensions
+# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = []
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix of source filenames.
+source_suffix = '.rst'
+
+# The encoding of source files.
+#source_encoding = 'utf-8'
+
+# The master toctree document.
+master_doc = 'index_TOC'
+
+# General information about the project.
+project = u'pyDOE3'
+if date.today().year!=2013:
+    copyright = u'2013–%d, Abraham Lee' % date.today().year
+else:
+    copyright = u'2013, Abraham Lee'
+
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+#
+# The short X.Y version.
+version = '1'
+# The full version, including alpha/beta/rc tags.
+release = pyDOE3.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#language = None
+
+# There are two options for replacing |today|: either, you set today to some
+# non-false value, then it is used:
+#today = ''
+# Else, today_fmt is used as the format for a strftime call.
+#today_fmt = '%B %d, %Y'
+
+# List of documents that shouldn't be included in the build.
+#unused_docs = []
+
+# List of directories, relative to source directory, that shouldn't be searched
+# for source files.
+exclude_trees = ['_build']
+
+# The reST default role (used for this markup: `text`) to use for all documents.
+#default_role = None
+
+# If true, '()' will be appended to :func: etc. cross-reference text.
+#add_function_parentheses = True
+
+# If true, the current module name will be prepended to all description
+# unit titles (such as .. function::).
+#add_module_names = True
+
+# If true, sectionauthor and moduleauthor directives will be shown in the
+# output. They are ignored by default.
+#show_authors = False
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# A list of ignored prefixes for module index sorting.
+#modindex_common_prefix = []
+
+
+# -- Options for HTML output ---------------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  Major themes that come with
+# Sphinx are currently 'default' and 'sphinxdoc'.
+html_theme = 'sphinxdoc'
+
+# Theme options are theme-specific and customize the look and feel of a theme
+# further.  For a list of options available for each theme, see the
+# documentation.
+# html_theme_options = {}
+
+# Add any paths that contain custom themes here, relative to this directory.
+#html_theme_path = []
+
+# The name for this set of Sphinx documents.  If None, it defaults to
+# "<project> v<release> documentation".
+#html_title = None
+
+# A shorter title for the navigation bar.  Default is the same as html_title.
+#html_short_title = None
+
+# The name of an image file (relative to this directory) to place at the top
+# of the sidebar.
+#html_logo = None
+
+# The name of an image file (within the static path) to use as favicon of the
+# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
+# pixels large.
+html_favicon = 'favicon.ico'
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
+# using the given strftime format.
+#html_last_updated_fmt = '%b %d, %Y'
+
+# If true, SmartyPants will be used to convert quotes and dashes to
+# typographically correct entities.
+#html_use_smartypants = True
+
+# Custom sidebar templates, maps document names to template names.
+#html_sidebars = {}
+
+# Additional templates that should be rendered to pages, maps page names to
+# template names.
+#html_additional_pages = {}
+
+# If false, no module index is generated.
+#html_use_modindex = True
+
+# If false, no index is generated.
+#html_use_index = True
+
+# If true, the index is split into individual pages for each letter.
+#html_split_index = False
+
+# If true, links to the reST sources are added to the pages.
+html_show_sourcelink = False
+
+# If true, an OpenSearch description file will be output, and all pages will
+# contain a <link> tag referring to it.  The value of this option must be the
+# base URL from which the finished HTML is served.
+#html_use_opensearch = ''
+
+# If nonempty, this is the file name suffix for HTML files (e.g. ".xhtml").
+#html_file_suffix = ''
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'pyDOEPythonPackagedoc'
+
+
+# -- Options for LaTeX output --------------------------------------------------
+
+# The paper size ('letter' or 'a4').
+#latex_paper_size = 'letter'
+
+# The font size ('10pt', '11pt' or '12pt').
+#latex_font_size = '10pt'
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass [howto/manual]).
+# latex_documents = [
+#   ('index_TOC', 'adPythonPackage.tex', u'ad Python package Documentation',
+#   u'Abraham Lee', 'manual'),
+# ]
+
+# The name of an image file (relative to this directory) to place at the top of
+# the title page.
+#latex_logo = None
+
+# For "manual" documents, if this is true, then toplevel headings are parts,
+# not chapters.
+#latex_use_parts = False
+
+# Additional stuff for the LaTeX preamble.
+#latex_preamble = ''
+
+# Documents to append as an appendix to all manuals.
+#latex_appendices = []
+
+# If false, no module index is generated.
+#latex_use_modindex = True
```

### Comparing `pydoe3-1.0.0/doc/randomized.rst` & `pydoe3-1.0.1/doc/randomized.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-.. index:: Randomized Designs
-
-.. _randomized:
-
-================================================================================
-Randomized Designs
-================================================================================
-
-In this section, the following kinds of *randomized designs* will 
-be described:
-
-- Latin-Hypercube
-
-.. hint::
-   All available designs can be accessed after a simple import statement::
-
-    >>> from pyDOE import *
-    
-.. index:: Latin-Hypercube
-
-.. _latin_hypercube:
-
-Latin-Hypercube (``lhs``)
-=========================
-
-.. image:: _static/lhs.png
-
-Latin-hypercube designs can be created using the following simple syntax::
-
-    >>> lhs(n, [samples, criterion, iterations])
-
-where 
-
-* **n**: an integer that designates the number of factors (required)
-* **samples**: an integer that designates the number of sample points to 
-  generate for each factor (default: n)
-* **criterion**: a string that tells ``lhs`` how to sample the points
-  (default: None, which simply randomizes the points within the intervals):
-  
-  - "center" or "c": center the points within the sampling intervals
-  - "maximin" or "m": maximize the minimum distance between points, but
-    place the point in a randomized location within its interval
-  - "centermaximin" or "cm": same as "maximin", but centered within the
-    intervals
-  - "correlation" or "corr": minimize the maximum correlation coefficient
-  - "lhsmu" : Latin hypercube with multifimensional Uniformity. Correlation between
-     variable can be enforced by setting a valid correlation matrix. Description of the
-     algorithm can be found in `Deutsch and Deutsch`_.
-  
-The output design scales all the variable ranges from zero to one which
-can then be transformed as the user wishes (like to a specific statistical
-distribution using the `scipy.stats.distributions`_ ``ppf`` (inverse
-cumulative distribution) function. An example of this is :ref:`shown below
-<statistical_distribution_usage>`.
-
-For example, if I wanted to transform the uniform distribution of 8 samples
-to a normal distribution (mean=0, standard deviation=1), I would do 
-something like::
-
-    >>> from scipy.stats.distributions import norm
-    >>> lhd = lhs(2, samples=5)
-    >>> lhd = norm(loc=0, scale=1).ppf(lhd)  # this applies to both factors here
-
-Graphically, each transformation would look like the following, going 
-from the blue sampled points (from using ``lhs``) to the green
-sampled points that are normally distributed:
-
-.. image:: _static/lhs_custom_distribution.png
-
-Examples
---------
-
-A basic 4-factor latin-hypercube design::
-
-    >>> lhs(4, criterion='center')
-    array([[ 0.875,  0.625,  0.875,  0.125],
-           [ 0.375,  0.125,  0.375,  0.375],
-           [ 0.625,  0.375,  0.125,  0.625],
-           [ 0.125,  0.875,  0.625,  0.875]])
-
-Let's say we want more samples, like 10::
-
-    >>> lhs(4, samples=10, criterion='center')
-    array([[ 0.05,  0.05,  0.15,  0.15],
-           [ 0.55,  0.85,  0.95,  0.75],
-           [ 0.25,  0.25,  0.45,  0.25],
-           [ 0.45,  0.35,  0.75,  0.45],
-           [ 0.75,  0.55,  0.25,  0.55],
-           [ 0.95,  0.45,  0.35,  0.05],
-           [ 0.35,  0.95,  0.05,  0.65],
-           [ 0.15,  0.65,  0.55,  0.35],
-           [ 0.85,  0.75,  0.85,  0.85],
-           [ 0.65,  0.15,  0.65,  0.95]])
-
-.. _statistical_distribution_usage:
-
-Customizing with Statistical Distributions
-------------------------------------------
-
-Now, let's say we want to transform these designs to be normally
-distributed with means = [1, 2, 3, 4] and standard deviations = [0.1,
-0.5, 1, 0.25]::
-
-    >>> design = lhs(4, samples=10)
-    >>> from scipy.stats.distributions import norm
-    >>> means = [1, 2, 3, 4]
-    >>> stdvs = [0.1, 0.5, 1, 0.25]
-    >>> for i in xrange(4):
-    ...     design[:, i] = norm(loc=means[i], scale=stdvs[i]).ppf(design[:, i])
-    ...
-    >>> design
-    array([[ 0.84947986,  2.16716215,  2.81669487,  3.96369414],
-           [ 1.15820413,  1.62692745,  2.28145071,  4.25062028],
-           [ 0.99159933,  2.6444164 ,  2.14908071,  3.45706066],
-           [ 1.02627463,  1.8568382 ,  3.8172492 ,  4.16756309],
-           [ 1.07459909,  2.30561153,  4.09567327,  4.3881782 ],
-           [ 0.896079  ,  2.0233295 ,  1.54235909,  3.81888286],
-           [ 1.00415   ,  2.4246118 ,  3.3500082 ,  4.07788558],
-           [ 0.91999246,  1.50179698,  2.70669743,  3.7826346 ],
-           [ 0.97030478,  1.99322045,  3.178122  ,  4.04955409],
-           [ 1.12124679,  1.22454846,  4.52414072,  3.8707982 ]])
-    
-.. note::
-   Methods for "space-filling" designs and "orthogonal" designs are in 
-   the works, so stay tuned! However, simply increasing the samples 
-   reduces the need for these anyway.
-
-.. index:: Latin-Hypercube Designs Support
-
-More Information
-================
-
-If the user needs more information about appropriate designs, please 
-consult the following articles on Wikipedia:
-
-- `Latin-Hypercube designs`_
-
-There is also a wealth of information on the `NIST`_ website about the
-various design matrices that can be created as well as detailed information
-about designing/setting-up/running experiments in general.
-
-Any questions, comments, bug-fixes, etc. can be forwarded to the `author`_.
-
-.. _author: mailto:tisimst@gmail.com
-.. _Latin-Hypercube designs: http://en.wikipedia.org/wiki/Latin_hypercube_sampling
-.. _NIST: http://www.itl.nist.gov/div898/handbook/pri/pri.htm
-.. _scipy.stats.distributions: http://docs.scipy.org/doc/scipy/reference/stats.html
+.. index:: Randomized Designs
+
+.. _randomized:
+
+================================================================================
+Randomized Designs
+================================================================================
+
+In this section, the following kinds of *randomized designs* will 
+be described:
+
+- Latin-Hypercube
+
+.. hint::
+   All available designs can be accessed after a simple import statement::
+
+    >>> from pyDOE3 import *
+    
+.. index:: Latin-Hypercube
+
+.. _latin_hypercube:
+
+Latin-Hypercube (``lhs``)
+=========================
+
+.. image:: _static/lhs.png
+
+Latin-hypercube designs can be created using the following simple syntax::
+
+    >>> lhs(n, [samples, criterion, iterations])
+
+where 
+
+* **n**: an integer that designates the number of factors (required)
+* **samples**: an integer that designates the number of sample points to 
+  generate for each factor (default: n)
+* **criterion**: a string that tells ``lhs`` how to sample the points
+  (default: None, which simply randomizes the points within the intervals):
+  
+  - "center" or "c": center the points within the sampling intervals
+  - "maximin" or "m": maximize the minimum distance between points, but
+    place the point in a randomized location within its interval
+  - "centermaximin" or "cm": same as "maximin", but centered within the
+    intervals
+  - "correlation" or "corr": minimize the maximum correlation coefficient
+  - "lhsmu" : Latin hypercube with multifimensional Uniformity. Correlation between
+     variable can be enforced by setting a valid correlation matrix. Description of the
+     algorithm can be found in `Deutsch and Deutsch`_.
+  
+The output design scales all the variable ranges from zero to one which
+can then be transformed as the user wishes (like to a specific statistical
+distribution using the `scipy.stats.distributions`_ ``ppf`` (inverse
+cumulative distribution) function. An example of this is :ref:`shown below
+<statistical_distribution_usage>`.
+
+For example, if I wanted to transform the uniform distribution of 8 samples
+to a normal distribution (mean=0, standard deviation=1), I would do 
+something like::
+
+    >>> from scipy.stats.distributions import norm
+    >>> lhd = lhs(2, samples=5)
+    >>> lhd = norm(loc=0, scale=1).ppf(lhd)  # this applies to both factors here
+
+Graphically, each transformation would look like the following, going 
+from the blue sampled points (from using ``lhs``) to the green
+sampled points that are normally distributed:
+
+.. image:: _static/lhs_custom_distribution.png
+
+Examples
+--------
+
+A basic 4-factor latin-hypercube design::
+
+    >>> lhs(4, criterion='center')
+    array([[ 0.875,  0.625,  0.875,  0.125],
+           [ 0.375,  0.125,  0.375,  0.375],
+           [ 0.625,  0.375,  0.125,  0.625],
+           [ 0.125,  0.875,  0.625,  0.875]])
+
+Let's say we want more samples, like 10::
+
+    >>> lhs(4, samples=10, criterion='center')
+    array([[ 0.05,  0.05,  0.15,  0.15],
+           [ 0.55,  0.85,  0.95,  0.75],
+           [ 0.25,  0.25,  0.45,  0.25],
+           [ 0.45,  0.35,  0.75,  0.45],
+           [ 0.75,  0.55,  0.25,  0.55],
+           [ 0.95,  0.45,  0.35,  0.05],
+           [ 0.35,  0.95,  0.05,  0.65],
+           [ 0.15,  0.65,  0.55,  0.35],
+           [ 0.85,  0.75,  0.85,  0.85],
+           [ 0.65,  0.15,  0.65,  0.95]])
+
+.. _statistical_distribution_usage:
+
+Customizing with Statistical Distributions
+------------------------------------------
+
+Now, let's say we want to transform these designs to be normally
+distributed with means = [1, 2, 3, 4] and standard deviations = [0.1,
+0.5, 1, 0.25]::
+
+    >>> design = lhs(4, samples=10)
+    >>> from scipy.stats.distributions import norm
+    >>> means = [1, 2, 3, 4]
+    >>> stdvs = [0.1, 0.5, 1, 0.25]
+    >>> for i in xrange(4):
+    ...     design[:, i] = norm(loc=means[i], scale=stdvs[i]).ppf(design[:, i])
+    ...
+    >>> design
+    array([[ 0.84947986,  2.16716215,  2.81669487,  3.96369414],
+           [ 1.15820413,  1.62692745,  2.28145071,  4.25062028],
+           [ 0.99159933,  2.6444164 ,  2.14908071,  3.45706066],
+           [ 1.02627463,  1.8568382 ,  3.8172492 ,  4.16756309],
+           [ 1.07459909,  2.30561153,  4.09567327,  4.3881782 ],
+           [ 0.896079  ,  2.0233295 ,  1.54235909,  3.81888286],
+           [ 1.00415   ,  2.4246118 ,  3.3500082 ,  4.07788558],
+           [ 0.91999246,  1.50179698,  2.70669743,  3.7826346 ],
+           [ 0.97030478,  1.99322045,  3.178122  ,  4.04955409],
+           [ 1.12124679,  1.22454846,  4.52414072,  3.8707982 ]])
+    
+.. note::
+   Methods for "space-filling" designs and "orthogonal" designs are in 
+   the works, so stay tuned! However, simply increasing the samples 
+   reduces the need for these anyway.
+
+.. index:: Latin-Hypercube Designs Support
+
+More Information
+================
+
+If the user needs more information about appropriate designs, please 
+consult the following articles on Wikipedia:
+
+- `Latin-Hypercube designs`_
+
+There is also a wealth of information on the `NIST`_ website about the
+various design matrices that can be created as well as detailed information
+about designing/setting-up/running experiments in general.
+
+Any questions, comments, bug-fixes, etc. can be forwarded to the `author`_.
+
+.. _author: mailto:tisimst@gmail.com
+.. _Latin-Hypercube designs: http://en.wikipedia.org/wiki/Latin_hypercube_sampling
+.. _NIST: http://www.itl.nist.gov/div898/handbook/pri/pri.htm
+.. _scipy.stats.distributions: http://docs.scipy.org/doc/scipy/reference/stats.html
 .. _Deutsch and Deutsch : https://www.sciencedirect.com/science/article/pii/S0378375811003776?via%3Dihub
```

### Comparing `pydoe3-1.0.0/doc/rsm.rst` & `pydoe3-1.0.1/doc/rsm.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-.. index:: Response Surface Designs, RSM
-
-.. _response_surface:
-
-================================================================================
-Response Surface Designs
-================================================================================
-
-In this section, the following kinds of *response surface designs* will 
-be described:
-
-- :ref:`Box-Behnken <box_behnken>`
-- :ref:`Central Composite <central_composite>`
-
-.. hint::
-   All available designs can be accessed after a simple import statement::
-
-    >>> from pyDOE import *
-    
-.. index:: Box-Behnken
-
-.. _box_behnken:
-
-Box-Behnken (``bbdesign``)
-==========================
-
-.. image:: http://www.itl.nist.gov/div898/handbook/pri/section3/gifs/bb.gif
-
-Box-Behnken designs can be created using the following simple syntax::
-
-    >>> bbdesign(n, center)
-
-where ``n`` is the number of factors (at least 3 required) and ``center`` 
-is the number of center points to include. If no inputs given to 
-``center``, then a pre-determined number of points are automatically
-included. 
-
-Examples
---------
-
-The default 3-factor Box-Behnken design::
-
-    >>> bbdesign(3)
-    array([[-1., -1.,  0.],
-           [ 1., -1.,  0.],
-           [-1.,  1.,  0.],
-           [ 1.,  1.,  0.],
-           [-1.,  0., -1.],
-           [ 1.,  0., -1.],
-           [-1.,  0.,  1.],
-           [ 1.,  0.,  1.],
-           [ 0., -1., -1.],
-           [ 0.,  1., -1.],
-           [ 0., -1.,  1.],
-           [ 0.,  1.,  1.],
-           [ 0.,  0.,  0.],
-           [ 0.,  0.,  0.],
-           [ 0.,  0.,  0.]])
-    
-A customized design with four factors, but only a single center point::
-
-    >>> bbdesign(4, center=1)
-    array([[-1., -1.,  0.,  0.],
-           [ 1., -1.,  0.,  0.],
-           [-1.,  1.,  0.,  0.],
-           [ 1.,  1.,  0.,  0.],
-           [-1.,  0., -1.,  0.],
-           [ 1.,  0., -1.,  0.],
-           [-1.,  0.,  1.,  0.],
-           [ 1.,  0.,  1.,  0.],
-           [-1.,  0.,  0., -1.],
-           [ 1.,  0.,  0., -1.],
-           [-1.,  0.,  0.,  1.],
-           [ 1.,  0.,  0.,  1.],
-           [ 0., -1., -1.,  0.],
-           [ 0.,  1., -1.,  0.],
-           [ 0., -1.,  1.,  0.],
-           [ 0.,  1.,  1.,  0.],
-           [ 0., -1.,  0., -1.],
-           [ 0.,  1.,  0., -1.],
-           [ 0., -1.,  0.,  1.],
-           [ 0.,  1.,  0.,  1.],
-           [ 0.,  0., -1., -1.],
-           [ 0.,  0.,  1., -1.],
-           [ 0.,  0., -1.,  1.],
-           [ 0.,  0.,  1.,  1.],
-           [ 0.,  0.,  0.,  0.]])
-
-.. index:: Central Composite
-
-.. _central_composite:
-
-Central Composite (``ccdesign``)
-================================
-
-.. image:: http://www.itl.nist.gov/div898/handbook/pri/section3/gifs/fig5.gif
-
-Central composite designs can be created and customized using the syntax::
-
-    >>> ccdesign(n, center, alpha, face)
-
-where 
-
-- ``n`` is the number of factors, 
-
-- ``center`` is a 2-tuple of center points (one for the factorial block,
-  one for the star block, default (4, 4)), 
-
-- ``alpha`` is either "orthogonal" (or "o", default) or "rotatable" 
-  (or "r")
-  
-- ``face`` is either "circumscribed" (or "ccc", default), "inscribed"
-  (or "cci"), or "faced" (or "ccf").
-
-.. image:: http://www.itl.nist.gov/div898/handbook/pri/section3/gifs/ccd2.gif
-
-The two optional keyword arguments ``alpha`` and ``face`` help describe
-how the variance in the quadratic approximation is distributed. Please
-see the `NIST`_ web pages if you are uncertain which options are suitable
-for your situation.
-
-.. note::
-   - 'ccc' and 'cci' can be rotatable designs, but 'ccf' cannot.
-   - If ``face`` is specified, while ``alpha`` is not, then the default
-     value of ``alpha`` is 'orthogonal'.
-
-Examples
---------
-
-Simplest input, assuming default kwargs::
-
-    >>> ccdesign(2)
-    array([[-1.        , -1.        ],
-           [ 1.        , -1.        ],
-           [-1.        ,  1.        ],
-           [ 1.        ,  1.        ],
-           [ 0.        ,  0.        ],
-           [ 0.        ,  0.        ],
-           [ 0.        ,  0.        ],
-           [ 0.        ,  0.        ],
-           [-1.41421356,  0.        ],
-           [ 1.41421356,  0.        ],
-           [ 0.        , -1.41421356],
-           [ 0.        ,  1.41421356],
-           [ 0.        ,  0.        ],
-           [ 0.        ,  0.        ],
-           [ 0.        ,  0.        ],
-           [ 0.        ,  0.        ]])
-
-More customized input, say, for a set of computer experiments where there
-isn't variability so we only need a single center point::
-
-    >>> ccdesign(3, center=(0, 1), alpha='r', face='cci')
-    array([[-0.59460356, -0.59460356, -0.59460356],
-           [ 0.59460356, -0.59460356, -0.59460356],
-           [-0.59460356,  0.59460356, -0.59460356],
-           [ 0.59460356,  0.59460356, -0.59460356],
-           [-0.59460356, -0.59460356,  0.59460356],
-           [ 0.59460356, -0.59460356,  0.59460356],
-           [-0.59460356,  0.59460356,  0.59460356],
-           [ 0.59460356,  0.59460356,  0.59460356],
-           [-1.        ,  0.        ,  0.        ],
-           [ 1.        ,  0.        ,  0.        ],
-           [ 0.        , -1.        ,  0.        ],
-           [ 0.        ,  1.        ,  0.        ],
-           [ 0.        ,  0.        , -1.        ],
-           [ 0.        ,  0.        ,  1.        ],
-           [ 0.        ,  0.        ,  0.        ]])
-
-.. index:: Response Surface Designs Support
-
-More Information
-================
-
-If the user needs more information about appropriate designs, please 
-consult the following articles on Wikipedia:
-
-- `Box-Behnken designs`_
-- `Central composite designs`_
-
-There is also a wealth of information on the `NIST`_ website about the
-various design matrices that can be created as well as detailed information
-about designing/setting-up/running experiments in general.
-
-Any questions, comments, bug-fixes, etc. can be forwarded to the `author`_.
-
-.. _author: mailto:tisimst@gmail.com
-.. _Box-Behnken designs: http://en.wikipedia.org/wiki/Box-Behnken_design
-.. _Central composite designs: http://en.wikipedia.org/wiki/Central_composite_design
+.. index:: Response Surface Designs, RSM
+
+.. _response_surface:
+
+================================================================================
+Response Surface Designs
+================================================================================
+
+In this section, the following kinds of *response surface designs* will 
+be described:
+
+- :ref:`Box-Behnken <box_behnken>`
+- :ref:`Central Composite <central_composite>`
+
+.. hint::
+   All available designs can be accessed after a simple import statement::
+
+    >>> from pyDOE3 import *
+    
+.. index:: Box-Behnken
+
+.. _box_behnken:
+
+Box-Behnken (``bbdesign``)
+==========================
+
+.. image:: http://www.itl.nist.gov/div898/handbook/pri/section3/gifs/bb.gif
+
+Box-Behnken designs can be created using the following simple syntax::
+
+    >>> bbdesign(n, center)
+
+where ``n`` is the number of factors (at least 3 required) and ``center`` 
+is the number of center points to include. If no inputs given to 
+``center``, then a pre-determined number of points are automatically
+included. 
+
+Examples
+--------
+
+The default 3-factor Box-Behnken design::
+
+    >>> bbdesign(3)
+    array([[-1., -1.,  0.],
+           [ 1., -1.,  0.],
+           [-1.,  1.,  0.],
+           [ 1.,  1.,  0.],
+           [-1.,  0., -1.],
+           [ 1.,  0., -1.],
+           [-1.,  0.,  1.],
+           [ 1.,  0.,  1.],
+           [ 0., -1., -1.],
+           [ 0.,  1., -1.],
+           [ 0., -1.,  1.],
+           [ 0.,  1.,  1.],
+           [ 0.,  0.,  0.],
+           [ 0.,  0.,  0.],
+           [ 0.,  0.,  0.]])
+    
+A customized design with four factors, but only a single center point::
+
+    >>> bbdesign(4, center=1)
+    array([[-1., -1.,  0.,  0.],
+           [ 1., -1.,  0.,  0.],
+           [-1.,  1.,  0.,  0.],
+           [ 1.,  1.,  0.,  0.],
+           [-1.,  0., -1.,  0.],
+           [ 1.,  0., -1.,  0.],
+           [-1.,  0.,  1.,  0.],
+           [ 1.,  0.,  1.,  0.],
+           [-1.,  0.,  0., -1.],
+           [ 1.,  0.,  0., -1.],
+           [-1.,  0.,  0.,  1.],
+           [ 1.,  0.,  0.,  1.],
+           [ 0., -1., -1.,  0.],
+           [ 0.,  1., -1.,  0.],
+           [ 0., -1.,  1.,  0.],
+           [ 0.,  1.,  1.,  0.],
+           [ 0., -1.,  0., -1.],
+           [ 0.,  1.,  0., -1.],
+           [ 0., -1.,  0.,  1.],
+           [ 0.,  1.,  0.,  1.],
+           [ 0.,  0., -1., -1.],
+           [ 0.,  0.,  1., -1.],
+           [ 0.,  0., -1.,  1.],
+           [ 0.,  0.,  1.,  1.],
+           [ 0.,  0.,  0.,  0.]])
+
+.. index:: Central Composite
+
+.. _central_composite:
+
+Central Composite (``ccdesign``)
+================================
+
+.. image:: http://www.itl.nist.gov/div898/handbook/pri/section3/gifs/fig5.gif
+
+Central composite designs can be created and customized using the syntax::
+
+    >>> ccdesign(n, center, alpha, face)
+
+where 
+
+- ``n`` is the number of factors, 
+
+- ``center`` is a 2-tuple of center points (one for the factorial block,
+  one for the star block, default (4, 4)), 
+
+- ``alpha`` is either "orthogonal" (or "o", default) or "rotatable" 
+  (or "r")
+  
+- ``face`` is either "circumscribed" (or "ccc", default), "inscribed"
+  (or "cci"), or "faced" (or "ccf").
+
+.. image:: http://www.itl.nist.gov/div898/handbook/pri/section3/gifs/ccd2.gif
+
+The two optional keyword arguments ``alpha`` and ``face`` help describe
+how the variance in the quadratic approximation is distributed. Please
+see the `NIST`_ web pages if you are uncertain which options are suitable
+for your situation.
+
+.. note::
+   - 'ccc' and 'cci' can be rotatable designs, but 'ccf' cannot.
+   - If ``face`` is specified, while ``alpha`` is not, then the default
+     value of ``alpha`` is 'orthogonal'.
+
+Examples
+--------
+
+Simplest input, assuming default kwargs::
+
+    >>> ccdesign(2)
+    array([[-1.        , -1.        ],
+           [ 1.        , -1.        ],
+           [-1.        ,  1.        ],
+           [ 1.        ,  1.        ],
+           [ 0.        ,  0.        ],
+           [ 0.        ,  0.        ],
+           [ 0.        ,  0.        ],
+           [ 0.        ,  0.        ],
+           [-1.41421356,  0.        ],
+           [ 1.41421356,  0.        ],
+           [ 0.        , -1.41421356],
+           [ 0.        ,  1.41421356],
+           [ 0.        ,  0.        ],
+           [ 0.        ,  0.        ],
+           [ 0.        ,  0.        ],
+           [ 0.        ,  0.        ]])
+
+More customized input, say, for a set of computer experiments where there
+isn't variability so we only need a single center point::
+
+    >>> ccdesign(3, center=(0, 1), alpha='r', face='cci')
+    array([[-0.59460356, -0.59460356, -0.59460356],
+           [ 0.59460356, -0.59460356, -0.59460356],
+           [-0.59460356,  0.59460356, -0.59460356],
+           [ 0.59460356,  0.59460356, -0.59460356],
+           [-0.59460356, -0.59460356,  0.59460356],
+           [ 0.59460356, -0.59460356,  0.59460356],
+           [-0.59460356,  0.59460356,  0.59460356],
+           [ 0.59460356,  0.59460356,  0.59460356],
+           [-1.        ,  0.        ,  0.        ],
+           [ 1.        ,  0.        ,  0.        ],
+           [ 0.        , -1.        ,  0.        ],
+           [ 0.        ,  1.        ,  0.        ],
+           [ 0.        ,  0.        , -1.        ],
+           [ 0.        ,  0.        ,  1.        ],
+           [ 0.        ,  0.        ,  0.        ]])
+
+.. index:: Response Surface Designs Support
+
+More Information
+================
+
+If the user needs more information about appropriate designs, please 
+consult the following articles on Wikipedia:
+
+- `Box-Behnken designs`_
+- `Central composite designs`_
+
+There is also a wealth of information on the `NIST`_ website about the
+various design matrices that can be created as well as detailed information
+about designing/setting-up/running experiments in general.
+
+Any questions, comments, bug-fixes, etc. can be forwarded to the `author`_.
+
+.. _author: mailto:tisimst@gmail.com
+.. _Box-Behnken designs: http://en.wikipedia.org/wiki/Box-Behnken_design
+.. _Central composite designs: http://en.wikipedia.org/wiki/Central_composite_design
 .. _NIST: http://www.itl.nist.gov/div898/handbook/pri/pri.htm
```

### Comparing `pydoe3-1.0.0/doc/_build/html/_images/lhs.png` & `pydoe3-1.0.1/doc/_static/lhs.png`

 * *Files identical despite different names*

### Comparing `pydoe3-1.0.0/doc/_build/html/_images/lhs_custom_distribution.png` & `pydoe3-1.0.1/doc/_static/lhs_custom_distribution.png`

 * *Files identical despite different names*

### Comparing `pydoe3-1.0.0/doc/_build/html/_static/_default.css` & `pydoe3-1.0.1/doc/_static/_default.css`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,507 +1,507 @@
-/**
- * Alternate Sphinx design
- * Originally created by Armin Ronacher for Werkzeug, adapted by Georg Brandl.
- */
-
-body {
-    font-family: 'Lucida Grande', 'Lucida Sans Unicode', 'Geneva', 'Verdana', sans-serif;
-    font-size: 14px;
-    letter-spacing: -0.01em;
-    line-height: 150%;
-    text-align: center;
-    /*background-color: #AFC1C4; */
-    background-color: #BFD1D4;
-    color: black;
-    padding: 0;
-    border: 1px solid #aaa;
-
-    margin: 0px 80px 0px 80px;
-    min-width: 740px;
-}
-
-a {
-    color: #CA7900;
-    text-decoration: none;
-}
-
-a:hover {
-    color: #2491CF;
-}
-
-pre {
-    font-family: 'Consolas', 'Deja Vu Sans Mono', 'Bitstream Vera Sans Mono', monospace;
-    font-size: 0.95em;
-    letter-spacing: 0.015em;
-    padding: 0.5em;
-    border: 1px solid #ccc;
-    background-color: #f8f8f8;
-}
-
-td.linenos pre {
-    padding: 0.5em 0;
-    border: 0;
-    background-color: transparent;
-    color: #aaa;
-}
-
-table.highlighttable {
-    margin-left: 0.5em;
-}
-
-table.highlighttable td {
-    padding: 0 0.5em 0 0.5em;
-}
-
-cite, code, tt {
-    font-family: 'Consolas', 'Deja Vu Sans Mono', 'Bitstream Vera Sans Mono', monospace;
-    font-size: 0.95em;
-    letter-spacing: 0.01em;
-}
-
-hr {
-    border: 1px solid #abc;
-    margin: 2em;
-}
-
-tt {
-    background-color: #f2f2f2;
-    border-bottom: 1px solid #ddd;
-    color: #333;
-}
-
-tt.descname {
-    background-color: transparent;
-    font-weight: bold;
-    font-size: 1.2em;
-    border: 0;
-}
-
-tt.descclassname {
-    background-color: transparent;
-    border: 0;
-}
-
-tt.xref {
-    background-color: transparent;
-    font-weight: bold;
-    border: 0;
-}
-
-a tt {
-    background-color: transparent;
-    font-weight: bold;
-    border: 0;
-    color: #CA7900;
-}
-
-a tt:hover {
-    color: #2491CF;
-}
-
-dl {
-    margin-bottom: 15px;
-}
-
-dd p {
-    margin-top: 0px;
-}
-
-dd ul, dd table {
-    margin-bottom: 10px;
-}
-
-dd {
-    margin-top: 3px;
-    margin-bottom: 10px;
-    margin-left: 30px;
-}
-
-.refcount {
-    color: #060;
-}
-
-dt:target,
-.highlight {
-    background-color: #fbe54e;
-}
-
-dl.class, dl.function {
-    border-top: 2px solid #888;
-}
-
-dl.method, dl.attribute {
-    border-top: 1px solid #aaa;
-}
-
-dl.glossary dt {
-    font-weight: bold;
-    font-size: 1.1em;
-}
-
-pre {
-    line-height: 120%;
-}
-
-pre a {
-    color: inherit;
-    text-decoration: underline;
-}
-
-.first {
-    margin-top: 0 !important;
-}
-
-div.document {
-    background-color: white;
-    text-align: left;
-    background-image: url(contents.png);
-    background-repeat: repeat-x;
-}
-
-/*
-div.documentwrapper {
-    width: 100%;
-}
-*/
-
-div.clearer {
-    clear: both;
-}
-
-div.related h3 {
-    display: none;
-}
-
-div.related ul {
-    background-image: url(navigation.png);
-    height: 2em;
-    list-style: none;
-    border-top: 1px solid #ddd;
-    border-bottom: 1px solid #ddd;
-    margin: 0;
-    padding-left: 10px;
-}
-
-div.related ul li {
-    margin: 0;
-    padding: 0;
-    height: 2em;
-    float: left;
-}
-
-div.related ul li.right {
-    float: right;
-    margin-right: 5px;
-}
-
-div.related ul li a {
-    margin: 0;
-    padding: 0 5px 0 5px;
-    line-height: 1.75em;
-    color: #EE9816;
-}
-
-div.related ul li a:hover {
-    color: #3CA8E7;
-}
-
-div.body {
-    margin: 0;
-    padding: 0.5em 20px 20px 20px;
-}
-
-div.bodywrapper {
-    margin: 0 240px 0 0;
-    border-right: 1px solid #ccc;
-}
-
-div.body a {
-    text-decoration: underline;
-}
-
-div.sphinxsidebar {
-    margin: 0;
-    padding: 0.5em 15px 15px 0;
-    width: 210px;
-    float: right;
-    text-align: left;
-/*    margin-left: -100%; */
-}
-
-div.sphinxsidebar h4, div.sphinxsidebar h3 {
-    margin: 1em 0 0.5em 0;
-    font-size: 0.9em;
-    padding: 0.1em 0 0.1em 0.5em;
-    color: white;
-    border: 1px solid #86989B;
-    background-color: #AFC1C4;
-}
-
-div.sphinxsidebar ul {
-    padding-left: 1.5em;
-    margin-top: 7px;
-    list-style: none;
-    padding: 0;
-    line-height: 130%;
-}
-
-div.sphinxsidebar ul ul {
-    list-style: square;
-    margin-left: 20px;
-}
-
-p {
-    margin: 0.8em 0 0.5em 0;
-}
-
-p.rubric {
-    font-weight: bold;
-}
-
-h1 {
-    margin: 0;
-    padding: 0.7em 0 0.3em 0;
-    font-size: 1.5em;
-    color: #11557C;
-}
-
-h2 {
-    margin: 1.3em 0 0.2em 0;
-    font-size: 1.35em;
-    padding: 0;
-}
-
-h3 {
-    margin: 1em 0 -0.3em 0;
-    font-size: 1.2em;
-}
-
-h1 a, h2 a, h3 a, h4 a, h5 a, h6 a {
-    color: black!important;
-}
-
-h1 a.anchor, h2 a.anchor, h3 a.anchor, h4 a.anchor, h5 a.anchor, h6 a.anchor {
-    display: none;
-    margin: 0 0 0 0.3em;
-    padding: 0 0.2em 0 0.2em;
-    color: #aaa!important;
-}
-
-h1:hover a.anchor, h2:hover a.anchor, h3:hover a.anchor, h4:hover a.anchor,
-h5:hover a.anchor, h6:hover a.anchor {
-    display: inline;
-}
-
-h1 a.anchor:hover, h2 a.anchor:hover, h3 a.anchor:hover, h4 a.anchor:hover,
-h5 a.anchor:hover, h6 a.anchor:hover {
-    color: #777;
-    background-color: #eee;
-}
-
-table {
-    border-collapse: collapse;
-    margin: 0 -0.5em 0 -0.5em;
-}
-
-table td, table th {
-    padding: 0.2em 0.5em 0.2em 0.5em;
-}
-
-div.footer {
-    background-color: #E3EFF1;
-    color: #86989B;
-    padding: 3px 8px 3px 0;
-    clear: both;
-    font-size: 0.8em;
-    text-align: right;
-}
-
-div.footer a {
-    color: #86989B;
-    text-decoration: underline;
-}
-
-div.pagination {
-    margin-top: 2em;
-    padding-top: 0.5em;
-    border-top: 1px solid black;
-    text-align: center;
-}
-
-div.sphinxsidebar ul.toc {
-    margin: 1em 0 1em 0;
-    padding: 0 0 0 0.5em;
-    list-style: none;
-}
-
-div.sphinxsidebar ul.toc li {
-    margin: 0.5em 0 0.5em 0;
-    font-size: 0.9em;
-    line-height: 130%;
-}
-
-div.sphinxsidebar ul.toc li p {
-    margin: 0;
-    padding: 0;
-}
-
-div.sphinxsidebar ul.toc ul {
-    margin: 0.2em 0 0.2em 0;
-    padding: 0 0 0 1.8em;
-}
-
-div.sphinxsidebar ul.toc ul li {
-    padding: 0;
-}
-
-div.admonition, div.warning {
-    font-size: 0.9em;
-    margin: 1em 0 0 0;
-    border: 1px solid #86989B;
-    background-color: #f7f7f7;
-}
-
-div.admonition p, div.warning p {
-    margin: 0.5em 1em 0.5em 1em;
-    padding: 0;
-}
-
-div.admonition pre, div.warning pre {
-    margin: 0.4em 1em 0.4em 1em;
-}
-
-div.admonition p.admonition-title,
-div.warning p.admonition-title {
-    margin: 0;
-    padding: 0.1em 0 0.1em 0.5em;
-    color: white;
-    border-bottom: 1px solid #86989B;
-    font-weight: bold;
-    background-color: #AFC1C4;
-}
-
-div.warning {
-    border: 1px solid #940000;
-}
-
-div.warning p.admonition-title {
-    background-color: #CF0000;
-    border-bottom-color: #940000;
-}
-
-div.admonition ul, div.admonition ol,
-div.warning ul, div.warning ol {
-    margin: 0.1em 0.5em 0.5em 3em;
-    padding: 0;
-}
-
-div.versioninfo {
-    margin: 1em 0 0 0;
-    border: 1px solid #ccc;
-    background-color: #DDEAF0;
-    padding: 8px;
-    line-height: 1.3em;
-    font-size: 0.9em;
-}
-
-
-a.headerlink {
-    color: #c60f0f!important;
-    font-size: 1em;
-    margin-left: 6px;
-    padding: 0 4px 0 4px;
-    text-decoration: none!important;
-    visibility: hidden;
-}
-
-h1:hover > a.headerlink,
-h2:hover > a.headerlink,
-h3:hover > a.headerlink,
-h4:hover > a.headerlink,
-h5:hover > a.headerlink,
-h6:hover > a.headerlink,
-dt:hover > a.headerlink {
-    visibility: visible;
-}
-
-a.headerlink:hover {
-    background-color: #ccc;
-    color: white!important;
-}
-
-table.indextable td {
-    text-align: left;
-    vertical-align: top;
-}
-
-table.indextable dl, table.indextable dd {
-    margin-top: 0;
-    margin-bottom: 0;
-}
-
-table.indextable tr.pcap {
-    height: 10px;
-}
-
-table.indextable tr.cap {
-    margin-top: 10px;
-    background-color: #f2f2f2;
-}
-
-img.toggler {
-    margin-right: 3px;
-    margin-top: 3px;
-    cursor: pointer;
-}
-
-img.inheritance {
-    border: 0px
-}
-
-form.pfform {
-    margin: 10px 0 20px 0;
-}
-
-table.contentstable {
-    width: 90%;
-}
-
-table.contentstable p.biglink {
-    line-height: 150%;
-}
-
-a.biglink {
-    font-size: 1.3em;
-}
-
-span.linkdescr {
-    font-style: italic;
-    padding-top: 5px;
-    font-size: 90%;
-}
-
-ul.search {
-    margin: 10px 0 0 20px;
-    padding: 0;
-}
-
-ul.search li {
-    padding: 5px 0 5px 20px;
-    background-image: url(file.png);
-    background-repeat: no-repeat;
-    background-position: 0 7px;
-}
-
-ul.search li a {
-    font-weight: bold;
-}
-
-ul.search li div.context {
-    color: #888;
-    margin: 2px 0 0 30px;
-    text-align: left;
-}
-
-ul.keywordmatches li.goodmatch a {
-    font-weight: bold;
-}
+/**
+ * Alternate Sphinx design
+ * Originally created by Armin Ronacher for Werkzeug, adapted by Georg Brandl.
+ */
+
+body {
+    font-family: 'Lucida Grande', 'Lucida Sans Unicode', 'Geneva', 'Verdana', sans-serif;
+    font-size: 14px;
+    letter-spacing: -0.01em;
+    line-height: 150%;
+    text-align: center;
+    /*background-color: #AFC1C4; */
+    background-color: #BFD1D4;
+    color: black;
+    padding: 0;
+    border: 1px solid #aaa;
+
+    margin: 0px 80px 0px 80px;
+    min-width: 740px;
+}
+
+a {
+    color: #CA7900;
+    text-decoration: none;
+}
+
+a:hover {
+    color: #2491CF;
+}
+
+pre {
+    font-family: 'Consolas', 'Deja Vu Sans Mono', 'Bitstream Vera Sans Mono', monospace;
+    font-size: 0.95em;
+    letter-spacing: 0.015em;
+    padding: 0.5em;
+    border: 1px solid #ccc;
+    background-color: #f8f8f8;
+}
+
+td.linenos pre {
+    padding: 0.5em 0;
+    border: 0;
+    background-color: transparent;
+    color: #aaa;
+}
+
+table.highlighttable {
+    margin-left: 0.5em;
+}
+
+table.highlighttable td {
+    padding: 0 0.5em 0 0.5em;
+}
+
+cite, code, tt {
+    font-family: 'Consolas', 'Deja Vu Sans Mono', 'Bitstream Vera Sans Mono', monospace;
+    font-size: 0.95em;
+    letter-spacing: 0.01em;
+}
+
+hr {
+    border: 1px solid #abc;
+    margin: 2em;
+}
+
+tt {
+    background-color: #f2f2f2;
+    border-bottom: 1px solid #ddd;
+    color: #333;
+}
+
+tt.descname {
+    background-color: transparent;
+    font-weight: bold;
+    font-size: 1.2em;
+    border: 0;
+}
+
+tt.descclassname {
+    background-color: transparent;
+    border: 0;
+}
+
+tt.xref {
+    background-color: transparent;
+    font-weight: bold;
+    border: 0;
+}
+
+a tt {
+    background-color: transparent;
+    font-weight: bold;
+    border: 0;
+    color: #CA7900;
+}
+
+a tt:hover {
+    color: #2491CF;
+}
+
+dl {
+    margin-bottom: 15px;
+}
+
+dd p {
+    margin-top: 0px;
+}
+
+dd ul, dd table {
+    margin-bottom: 10px;
+}
+
+dd {
+    margin-top: 3px;
+    margin-bottom: 10px;
+    margin-left: 30px;
+}
+
+.refcount {
+    color: #060;
+}
+
+dt:target,
+.highlight {
+    background-color: #fbe54e;
+}
+
+dl.class, dl.function {
+    border-top: 2px solid #888;
+}
+
+dl.method, dl.attribute {
+    border-top: 1px solid #aaa;
+}
+
+dl.glossary dt {
+    font-weight: bold;
+    font-size: 1.1em;
+}
+
+pre {
+    line-height: 120%;
+}
+
+pre a {
+    color: inherit;
+    text-decoration: underline;
+}
+
+.first {
+    margin-top: 0 !important;
+}
+
+div.document {
+    background-color: white;
+    text-align: left;
+    background-image: url(contents.png);
+    background-repeat: repeat-x;
+}
+
+/*
+div.documentwrapper {
+    width: 100%;
+}
+*/
+
+div.clearer {
+    clear: both;
+}
+
+div.related h3 {
+    display: none;
+}
+
+div.related ul {
+    background-image: url(navigation.png);
+    height: 2em;
+    list-style: none;
+    border-top: 1px solid #ddd;
+    border-bottom: 1px solid #ddd;
+    margin: 0;
+    padding-left: 10px;
+}
+
+div.related ul li {
+    margin: 0;
+    padding: 0;
+    height: 2em;
+    float: left;
+}
+
+div.related ul li.right {
+    float: right;
+    margin-right: 5px;
+}
+
+div.related ul li a {
+    margin: 0;
+    padding: 0 5px 0 5px;
+    line-height: 1.75em;
+    color: #EE9816;
+}
+
+div.related ul li a:hover {
+    color: #3CA8E7;
+}
+
+div.body {
+    margin: 0;
+    padding: 0.5em 20px 20px 20px;
+}
+
+div.bodywrapper {
+    margin: 0 240px 0 0;
+    border-right: 1px solid #ccc;
+}
+
+div.body a {
+    text-decoration: underline;
+}
+
+div.sphinxsidebar {
+    margin: 0;
+    padding: 0.5em 15px 15px 0;
+    width: 210px;
+    float: right;
+    text-align: left;
+/*    margin-left: -100%; */
+}
+
+div.sphinxsidebar h4, div.sphinxsidebar h3 {
+    margin: 1em 0 0.5em 0;
+    font-size: 0.9em;
+    padding: 0.1em 0 0.1em 0.5em;
+    color: white;
+    border: 1px solid #86989B;
+    background-color: #AFC1C4;
+}
+
+div.sphinxsidebar ul {
+    padding-left: 1.5em;
+    margin-top: 7px;
+    list-style: none;
+    padding: 0;
+    line-height: 130%;
+}
+
+div.sphinxsidebar ul ul {
+    list-style: square;
+    margin-left: 20px;
+}
+
+p {
+    margin: 0.8em 0 0.5em 0;
+}
+
+p.rubric {
+    font-weight: bold;
+}
+
+h1 {
+    margin: 0;
+    padding: 0.7em 0 0.3em 0;
+    font-size: 1.5em;
+    color: #11557C;
+}
+
+h2 {
+    margin: 1.3em 0 0.2em 0;
+    font-size: 1.35em;
+    padding: 0;
+}
+
+h3 {
+    margin: 1em 0 -0.3em 0;
+    font-size: 1.2em;
+}
+
+h1 a, h2 a, h3 a, h4 a, h5 a, h6 a {
+    color: black!important;
+}
+
+h1 a.anchor, h2 a.anchor, h3 a.anchor, h4 a.anchor, h5 a.anchor, h6 a.anchor {
+    display: none;
+    margin: 0 0 0 0.3em;
+    padding: 0 0.2em 0 0.2em;
+    color: #aaa!important;
+}
+
+h1:hover a.anchor, h2:hover a.anchor, h3:hover a.anchor, h4:hover a.anchor,
+h5:hover a.anchor, h6:hover a.anchor {
+    display: inline;
+}
+
+h1 a.anchor:hover, h2 a.anchor:hover, h3 a.anchor:hover, h4 a.anchor:hover,
+h5 a.anchor:hover, h6 a.anchor:hover {
+    color: #777;
+    background-color: #eee;
+}
+
+table {
+    border-collapse: collapse;
+    margin: 0 -0.5em 0 -0.5em;
+}
+
+table td, table th {
+    padding: 0.2em 0.5em 0.2em 0.5em;
+}
+
+div.footer {
+    background-color: #E3EFF1;
+    color: #86989B;
+    padding: 3px 8px 3px 0;
+    clear: both;
+    font-size: 0.8em;
+    text-align: right;
+}
+
+div.footer a {
+    color: #86989B;
+    text-decoration: underline;
+}
+
+div.pagination {
+    margin-top: 2em;
+    padding-top: 0.5em;
+    border-top: 1px solid black;
+    text-align: center;
+}
+
+div.sphinxsidebar ul.toc {
+    margin: 1em 0 1em 0;
+    padding: 0 0 0 0.5em;
+    list-style: none;
+}
+
+div.sphinxsidebar ul.toc li {
+    margin: 0.5em 0 0.5em 0;
+    font-size: 0.9em;
+    line-height: 130%;
+}
+
+div.sphinxsidebar ul.toc li p {
+    margin: 0;
+    padding: 0;
+}
+
+div.sphinxsidebar ul.toc ul {
+    margin: 0.2em 0 0.2em 0;
+    padding: 0 0 0 1.8em;
+}
+
+div.sphinxsidebar ul.toc ul li {
+    padding: 0;
+}
+
+div.admonition, div.warning {
+    font-size: 0.9em;
+    margin: 1em 0 0 0;
+    border: 1px solid #86989B;
+    background-color: #f7f7f7;
+}
+
+div.admonition p, div.warning p {
+    margin: 0.5em 1em 0.5em 1em;
+    padding: 0;
+}
+
+div.admonition pre, div.warning pre {
+    margin: 0.4em 1em 0.4em 1em;
+}
+
+div.admonition p.admonition-title,
+div.warning p.admonition-title {
+    margin: 0;
+    padding: 0.1em 0 0.1em 0.5em;
+    color: white;
+    border-bottom: 1px solid #86989B;
+    font-weight: bold;
+    background-color: #AFC1C4;
+}
+
+div.warning {
+    border: 1px solid #940000;
+}
+
+div.warning p.admonition-title {
+    background-color: #CF0000;
+    border-bottom-color: #940000;
+}
+
+div.admonition ul, div.admonition ol,
+div.warning ul, div.warning ol {
+    margin: 0.1em 0.5em 0.5em 3em;
+    padding: 0;
+}
+
+div.versioninfo {
+    margin: 1em 0 0 0;
+    border: 1px solid #ccc;
+    background-color: #DDEAF0;
+    padding: 8px;
+    line-height: 1.3em;
+    font-size: 0.9em;
+}
+
+
+a.headerlink {
+    color: #c60f0f!important;
+    font-size: 1em;
+    margin-left: 6px;
+    padding: 0 4px 0 4px;
+    text-decoration: none!important;
+    visibility: hidden;
+}
+
+h1:hover > a.headerlink,
+h2:hover > a.headerlink,
+h3:hover > a.headerlink,
+h4:hover > a.headerlink,
+h5:hover > a.headerlink,
+h6:hover > a.headerlink,
+dt:hover > a.headerlink {
+    visibility: visible;
+}
+
+a.headerlink:hover {
+    background-color: #ccc;
+    color: white!important;
+}
+
+table.indextable td {
+    text-align: left;
+    vertical-align: top;
+}
+
+table.indextable dl, table.indextable dd {
+    margin-top: 0;
+    margin-bottom: 0;
+}
+
+table.indextable tr.pcap {
+    height: 10px;
+}
+
+table.indextable tr.cap {
+    margin-top: 10px;
+    background-color: #f2f2f2;
+}
+
+img.toggler {
+    margin-right: 3px;
+    margin-top: 3px;
+    cursor: pointer;
+}
+
+img.inheritance {
+    border: 0px
+}
+
+form.pfform {
+    margin: 10px 0 20px 0;
+}
+
+table.contentstable {
+    width: 90%;
+}
+
+table.contentstable p.biglink {
+    line-height: 150%;
+}
+
+a.biglink {
+    font-size: 1.3em;
+}
+
+span.linkdescr {
+    font-style: italic;
+    padding-top: 5px;
+    font-size: 90%;
+}
+
+ul.search {
+    margin: 10px 0 0 20px;
+    padding: 0;
+}
+
+ul.search li {
+    padding: 5px 0 5px 20px;
+    background-image: url(file.png);
+    background-repeat: no-repeat;
+    background-position: 0 7px;
+}
+
+ul.search li a {
+    font-weight: bold;
+}
+
+ul.search li div.context {
+    color: #888;
+    margin: 2px 0 0 30px;
+    text-align: left;
+}
+
+ul.keywordmatches li.goodmatch a {
+    font-weight: bold;
+}
```

### Comparing `pydoe3-1.0.0/doc/_build/html/_static/drawing.svg` & `pydoe3-1.0.1/doc/_static/drawing.svg`

 * *Files 11% similar despite different names*

```diff
@@ -1,893 +1,873 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
-00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
-00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
-00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
-00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 786d  >....<svg..   xm
-00000080: 6c6e 733a 6463 3d22 6874 7470 3a2f 2f70  lns:dc="http://p
-00000090: 7572 6c2e 6f72 672f 6463 2f65 6c65 6d65  url.org/dc/eleme
-000000a0: 6e74 732f 312e 312f 220d 0a20 2020 786d  nts/1.1/"..   xm
-000000b0: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
-000000c0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000000d0: 7267 2f6e 7323 220d 0a20 2020 786d 6c6e  rg/ns#"..   xmln
-000000e0: 733a 7264 663d 2268 7474 703a 2f2f 7777  s:rdf="http://ww
-000000f0: 772e 7733 2e6f 7267 2f31 3939 392f 3032  w.w3.org/1999/02
-00000100: 2f32 322d 7264 662d 7379 6e74 6178 2d6e  /22-rdf-syntax-n
-00000110: 7323 220d 0a20 2020 786d 6c6e 733a 7376  s#"..   xmlns:sv
-00000120: 673d 2268 7474 703a 2f2f 7777 772e 7733  g="http://www.w3
-00000130: 2e6f 7267 2f32 3030 302f 7376 6722 0d0a  .org/2000/svg"..
-00000140: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
-00000150: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000160: 2f73 7667 220d 0a20 2020 786d 6c6e 733a  /svg"..   xmlns:
-00000170: 786c 696e 6b3d 2268 7474 703a 2f2f 7777  xlink="http://ww
-00000180: 772e 7733 2e6f 7267 2f31 3939 392f 786c  w.w3.org/1999/xl
-00000190: 696e 6b22 0d0a 2020 2078 6d6c 6e73 3a73  ink"..   xmlns:s
-000001a0: 6f64 6970 6f64 693d 2268 7474 703a 2f2f  odipodi="http://
-000001b0: 736f 6469 706f 6469 2e73 6f75 7263 6566  sodipodi.sourcef
-000001c0: 6f72 6765 2e6e 6574 2f44 5444 2f73 6f64  orge.net/DTD/sod
-000001d0: 6970 6f64 692d 302e 6474 6422 0d0a 2020  ipodi-0.dtd"..  
-000001e0: 2078 6d6c 6e73 3a69 6e6b 7363 6170 653d   xmlns:inkscape=
-000001f0: 2268 7474 703a 2f2f 7777 772e 696e 6b73  "http://www.inks
-00000200: 6361 7065 2e6f 7267 2f6e 616d 6573 7061  cape.org/namespa
-00000210: 6365 732f 696e 6b73 6361 7065 220d 0a20  ces/inkscape".. 
-00000220: 2020 7769 6474 683d 2235 3030 220d 0a20    width="500".. 
-00000230: 2020 6865 6967 6874 3d22 3130 3022 0d0a    height="100"..
-00000240: 2020 2069 643d 2273 7667 3222 0d0a 2020     id="svg2"..  
-00000250: 2076 6572 7369 6f6e 3d22 312e 3122 0d0a   version="1.1"..
-00000260: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
-00000270: 696f 6e3d 2230 2e34 382e 3420 7239 3933  ion="0.48.4 r993
-00000280: 3922 0d0a 2020 2073 6f64 6970 6f64 693a  9"..   sodipodi:
-00000290: 646f 636e 616d 653d 224e 6577 2064 6f63  docname="New doc
-000002a0: 756d 656e 7420 3122 3e0d 0a20 203c 6465  ument 1">..  <de
-000002b0: 6673 0d0a 2020 2020 2069 643d 2264 6566  fs..     id="def
-000002c0: 7334 223e 0d0a 2020 2020 3c69 6e6b 7363  s4">..    <inksc
-000002d0: 6170 653a 7065 7273 7065 6374 6976 650d  ape:perspective.
-000002e0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-000002f0: 3a74 7970 653d 2269 6e6b 7363 6170 653a  :type="inkscape:
-00000300: 7065 7273 7033 6422 0d0a 2020 2020 2020  persp3d"..      
-00000310: 2069 6e6b 7363 6170 653a 7670 5f78 3d22   inkscape:vp_x="
-00000320: 3020 3a20 3530 203a 2031 220d 0a20 2020  0 : 50 : 1"..   
-00000330: 2020 2020 696e 6b73 6361 7065 3a76 705f      inkscape:vp_
-00000340: 793d 2230 203a 2031 3030 3020 3a20 3022  y="0 : 1000 : 0"
-00000350: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
-00000360: 653a 7670 5f7a 3d22 3530 3020 3a20 3530  e:vp_z="500 : 50
-00000370: 203a 2031 220d 0a20 2020 2020 2020 696e   : 1"..       in
-00000380: 6b73 6361 7065 3a70 6572 7370 3364 2d6f  kscape:persp3d-o
-00000390: 7269 6769 6e3d 2232 3530 203a 2033 332e  rigin="250 : 33.
-000003a0: 3333 3333 3333 203a 2031 220d 0a20 2020  333333 : 1"..   
-000003b0: 2020 2020 6964 3d22 7065 7273 7065 6374      id="perspect
-000003c0: 6976 6533 3833 3222 202f 3e0d 0a20 2020  ive3832" />..   
-000003d0: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
-000003e0: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
-000003f0: 6561 7247 7261 6469 656e 7433 3735 3522  earGradient3755"
-00000400: 3e0d 0a20 2020 2020 203c 7374 6f70 0d0a  >..      <stop..
-00000410: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00000420: 7374 6f70 2d63 6f6c 6f72 3a23 6666 6361  stop-color:#ffca
-00000430: 6361 3b73 746f 702d 6f70 6163 6974 793a  ca;stop-opacity:
-00000440: 313b 220d 0a20 2020 2020 2020 2020 6f66  1;"..         of
-00000450: 6673 6574 3d22 3022 0d0a 2020 2020 2020  fset="0"..      
-00000460: 2020 2069 643d 2273 746f 7033 3735 3722     id="stop3757"
-00000470: 202f 3e0d 0a20 2020 2020 203c 7374 6f70   />..      <stop
-00000480: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
-00000490: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6664  ="stop-color:#fd
-000004a0: 3030 3030 3b73 746f 702d 6f70 6163 6974  0000;stop-opacit
-000004b0: 793a 313b 220d 0a20 2020 2020 2020 2020  y:1;"..         
-000004c0: 6f66 6673 6574 3d22 3122 0d0a 2020 2020  offset="1"..    
-000004d0: 2020 2020 2069 643d 2273 746f 7033 3735       id="stop375
-000004e0: 3922 202f 3e0d 0a20 2020 203c 2f6c 696e  9" />..    </lin
-000004f0: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
-00000500: 2020 3c72 6164 6961 6c47 7261 6469 656e    <radialGradien
-00000510: 740d 0a20 2020 2020 2020 696e 6b73 6361  t..       inksca
-00000520: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
-00000530: 7973 220d 0a20 2020 2020 2020 786c 696e  ys"..       xlin
-00000540: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-00000550: 7261 6469 656e 7433 3735 3522 0d0a 2020  radient3755"..  
-00000560: 2020 2020 2069 643d 2272 6164 6961 6c47       id="radialG
-00000570: 7261 6469 656e 7433 3736 3122 0d0a 2020  radient3761"..  
-00000580: 2020 2020 2063 783d 2234 362e 3533 3838       cx="46.5388
-00000590: 3322 0d0a 2020 2020 2020 2063 793d 2233  3"..       cy="3
-000005a0: 332e 3232 3933 3238 220d 0a20 2020 2020  3.229328"..     
-000005b0: 2020 6678 3d22 3436 2e35 3338 3833 220d    fx="46.53883".
-000005c0: 0a20 2020 2020 2020 6679 3d22 3333 2e32  .       fy="33.2
-000005d0: 3239 3332 3822 0d0a 2020 2020 2020 2072  29328"..       r
-000005e0: 3d22 362e 3435 3934 3735 3522 0d0a 2020  ="6.4594755"..  
-000005f0: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
-00000600: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
-00000610: 7365 2220 2f3e 0d0a 2020 2020 3c72 6164  se" />..    <rad
-00000620: 6961 6c47 7261 6469 656e 740d 0a20 2020  ialGradient..   
-00000630: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
-00000640: 6c65 6374 3d22 616c 7761 7973 220d 0a20  lect="always".. 
-00000650: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
-00000660: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
-00000670: 7433 3735 3522 0d0a 2020 2020 2020 2069  t3755"..       i
-00000680: 643d 2272 6164 6961 6c47 7261 6469 656e  d="radialGradien
-00000690: 7433 3736 3522 0d0a 2020 2020 2020 2067  t3765"..       g
-000006a0: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
-000006b0: 6572 5370 6163 654f 6e55 7365 220d 0a20  erSpaceOnUse".. 
-000006c0: 2020 2020 2020 6378 3d22 3436 2e35 3338        cx="46.538
-000006d0: 3833 220d 0a20 2020 2020 2020 6379 3d22  83"..       cy="
-000006e0: 3333 2e32 3239 3332 3822 0d0a 2020 2020  33.229328"..    
-000006f0: 2020 2066 783d 2234 362e 3533 3838 3322     fx="46.53883"
-00000700: 0d0a 2020 2020 2020 2066 793d 2233 332e  ..       fy="33.
-00000710: 3232 3933 3238 220d 0a20 2020 2020 2020  229328"..       
-00000720: 723d 2236 2e34 3539 3437 3535 2220 2f3e  r="6.4594755" />
-00000730: 0d0a 2020 2020 3c72 6164 6961 6c47 7261  ..    <radialGra
-00000740: 6469 656e 740d 0a20 2020 2020 2020 696e  dient..       in
-00000750: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
-00000760: 616c 7761 7973 220d 0a20 2020 2020 2020  always"..       
-00000770: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
-00000780: 6561 7247 7261 6469 656e 7433 3735 3522  earGradient3755"
-00000790: 0d0a 2020 2020 2020 2069 643d 2272 6164  ..       id="rad
-000007a0: 6961 6c47 7261 6469 656e 7433 3736 3922  ialGradient3769"
-000007b0: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
-000007c0: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
-000007d0: 654f 6e55 7365 220d 0a20 2020 2020 2020  eOnUse"..       
-000007e0: 6378 3d22 3436 2e35 3338 3833 220d 0a20  cx="46.53883".. 
-000007f0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
-00000800: 3332 3822 0d0a 2020 2020 2020 2066 783d  328"..       fx=
-00000810: 2234 362e 3533 3838 3322 0d0a 2020 2020  "46.53883"..    
-00000820: 2020 2066 793d 2233 332e 3232 3933 3238     fy="33.229328
-00000830: 220d 0a20 2020 2020 2020 723d 2236 2e34  "..       r="6.4
-00000840: 3539 3437 3535 2220 2f3e 0d0a 2020 2020  594755" />..    
-00000850: 3c72 6164 6961 6c47 7261 6469 656e 740d  <radialGradient.
-00000860: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000870: 3a63 6f6c 6c65 6374 3d22 616c 7761 7973  :collect="always
-00000880: 220d 0a20 2020 2020 2020 786c 696e 6b3a  "..       xlink:
-00000890: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
-000008a0: 6469 656e 7433 3735 3522 0d0a 2020 2020  dient3755"..    
-000008b0: 2020 2069 643d 2272 6164 6961 6c47 7261     id="radialGra
-000008c0: 6469 656e 7433 3737 3322 0d0a 2020 2020  dient3773"..    
-000008d0: 2020 2067 7261 6469 656e 7455 6e69 7473     gradientUnits
-000008e0: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
-000008f0: 220d 0a20 2020 2020 2020 6378 3d22 3436  "..       cx="46
-00000900: 2e35 3338 3833 220d 0a20 2020 2020 2020  .53883"..       
-00000910: 6379 3d22 3333 2e32 3239 3332 3822 0d0a  cy="33.229328"..
-00000920: 2020 2020 2020 2066 783d 2234 362e 3533         fx="46.53
-00000930: 3838 3322 0d0a 2020 2020 2020 2066 793d  883"..       fy=
-00000940: 2233 332e 3232 3933 3238 220d 0a20 2020  "33.229328"..   
-00000950: 2020 2020 723d 2236 2e34 3539 3437 3535      r="6.4594755
-00000960: 2220 2f3e 0d0a 2020 2020 3c72 6164 6961  " />..    <radia
-00000970: 6c47 7261 6469 656e 740d 0a20 2020 2020  lGradient..     
-00000980: 2020 696e 6b73 6361 7065 3a63 6f6c 6c65    inkscape:colle
-00000990: 6374 3d22 616c 7761 7973 220d 0a20 2020  ct="always"..   
-000009a0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
-000009b0: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
-000009c0: 3735 3522 0d0a 2020 2020 2020 2069 643d  755"..       id=
-000009d0: 2272 6164 6961 6c47 7261 6469 656e 7433  "radialGradient3
-000009e0: 3836 3622 0d0a 2020 2020 2020 2067 7261  866"..       gra
-000009f0: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
-00000a00: 5370 6163 654f 6e55 7365 220d 0a20 2020  SpaceOnUse"..   
-00000a10: 2020 2020 6378 3d22 3436 2e35 3338 3833      cx="46.53883
-00000a20: 220d 0a20 2020 2020 2020 6379 3d22 3333  "..       cy="33
-00000a30: 2e32 3239 3332 3822 0d0a 2020 2020 2020  .229328"..      
-00000a40: 2066 783d 2234 362e 3533 3838 3322 0d0a   fx="46.53883"..
-00000a50: 2020 2020 2020 2066 793d 2233 332e 3232         fy="33.22
-00000a60: 3933 3238 220d 0a20 2020 2020 2020 723d  9328"..       r=
-00000a70: 2236 2e34 3539 3437 3535 2220 2f3e 0d0a  "6.4594755" />..
-00000a80: 2020 2020 3c72 6164 6961 6c47 7261 6469      <radialGradi
-00000a90: 656e 740d 0a20 2020 2020 2020 696e 6b73  ent..       inks
-00000aa0: 6361 7065 3a63 6f6c 6c65 6374 3d22 616c  cape:collect="al
-00000ab0: 7761 7973 220d 0a20 2020 2020 2020 786c  ways"..       xl
-00000ac0: 696e 6b3a 6872 6566 3d22 236c 696e 6561  ink:href="#linea
-00000ad0: 7247 7261 6469 656e 7433 3735 3522 0d0a  rGradient3755"..
-00000ae0: 2020 2020 2020 2069 643d 2272 6164 6961         id="radia
-00000af0: 6c47 7261 6469 656e 7433 3836 3822 0d0a  lGradient3868"..
-00000b00: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-00000b10: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00000b20: 6e55 7365 220d 0a20 2020 2020 2020 6378  nUse"..       cx
-00000b30: 3d22 3436 2e35 3338 3833 220d 0a20 2020  ="46.53883"..   
-00000b40: 2020 2020 6379 3d22 3333 2e32 3239 3332      cy="33.22932
-00000b50: 3822 0d0a 2020 2020 2020 2066 783d 2234  8"..       fx="4
-00000b60: 362e 3533 3838 3322 0d0a 2020 2020 2020  6.53883"..      
-00000b70: 2066 793d 2233 332e 3232 3933 3238 220d   fy="33.229328".
-00000b80: 0a20 2020 2020 2020 723d 2236 2e34 3539  .       r="6.459
-00000b90: 3437 3535 2220 2f3e 0d0a 2020 2020 3c72  4755" />..    <r
-00000ba0: 6164 6961 6c47 7261 6469 656e 740d 0a20  adialGradient.. 
-00000bb0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00000bc0: 6f6c 6c65 6374 3d22 616c 7761 7973 220d  ollect="always".
-00000bd0: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-00000be0: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
-00000bf0: 656e 7433 3735 3522 0d0a 2020 2020 2020  ent3755"..      
-00000c00: 2069 643d 2272 6164 6961 6c47 7261 6469   id="radialGradi
-00000c10: 656e 7433 3837 3022 0d0a 2020 2020 2020  ent3870"..      
-00000c20: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
-00000c30: 7573 6572 5370 6163 654f 6e55 7365 220d  userSpaceOnUse".
-00000c40: 0a20 2020 2020 2020 6378 3d22 3436 2e35  .       cx="46.5
-00000c50: 3338 3833 220d 0a20 2020 2020 2020 6379  3883"..       cy
-00000c60: 3d22 3333 2e32 3239 3332 3822 0d0a 2020  ="33.229328"..  
-00000c70: 2020 2020 2066 783d 2234 362e 3533 3838       fx="46.5388
-00000c80: 3322 0d0a 2020 2020 2020 2066 793d 2233  3"..       fy="3
-00000c90: 332e 3232 3933 3238 220d 0a20 2020 2020  3.229328"..     
-00000ca0: 2020 723d 2236 2e34 3539 3437 3535 2220    r="6.4594755" 
-00000cb0: 2f3e 0d0a 2020 2020 3c72 6164 6961 6c47  />..    <radialG
-00000cc0: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
-00000cd0: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
-00000ce0: 3d22 616c 7761 7973 220d 0a20 2020 2020  ="always"..     
-00000cf0: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
-00000d00: 696e 6561 7247 7261 6469 656e 7433 3735  inearGradient375
-00000d10: 3522 0d0a 2020 2020 2020 2069 643d 2272  5"..       id="r
-00000d20: 6164 6961 6c47 7261 6469 656e 7433 3837  adialGradient387
-00000d30: 3222 0d0a 2020 2020 2020 2067 7261 6469  2"..       gradi
-00000d40: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
-00000d50: 6163 654f 6e55 7365 220d 0a20 2020 2020  aceOnUse"..     
-00000d60: 2020 6378 3d22 3436 2e35 3338 3833 220d    cx="46.53883".
-00000d70: 0a20 2020 2020 2020 6379 3d22 3333 2e32  .       cy="33.2
-00000d80: 3239 3332 3822 0d0a 2020 2020 2020 2066  29328"..       f
-00000d90: 783d 2234 362e 3533 3838 3322 0d0a 2020  x="46.53883"..  
-00000da0: 2020 2020 2066 793d 2233 332e 3232 3933       fy="33.2293
-00000db0: 3238 220d 0a20 2020 2020 2020 723d 2236  28"..       r="6
-00000dc0: 2e34 3539 3437 3535 2220 2f3e 0d0a 2020  .4594755" />..  
-00000dd0: 3c2f 6465 6673 3e0d 0a20 203c 736f 6469  </defs>..  <sodi
-00000de0: 706f 6469 3a6e 616d 6564 7669 6577 0d0a  podi:namedview..
-00000df0: 2020 2020 2069 643d 2262 6173 6522 0d0a       id="base"..
-00000e00: 2020 2020 2070 6167 6563 6f6c 6f72 3d22       pagecolor="
-00000e10: 2366 6666 6666 6622 0d0a 2020 2020 2062  #ffffff"..     b
-00000e20: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
-00000e30: 3636 3622 0d0a 2020 2020 2062 6f72 6465  666"..     borde
-00000e40: 726f 7061 6369 7479 3d22 312e 3022 0d0a  ropacity="1.0"..
-00000e50: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
-00000e60: 6765 6f70 6163 6974 793d 2230 2e30 220d  geopacity="0.0".
-00000e70: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
-00000e80: 6167 6573 6861 646f 773d 2232 220d 0a20  ageshadow="2".. 
-00000e90: 2020 2020 696e 6b73 6361 7065 3a7a 6f6f      inkscape:zoo
-00000ea0: 6d3d 2232 2e32 3222 0d0a 2020 2020 2069  m="2.22"..     i
-00000eb0: 6e6b 7363 6170 653a 6378 3d22 3235 3022  nkscape:cx="250"
-00000ec0: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
-00000ed0: 6379 3d22 3530 220d 0a20 2020 2020 696e  cy="50"..     in
-00000ee0: 6b73 6361 7065 3a64 6f63 756d 656e 742d  kscape:document-
-00000ef0: 756e 6974 733d 2270 7822 0d0a 2020 2020  units="px"..    
-00000f00: 2069 6e6b 7363 6170 653a 6375 7272 656e   inkscape:curren
-00000f10: 742d 6c61 7965 723d 226c 6179 6572 3122  t-layer="layer1"
-00000f20: 0d0a 2020 2020 2073 686f 7767 7269 643d  ..     showgrid=
-00000f30: 2266 616c 7365 220d 0a20 2020 2020 696e  "false"..     in
-00000f40: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
-00000f50: 6474 683d 2231 3537 3522 0d0a 2020 2020  dth="1575"..    
-00000f60: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-00000f70: 2d68 6569 6768 743d 2238 3830 220d 0a20  -height="880".. 
-00000f80: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-00000f90: 646f 772d 783d 2232 3322 0d0a 2020 2020  dow-x="23"..    
-00000fa0: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-00000fb0: 2d79 3d22 2d33 220d 0a20 2020 2020 696e  -y="-3"..     in
-00000fc0: 6b73 6361 7065 3a77 696e 646f 772d 6d61  kscape:window-ma
-00000fd0: 7869 6d69 7a65 643d 2231 2220 2f3e 0d0a  ximized="1" />..
-00000fe0: 2020 3c6d 6574 6164 6174 610d 0a20 2020    <metadata..   
-00000ff0: 2020 6964 3d22 6d65 7461 6461 7461 3722    id="metadata7"
-00001000: 3e0d 0a20 2020 203c 7264 663a 5244 463e  >..    <rdf:RDF>
-00001010: 0d0a 2020 2020 2020 3c63 633a 576f 726b  ..      <cc:Work
-00001020: 0d0a 2020 2020 2020 2020 2072 6466 3a61  ..         rdf:a
-00001030: 626f 7574 3d22 223e 0d0a 2020 2020 2020  bout="">..      
-00001040: 2020 3c64 633a 666f 726d 6174 3e69 6d61    <dc:format>ima
-00001050: 6765 2f73 7667 2b78 6d6c 3c2f 6463 3a66  ge/svg+xml</dc:f
-00001060: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
-00001070: 3c64 633a 7479 7065 0d0a 2020 2020 2020  <dc:type..      
-00001080: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
-00001090: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
-000010a0: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
-000010b0: 7469 6c6c 496d 6167 6522 202f 3e0d 0a20  tillImage" />.. 
-000010c0: 2020 2020 2020 203c 6463 3a74 6974 6c65         <dc:title
-000010d0: 3e3c 2f64 633a 7469 746c 653e 0d0a 2020  ></dc:title>..  
-000010e0: 2020 2020 3c2f 6363 3a57 6f72 6b3e 0d0a      </cc:Work>..
-000010f0: 2020 2020 3c2f 7264 663a 5244 463e 0d0a      </rdf:RDF>..
-00001100: 2020 3c2f 6d65 7461 6461 7461 3e0d 0a20    </metadata>.. 
-00001110: 203c 670d 0a20 2020 2020 696e 6b73 6361   <g..     inksca
-00001120: 7065 3a6c 6162 656c 3d22 4c61 7965 7220  pe:label="Layer 
-00001130: 3122 0d0a 2020 2020 2069 6e6b 7363 6170  1"..     inkscap
-00001140: 653a 6772 6f75 706d 6f64 653d 226c 6179  e:groupmode="lay
-00001150: 6572 220d 0a20 2020 2020 6964 3d22 6c61  er"..     id="la
-00001160: 7965 7231 220d 0a20 2020 2020 7472 616e  yer1"..     tran
-00001170: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00001180: 2830 2c2d 3935 322e 3336 3231 3829 223e  (0,-952.36218)">
-00001190: 0d0a 2020 2020 3c67 0d0a 2020 2020 2020  ..    <g..      
-000011a0: 2069 643d 2267 3338 3438 220d 0a20 2020   id="g3848"..   
-000011b0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-000011c0: 7261 6e73 6c61 7465 282d 3136 2c30 2922  ranslate(-16,0)"
-000011d0: 3e0d 0a20 2020 2020 203c 7061 7468 0d0a  >..      <path..
-000011e0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-000011f0: 6f70 6163 6974 793a 302e 353b 6669 6c6c  opacity:0.5;fill
-00001200: 3a6e 6f6e 653b 7374 726f 6b65 3a23 3030  :none;stroke:#00
-00001210: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-00001220: 683a 3170 783b 7374 726f 6b65 2d6c 696e  h:1px;stroke-lin
-00001230: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00001240: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00001250: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00001260: 220d 0a20 2020 2020 2020 2020 643d 226d  "..         d="m
-00001270: 2037 322e 3933 3439 3738 2c39 3732 2e30   72.934978,972.0
-00001280: 3033 3635 202d 312e 3937 3731 362c 3334  0365 -1.97716,34
-00001290: 2e37 3130 3035 220d 0a20 2020 2020 2020  .71005"..       
-000012a0: 2020 6964 3d22 7061 7468 3337 3831 220d    id="path3781".
-000012b0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000012c0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-000012d0: 7661 7475 7265 3d22 3022 202f 3e0d 0a20  vature="0" />.. 
-000012e0: 2020 2020 203c 7061 7468 0d0a 2020 2020       <path..    
-000012f0: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
-00001300: 7472 616e 736c 6174 6528 302c 3935 322e  translate(0,952.
-00001310: 3336 3231 3829 220d 0a20 2020 2020 2020  36218)"..       
-00001320: 2020 643d 226d 2035 322e 3434 3333 3835    d="m 52.443385
-00001330: 2c33 352e 3034 3137 3138 2063 2030 2c33  ,35.041718 c 0,3
-00001340: 2e32 3931 3332 3720 2d32 2e36 3638 3134  .291327 -2.66814
-00001350: 382c 352e 3935 3934 3735 202d 352e 3935  8,5.959475 -5.95
-00001360: 3934 3735 2c35 2e39 3539 3437 3520 2d33  9475,5.959475 -3
-00001370: 2e32 3931 3332 382c 3020 2d35 2e39 3539  .291328,0 -5.959
-00001380: 3437 362c 2d32 2e36 3638 3134 3820 2d35  476,-2.668148 -5
-00001390: 2e39 3539 3437 362c 2d35 2e39 3539 3437  .959476,-5.95947
-000013a0: 3520 302c 2d33 2e32 3931 3332 3820 322e  5 0,-3.291328 2.
-000013b0: 3636 3831 3438 2c2d 352e 3935 3934 3736  668148,-5.959476
-000013c0: 2035 2e39 3539 3437 362c 2d35 2e39 3539   5.959476,-5.959
-000013d0: 3437 3620 332e 3239 3133 3237 2c30 2035  476 3.291327,0 5
-000013e0: 2e39 3539 3437 352c 322e 3636 3831 3438  .959475,2.668148
-000013f0: 2035 2e39 3539 3437 352c 352e 3935 3934   5.959475,5.9594
-00001400: 3736 207a 220d 0a20 2020 2020 2020 2020  76 z"..         
-00001410: 736f 6469 706f 6469 3a72 793d 2235 2e39  sodipodi:ry="5.9
-00001420: 3539 3437 3535 220d 0a20 2020 2020 2020  594755"..       
-00001430: 2020 736f 6469 706f 6469 3a72 783d 2235    sodipodi:rx="5
-00001440: 2e39 3539 3437 3535 220d 0a20 2020 2020  .9594755"..     
-00001450: 2020 2020 736f 6469 706f 6469 3a63 793d      sodipodi:cy=
-00001460: 2233 352e 3034 3137 3138 220d 0a20 2020  "35.041718"..   
-00001470: 2020 2020 2020 736f 6469 706f 6469 3a63        sodipodi:c
-00001480: 783d 2234 362e 3438 3339 3122 0d0a 2020  x="46.48391"..  
-00001490: 2020 2020 2020 2069 643d 2270 6174 6832         id="path2
-000014a0: 3938 3522 0d0a 2020 2020 2020 2020 2073  985"..         s
-000014b0: 7479 6c65 3d22 6669 6c6c 3a75 726c 2823  tyle="fill:url(#
-000014c0: 7261 6469 616c 4772 6164 6965 6e74 3338  radialGradient38
-000014d0: 3636 293b 6669 6c6c 2d6f 7061 6369 7479  66);fill-opacity
-000014e0: 3a31 3b73 7472 6f6b 653a 2330 3030 3030  :1;stroke:#00000
-000014f0: 303b 7374 726f 6b65 2d77 6964 7468 3a31  0;stroke-width:1
-00001500: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00001510: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6d69  :round;stroke-mi
-00001520: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00001530: 652d 6f70 6163 6974 793a 313b 7374 726f  e-opacity:1;stro
-00001540: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00001550: 6522 0d0a 2020 2020 2020 2020 2073 6f64  e"..         sod
-00001560: 6970 6f64 693a 7479 7065 3d22 6172 6322  ipodi:type="arc"
-00001570: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00001580: 0d0a 2020 2020 2020 2020 2073 6f64 6970  ..         sodip
-00001590: 6f64 693a 7479 7065 3d22 6172 6322 0d0a  odi:type="arc"..
-000015a0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-000015b0: 6669 6c6c 3a75 726c 2823 7261 6469 616c  fill:url(#radial
-000015c0: 4772 6164 6965 6e74 3338 3638 293b 6669  Gradient3868);fi
-000015d0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-000015e0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-000015f0: 6b65 2d77 6964 7468 3a31 3b73 7472 6f6b  ke-width:1;strok
-00001600: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
-00001610: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00001620: 6974 3a34 3b73 7472 6f6b 652d 6f70 6163  it:4;stroke-opac
-00001630: 6974 793a 313b 7374 726f 6b65 2d64 6173  ity:1;stroke-das
-00001640: 6861 7272 6179 3a6e 6f6e 6522 0d0a 2020  harray:none"..  
-00001650: 2020 2020 2020 2069 643d 2270 6174 6833         id="path3
-00001660: 3736 3322 0d0a 2020 2020 2020 2020 2073  763"..         s
-00001670: 6f64 6970 6f64 693a 6378 3d22 3436 2e34  odipodi:cx="46.4
-00001680: 3833 3931 220d 0a20 2020 2020 2020 2020  8391"..         
-00001690: 736f 6469 706f 6469 3a63 793d 2233 352e  sodipodi:cy="35.
-000016a0: 3034 3137 3138 220d 0a20 2020 2020 2020  041718"..       
-000016b0: 2020 736f 6469 706f 6469 3a72 783d 2235    sodipodi:rx="5
-000016c0: 2e39 3539 3437 3535 220d 0a20 2020 2020  .9594755"..     
-000016d0: 2020 2020 736f 6469 706f 6469 3a72 793d      sodipodi:ry=
-000016e0: 2235 2e39 3539 3437 3535 220d 0a20 2020  "5.9594755"..   
-000016f0: 2020 2020 2020 643d 226d 2035 322e 3434        d="m 52.44
-00001700: 3333 3835 2c33 352e 3034 3137 3138 2063  3385,35.041718 c
-00001710: 2030 2c33 2e32 3931 3332 3720 2d32 2e36   0,3.291327 -2.6
-00001720: 3638 3134 382c 352e 3935 3934 3735 202d  68148,5.959475 -
-00001730: 352e 3935 3934 3735 2c35 2e39 3539 3437  5.959475,5.95947
-00001740: 3520 2d33 2e32 3931 3332 382c 3020 2d35  5 -3.291328,0 -5
-00001750: 2e39 3539 3437 362c 2d32 2e36 3638 3134  .959476,-2.66814
-00001760: 3820 2d35 2e39 3539 3437 362c 2d35 2e39  8 -5.959476,-5.9
-00001770: 3539 3437 3520 302c 2d33 2e32 3931 3332  59475 0,-3.29132
-00001780: 3820 322e 3636 3831 3438 2c2d 352e 3935  8 2.668148,-5.95
-00001790: 3934 3736 2035 2e39 3539 3437 362c 2d35  9476 5.959476,-5
-000017a0: 2e39 3539 3437 3620 332e 3239 3133 3237  .959476 3.291327
-000017b0: 2c30 2035 2e39 3539 3437 352c 322e 3636  ,0 5.959475,2.66
-000017c0: 3831 3438 2035 2e39 3539 3437 352c 352e  8148 5.959475,5.
-000017d0: 3935 3934 3736 207a 220d 0a20 2020 2020  959476 z"..     
-000017e0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-000017f0: 7261 6e73 6c61 7465 2837 362e 3031 3035  ranslate(76.0105
-00001800: 3435 2c39 3432 2e30 3337 3035 2922 202f  45,942.03705)" /
-00001810: 3e0d 0a20 2020 2020 203c 7061 7468 0d0a  >..      <path..
-00001820: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-00001830: 726d 3d22 7472 616e 736c 6174 6528 3437  rm="translate(47
-00001840: 2e34 3531 3637 2c39 3936 2e37 3833 3937  .45167,996.78397
-00001850: 2922 0d0a 2020 2020 2020 2020 2064 3d22  )"..         d="
-00001860: 6d20 3532 2e34 3433 3338 352c 3335 2e30  m 52.443385,35.0
-00001870: 3431 3731 3820 6320 302c 332e 3239 3133  41718 c 0,3.2913
-00001880: 3237 202d 322e 3636 3831 3438 2c35 2e39  27 -2.668148,5.9
-00001890: 3539 3437 3520 2d35 2e39 3539 3437 352c  59475 -5.959475,
-000018a0: 352e 3935 3934 3735 202d 332e 3239 3133  5.959475 -3.2913
-000018b0: 3238 2c30 202d 352e 3935 3934 3736 2c2d  28,0 -5.959476,-
-000018c0: 322e 3636 3831 3438 202d 352e 3935 3934  2.668148 -5.9594
-000018d0: 3736 2c2d 352e 3935 3934 3735 2030 2c2d  76,-5.959475 0,-
-000018e0: 332e 3239 3133 3238 2032 2e36 3638 3134  3.291328 2.66814
-000018f0: 382c 2d35 2e39 3539 3437 3620 352e 3935  8,-5.959476 5.95
-00001900: 3934 3736 2c2d 352e 3935 3934 3736 2033  9476,-5.959476 3
-00001910: 2e32 3931 3332 372c 3020 352e 3935 3934  .291327,0 5.9594
-00001920: 3735 2c32 2e36 3638 3134 3820 352e 3935  75,2.668148 5.95
-00001930: 3934 3735 2c35 2e39 3539 3437 3620 7a22  9475,5.959476 z"
-00001940: 0d0a 2020 2020 2020 2020 2073 6f64 6970  ..         sodip
-00001950: 6f64 693a 7279 3d22 352e 3935 3934 3735  odi:ry="5.959475
-00001960: 3522 0d0a 2020 2020 2020 2020 2073 6f64  5"..         sod
-00001970: 6970 6f64 693a 7278 3d22 352e 3935 3934  ipodi:rx="5.9594
-00001980: 3735 3522 0d0a 2020 2020 2020 2020 2073  755"..         s
-00001990: 6f64 6970 6f64 693a 6379 3d22 3335 2e30  odipodi:cy="35.0
-000019a0: 3431 3731 3822 0d0a 2020 2020 2020 2020  41718"..        
-000019b0: 2073 6f64 6970 6f64 693a 6378 3d22 3436   sodipodi:cx="46
-000019c0: 2e34 3833 3931 220d 0a20 2020 2020 2020  .48391"..       
-000019d0: 2020 6964 3d22 7061 7468 3337 3637 220d    id="path3767".
-000019e0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-000019f0: 2266 696c 6c3a 7572 6c28 2372 6164 6961  "fill:url(#radia
-00001a00: 6c47 7261 6469 656e 7433 3837 3029 3b66  lGradient3870);f
-00001a10: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00001a20: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00001a30: 6f6b 652d 7769 6474 683a 313b 7374 726f  oke-width:1;stro
-00001a40: 6b65 2d6c 696e 656a 6f69 6e3a 726f 756e  ke-linejoin:roun
-00001a50: 643b 7374 726f 6b65 2d6d 6974 6572 6c69  d;stroke-miterli
-00001a60: 6d69 743a 343b 7374 726f 6b65 2d6f 7061  mit:4;stroke-opa
-00001a70: 6369 7479 3a31 3b73 7472 6f6b 652d 6461  city:1;stroke-da
-00001a80: 7368 6172 7261 793a 6e6f 6e65 220d 0a20  sharray:none".. 
-00001a90: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-00001aa0: 3a74 7970 653d 2261 7263 2220 2f3e 0d0a  :type="arc" />..
-00001ab0: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
-00001ac0: 2020 2020 2020 736f 6469 706f 6469 3a74        sodipodi:t
-00001ad0: 7970 653d 2261 7263 220d 0a20 2020 2020  ype="arc"..     
-00001ae0: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
-00001af0: 7479 3a30 2e35 3b66 696c 6c3a 7572 6c28  ty:0.5;fill:url(
-00001b00: 2372 6164 6961 6c47 7261 6469 656e 7433  #radialGradient3
-00001b10: 3837 3229 3b66 696c 6c2d 6f70 6163 6974  872);fill-opacit
-00001b20: 793a 313b 7374 726f 6b65 3a23 3030 3030  y:1;stroke:#0000
-00001b30: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-00001b40: 313b 7374 726f 6b65 2d6c 696e 656a 6f69  1;stroke-linejoi
-00001b50: 6e3a 726f 756e 643b 7374 726f 6b65 2d6d  n:round;stroke-m
-00001b60: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00001b70: 6b65 2d6f 7061 6369 7479 3a31 3b73 7472  ke-opacity:1;str
-00001b80: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00001b90: 6e65 220d 0a20 2020 2020 2020 2020 6964  ne"..         id
-00001ba0: 3d22 7061 7468 3337 3731 220d 0a20 2020  ="path3771"..   
-00001bb0: 2020 2020 2020 736f 6469 706f 6469 3a63        sodipodi:c
-00001bc0: 783d 2234 362e 3438 3339 3122 0d0a 2020  x="46.48391"..  
-00001bd0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00001be0: 6379 3d22 3335 2e30 3431 3731 3822 0d0a  cy="35.041718"..
-00001bf0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00001c00: 693a 7278 3d22 352e 3935 3934 3735 3522  i:rx="5.9594755"
-00001c10: 0d0a 2020 2020 2020 2020 2073 6f64 6970  ..         sodip
-00001c20: 6f64 693a 7279 3d22 352e 3935 3934 3735  odi:ry="5.959475
-00001c30: 3522 0d0a 2020 2020 2020 2020 2064 3d22  5"..         d="
-00001c40: 6d20 3532 2e34 3433 3338 352c 3335 2e30  m 52.443385,35.0
-00001c50: 3431 3731 3820 6320 302c 332e 3239 3133  41718 c 0,3.2913
-00001c60: 3237 202d 322e 3636 3831 3438 2c35 2e39  27 -2.668148,5.9
-00001c70: 3539 3437 3520 2d35 2e39 3539 3437 352c  59475 -5.959475,
-00001c80: 352e 3935 3934 3735 202d 332e 3239 3133  5.959475 -3.2913
-00001c90: 3238 2c30 202d 352e 3935 3934 3736 2c2d  28,0 -5.959476,-
-00001ca0: 322e 3636 3831 3438 202d 352e 3935 3934  2.668148 -5.9594
-00001cb0: 3736 2c2d 352e 3935 3934 3735 2030 2c2d  76,-5.959475 0,-
-00001cc0: 332e 3239 3133 3238 2032 2e36 3638 3134  3.291328 2.66814
-00001cd0: 382c 2d35 2e39 3539 3437 3620 352e 3935  8,-5.959476 5.95
-00001ce0: 3934 3736 2c2d 352e 3935 3934 3736 2033  9476,-5.959476 3
-00001cf0: 2e32 3931 3332 372c 3020 352e 3935 3934  .291327,0 5.9594
-00001d00: 3735 2c32 2e36 3638 3134 3820 352e 3935  75,2.668148 5.95
-00001d10: 3934 3735 2c35 2e39 3539 3437 3620 7a22  9475,5.959476 z"
-00001d20: 0d0a 2020 2020 2020 2020 2074 7261 6e73  ..         trans
-00001d30: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00001d40: 3233 2e39 3435 3531 392c 3937 372e 3233  23.945519,977.23
-00001d50: 3231 3229 2220 2f3e 0d0a 2020 2020 2020  212)" />..      
-00001d60: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
-00001d70: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00001d80: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00001d90: 0d0a 2020 2020 2020 2020 2069 643d 2270  ..         id="p
-00001da0: 6174 6833 3737 3522 0d0a 2020 2020 2020  ath3775"..      
-00001db0: 2020 2064 3d22 4d20 3435 2e39 3133 3838     d="M 45.91388
-00001dc0: 342c 3939 332e 3438 3639 3620 3433 2e39  4,993.48696 43.9
-00001dd0: 3336 3733 312c 3130 3238 2e31 3937 220d  36731,1028.197".
-00001de0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00001df0: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
-00001e00: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00001e10: 2d77 6964 7468 3a31 7078 3b73 7472 6f6b  -width:1px;strok
-00001e20: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00001e30: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00001e40: 6974 6572 3b73 7472 6f6b 652d 6f70 6163  iter;stroke-opac
-00001e50: 6974 793a 3122 202f 3e0d 0a20 2020 2020  ity:1" />..     
-00001e60: 203c 7061 7468 0d0a 2020 2020 2020 2020   <path..        
-00001e70: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
-00001e80: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-00001e90: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
-00001ea0: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00001eb0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00001ec0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00001ed0: 6b65 2d6f 7061 6369 7479 3a31 220d 0a20  ke-opacity:1".. 
-00001ee0: 2020 2020 2020 2020 643d 226d 2039 362e          d="m 96.
-00001ef0: 3232 3134 3431 2c39 3931 2e35 3535 3520  221441,991.5555 
-00001f00: 2d31 2e39 3737 3135 332c 3334 2e37 3122  -1.977153,34.71"
-00001f10: 0d0a 2020 2020 2020 2020 2069 643d 2270  ..         id="p
-00001f20: 6174 6833 3737 3722 0d0a 2020 2020 2020  ath3777"..      
-00001f30: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00001f40: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00001f50: 2230 2220 2f3e 0d0a 2020 2020 2020 3c70  "0" />..      <p
-00001f60: 6174 680d 0a20 2020 2020 2020 2020 696e  ath..         in
-00001f70: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00001f80: 2d63 7572 7661 7475 7265 3d22 3022 0d0a  -curvature="0"..
-00001f90: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00001fa0: 6833 3737 3922 0d0a 2020 2020 2020 2020  h3779"..        
-00001fb0: 2064 3d22 6d20 3132 322e 3336 3338 2c39   d="m 122.3638,9
-00001fc0: 3833 2e33 3831 3531 202d 312e 3937 3731  83.38151 -1.9771
-00001fd0: 362c 3334 2e37 3039 3939 220d 0a20 2020  6,34.70999"..   
-00001fe0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00001ff0: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
-00002000: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-00002010: 7468 3a31 7078 3b73 7472 6f6b 652d 6c69  th:1px;stroke-li
-00002020: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00002030: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00002040: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00002050: 3122 202f 3e0d 0a20 2020 2020 203c 7061  1" />..      <pa
-00002060: 7468 0d0a 2020 2020 2020 2020 2074 7261  th..         tra
-00002070: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00002080: 6528 302c 3935 322e 3336 3231 3829 220d  e(0,952.36218)".
-00002090: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000020a0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-000020b0: 7661 7475 7265 3d22 3022 0d0a 2020 2020  vature="0"..    
-000020c0: 2020 2020 2069 643d 2270 6174 6833 3738       id="path378
-000020d0: 3322 0d0a 2020 2020 2020 2020 2064 3d22  3"..         d="
-000020e0: 6d20 3434 2e31 3536 3431 352c 3735 2e33  m 44.156415,75.3
-000020f0: 3935 3433 3120 3433 2e34 3937 3336 342c  95431 43.497364,
-00002100: 332e 3935 3433 3035 220d 0a20 2020 2020  3.954305"..     
-00002110: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00002120: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
-00002130: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-00002140: 3a31 7078 3b73 7472 6f6b 652d 6c69 6e65  :1px;stroke-line
-00002150: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00002160: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00002170: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00002180: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00002190: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
-000021a0: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
-000021b0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
-000021c0: 652d 7769 6474 683a 3170 783b 7374 726f  e-width:1px;stro
-000021d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000021e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000021f0: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
-00002200: 6369 7479 3a31 220d 0a20 2020 2020 2020  city:1"..       
-00002210: 2020 643d 226d 2037 322e 3731 3532 392c    d="m 72.71529,
-00002220: 3937 322e 3339 3733 3320 3433 2e34 3937  972.39733 43.497
-00002230: 3336 2c33 2e39 3534 3322 0d0a 2020 2020  36,3.9543"..    
-00002240: 2020 2020 2069 643d 2270 6174 6833 3738       id="path378
-00002250: 3522 0d0a 2020 2020 2020 2020 2069 6e6b  5"..         ink
-00002260: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-00002270: 6375 7276 6174 7572 653d 2230 2220 2f3e  curvature="0" />
-00002280: 0d0a 2020 2020 2020 3c70 6174 680d 0a20  ..      <path.. 
-00002290: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000022a0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-000022b0: 7475 7265 3d22 3022 0d0a 2020 2020 2020  ture="0"..      
-000022c0: 2020 2069 643d 2270 6174 6833 3738 3722     id="path3787"
-000022d0: 0d0a 2020 2020 2020 2020 2064 3d22 6d20  ..         d="m 
-000022e0: 3736 2e34 3439 3931 322c 3130 3133 2e34  76.449912,1013.4
-000022f0: 3738 3220 3433 2e34 3937 3335 382c 332e  782 43.497358,3.
-00002300: 3935 3433 220d 0a20 2020 2020 2020 2020  9543"..         
-00002310: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
-00002320: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00002330: 7374 726f 6b65 2d77 6964 7468 3a31 7078  stroke-width:1px
-00002340: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00002350: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00002360: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00002370: 652d 6f70 6163 6974 793a 3122 202f 3e0d  e-opacity:1" />.
-00002380: 0a20 2020 2020 203c 7061 7468 0d0a 2020  .      <path..  
-00002390: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000023a0: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
-000023b0: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-000023c0: 6474 683a 3170 783b 7374 726f 6b65 2d6c  dth:1px;stroke-l
-000023d0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-000023e0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-000023f0: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
-00002400: 3a31 220d 0a20 2020 2020 2020 2020 643d  :1"..         d=
-00002410: 226d 2035 322e 3530 3433 3934 2c39 3837  "m 52.504394,987
-00002420: 2e39 3934 3837 2034 332e 3439 3733 3634  .99487 43.497364
-00002430: 2c33 2e39 3534 3322 0d0a 2020 2020 2020  ,3.9543"..      
-00002440: 2020 2069 643d 2270 6174 6833 3738 3922     id="path3789"
-00002450: 0d0a 2020 2020 2020 2020 2069 6e6b 7363  ..         inksc
-00002460: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00002470: 7276 6174 7572 653d 2230 2220 2f3e 0d0a  rvature="0" />..
-00002480: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
-00002490: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-000024a0: 2274 7261 6e73 6c61 7465 2830 2c39 3532  "translate(0,952
-000024b0: 2e33 3632 3138 2922 0d0a 2020 2020 2020  .36218)"..      
-000024c0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-000024d0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-000024e0: 2230 220d 0a20 2020 2020 2020 2020 6964  "0"..         id
-000024f0: 3d22 7061 7468 3337 3931 220d 0a20 2020  ="path3791"..   
-00002500: 2020 2020 2020 643d 224d 2034 342e 3135        d="M 44.15
-00002510: 3634 3135 2c37 352e 3137 3537 3437 2036  6415,75.175747 6
-00002520: 352e 3436 3537 3239 2c36 332e 3533 3235  5.465729,63.5325
-00002530: 3133 220d 0a20 2020 2020 2020 2020 7374  13"..         st
-00002540: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
-00002550: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
-00002560: 726f 6b65 2d77 6964 7468 3a31 7078 3b73  roke-width:1px;s
-00002570: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00002580: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00002590: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-000025a0: 6f70 6163 6974 793a 3122 202f 3e0d 0a20  opacity:1" />.. 
-000025b0: 2020 2020 203c 7061 7468 0d0a 2020 2020       <path..    
-000025c0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000025d0: 3a6e 6f6e 653b 7374 726f 6b65 3a23 3030  :none;stroke:#00
-000025e0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-000025f0: 683a 3170 783b 7374 726f 6b65 2d6c 696e  h:1px;stroke-lin
-00002600: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00002610: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00002620: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00002630: 220d 0a20 2020 2020 2020 2020 643d 224d  "..         d="M
-00002640: 2035 312e 3430 3539 3736 2c39 3834 2e30   51.405976,984.0
-00002650: 3430 3536 2037 322e 3731 3532 392c 3937  4056 72.71529,97
-00002660: 322e 3339 3733 3322 0d0a 2020 2020 2020  2.39733"..      
-00002670: 2020 2069 643d 2270 6174 6833 3739 3322     id="path3793"
-00002680: 0d0a 2020 2020 2020 2020 2069 6e6b 7363  ..         inksc
-00002690: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-000026a0: 7276 6174 7572 653d 2230 2220 2f3e 0d0a  rvature="0" />..
-000026b0: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
-000026c0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-000026d0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-000026e0: 7265 3d22 3022 0d0a 2020 2020 2020 2020  re="0"..        
-000026f0: 2069 643d 2270 6174 6833 3739 3522 0d0a   id="path3795"..
-00002700: 2020 2020 2020 2020 2064 3d22 4d20 3936           d="M 96
-00002710: 2e32 3231 3434 322c 3939 322e 3136 3838  .221442,992.1688
-00002720: 3620 3131 372e 3533 3037 362c 3938 302e  6 117.53076,980.
-00002730: 3532 3536 3322 0d0a 2020 2020 2020 2020  52563"..        
-00002740: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
-00002750: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-00002760: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
-00002770: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00002780: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00002790: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-000027a0: 6b65 2d6f 7061 6369 7479 3a31 2220 2f3e  ke-opacity:1" />
-000027b0: 0d0a 2020 2020 2020 3c70 6174 680d 0a20  ..      <path.. 
-000027c0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-000027d0: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
-000027e0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-000027f0: 6964 7468 3a31 7078 3b73 7472 6f6b 652d  idth:1px;stroke-
-00002800: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00002810: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00002820: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-00002830: 793a 3122 0d0a 2020 2020 2020 2020 2064  y:1"..         d
-00002840: 3d22 6d20 3939 2e30 3737 3333 2c31 3032  ="m 99.07733,102
-00002850: 392e 3037 3537 2032 312e 3330 3933 322c  9.0757 21.30932,
-00002860: 2d31 312e 3634 3332 220d 0a20 2020 2020  -11.6432"..     
-00002870: 2020 2020 6964 3d22 7061 7468 3337 3937      id="path3797
-00002880: 220d 0a20 2020 2020 2020 2020 696e 6b73  "..         inks
-00002890: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-000028a0: 7572 7661 7475 7265 3d22 3022 202f 3e0d  urvature="0" />.
-000028b0: 0a20 2020 203c 2f67 3e0d 0a20 2020 203c  .    </g>..    <
-000028c0: 7465 7874 0d0a 2020 2020 2020 2078 6d6c  text..       xml
-000028d0: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-000028e0: 220d 0a20 2020 2020 2020 7374 796c 653d  "..       style=
-000028f0: 2266 6f6e 742d 7369 7a65 3a34 3070 783b  "font-size:40px;
-00002900: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
-00002910: 6c3b 666f 6e74 2d77 6569 6768 743a 6e6f  l;font-weight:no
-00002920: 726d 616c 3b6c 696e 652d 6865 6967 6874  rmal;line-height
-00002930: 3a31 3235 253b 6c65 7474 6572 2d73 7061  :125%;letter-spa
-00002940: 6369 6e67 3a30 7078 3b77 6f72 642d 7370  cing:0px;word-sp
-00002950: 6163 696e 673a 3070 783b 6669 6c6c 3a23  acing:0px;fill:#
-00002960: 3030 3030 3030 3b66 696c 6c2d 6f70 6163  000000;fill-opac
-00002970: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
-00002980: 653b 666f 6e74 2d66 616d 696c 793a 5361  e;font-family:Sa
-00002990: 6e73 220d 0a20 2020 2020 2020 783d 2231  ns"..       x="1
-000029a0: 3538 2e39 3834 3338 220d 0a20 2020 2020  58.98438"..     
-000029b0: 2020 793d 2231 3031 302e 3631 3232 220d    y="1010.6122".
-000029c0: 0a20 2020 2020 2020 6964 3d22 7465 7874  .       id="text
-000029d0: 3337 3939 220d 0a20 2020 2020 2020 736f  3799"..       so
-000029e0: 6469 706f 6469 3a6c 696e 6573 7061 6369  dipodi:linespaci
-000029f0: 6e67 3d22 3132 3525 223e 3c74 7370 616e  ng="125%"><tspan
-00002a00: 0d0a 2020 2020 2020 2020 2073 6f64 6970  ..         sodip
-00002a10: 6f64 693a 726f 6c65 3d22 6c69 6e65 220d  odi:role="line".
-00002a20: 0a20 2020 2020 2020 2020 6964 3d22 7473  .         id="ts
-00002a30: 7061 6e33 3830 3122 0d0a 2020 2020 2020  pan3801"..      
-00002a40: 2020 2078 3d22 3135 382e 3938 3433 3822     x="158.98438"
-00002a50: 0d0a 2020 2020 2020 2020 2079 3d22 3130  ..         y="10
-00002a60: 3130 2e36 3132 3222 0d0a 2020 2020 2020  10.6122"..      
-00002a70: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
-00002a80: 697a 653a 3634 7078 3b66 6f6e 742d 7374  ize:64px;font-st
-00002a90: 796c 653a 6974 616c 6963 3b66 6f6e 742d  yle:italic;font-
-00002aa0: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
-00002ab0: 6f6e 742d 7765 6967 6874 3a6e 6f72 6d61  ont-weight:norma
-00002ac0: 6c3b 666f 6e74 2d73 7472 6574 6368 3a6e  l;font-stretch:n
-00002ad0: 6f72 6d61 6c3b 666f 6e74 2d66 616d 696c  ormal;font-famil
-00002ae0: 793a 526f 626f 746f 3b2d 696e 6b73 6361  y:Roboto;-inksca
-00002af0: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
-00002b00: 6174 696f 6e3a 526f 626f 746f 2049 7461  ation:Roboto Ita
-00002b10: 6c69 6322 3e70 7944 4f45 3c2f 7473 7061  lic">pyDOE</tspa
-00002b20: 6e3e 3c2f 7465 7874 3e0d 0a20 2020 203c  n></text>..    <
-00002b30: 670d 0a20 2020 2020 2020 6964 3d22 6733  g..       id="g3
-00002b40: 3831 3922 0d0a 2020 2020 2020 2074 7261  819"..       tra
-00002b50: 6e73 666f 726d 3d22 6d61 7472 6978 2831  nsform="matrix(1
-00002b60: 2e30 3832 3230 3131 2c2d 302e 3231 3936  .0822011,-0.2196
-00002b70: 3134 3037 2c30 2e32 3139 3631 3430 372c  1407,0.21961407,
-00002b80: 312e 3038 3232 3031 312c 2d32 3431 2e30  1.0822011,-241.0
-00002b90: 3832 3836 2c31 322e 3430 3636 3036 2922  8286,12.406606)"
-00002ba0: 0d0a 2020 2020 2020 2073 7479 6c65 3d22  ..       style="
-00002bb0: 6f70 6163 6974 793a 302e 3735 3b66 696c  opacity:0.75;fil
-00002bc0: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
-00002bd0: 7061 6369 7479 3a31 223e 0d0a 2020 2020  pacity:1">..    
-00002be0: 2020 3c74 6578 740d 0a20 2020 2020 2020    <text..       
-00002bf0: 2020 736f 6469 706f 6469 3a6c 696e 6573    sodipodi:lines
-00002c00: 7061 6369 6e67 3d22 3132 3525 220d 0a20  pacing="125%".. 
-00002c10: 2020 2020 2020 2020 6964 3d22 7465 7874          id="text
-00002c20: 3338 3033 220d 0a20 2020 2020 2020 2020  3803"..         
-00002c30: 793d 2239 3636 2e39 3839 3522 0d0a 2020  y="966.9895"..  
-00002c40: 2020 2020 2020 2078 3d22 3430 312e 3030         x="401.00
-00002c50: 3731 3722 0d0a 2020 2020 2020 2020 2073  717"..         s
-00002c60: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00002c70: 3230 2e30 3434 3535 3536 3670 783b 666f  20.04455566px;fo
-00002c80: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
-00002c90: 666f 6e74 2d77 6569 6768 743a 6e6f 726d  font-weight:norm
-00002ca0: 616c 3b6c 696e 652d 6865 6967 6874 3a31  al;line-height:1
-00002cb0: 3235 253b 6c65 7474 6572 2d73 7061 6369  25%;letter-spaci
-00002cc0: 6e67 3a30 7078 3b77 6f72 642d 7370 6163  ng:0px;word-spac
-00002cd0: 696e 673a 3070 783b 6669 6c6c 3a23 3030  ing:0px;fill:#00
-00002ce0: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
-00002cf0: 793a 313b 7374 726f 6b65 3a6e 6f6e 653b  y:1;stroke:none;
-00002d00: 666f 6e74 2d66 616d 696c 793a 5361 6e73  font-family:Sans
-00002d10: 220d 0a20 2020 2020 2020 2020 786d 6c3a  "..         xml:
-00002d20: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
-00002d30: 3e3c 7473 7061 6e0d 0a20 2020 2020 2020  ><tspan..       
-00002d40: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
-00002d50: 7369 7a65 3a31 3670 783b 666f 6e74 2d73  size:16px;font-s
-00002d60: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
-00002d70: 2d76 6172 6961 6e74 3a6e 6f72 6d61 6c3b  -variant:normal;
-00002d80: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
-00002d90: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
-00002da0: 726d 616c 3b66 696c 6c3a 2330 3030 3030  rmal;fill:#00000
-00002db0: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
-00002dc0: 3b66 6f6e 742d 6661 6d69 6c79 3a54 6558  ;font-family:TeX
-00002dd0: 2047 7972 6520 4375 7273 6f72 3b2d 696e   Gyre Cursor;-in
-00002de0: 6b73 6361 7065 2d66 6f6e 742d 7370 6563  kscape-font-spec
-00002df0: 6966 6963 6174 696f 6e3a 5465 5820 4779  ification:TeX Gy
-00002e00: 7265 2043 7572 736f 7220 426f 6c64 220d  re Cursor Bold".
-00002e10: 0a20 2020 2020 2020 2020 2020 793d 2239  .           y="9
-00002e20: 3636 2e39 3839 3522 0d0a 2020 2020 2020  66.9895"..      
-00002e30: 2020 2020 2078 3d22 3430 312e 3030 3731       x="401.0071
-00002e40: 3722 0d0a 2020 2020 2020 2020 2020 2069  7"..           i
-00002e50: 643d 2274 7370 616e 3338 3035 220d 0a20  d="tspan3805".. 
-00002e60: 2020 2020 2020 2020 2020 736f 6469 706f            sodipo
-00002e70: 6469 3a72 6f6c 653d 226c 696e 6522 3e41  di:role="line">A
-00002e80: 2042 2043 3c2f 7473 7061 6e3e 3c74 7370   B C</tspan><tsp
-00002e90: 616e 0d0a 2020 2020 2020 2020 2020 2073  an..           s
-00002ea0: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00002eb0: 3136 7078 3b66 6f6e 742d 7374 796c 653a  16px;font-style:
-00002ec0: 6e6f 726d 616c 3b66 6f6e 742d 7661 7269  normal;font-vari
-00002ed0: 616e 743a 6e6f 726d 616c 3b66 6f6e 742d  ant:normal;font-
-00002ee0: 7765 6967 6874 3a62 6f6c 643b 666f 6e74  weight:bold;font
-00002ef0: 2d73 7472 6574 6368 3a6e 6f72 6d61 6c3b  -stretch:normal;
-00002f00: 6669 6c6c 3a23 3030 3030 3030 3b66 696c  fill:#000000;fil
-00002f10: 6c2d 6f70 6163 6974 793a 313b 666f 6e74  l-opacity:1;font
-00002f20: 2d66 616d 696c 793a 5465 5820 4779 7265  -family:TeX Gyre
-00002f30: 2043 7572 736f 723b 2d69 6e6b 7363 6170   Cursor;-inkscap
-00002f40: 652d 666f 6e74 2d73 7065 6369 6669 6361  e-font-specifica
-00002f50: 7469 6f6e 3a54 6558 2047 7972 6520 4375  tion:TeX Gyre Cu
-00002f60: 7273 6f72 2042 6f6c 6422 0d0a 2020 2020  rsor Bold"..    
-00002f70: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
-00002f80: 3338 3037 220d 0a20 2020 2020 2020 2020  3807"..         
-00002f90: 2020 793d 2239 3836 2e39 3839 3522 0d0a    y="986.9895"..
-00002fa0: 2020 2020 2020 2020 2020 2078 3d22 3430             x="40
-00002fb0: 312e 3030 3731 3722 0d0a 2020 2020 2020  1.00717"..      
-00002fc0: 2020 2020 2073 6f64 6970 6f64 693a 726f       sodipodi:ro
-00002fd0: 6c65 3d22 6c69 6e65 223e 3020 3020 313c  le="line">0 0 1<
-00002fe0: 2f74 7370 616e 3e3c 7473 7061 6e0d 0a20  /tspan><tspan.. 
-00002ff0: 2020 2020 2020 2020 2020 7374 796c 653d            style=
-00003000: 2266 6f6e 742d 7369 7a65 3a31 3670 783b  "font-size:16px;
-00003010: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
-00003020: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
-00003030: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
-00003040: 743a 626f 6c64 3b66 6f6e 742d 7374 7265  t:bold;font-stre
-00003050: 7463 683a 6e6f 726d 616c 3b66 696c 6c3a  tch:normal;fill:
-00003060: 2330 3030 3030 303b 6669 6c6c 2d6f 7061  #000000;fill-opa
-00003070: 6369 7479 3a31 3b66 6f6e 742d 6661 6d69  city:1;font-fami
-00003080: 6c79 3a54 6558 2047 7972 6520 4375 7273  ly:TeX Gyre Curs
-00003090: 6f72 3b2d 696e 6b73 6361 7065 2d66 6f6e  or;-inkscape-fon
-000030a0: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
-000030b0: 5465 5820 4779 7265 2043 7572 736f 7220  TeX Gyre Cursor 
-000030c0: 426f 6c64 220d 0a20 2020 2020 2020 2020  Bold"..         
-000030d0: 2020 6964 3d22 7473 7061 6e33 3830 3922    id="tspan3809"
-000030e0: 0d0a 2020 2020 2020 2020 2020 2079 3d22  ..           y="
-000030f0: 3130 3036 2e39 3839 3522 0d0a 2020 2020  1006.9895"..    
-00003100: 2020 2020 2020 2078 3d22 3430 312e 3030         x="401.00
-00003110: 3731 3722 0d0a 2020 2020 2020 2020 2020  717"..          
-00003120: 2073 6f64 6970 6f64 693a 726f 6c65 3d22   sodipodi:role="
-00003130: 6c69 6e65 223e 3120 3020 303c 2f74 7370  line">1 0 0</tsp
-00003140: 616e 3e3c 7473 7061 6e0d 0a20 2020 2020  an><tspan..     
-00003150: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
-00003160: 742d 7369 7a65 3a31 3670 783b 666f 6e74  t-size:16px;font
-00003170: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
-00003180: 6e74 2d76 6172 6961 6e74 3a6e 6f72 6d61  nt-variant:norma
-00003190: 6c3b 666f 6e74 2d77 6569 6768 743a 626f  l;font-weight:bo
-000031a0: 6c64 3b66 6f6e 742d 7374 7265 7463 683a  ld;font-stretch:
-000031b0: 6e6f 726d 616c 3b66 696c 6c3a 2330 3030  normal;fill:#000
-000031c0: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
-000031d0: 3a31 3b66 6f6e 742d 6661 6d69 6c79 3a54  :1;font-family:T
-000031e0: 6558 2047 7972 6520 4375 7273 6f72 3b2d  eX Gyre Cursor;-
-000031f0: 696e 6b73 6361 7065 2d66 6f6e 742d 7370  inkscape-font-sp
-00003200: 6563 6966 6963 6174 696f 6e3a 5465 5820  ecification:TeX 
-00003210: 4779 7265 2043 7572 736f 7220 426f 6c64  Gyre Cursor Bold
-00003220: 220d 0a20 2020 2020 2020 2020 2020 6964  "..           id
-00003230: 3d22 7473 7061 6e33 3831 3122 0d0a 2020  ="tspan3811"..  
-00003240: 2020 2020 2020 2020 2079 3d22 3130 3236           y="1026
-00003250: 2e39 3839 3522 0d0a 2020 2020 2020 2020  .9895"..        
-00003260: 2020 2078 3d22 3430 312e 3030 3731 3722     x="401.00717"
-00003270: 0d0a 2020 2020 2020 2020 2020 2073 6f64  ..           sod
-00003280: 6970 6f64 693a 726f 6c65 3d22 6c69 6e65  ipodi:role="line
-00003290: 223e 3020 3120 303c 2f74 7370 616e 3e3c  ">0 1 0</tspan><
-000032a0: 7473 7061 6e0d 0a20 2020 2020 2020 2020  tspan..         
-000032b0: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
-000032c0: 7a65 3a31 3670 783b 666f 6e74 2d73 7479  ze:16px;font-sty
-000032d0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
-000032e0: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
-000032f0: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
-00003300: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
-00003310: 616c 3b66 696c 6c3a 2330 3030 3030 303b  al;fill:#000000;
-00003320: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-00003330: 6f6e 742d 6661 6d69 6c79 3a54 6558 2047  ont-family:TeX G
-00003340: 7972 6520 4375 7273 6f72 3b2d 696e 6b73  yre Cursor;-inks
-00003350: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
-00003360: 6963 6174 696f 6e3a 5465 5820 4779 7265  ication:TeX Gyre
-00003370: 2043 7572 736f 7220 426f 6c64 220d 0a20   Cursor Bold".. 
-00003380: 2020 2020 2020 2020 2020 6964 3d22 7473            id="ts
-00003390: 7061 6e33 3831 3322 0d0a 2020 2020 2020  pan3813"..      
-000033a0: 2020 2020 2079 3d22 3130 3436 2e39 3839       y="1046.989
-000033b0: 3522 0d0a 2020 2020 2020 2020 2020 2078  5"..           x
-000033c0: 3d22 3430 312e 3030 3731 3722 0d0a 2020  ="401.00717"..  
-000033d0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-000033e0: 693a 726f 6c65 3d22 6c69 6e65 223e 3120  i:role="line">1 
-000033f0: 3120 313c 2f74 7370 616e 3e3c 2f74 6578  1 1</tspan></tex
-00003400: 743e 0d0a 2020 2020 2020 3c70 6174 680d  t>..      <path.
-00003410: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00003420: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00003430: 7661 7475 7265 3d22 3022 0d0a 2020 2020  vature="0"..    
-00003440: 2020 2020 2069 643d 2270 6174 6833 3831       id="path381
-00003450: 3722 0d0a 2020 2020 2020 2020 2064 3d22  7"..         d="
-00003460: 6d20 3339 362e 3936 3833 362c 3937 312e  m 396.96836,971.
-00003470: 3037 3932 3320 3535 2e31 3430 362c 3022  07923 55.1406,0"
-00003480: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
-00003490: 3d22 6669 6c6c 3a23 3030 3030 3030 3b66  ="fill:#000000;f
-000034a0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-000034b0: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-000034c0: 6f6b 652d 7769 6474 683a 302e 3930 3535  oke-width:0.9055
-000034d0: 3833 3938 7078 3b73 7472 6f6b 652d 6c69  8398px;stroke-li
-000034e0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-000034f0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00003500: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00003510: 3122 202f 3e0d 0a20 2020 203c 2f67 3e0d  1" />..    </g>.
-00003520: 0a20 2020 203c 7465 7874 0d0a 2020 2020  .    <text..    
-00003530: 2020 2073 6f64 6970 6f64 693a 6c69 6e65     sodipodi:line
-00003540: 7370 6163 696e 673d 2231 3235 2522 0d0a  spacing="125%"..
-00003550: 2020 2020 2020 2069 643d 2274 6578 7433         id="text3
-00003560: 3832 3822 0d0a 2020 2020 2020 2079 3d22  828"..       y="
-00003570: 3130 3434 2e33 3032 3722 0d0a 2020 2020  1044.3027"..    
-00003580: 2020 2078 3d22 3131 362e 3839 3637 3122     x="116.89671"
-00003590: 0d0a 2020 2020 2020 2073 7479 6c65 3d22  ..       style="
-000035a0: 666f 6e74 2d73 697a 653a 3338 2e31 3731  font-size:38.171
-000035b0: 3431 3334 3270 783b 666f 6e74 2d73 7479  41342px;font-sty
-000035c0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
-000035d0: 6569 6768 743a 6e6f 726d 616c 3b6c 696e  eight:normal;lin
-000035e0: 652d 6865 6967 6874 3a31 3235 253b 6c65  e-height:125%;le
-000035f0: 7474 6572 2d73 7061 6369 6e67 3a30 7078  tter-spacing:0px
-00003600: 3b77 6f72 642d 7370 6163 696e 673a 3070  ;word-spacing:0p
-00003610: 783b 6669 6c6c 3a23 3030 3030 3030 3b66  x;fill:#000000;f
-00003620: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00003630: 726f 6b65 3a6e 6f6e 653b 666f 6e74 2d66  roke:none;font-f
-00003640: 616d 696c 793a 5361 6e73 220d 0a20 2020  amily:Sans"..   
-00003650: 2020 2020 786d 6c3a 7370 6163 653d 2270      xml:space="p
-00003660: 7265 7365 7276 6522 3e3c 7473 7061 6e0d  reserve"><tspan.
-00003670: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00003680: 2266 6f6e 742d 7369 7a65 3a31 392e 3038  "font-size:19.08
-00003690: 3537 3036 3731 7078 3b66 6f6e 742d 7374  570671px;font-st
-000036a0: 796c 653a 6974 616c 6963 3b66 6f6e 742d  yle:italic;font-
-000036b0: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
-000036c0: 6f6e 742d 7765 6967 6874 3a6e 6f72 6d61  ont-weight:norma
-000036d0: 6c3b 666f 6e74 2d73 7472 6574 6368 3a6e  l;font-stretch:n
-000036e0: 6f72 6d61 6c3b 666f 6e74 2d66 616d 696c  ormal;font-famil
-000036f0: 793a 526f 626f 746f 3b2d 696e 6b73 6361  y:Roboto;-inksca
-00003700: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
-00003710: 6174 696f 6e3a 526f 626f 746f 2049 7461  ation:Roboto Ita
-00003720: 6c69 6322 0d0a 2020 2020 2020 2020 2079  lic"..         y
-00003730: 3d22 3130 3434 2e33 3032 3722 0d0a 2020  ="1044.3027"..  
-00003740: 2020 2020 2020 2078 3d22 3131 362e 3839         x="116.89
-00003750: 3637 3122 0d0a 2020 2020 2020 2020 2069  671"..         i
-00003760: 643d 2274 7370 616e 3338 3330 220d 0a20  d="tspan3830".. 
-00003770: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-00003780: 3a72 6f6c 653d 226c 696e 6522 3e44 6573  :role="line">Des
-00003790: 6967 6e20 6f66 2045 7870 6572 696d 656e  ign of Experimen
-000037a0: 7473 2066 6f72 2050 7974 686f 6e3c 2f74  ts for Python</t
-000037b0: 7370 616e 3e3c 2f74 6578 743e 0d0a 2020  span></text>..  
-000037c0: 3c2f 673e 0d0a 3c2f 7376 673e 0d0a       </g>..</svg>..
+00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
+00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
+00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
+00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
+00000070: 0a0a 3c73 7667 0a20 2020 786d 6c6e 733a  ..<svg.   xmlns:
+00000080: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
+00000090: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
+000000a0: 312e 312f 220a 2020 2078 6d6c 6e73 3a63  1.1/".   xmlns:c
+000000b0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
+000000c0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
+000000d0: 2322 0a20 2020 786d 6c6e 733a 7264 663d  #".   xmlns:rdf=
+000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000000f0: 7267 2f31 3939 392f 3032 2f32 322d 7264  rg/1999/02/22-rd
+00000100: 662d 7379 6e74 6178 2d6e 7323 220a 2020  f-syntax-ns#".  
+00000110: 2078 6d6c 6e73 3a73 7667 3d22 6874 7470   xmlns:svg="http
+00000120: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000130: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
+00000140: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+00000150: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
+00000160: 2078 6d6c 6e73 3a78 6c69 6e6b 3d22 6874   xmlns:xlink="ht
+00000170: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000180: 3139 3939 2f78 6c69 6e6b 220a 2020 2078  1999/xlink".   x
+00000190: 6d6c 6e73 3a73 6f64 6970 6f64 693d 2268  mlns:sodipodi="h
+000001a0: 7474 703a 2f2f 736f 6469 706f 6469 2e73  ttp://sodipodi.s
+000001b0: 6f75 7263 6566 6f72 6765 2e6e 6574 2f44  ourceforge.net/D
+000001c0: 5444 2f73 6f64 6970 6f64 692d 302e 6474  TD/sodipodi-0.dt
+000001d0: 6422 0a20 2020 786d 6c6e 733a 696e 6b73  d".   xmlns:inks
+000001e0: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
+000001f0: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
+00000200: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
+00000210: 6522 0a20 2020 7769 6474 683d 2235 3030  e".   width="500
+00000220: 220a 2020 2068 6569 6768 743d 2231 3030  ".   height="100
+00000230: 220a 2020 2069 643d 2273 7667 3222 0a20  ".   id="svg2". 
+00000240: 2020 7665 7273 696f 6e3d 2231 2e31 220a    version="1.1".
+00000250: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
+00000260: 696f 6e3d 2230 2e34 382e 3420 7239 3933  ion="0.48.4 r993
+00000270: 3922 0a20 2020 736f 6469 706f 6469 3a64  9".   sodipodi:d
+00000280: 6f63 6e61 6d65 3d22 4e65 7720 646f 6375  ocname="New docu
+00000290: 6d65 6e74 2031 223e 0a20 203c 6465 6673  ment 1">.  <defs
+000002a0: 0a20 2020 2020 6964 3d22 6465 6673 3422  .     id="defs4"
+000002b0: 3e0a 2020 2020 3c69 6e6b 7363 6170 653a  >.    <inkscape:
+000002c0: 7065 7273 7065 6374 6976 650a 2020 2020  perspective.    
+000002d0: 2020 2073 6f64 6970 6f64 693a 7479 7065     sodipodi:type
+000002e0: 3d22 696e 6b73 6361 7065 3a70 6572 7370  ="inkscape:persp
+000002f0: 3364 220a 2020 2020 2020 2069 6e6b 7363  3d".       inksc
+00000300: 6170 653a 7670 5f78 3d22 3020 3a20 3530  ape:vp_x="0 : 50
+00000310: 203a 2031 220a 2020 2020 2020 2069 6e6b   : 1".       ink
+00000320: 7363 6170 653a 7670 5f79 3d22 3020 3a20  scape:vp_y="0 : 
+00000330: 3130 3030 203a 2030 220a 2020 2020 2020  1000 : 0".      
+00000340: 2069 6e6b 7363 6170 653a 7670 5f7a 3d22   inkscape:vp_z="
+00000350: 3530 3020 3a20 3530 203a 2031 220a 2020  500 : 50 : 1".  
+00000360: 2020 2020 2069 6e6b 7363 6170 653a 7065       inkscape:pe
+00000370: 7273 7033 642d 6f72 6967 696e 3d22 3235  rsp3d-origin="25
+00000380: 3020 3a20 3333 2e33 3333 3333 3320 3a20  0 : 33.333333 : 
+00000390: 3122 0a20 2020 2020 2020 6964 3d22 7065  1".       id="pe
+000003a0: 7273 7065 6374 6976 6533 3833 3222 202f  rspective3832" /
+000003b0: 3e0a 2020 2020 3c6c 696e 6561 7247 7261  >.    <linearGra
+000003c0: 6469 656e 740a 2020 2020 2020 2069 643d  dient.       id=
+000003d0: 226c 696e 6561 7247 7261 6469 656e 7433  "linearGradient3
+000003e0: 3735 3522 3e0a 2020 2020 2020 3c73 746f  755">.      <sto
+000003f0: 700a 2020 2020 2020 2020 2073 7479 6c65  p.         style
+00000400: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6666  ="stop-color:#ff
+00000410: 6361 6361 3b73 746f 702d 6f70 6163 6974  caca;stop-opacit
+00000420: 793a 313b 220a 2020 2020 2020 2020 206f  y:1;".         o
+00000430: 6666 7365 743d 2230 220a 2020 2020 2020  ffset="0".      
+00000440: 2020 2069 643d 2273 746f 7033 3735 3722     id="stop3757"
+00000450: 202f 3e0a 2020 2020 2020 3c73 746f 700a   />.      <stop.
+00000460: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000470: 7374 6f70 2d63 6f6c 6f72 3a23 6664 3030  stop-color:#fd00
+00000480: 3030 3b73 746f 702d 6f70 6163 6974 793a  00;stop-opacity:
+00000490: 313b 220a 2020 2020 2020 2020 206f 6666  1;".         off
+000004a0: 7365 743d 2231 220a 2020 2020 2020 2020  set="1".        
+000004b0: 2069 643d 2273 746f 7033 3735 3922 202f   id="stop3759" /
+000004c0: 3e0a 2020 2020 3c2f 6c69 6e65 6172 4772  >.    </linearGr
+000004d0: 6164 6965 6e74 3e0a 2020 2020 3c72 6164  adient>.    <rad
+000004e0: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+000004f0: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000500: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000510: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000520: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000530: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000540: 7261 6469 616c 4772 6164 6965 6e74 3337  radialGradient37
+00000550: 3631 220a 2020 2020 2020 2063 783d 2234  61".       cx="4
+00000560: 362e 3533 3838 3322 0a20 2020 2020 2020  6.53883".       
+00000570: 6379 3d22 3333 2e32 3239 3332 3822 0a20  cy="33.229328". 
+00000580: 2020 2020 2020 6678 3d22 3436 2e35 3338        fx="46.538
+00000590: 3833 220a 2020 2020 2020 2066 793d 2233  83".       fy="3
+000005a0: 332e 3232 3933 3238 220a 2020 2020 2020  3.229328".      
+000005b0: 2072 3d22 362e 3435 3934 3735 3522 0a20   r="6.4594755". 
+000005c0: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
+000005d0: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
+000005e0: 5573 6522 202f 3e0a 2020 2020 3c72 6164  Use" />.    <rad
+000005f0: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000600: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000610: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000620: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000630: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000640: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000650: 7261 6469 616c 4772 6164 6965 6e74 3337  radialGradient37
+00000660: 3635 220a 2020 2020 2020 2067 7261 6469  65".       gradi
+00000670: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00000680: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+00000690: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+000006a0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+000006b0: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+000006c0: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+000006d0: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+000006e0: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+000006f0: 3735 3522 202f 3e0a 2020 2020 3c72 6164  755" />.    <rad
+00000700: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000710: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000720: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000730: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000740: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000750: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000760: 7261 6469 616c 4772 6164 6965 6e74 3337  radialGradient37
+00000770: 3639 220a 2020 2020 2020 2067 7261 6469  69".       gradi
+00000780: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00000790: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+000007a0: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+000007b0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+000007c0: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+000007d0: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+000007e0: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+000007f0: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+00000800: 3735 3522 202f 3e0a 2020 2020 3c72 6164  755" />.    <rad
+00000810: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000820: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000830: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000840: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000850: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000860: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000870: 7261 6469 616c 4772 6164 6965 6e74 3337  radialGradient37
+00000880: 3733 220a 2020 2020 2020 2067 7261 6469  73".       gradi
+00000890: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+000008a0: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+000008b0: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+000008c0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+000008d0: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+000008e0: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+000008f0: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+00000900: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+00000910: 3735 3522 202f 3e0a 2020 2020 3c72 6164  755" />.    <rad
+00000920: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000930: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000940: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000950: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000960: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000970: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000980: 7261 6469 616c 4772 6164 6965 6e74 3338  radialGradient38
+00000990: 3636 220a 2020 2020 2020 2067 7261 6469  66".       gradi
+000009a0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+000009b0: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+000009c0: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+000009d0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+000009e0: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+000009f0: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+00000a00: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+00000a10: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+00000a20: 3735 3522 202f 3e0a 2020 2020 3c72 6164  755" />.    <rad
+00000a30: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000a40: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000a50: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000a60: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000a70: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000a80: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000a90: 7261 6469 616c 4772 6164 6965 6e74 3338  radialGradient38
+00000aa0: 3638 220a 2020 2020 2020 2067 7261 6469  68".       gradi
+00000ab0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00000ac0: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+00000ad0: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+00000ae0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+00000af0: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+00000b00: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+00000b10: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+00000b20: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+00000b30: 3735 3522 202f 3e0a 2020 2020 3c72 6164  755" />.    <rad
+00000b40: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000b50: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000b60: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000b70: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000b80: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000b90: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000ba0: 7261 6469 616c 4772 6164 6965 6e74 3338  radialGradient38
+00000bb0: 3730 220a 2020 2020 2020 2067 7261 6469  70".       gradi
+00000bc0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00000bd0: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+00000be0: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+00000bf0: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+00000c00: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+00000c10: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+00000c20: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+00000c30: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+00000c40: 3735 3522 202f 3e0a 2020 2020 3c72 6164  755" />.    <rad
+00000c50: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+00000c60: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000c70: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000c80: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000c90: 236c 696e 6561 7247 7261 6469 656e 7433  #linearGradient3
+00000ca0: 3735 3522 0a20 2020 2020 2020 6964 3d22  755".       id="
+00000cb0: 7261 6469 616c 4772 6164 6965 6e74 3338  radialGradient38
+00000cc0: 3732 220a 2020 2020 2020 2067 7261 6469  72".       gradi
+00000cd0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00000ce0: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+00000cf0: 2063 783d 2234 362e 3533 3838 3322 0a20   cx="46.53883". 
+00000d00: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
+00000d10: 3332 3822 0a20 2020 2020 2020 6678 3d22  328".       fx="
+00000d20: 3436 2e35 3338 3833 220a 2020 2020 2020  46.53883".      
+00000d30: 2066 793d 2233 332e 3232 3933 3238 220a   fy="33.229328".
+00000d40: 2020 2020 2020 2072 3d22 362e 3435 3934         r="6.4594
+00000d50: 3735 3522 202f 3e0a 2020 3c2f 6465 6673  755" />.  </defs
+00000d60: 3e0a 2020 3c73 6f64 6970 6f64 693a 6e61  >.  <sodipodi:na
+00000d70: 6d65 6476 6965 770a 2020 2020 2069 643d  medview.     id=
+00000d80: 2262 6173 6522 0a20 2020 2020 7061 6765  "base".     page
+00000d90: 636f 6c6f 723d 2223 6666 6666 6666 220a  color="#ffffff".
+00000da0: 2020 2020 2062 6f72 6465 7263 6f6c 6f72       bordercolor
+00000db0: 3d22 2336 3636 3636 3622 0a20 2020 2020  ="#666666".     
+00000dc0: 626f 7264 6572 6f70 6163 6974 793d 2231  borderopacity="1
+00000dd0: 2e30 220a 2020 2020 2069 6e6b 7363 6170  .0".     inkscap
+00000de0: 653a 7061 6765 6f70 6163 6974 793d 2230  e:pageopacity="0
+00000df0: 2e30 220a 2020 2020 2069 6e6b 7363 6170  .0".     inkscap
+00000e00: 653a 7061 6765 7368 6164 6f77 3d22 3222  e:pageshadow="2"
+00000e10: 0a20 2020 2020 696e 6b73 6361 7065 3a7a  .     inkscape:z
+00000e20: 6f6f 6d3d 2232 2e32 3222 0a20 2020 2020  oom="2.22".     
+00000e30: 696e 6b73 6361 7065 3a63 783d 2232 3530  inkscape:cx="250
+00000e40: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000e50: 6379 3d22 3530 220a 2020 2020 2069 6e6b  cy="50".     ink
+00000e60: 7363 6170 653a 646f 6375 6d65 6e74 2d75  scape:document-u
+00000e70: 6e69 7473 3d22 7078 220a 2020 2020 2069  nits="px".     i
+00000e80: 6e6b 7363 6170 653a 6375 7272 656e 742d  nkscape:current-
+00000e90: 6c61 7965 723d 226c 6179 6572 3122 0a20  layer="layer1". 
+00000ea0: 2020 2020 7368 6f77 6772 6964 3d22 6661      showgrid="fa
+00000eb0: 6c73 6522 0a20 2020 2020 696e 6b73 6361  lse".     inksca
+00000ec0: 7065 3a77 696e 646f 772d 7769 6474 683d  pe:window-width=
+00000ed0: 2231 3537 3522 0a20 2020 2020 696e 6b73  "1575".     inks
+00000ee0: 6361 7065 3a77 696e 646f 772d 6865 6967  cape:window-heig
+00000ef0: 6874 3d22 3838 3022 0a20 2020 2020 696e  ht="880".     in
+00000f00: 6b73 6361 7065 3a77 696e 646f 772d 783d  kscape:window-x=
+00000f10: 2232 3322 0a20 2020 2020 696e 6b73 6361  "23".     inksca
+00000f20: 7065 3a77 696e 646f 772d 793d 222d 3322  pe:window-y="-3"
+00000f30: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
+00000f40: 696e 646f 772d 6d61 7869 6d69 7a65 643d  indow-maximized=
+00000f50: 2231 2220 2f3e 0a20 203c 6d65 7461 6461  "1" />.  <metada
+00000f60: 7461 0a20 2020 2020 6964 3d22 6d65 7461  ta.     id="meta
+00000f70: 6461 7461 3722 3e0a 2020 2020 3c72 6466  data7">.    <rdf
+00000f80: 3a52 4446 3e0a 2020 2020 2020 3c63 633a  :RDF>.      <cc:
+00000f90: 576f 726b 0a20 2020 2020 2020 2020 7264  Work.         rd
+00000fa0: 663a 6162 6f75 743d 2222 3e0a 2020 2020  f:about="">.    
+00000fb0: 2020 2020 3c64 633a 666f 726d 6174 3e69      <dc:format>i
+00000fc0: 6d61 6765 2f73 7667 2b78 6d6c 3c2f 6463  mage/svg+xml</dc
+00000fd0: 3a66 6f72 6d61 743e 0a20 2020 2020 2020  :format>.       
+00000fe0: 203c 6463 3a74 7970 650a 2020 2020 2020   <dc:type.      
+00000ff0: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
+00001000: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
+00001010: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
+00001020: 7469 6c6c 496d 6167 6522 202f 3e0a 2020  tillImage" />.  
+00001030: 2020 2020 2020 3c64 633a 7469 746c 653e        <dc:title>
+00001040: 3c2f 6463 3a74 6974 6c65 3e0a 2020 2020  </dc:title>.    
+00001050: 2020 3c2f 6363 3a57 6f72 6b3e 0a20 2020    </cc:Work>.   
+00001060: 203c 2f72 6466 3a52 4446 3e0a 2020 3c2f   </rdf:RDF>.  </
+00001070: 6d65 7461 6461 7461 3e0a 2020 3c67 0a20  metadata>.  <g. 
+00001080: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
+00001090: 656c 3d22 4c61 7965 7220 3122 0a20 2020  el="Layer 1".   
+000010a0: 2020 696e 6b73 6361 7065 3a67 726f 7570    inkscape:group
+000010b0: 6d6f 6465 3d22 6c61 7965 7222 0a20 2020  mode="layer".   
+000010c0: 2020 6964 3d22 6c61 7965 7231 220a 2020    id="layer1".  
+000010d0: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+000010e0: 616e 736c 6174 6528 302c 2d39 3532 2e33  anslate(0,-952.3
+000010f0: 3632 3138 2922 3e0a 2020 2020 3c67 0a20  6218)">.    <g. 
+00001100: 2020 2020 2020 6964 3d22 6733 3834 3822        id="g3848"
+00001110: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
+00001120: 6d3d 2274 7261 6e73 6c61 7465 282d 3136  m="translate(-16
+00001130: 2c30 2922 3e0a 2020 2020 2020 3c70 6174  ,0)">.      <pat
+00001140: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00001150: 3d22 6f70 6163 6974 793a 302e 353b 6669  ="opacity:0.5;fi
+00001160: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
+00001170: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
+00001180: 6474 683a 3170 783b 7374 726f 6b65 2d6c  dth:1px;stroke-l
+00001190: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+000011a0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+000011b0: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
+000011c0: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+000011d0: 6d20 3732 2e39 3334 3937 382c 3937 322e  m 72.934978,972.
+000011e0: 3030 3336 3520 2d31 2e39 3737 3136 2c33  00365 -1.97716,3
+000011f0: 342e 3731 3030 3522 0a20 2020 2020 2020  4.71005".       
+00001200: 2020 6964 3d22 7061 7468 3337 3831 220a    id="path3781".
+00001210: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00001220: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001230: 6174 7572 653d 2230 2220 2f3e 0a20 2020  ature="0" />.   
+00001240: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00001250: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00001260: 6e73 6c61 7465 2830 2c39 3532 2e33 3632  nslate(0,952.362
+00001270: 3138 2922 0a20 2020 2020 2020 2020 643d  18)".         d=
+00001280: 226d 2035 322e 3434 3333 3835 2c33 352e  "m 52.443385,35.
+00001290: 3034 3137 3138 2063 2030 2c33 2e32 3931  041718 c 0,3.291
+000012a0: 3332 3720 2d32 2e36 3638 3134 382c 352e  327 -2.668148,5.
+000012b0: 3935 3934 3735 202d 352e 3935 3934 3735  959475 -5.959475
+000012c0: 2c35 2e39 3539 3437 3520 2d33 2e32 3931  ,5.959475 -3.291
+000012d0: 3332 382c 3020 2d35 2e39 3539 3437 362c  328,0 -5.959476,
+000012e0: 2d32 2e36 3638 3134 3820 2d35 2e39 3539  -2.668148 -5.959
+000012f0: 3437 362c 2d35 2e39 3539 3437 3520 302c  476,-5.959475 0,
+00001300: 2d33 2e32 3931 3332 3820 322e 3636 3831  -3.291328 2.6681
+00001310: 3438 2c2d 352e 3935 3934 3736 2035 2e39  48,-5.959476 5.9
+00001320: 3539 3437 362c 2d35 2e39 3539 3437 3620  59476,-5.959476 
+00001330: 332e 3239 3133 3237 2c30 2035 2e39 3539  3.291327,0 5.959
+00001340: 3437 352c 322e 3636 3831 3438 2035 2e39  475,2.668148 5.9
+00001350: 3539 3437 352c 352e 3935 3934 3736 207a  59475,5.959476 z
+00001360: 220a 2020 2020 2020 2020 2073 6f64 6970  ".         sodip
+00001370: 6f64 693a 7279 3d22 352e 3935 3934 3735  odi:ry="5.959475
+00001380: 3522 0a20 2020 2020 2020 2020 736f 6469  5".         sodi
+00001390: 706f 6469 3a72 783d 2235 2e39 3539 3437  podi:rx="5.95947
+000013a0: 3535 220a 2020 2020 2020 2020 2073 6f64  55".         sod
+000013b0: 6970 6f64 693a 6379 3d22 3335 2e30 3431  ipodi:cy="35.041
+000013c0: 3731 3822 0a20 2020 2020 2020 2020 736f  718".         so
+000013d0: 6469 706f 6469 3a63 783d 2234 362e 3438  dipodi:cx="46.48
+000013e0: 3339 3122 0a20 2020 2020 2020 2020 6964  391".         id
+000013f0: 3d22 7061 7468 3239 3835 220a 2020 2020  ="path2985".    
+00001400: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00001410: 3a75 726c 2823 7261 6469 616c 4772 6164  :url(#radialGrad
+00001420: 6965 6e74 3338 3636 293b 6669 6c6c 2d6f  ient3866);fill-o
+00001430: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00001440: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00001450: 6964 7468 3a31 3b73 7472 6f6b 652d 6c69  idth:1;stroke-li
+00001460: 6e65 6a6f 696e 3a72 6f75 6e64 3b73 7472  nejoin:round;str
+00001470: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00001480: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00001490: 313b 7374 726f 6b65 2d64 6173 6861 7272  1;stroke-dasharr
+000014a0: 6179 3a6e 6f6e 6522 0a20 2020 2020 2020  ay:none".       
+000014b0: 2020 736f 6469 706f 6469 3a74 7970 653d    sodipodi:type=
+000014c0: 2261 7263 2220 2f3e 0a20 2020 2020 203c  "arc" />.      <
+000014d0: 7061 7468 0a20 2020 2020 2020 2020 736f  path.         so
+000014e0: 6469 706f 6469 3a74 7970 653d 2261 7263  dipodi:type="arc
+000014f0: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+00001500: 3d22 6669 6c6c 3a75 726c 2823 7261 6469  ="fill:url(#radi
+00001510: 616c 4772 6164 6965 6e74 3338 3638 293b  alGradient3868);
+00001520: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00001530: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+00001540: 726f 6b65 2d77 6964 7468 3a31 3b73 7472  roke-width:1;str
+00001550: 6f6b 652d 6c69 6e65 6a6f 696e 3a72 6f75  oke-linejoin:rou
+00001560: 6e64 3b73 7472 6f6b 652d 6d69 7465 726c  nd;stroke-miterl
+00001570: 696d 6974 3a34 3b73 7472 6f6b 652d 6f70  imit:4;stroke-op
+00001580: 6163 6974 793a 313b 7374 726f 6b65 2d64  acity:1;stroke-d
+00001590: 6173 6861 7272 6179 3a6e 6f6e 6522 0a20  asharray:none". 
+000015a0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+000015b0: 3337 3633 220a 2020 2020 2020 2020 2073  3763".         s
+000015c0: 6f64 6970 6f64 693a 6378 3d22 3436 2e34  odipodi:cx="46.4
+000015d0: 3833 3931 220a 2020 2020 2020 2020 2073  8391".         s
+000015e0: 6f64 6970 6f64 693a 6379 3d22 3335 2e30  odipodi:cy="35.0
+000015f0: 3431 3731 3822 0a20 2020 2020 2020 2020  41718".         
+00001600: 736f 6469 706f 6469 3a72 783d 2235 2e39  sodipodi:rx="5.9
+00001610: 3539 3437 3535 220a 2020 2020 2020 2020  594755".        
+00001620: 2073 6f64 6970 6f64 693a 7279 3d22 352e   sodipodi:ry="5.
+00001630: 3935 3934 3735 3522 0a20 2020 2020 2020  9594755".       
+00001640: 2020 643d 226d 2035 322e 3434 3333 3835    d="m 52.443385
+00001650: 2c33 352e 3034 3137 3138 2063 2030 2c33  ,35.041718 c 0,3
+00001660: 2e32 3931 3332 3720 2d32 2e36 3638 3134  .291327 -2.66814
+00001670: 382c 352e 3935 3934 3735 202d 352e 3935  8,5.959475 -5.95
+00001680: 3934 3735 2c35 2e39 3539 3437 3520 2d33  9475,5.959475 -3
+00001690: 2e32 3931 3332 382c 3020 2d35 2e39 3539  .291328,0 -5.959
+000016a0: 3437 362c 2d32 2e36 3638 3134 3820 2d35  476,-2.668148 -5
+000016b0: 2e39 3539 3437 362c 2d35 2e39 3539 3437  .959476,-5.95947
+000016c0: 3520 302c 2d33 2e32 3931 3332 3820 322e  5 0,-3.291328 2.
+000016d0: 3636 3831 3438 2c2d 352e 3935 3934 3736  668148,-5.959476
+000016e0: 2035 2e39 3539 3437 362c 2d35 2e39 3539   5.959476,-5.959
+000016f0: 3437 3620 332e 3239 3133 3237 2c30 2035  476 3.291327,0 5
+00001700: 2e39 3539 3437 352c 322e 3636 3831 3438  .959475,2.668148
+00001710: 2035 2e39 3539 3437 352c 352e 3935 3934   5.959475,5.9594
+00001720: 3736 207a 220a 2020 2020 2020 2020 2074  76 z".         t
+00001730: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00001740: 6174 6528 3736 2e30 3130 3534 352c 3934  ate(76.010545,94
+00001750: 322e 3033 3730 3529 2220 2f3e 0a20 2020  2.03705)" />.   
+00001760: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00001770: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00001780: 6e73 6c61 7465 2834 372e 3435 3136 372c  nslate(47.45167,
+00001790: 3939 362e 3738 3339 3729 220a 2020 2020  996.78397)".    
+000017a0: 2020 2020 2064 3d22 6d20 3532 2e34 3433       d="m 52.443
+000017b0: 3338 352c 3335 2e30 3431 3731 3820 6320  385,35.041718 c 
+000017c0: 302c 332e 3239 3133 3237 202d 322e 3636  0,3.291327 -2.66
+000017d0: 3831 3438 2c35 2e39 3539 3437 3520 2d35  8148,5.959475 -5
+000017e0: 2e39 3539 3437 352c 352e 3935 3934 3735  .959475,5.959475
+000017f0: 202d 332e 3239 3133 3238 2c30 202d 352e   -3.291328,0 -5.
+00001800: 3935 3934 3736 2c2d 322e 3636 3831 3438  959476,-2.668148
+00001810: 202d 352e 3935 3934 3736 2c2d 352e 3935   -5.959476,-5.95
+00001820: 3934 3735 2030 2c2d 332e 3239 3133 3238  9475 0,-3.291328
+00001830: 2032 2e36 3638 3134 382c 2d35 2e39 3539   2.668148,-5.959
+00001840: 3437 3620 352e 3935 3934 3736 2c2d 352e  476 5.959476,-5.
+00001850: 3935 3934 3736 2033 2e32 3931 3332 372c  959476 3.291327,
+00001860: 3020 352e 3935 3934 3735 2c32 2e36 3638  0 5.959475,2.668
+00001870: 3134 3820 352e 3935 3934 3735 2c35 2e39  148 5.959475,5.9
+00001880: 3539 3437 3620 7a22 0a20 2020 2020 2020  59476 z".       
+00001890: 2020 736f 6469 706f 6469 3a72 793d 2235    sodipodi:ry="5
+000018a0: 2e39 3539 3437 3535 220a 2020 2020 2020  .9594755".      
+000018b0: 2020 2073 6f64 6970 6f64 693a 7278 3d22     sodipodi:rx="
+000018c0: 352e 3935 3934 3735 3522 0a20 2020 2020  5.9594755".     
+000018d0: 2020 2020 736f 6469 706f 6469 3a63 793d      sodipodi:cy=
+000018e0: 2233 352e 3034 3137 3138 220a 2020 2020  "35.041718".    
+000018f0: 2020 2020 2073 6f64 6970 6f64 693a 6378       sodipodi:cx
+00001900: 3d22 3436 2e34 3833 3931 220a 2020 2020  ="46.48391".    
+00001910: 2020 2020 2069 643d 2270 6174 6833 3736       id="path376
+00001920: 3722 0a20 2020 2020 2020 2020 7374 796c  7".         styl
+00001930: 653d 2266 696c 6c3a 7572 6c28 2372 6164  e="fill:url(#rad
+00001940: 6961 6c47 7261 6469 656e 7433 3837 3029  ialGradient3870)
+00001950: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00001960: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+00001970: 7472 6f6b 652d 7769 6474 683a 313b 7374  troke-width:1;st
+00001980: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
+00001990: 756e 643b 7374 726f 6b65 2d6d 6974 6572  und;stroke-miter
+000019a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d6f  limit:4;stroke-o
+000019b0: 7061 6369 7479 3a31 3b73 7472 6f6b 652d  pacity:1;stroke-
+000019c0: 6461 7368 6172 7261 793a 6e6f 6e65 220a  dasharray:none".
+000019d0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+000019e0: 693a 7479 7065 3d22 6172 6322 202f 3e0a  i:type="arc" />.
+000019f0: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00001a00: 2020 2020 2073 6f64 6970 6f64 693a 7479       sodipodi:ty
+00001a10: 7065 3d22 6172 6322 0a20 2020 2020 2020  pe="arc".       
+00001a20: 2020 7374 796c 653d 226f 7061 6369 7479    style="opacity
+00001a30: 3a30 2e35 3b66 696c 6c3a 7572 6c28 2372  :0.5;fill:url(#r
+00001a40: 6164 6961 6c47 7261 6469 656e 7433 3837  adialGradient387
+00001a50: 3229 3b66 696c 6c2d 6f70 6163 6974 793a  2);fill-opacity:
+00001a60: 313b 7374 726f 6b65 3a23 3030 3030 3030  1;stroke:#000000
+00001a70: 3b73 7472 6f6b 652d 7769 6474 683a 313b  ;stroke-width:1;
+00001a80: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00001a90: 726f 756e 643b 7374 726f 6b65 2d6d 6974  round;stroke-mit
+00001aa0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00001ab0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00001ac0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00001ad0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00001ae0: 6174 6833 3737 3122 0a20 2020 2020 2020  ath3771".       
+00001af0: 2020 736f 6469 706f 6469 3a63 783d 2234    sodipodi:cx="4
+00001b00: 362e 3438 3339 3122 0a20 2020 2020 2020  6.48391".       
+00001b10: 2020 736f 6469 706f 6469 3a63 793d 2233    sodipodi:cy="3
+00001b20: 352e 3034 3137 3138 220a 2020 2020 2020  5.041718".      
+00001b30: 2020 2073 6f64 6970 6f64 693a 7278 3d22     sodipodi:rx="
+00001b40: 352e 3935 3934 3735 3522 0a20 2020 2020  5.9594755".     
+00001b50: 2020 2020 736f 6469 706f 6469 3a72 793d      sodipodi:ry=
+00001b60: 2235 2e39 3539 3437 3535 220a 2020 2020  "5.9594755".    
+00001b70: 2020 2020 2064 3d22 6d20 3532 2e34 3433       d="m 52.443
+00001b80: 3338 352c 3335 2e30 3431 3731 3820 6320  385,35.041718 c 
+00001b90: 302c 332e 3239 3133 3237 202d 322e 3636  0,3.291327 -2.66
+00001ba0: 3831 3438 2c35 2e39 3539 3437 3520 2d35  8148,5.959475 -5
+00001bb0: 2e39 3539 3437 352c 352e 3935 3934 3735  .959475,5.959475
+00001bc0: 202d 332e 3239 3133 3238 2c30 202d 352e   -3.291328,0 -5.
+00001bd0: 3935 3934 3736 2c2d 322e 3636 3831 3438  959476,-2.668148
+00001be0: 202d 352e 3935 3934 3736 2c2d 352e 3935   -5.959476,-5.95
+00001bf0: 3934 3735 2030 2c2d 332e 3239 3133 3238  9475 0,-3.291328
+00001c00: 2032 2e36 3638 3134 382c 2d35 2e39 3539   2.668148,-5.959
+00001c10: 3437 3620 352e 3935 3934 3736 2c2d 352e  476 5.959476,-5.
+00001c20: 3935 3934 3736 2033 2e32 3931 3332 372c  959476 3.291327,
+00001c30: 3020 352e 3935 3934 3735 2c32 2e36 3638  0 5.959475,2.668
+00001c40: 3134 3820 352e 3935 3934 3735 2c35 2e39  148 5.959475,5.9
+00001c50: 3539 3437 3620 7a22 0a20 2020 2020 2020  59476 z".       
+00001c60: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+00001c70: 6e73 6c61 7465 2832 332e 3934 3535 3139  nslate(23.945519
+00001c80: 2c39 3737 2e32 3332 3132 2922 202f 3e0a  ,977.23212)" />.
+00001c90: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00001ca0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00001cb0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+00001cc0: 653d 2230 220a 2020 2020 2020 2020 2069  e="0".         i
+00001cd0: 643d 2270 6174 6833 3737 3522 0a20 2020  d="path3775".   
+00001ce0: 2020 2020 2020 643d 224d 2034 352e 3931        d="M 45.91
+00001cf0: 3338 3834 2c39 3933 2e34 3836 3936 2034  3884,993.48696 4
+00001d00: 332e 3933 3637 3331 2c31 3032 382e 3139  3.936731,1028.19
+00001d10: 3722 0a20 2020 2020 2020 2020 7374 796c  7".         styl
+00001d20: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
+00001d30: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00001d40: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
+00001d50: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00001d60: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00001d70: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+00001d80: 6163 6974 793a 3122 202f 3e0a 2020 2020  acity:1" />.    
+00001d90: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00001da0: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
+00001db0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
+00001dc0: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
+00001dd0: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
+00001de0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00001df0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00001e00: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00001e10: 2020 2020 2020 2064 3d22 6d20 3936 2e32         d="m 96.2
+00001e20: 3231 3434 312c 3939 312e 3535 3535 202d  21441,991.5555 -
+00001e30: 312e 3937 3731 3533 2c33 342e 3731 220a  1.977153,34.71".
+00001e40: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00001e50: 6833 3737 3722 0a20 2020 2020 2020 2020  h3777".         
+00001e60: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00001e70: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00001e80: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00001e90: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00001ea0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001eb0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+00001ec0: 2020 2069 643d 2270 6174 6833 3737 3922     id="path3779"
+00001ed0: 0a20 2020 2020 2020 2020 643d 226d 2031  .         d="m 1
+00001ee0: 3232 2e33 3633 382c 3938 332e 3338 3135  22.3638,983.3815
+00001ef0: 3120 2d31 2e39 3737 3136 2c33 342e 3730  1 -1.97716,34.70
+00001f00: 3939 3922 0a20 2020 2020 2020 2020 7374  999".         st
+00001f10: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
+00001f20: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+00001f30: 726f 6b65 2d77 6964 7468 3a31 7078 3b73  roke-width:1px;s
+00001f40: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00001f50: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00001f60: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00001f70: 6f70 6163 6974 793a 3122 202f 3e0a 2020  opacity:1" />.  
+00001f80: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00001f90: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+00001fa0: 616e 736c 6174 6528 302c 3935 322e 3336  anslate(0,952.36
+00001fb0: 3231 3829 220a 2020 2020 2020 2020 2069  218)".         i
+00001fc0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00001fd0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+00001fe0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00001ff0: 6833 3738 3322 0a20 2020 2020 2020 2020  h3783".         
+00002000: 643d 226d 2034 342e 3135 3634 3135 2c37  d="m 44.156415,7
+00002010: 352e 3339 3534 3331 2034 332e 3439 3733  5.395431 43.4973
+00002020: 3634 2c33 2e39 3534 3330 3522 0a20 2020  64,3.954305".   
+00002030: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00002040: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
+00002050: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00002060: 7468 3a31 7078 3b73 7472 6f6b 652d 6c69  th:1px;stroke-li
+00002070: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00002080: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00002090: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+000020a0: 3122 202f 3e0a 2020 2020 2020 3c70 6174  1" />.      <pat
+000020b0: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+000020c0: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+000020d0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+000020e0: 652d 7769 6474 683a 3170 783b 7374 726f  e-width:1px;stro
+000020f0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00002100: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00002110: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+00002120: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00002130: 2064 3d22 6d20 3732 2e37 3135 3239 2c39   d="m 72.71529,9
+00002140: 3732 2e33 3937 3333 2034 332e 3439 3733  72.39733 43.4973
+00002150: 362c 332e 3935 3433 220a 2020 2020 2020  6,3.9543".      
+00002160: 2020 2069 643d 2270 6174 6833 3738 3522     id="path3785"
+00002170: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00002180: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00002190: 7661 7475 7265 3d22 3022 202f 3e0a 2020  vature="0" />.  
+000021a0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+000021b0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+000021c0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000021d0: 2230 220a 2020 2020 2020 2020 2069 643d  "0".         id=
+000021e0: 2270 6174 6833 3738 3722 0a20 2020 2020  "path3787".     
+000021f0: 2020 2020 643d 226d 2037 362e 3434 3939      d="m 76.4499
+00002200: 3132 2c31 3031 332e 3437 3832 2034 332e  12,1013.4782 43.
+00002210: 3439 3733 3538 2c33 2e39 3534 3322 0a20  497358,3.9543". 
+00002220: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00002230: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
+00002240: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00002250: 6964 7468 3a31 7078 3b73 7472 6f6b 652d  idth:1px;stroke-
+00002260: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00002270: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00002280: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
+00002290: 793a 3122 202f 3e0a 2020 2020 2020 3c70  y:1" />.      <p
+000022a0: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
+000022b0: 6c65 3d22 6669 6c6c 3a6e 6f6e 653b 7374  le="fill:none;st
+000022c0: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
+000022d0: 6f6b 652d 7769 6474 683a 3170 783b 7374  oke-width:1px;st
+000022e0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+000022f0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00002300: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00002310: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00002320: 2020 2064 3d22 6d20 3532 2e35 3034 3339     d="m 52.50439
+00002330: 342c 3938 372e 3939 3438 3720 3433 2e34  4,987.99487 43.4
+00002340: 3937 3336 342c 332e 3935 3433 220a 2020  97364,3.9543".  
+00002350: 2020 2020 2020 2069 643d 2270 6174 6833         id="path3
+00002360: 3738 3922 0a20 2020 2020 2020 2020 696e  789".         in
+00002370: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00002380: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00002390: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+000023a0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000023b0: 3d22 7472 616e 736c 6174 6528 302c 3935  ="translate(0,95
+000023c0: 322e 3336 3231 3829 220a 2020 2020 2020  2.36218)".      
+000023d0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+000023e0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000023f0: 2230 220a 2020 2020 2020 2020 2069 643d  "0".         id=
+00002400: 2270 6174 6833 3739 3122 0a20 2020 2020  "path3791".     
+00002410: 2020 2020 643d 224d 2034 342e 3135 3634      d="M 44.1564
+00002420: 3135 2c37 352e 3137 3537 3437 2036 352e  15,75.175747 65.
+00002430: 3436 3537 3239 2c36 332e 3533 3235 3133  465729,63.532513
+00002440: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+00002450: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+00002460: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+00002470: 652d 7769 6474 683a 3170 783b 7374 726f  e-width:1px;stro
+00002480: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00002490: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000024a0: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+000024b0: 6369 7479 3a31 2220 2f3e 0a20 2020 2020  city:1" />.     
+000024c0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+000024d0: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
+000024e0: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
+000024f0: 7374 726f 6b65 2d77 6964 7468 3a31 7078  stroke-width:1px
+00002500: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00002510: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00002520: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00002530: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00002540: 2020 2020 2020 643d 224d 2035 312e 3430        d="M 51.40
+00002550: 3539 3736 2c39 3834 2e30 3430 3536 2037  5976,984.04056 7
+00002560: 322e 3731 3532 392c 3937 322e 3339 3733  2.71529,972.3973
+00002570: 3322 0a20 2020 2020 2020 2020 6964 3d22  3".         id="
+00002580: 7061 7468 3337 3933 220a 2020 2020 2020  path3793".      
+00002590: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+000025a0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000025b0: 2230 2220 2f3e 0a20 2020 2020 203c 7061  "0" />.      <pa
+000025c0: 7468 0a20 2020 2020 2020 2020 696e 6b73  th.         inks
+000025d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+000025e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+000025f0: 2020 2020 2020 6964 3d22 7061 7468 3337        id="path37
+00002600: 3935 220a 2020 2020 2020 2020 2064 3d22  95".         d="
+00002610: 4d20 3936 2e32 3231 3434 322c 3939 322e  M 96.221442,992.
+00002620: 3136 3838 3620 3131 372e 3533 3037 362c  16886 117.53076,
+00002630: 3938 302e 3532 3536 3322 0a20 2020 2020  980.52563".     
+00002640: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00002650: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
+00002660: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00002670: 3a31 7078 3b73 7472 6f6b 652d 6c69 6e65  :1px;stroke-line
+00002680: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00002690: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+000026a0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+000026b0: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+000026c0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+000026d0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+000026e0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+000026f0: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
+00002700: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00002710: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00002720: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+00002730: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00002740: 3d22 6d20 3939 2e30 3737 3333 2c31 3032  ="m 99.07733,102
+00002750: 392e 3037 3537 2032 312e 3330 3933 322c  9.0757 21.30932,
+00002760: 2d31 312e 3634 3332 220a 2020 2020 2020  -11.6432".      
+00002770: 2020 2069 643d 2270 6174 6833 3739 3722     id="path3797"
+00002780: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00002790: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+000027a0: 7661 7475 7265 3d22 3022 202f 3e0a 2020  vature="0" />.  
+000027b0: 2020 3c2f 673e 0a20 2020 203c 7465 7874    </g>.    <text
+000027c0: 0a20 2020 2020 2020 786d 6c3a 7370 6163  .       xml:spac
+000027d0: 653d 2270 7265 7365 7276 6522 0a20 2020  e="preserve".   
+000027e0: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
+000027f0: 7369 7a65 3a34 3070 783b 666f 6e74 2d73  size:40px;font-s
+00002800: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
+00002810: 2d77 6569 6768 743a 6e6f 726d 616c 3b6c  -weight:normal;l
+00002820: 696e 652d 6865 6967 6874 3a31 3235 253b  ine-height:125%;
+00002830: 6c65 7474 6572 2d73 7061 6369 6e67 3a30  letter-spacing:0
+00002840: 7078 3b77 6f72 642d 7370 6163 696e 673a  px;word-spacing:
+00002850: 3070 783b 6669 6c6c 3a23 3030 3030 3030  0px;fill:#000000
+00002860: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00002870: 7374 726f 6b65 3a6e 6f6e 653b 666f 6e74  stroke:none;font
+00002880: 2d66 616d 696c 793a 5361 6e73 220a 2020  -family:Sans".  
+00002890: 2020 2020 2078 3d22 3135 382e 3938 3433       x="158.9843
+000028a0: 3822 0a20 2020 2020 2020 793d 2231 3031  8".       y="101
+000028b0: 302e 3631 3232 220a 2020 2020 2020 2069  0.6122".       i
+000028c0: 643d 2274 6578 7433 3739 3922 0a20 2020  d="text3799".   
+000028d0: 2020 2020 736f 6469 706f 6469 3a6c 696e      sodipodi:lin
+000028e0: 6573 7061 6369 6e67 3d22 3132 3525 223e  espacing="125%">
+000028f0: 3c74 7370 616e 0a20 2020 2020 2020 2020  <tspan.         
+00002900: 736f 6469 706f 6469 3a72 6f6c 653d 226c  sodipodi:role="l
+00002910: 696e 6522 0a20 2020 2020 2020 2020 6964  ine".         id
+00002920: 3d22 7473 7061 6e33 3830 3122 0a20 2020  ="tspan3801".   
+00002930: 2020 2020 2020 783d 2231 3538 2e39 3834        x="158.984
+00002940: 3338 220a 2020 2020 2020 2020 2079 3d22  38".         y="
+00002950: 3130 3130 2e36 3132 3222 0a20 2020 2020  1010.6122".     
+00002960: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
+00002970: 7369 7a65 3a36 3470 783b 666f 6e74 2d73  size:64px;font-s
+00002980: 7479 6c65 3a69 7461 6c69 633b 666f 6e74  tyle:italic;font
+00002990: 2d76 6172 6961 6e74 3a6e 6f72 6d61 6c3b  -variant:normal;
+000029a0: 666f 6e74 2d77 6569 6768 743a 6e6f 726d  font-weight:norm
+000029b0: 616c 3b66 6f6e 742d 7374 7265 7463 683a  al;font-stretch:
+000029c0: 6e6f 726d 616c 3b66 6f6e 742d 6661 6d69  normal;font-fami
+000029d0: 6c79 3a52 6f62 6f74 6f3b 2d69 6e6b 7363  ly:Roboto;-inksc
+000029e0: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
+000029f0: 6361 7469 6f6e 3a52 6f62 6f74 6f20 4974  cation:Roboto It
+00002a00: 616c 6963 223e 7079 444f 4533 3c2f 7473  alic">pyDOE3</ts
+00002a10: 7061 6e3e 3c2f 7465 7874 3e0a 2020 2020  pan></text>.    
+00002a20: 3c67 0a20 2020 2020 2020 6964 3d22 6733  <g.       id="g3
+00002a30: 3831 3922 0a20 2020 2020 2020 7472 616e  819".       tran
+00002a40: 7366 6f72 6d3d 226d 6174 7269 7828 312e  sform="matrix(1.
+00002a50: 3038 3232 3031 312c 2d30 2e32 3139 3631  0822011,-0.21961
+00002a60: 3430 372c 302e 3231 3936 3134 3037 2c31  407,0.21961407,1
+00002a70: 2e30 3832 3230 3131 2c2d 3234 312e 3038  .0822011,-241.08
+00002a80: 3238 362c 3132 2e34 3036 3630 3629 220a  286,12.406606)".
+00002a90: 2020 2020 2020 2073 7479 6c65 3d22 6f70         style="op
+00002aa0: 6163 6974 793a 302e 3735 3b66 696c 6c3a  acity:0.75;fill:
+00002ab0: 2330 3030 3030 303b 6669 6c6c 2d6f 7061  #000000;fill-opa
+00002ac0: 6369 7479 3a31 223e 0a20 2020 2020 203c  city:1">.      <
+00002ad0: 7465 7874 0a20 2020 2020 2020 2020 736f  text.         so
+00002ae0: 6469 706f 6469 3a6c 696e 6573 7061 6369  dipodi:linespaci
+00002af0: 6e67 3d22 3132 3525 220a 2020 2020 2020  ng="125%".      
+00002b00: 2020 2069 643d 2274 6578 7433 3830 3322     id="text3803"
+00002b10: 0a20 2020 2020 2020 2020 793d 2239 3636  .         y="966
+00002b20: 2e39 3839 3522 0a20 2020 2020 2020 2020  .9895".         
+00002b30: 783d 2234 3031 2e30 3037 3137 220a 2020  x="401.00717".  
+00002b40: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
+00002b50: 6e74 2d73 697a 653a 3230 2e30 3434 3535  nt-size:20.04455
+00002b60: 3536 3670 783b 666f 6e74 2d73 7479 6c65  566px;font-style
+00002b70: 3a6e 6f72 6d61 6c3b 666f 6e74 2d77 6569  :normal;font-wei
+00002b80: 6768 743a 6e6f 726d 616c 3b6c 696e 652d  ght:normal;line-
+00002b90: 6865 6967 6874 3a31 3235 253b 6c65 7474  height:125%;lett
+00002ba0: 6572 2d73 7061 6369 6e67 3a30 7078 3b77  er-spacing:0px;w
+00002bb0: 6f72 642d 7370 6163 696e 673a 3070 783b  ord-spacing:0px;
+00002bc0: 6669 6c6c 3a23 3030 3030 3030 3b66 696c  fill:#000000;fil
+00002bd0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00002be0: 6b65 3a6e 6f6e 653b 666f 6e74 2d66 616d  ke:none;font-fam
+00002bf0: 696c 793a 5361 6e73 220a 2020 2020 2020  ily:Sans".      
+00002c00: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
+00002c10: 6573 6572 7665 223e 3c74 7370 616e 0a20  eserve"><tspan. 
+00002c20: 2020 2020 2020 2020 2020 7374 796c 653d            style=
+00002c30: 2266 6f6e 742d 7369 7a65 3a31 3670 783b  "font-size:16px;
+00002c40: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
+00002c50: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
+00002c60: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
+00002c70: 743a 626f 6c64 3b66 6f6e 742d 7374 7265  t:bold;font-stre
+00002c80: 7463 683a 6e6f 726d 616c 3b66 696c 6c3a  tch:normal;fill:
+00002c90: 2330 3030 3030 303b 6669 6c6c 2d6f 7061  #000000;fill-opa
+00002ca0: 6369 7479 3a31 3b66 6f6e 742d 6661 6d69  city:1;font-fami
+00002cb0: 6c79 3a54 6558 2047 7972 6520 4375 7273  ly:TeX Gyre Curs
+00002cc0: 6f72 3b2d 696e 6b73 6361 7065 2d66 6f6e  or;-inkscape-fon
+00002cd0: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
+00002ce0: 5465 5820 4779 7265 2043 7572 736f 7220  TeX Gyre Cursor 
+00002cf0: 426f 6c64 220a 2020 2020 2020 2020 2020  Bold".          
+00002d00: 2079 3d22 3936 362e 3938 3935 220a 2020   y="966.9895".  
+00002d10: 2020 2020 2020 2020 2078 3d22 3430 312e           x="401.
+00002d20: 3030 3731 3722 0a20 2020 2020 2020 2020  00717".         
+00002d30: 2020 6964 3d22 7473 7061 6e33 3830 3522    id="tspan3805"
+00002d40: 0a20 2020 2020 2020 2020 2020 736f 6469  .           sodi
+00002d50: 706f 6469 3a72 6f6c 653d 226c 696e 6522  podi:role="line"
+00002d60: 3e41 2042 2043 3c2f 7473 7061 6e3e 3c74  >A B C</tspan><t
+00002d70: 7370 616e 0a20 2020 2020 2020 2020 2020  span.           
+00002d80: 7374 796c 653d 2266 6f6e 742d 7369 7a65  style="font-size
+00002d90: 3a31 3670 783b 666f 6e74 2d73 7479 6c65  :16px;font-style
+00002da0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
+00002db0: 6961 6e74 3a6e 6f72 6d61 6c3b 666f 6e74  iant:normal;font
+00002dc0: 2d77 6569 6768 743a 626f 6c64 3b66 6f6e  -weight:bold;fon
+00002dd0: 742d 7374 7265 7463 683a 6e6f 726d 616c  t-stretch:normal
+00002de0: 3b66 696c 6c3a 2330 3030 3030 303b 6669  ;fill:#000000;fi
+00002df0: 6c6c 2d6f 7061 6369 7479 3a31 3b66 6f6e  ll-opacity:1;fon
+00002e00: 742d 6661 6d69 6c79 3a54 6558 2047 7972  t-family:TeX Gyr
+00002e10: 6520 4375 7273 6f72 3b2d 696e 6b73 6361  e Cursor;-inksca
+00002e20: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
+00002e30: 6174 696f 6e3a 5465 5820 4779 7265 2043  ation:TeX Gyre C
+00002e40: 7572 736f 7220 426f 6c64 220a 2020 2020  ursor Bold".    
+00002e50: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
+00002e60: 3338 3037 220a 2020 2020 2020 2020 2020  3807".          
+00002e70: 2079 3d22 3938 362e 3938 3935 220a 2020   y="986.9895".  
+00002e80: 2020 2020 2020 2020 2078 3d22 3430 312e           x="401.
+00002e90: 3030 3731 3722 0a20 2020 2020 2020 2020  00717".         
+00002ea0: 2020 736f 6469 706f 6469 3a72 6f6c 653d    sodipodi:role=
+00002eb0: 226c 696e 6522 3e30 2030 2031 3c2f 7473  "line">0 0 1</ts
+00002ec0: 7061 6e3e 3c74 7370 616e 0a20 2020 2020  pan><tspan.     
+00002ed0: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
+00002ee0: 742d 7369 7a65 3a31 3670 783b 666f 6e74  t-size:16px;font
+00002ef0: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
+00002f00: 6e74 2d76 6172 6961 6e74 3a6e 6f72 6d61  nt-variant:norma
+00002f10: 6c3b 666f 6e74 2d77 6569 6768 743a 626f  l;font-weight:bo
+00002f20: 6c64 3b66 6f6e 742d 7374 7265 7463 683a  ld;font-stretch:
+00002f30: 6e6f 726d 616c 3b66 696c 6c3a 2330 3030  normal;fill:#000
+00002f40: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
+00002f50: 3a31 3b66 6f6e 742d 6661 6d69 6c79 3a54  :1;font-family:T
+00002f60: 6558 2047 7972 6520 4375 7273 6f72 3b2d  eX Gyre Cursor;-
+00002f70: 696e 6b73 6361 7065 2d66 6f6e 742d 7370  inkscape-font-sp
+00002f80: 6563 6966 6963 6174 696f 6e3a 5465 5820  ecification:TeX 
+00002f90: 4779 7265 2043 7572 736f 7220 426f 6c64  Gyre Cursor Bold
+00002fa0: 220a 2020 2020 2020 2020 2020 2069 643d  ".           id=
+00002fb0: 2274 7370 616e 3338 3039 220a 2020 2020  "tspan3809".    
+00002fc0: 2020 2020 2020 2079 3d22 3130 3036 2e39         y="1006.9
+00002fd0: 3839 3522 0a20 2020 2020 2020 2020 2020  895".           
+00002fe0: 783d 2234 3031 2e30 3037 3137 220a 2020  x="401.00717".  
+00002ff0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00003000: 693a 726f 6c65 3d22 6c69 6e65 223e 3120  i:role="line">1 
+00003010: 3020 303c 2f74 7370 616e 3e3c 7473 7061  0 0</tspan><tspa
+00003020: 6e0a 2020 2020 2020 2020 2020 2073 7479  n.           sty
+00003030: 6c65 3d22 666f 6e74 2d73 697a 653a 3136  le="font-size:16
+00003040: 7078 3b66 6f6e 742d 7374 796c 653a 6e6f  px;font-style:no
+00003050: 726d 616c 3b66 6f6e 742d 7661 7269 616e  rmal;font-varian
+00003060: 743a 6e6f 726d 616c 3b66 6f6e 742d 7765  t:normal;font-we
+00003070: 6967 6874 3a62 6f6c 643b 666f 6e74 2d73  ight:bold;font-s
+00003080: 7472 6574 6368 3a6e 6f72 6d61 6c3b 6669  tretch:normal;fi
+00003090: 6c6c 3a23 3030 3030 3030 3b66 696c 6c2d  ll:#000000;fill-
+000030a0: 6f70 6163 6974 793a 313b 666f 6e74 2d66  opacity:1;font-f
+000030b0: 616d 696c 793a 5465 5820 4779 7265 2043  amily:TeX Gyre C
+000030c0: 7572 736f 723b 2d69 6e6b 7363 6170 652d  ursor;-inkscape-
+000030d0: 666f 6e74 2d73 7065 6369 6669 6361 7469  font-specificati
+000030e0: 6f6e 3a54 6558 2047 7972 6520 4375 7273  on:TeX Gyre Curs
+000030f0: 6f72 2042 6f6c 6422 0a20 2020 2020 2020  or Bold".       
+00003100: 2020 2020 6964 3d22 7473 7061 6e33 3831      id="tspan381
+00003110: 3122 0a20 2020 2020 2020 2020 2020 793d  1".           y=
+00003120: 2231 3032 362e 3938 3935 220a 2020 2020  "1026.9895".    
+00003130: 2020 2020 2020 2078 3d22 3430 312e 3030         x="401.00
+00003140: 3731 3722 0a20 2020 2020 2020 2020 2020  717".           
+00003150: 736f 6469 706f 6469 3a72 6f6c 653d 226c  sodipodi:role="l
+00003160: 696e 6522 3e30 2031 2030 3c2f 7473 7061  ine">0 1 0</tspa
+00003170: 6e3e 3c74 7370 616e 0a20 2020 2020 2020  n><tspan.       
+00003180: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
+00003190: 7369 7a65 3a31 3670 783b 666f 6e74 2d73  size:16px;font-s
+000031a0: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
+000031b0: 2d76 6172 6961 6e74 3a6e 6f72 6d61 6c3b  -variant:normal;
+000031c0: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+000031d0: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
+000031e0: 726d 616c 3b66 696c 6c3a 2330 3030 3030  rmal;fill:#00000
+000031f0: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
+00003200: 3b66 6f6e 742d 6661 6d69 6c79 3a54 6558  ;font-family:TeX
+00003210: 2047 7972 6520 4375 7273 6f72 3b2d 696e   Gyre Cursor;-in
+00003220: 6b73 6361 7065 2d66 6f6e 742d 7370 6563  kscape-font-spec
+00003230: 6966 6963 6174 696f 6e3a 5465 5820 4779  ification:TeX Gy
+00003240: 7265 2043 7572 736f 7220 426f 6c64 220a  re Cursor Bold".
+00003250: 2020 2020 2020 2020 2020 2069 643d 2274             id="t
+00003260: 7370 616e 3338 3133 220a 2020 2020 2020  span3813".      
+00003270: 2020 2020 2079 3d22 3130 3436 2e39 3839       y="1046.989
+00003280: 3522 0a20 2020 2020 2020 2020 2020 783d  5".           x=
+00003290: 2234 3031 2e30 3037 3137 220a 2020 2020  "401.00717".    
+000032a0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000032b0: 726f 6c65 3d22 6c69 6e65 223e 3120 3120  role="line">1 1 
+000032c0: 313c 2f74 7370 616e 3e3c 2f74 6578 743e  1</tspan></text>
+000032d0: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
+000032e0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+000032f0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00003300: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
+00003310: 6964 3d22 7061 7468 3338 3137 220a 2020  id="path3817".  
+00003320: 2020 2020 2020 2064 3d22 6d20 3339 362e         d="m 396.
+00003330: 3936 3833 362c 3937 312e 3037 3932 3320  96836,971.07923 
+00003340: 3535 2e31 3430 362c 3022 0a20 2020 2020  55.1406,0".     
+00003350: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00003360: 2330 3030 3030 303b 6669 6c6c 2d6f 7061  #000000;fill-opa
+00003370: 6369 7479 3a31 3b73 7472 6f6b 653a 2330  city:1;stroke:#0
+00003380: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00003390: 7468 3a30 2e39 3035 3538 3339 3870 783b  th:0.90558398px;
+000033a0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+000033b0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+000033c0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+000033d0: 2d6f 7061 6369 7479 3a31 2220 2f3e 0a20  -opacity:1" />. 
+000033e0: 2020 203c 2f67 3e0a 2020 2020 3c74 6578     </g>.    <tex
+000033f0: 740a 2020 2020 2020 2073 6f64 6970 6f64  t.       sodipod
+00003400: 693a 6c69 6e65 7370 6163 696e 673d 2231  i:linespacing="1
+00003410: 3235 2522 0a20 2020 2020 2020 6964 3d22  25%".       id="
+00003420: 7465 7874 3338 3238 220a 2020 2020 2020  text3828".      
+00003430: 2079 3d22 3130 3434 2e33 3032 3722 0a20   y="1044.3027". 
+00003440: 2020 2020 2020 783d 2231 3136 2e38 3936        x="116.896
+00003450: 3731 220a 2020 2020 2020 2073 7479 6c65  71".       style
+00003460: 3d22 666f 6e74 2d73 697a 653a 3338 2e31  ="font-size:38.1
+00003470: 3731 3431 3334 3270 783b 666f 6e74 2d73  7141342px;font-s
+00003480: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
+00003490: 2d77 6569 6768 743a 6e6f 726d 616c 3b6c  -weight:normal;l
+000034a0: 696e 652d 6865 6967 6874 3a31 3235 253b  ine-height:125%;
+000034b0: 6c65 7474 6572 2d73 7061 6369 6e67 3a30  letter-spacing:0
+000034c0: 7078 3b77 6f72 642d 7370 6163 696e 673a  px;word-spacing:
+000034d0: 3070 783b 6669 6c6c 3a23 3030 3030 3030  0px;fill:#000000
+000034e0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+000034f0: 7374 726f 6b65 3a6e 6f6e 653b 666f 6e74  stroke:none;font
+00003500: 2d66 616d 696c 793a 5361 6e73 220a 2020  -family:Sans".  
+00003510: 2020 2020 2078 6d6c 3a73 7061 6365 3d22       xml:space="
+00003520: 7072 6573 6572 7665 223e 3c74 7370 616e  preserve"><tspan
+00003530: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00003540: 2266 6f6e 742d 7369 7a65 3a31 392e 3038  "font-size:19.08
+00003550: 3537 3036 3731 7078 3b66 6f6e 742d 7374  570671px;font-st
+00003560: 796c 653a 6974 616c 6963 3b66 6f6e 742d  yle:italic;font-
+00003570: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
+00003580: 6f6e 742d 7765 6967 6874 3a6e 6f72 6d61  ont-weight:norma
+00003590: 6c3b 666f 6e74 2d73 7472 6574 6368 3a6e  l;font-stretch:n
+000035a0: 6f72 6d61 6c3b 666f 6e74 2d66 616d 696c  ormal;font-famil
+000035b0: 793a 526f 626f 746f 3b2d 696e 6b73 6361  y:Roboto;-inksca
+000035c0: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
+000035d0: 6174 696f 6e3a 526f 626f 746f 2049 7461  ation:Roboto Ita
+000035e0: 6c69 6322 0a20 2020 2020 2020 2020 793d  lic".         y=
+000035f0: 2231 3034 342e 3330 3237 220a 2020 2020  "1044.3027".    
+00003600: 2020 2020 2078 3d22 3131 362e 3839 3637       x="116.8967
+00003610: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
+00003620: 7473 7061 6e33 3833 3022 0a20 2020 2020  tspan3830".     
+00003630: 2020 2020 736f 6469 706f 6469 3a72 6f6c      sodipodi:rol
+00003640: 653d 226c 696e 6522 3e44 6573 6967 6e20  e="line">Design 
+00003650: 6f66 2045 7870 6572 696d 656e 7473 2066  of Experiments f
+00003660: 6f72 2050 7974 686f 6e3c 2f74 7370 616e  or Python</tspan
+00003670: 3e3c 2f74 6578 743e 0a20 203c 2f67 3e0a  ></text>.  </g>.
+00003680: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `pydoe3-1.0.0/doc/_build/html/_static/favicon.ico` & `pydoe3-1.0.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pydoe3-1.0.0/doc/_build/html/_static/logo.png` & `pydoe3-1.0.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pydoe3-1.0.0/doc/_build/html/_static/logo.svg` & `pydoe3-1.0.1/doc/_static/logo.svg`

 * *Files 14% similar despite different names*

```diff
@@ -1,931 +1,912 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
-00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
-00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
-00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
-00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 786d  >....<svg..   xm
-00000080: 6c6e 733a 6463 3d22 6874 7470 3a2f 2f70  lns:dc="http://p
-00000090: 7572 6c2e 6f72 672f 6463 2f65 6c65 6d65  url.org/dc/eleme
-000000a0: 6e74 732f 312e 312f 220d 0a20 2020 786d  nts/1.1/"..   xm
-000000b0: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
-000000c0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-000000d0: 7267 2f6e 7323 220d 0a20 2020 786d 6c6e  rg/ns#"..   xmln
-000000e0: 733a 7264 663d 2268 7474 703a 2f2f 7777  s:rdf="http://ww
-000000f0: 772e 7733 2e6f 7267 2f31 3939 392f 3032  w.w3.org/1999/02
-00000100: 2f32 322d 7264 662d 7379 6e74 6178 2d6e  /22-rdf-syntax-n
-00000110: 7323 220d 0a20 2020 786d 6c6e 733a 7376  s#"..   xmlns:sv
-00000120: 673d 2268 7474 703a 2f2f 7777 772e 7733  g="http://www.w3
-00000130: 2e6f 7267 2f32 3030 302f 7376 6722 0d0a  .org/2000/svg"..
-00000140: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
-00000150: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000160: 2f73 7667 220d 0a20 2020 786d 6c6e 733a  /svg"..   xmlns:
-00000170: 786c 696e 6b3d 2268 7474 703a 2f2f 7777  xlink="http://ww
-00000180: 772e 7733 2e6f 7267 2f31 3939 392f 786c  w.w3.org/1999/xl
-00000190: 696e 6b22 0d0a 2020 2078 6d6c 6e73 3a73  ink"..   xmlns:s
-000001a0: 6f64 6970 6f64 693d 2268 7474 703a 2f2f  odipodi="http://
-000001b0: 736f 6469 706f 6469 2e73 6f75 7263 6566  sodipodi.sourcef
-000001c0: 6f72 6765 2e6e 6574 2f44 5444 2f73 6f64  orge.net/DTD/sod
-000001d0: 6970 6f64 692d 302e 6474 6422 0d0a 2020  ipodi-0.dtd"..  
-000001e0: 2078 6d6c 6e73 3a69 6e6b 7363 6170 653d   xmlns:inkscape=
-000001f0: 2268 7474 703a 2f2f 7777 772e 696e 6b73  "http://www.inks
-00000200: 6361 7065 2e6f 7267 2f6e 616d 6573 7061  cape.org/namespa
-00000210: 6365 732f 696e 6b73 6361 7065 220d 0a20  ces/inkscape".. 
-00000220: 2020 7769 6474 683d 2235 3030 220d 0a20    width="500".. 
-00000230: 2020 6865 6967 6874 3d22 3130 3022 0d0a    height="100"..
-00000240: 2020 2069 643d 2273 7667 3222 0d0a 2020     id="svg2"..  
-00000250: 2076 6572 7369 6f6e 3d22 312e 3122 0d0a   version="1.1"..
-00000260: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
-00000270: 696f 6e3d 2230 2e34 382e 3420 7239 3933  ion="0.48.4 r993
-00000280: 3922 0d0a 2020 2073 6f64 6970 6f64 693a  9"..   sodipodi:
-00000290: 646f 636e 616d 653d 2264 7261 7769 6e67  docname="drawing
-000002a0: 2e73 7667 220d 0a20 2020 696e 6b73 6361  .svg"..   inksca
-000002b0: 7065 3a65 7870 6f72 742d 6669 6c65 6e61  pe:export-filena
-000002c0: 6d65 3d22 2f6d 6564 6961 2f4c 696d 626f  me="/media/Limbo
-000002d0: 2f70 7974 686f 6e2f 7079 7468 6f6e 3237  /python/python27
-000002e0: 2f70 7944 4f45 2f64 6f63 2f5f 7374 6174  /pyDOE/doc/_stat
-000002f0: 6963 2f6c 6f67 6f2e 706e 6722 0d0a 2020  ic/logo.png"..  
-00000300: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00000310: 2d78 6470 693d 2239 3022 0d0a 2020 2069  -xdpi="90"..   i
-00000320: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-00000330: 6470 693d 2239 3022 3e0d 0a20 203c 6465  dpi="90">..  <de
-00000340: 6673 0d0a 2020 2020 2069 643d 2264 6566  fs..     id="def
-00000350: 7334 223e 0d0a 2020 2020 3c69 6e6b 7363  s4">..    <inksc
-00000360: 6170 653a 7065 7273 7065 6374 6976 650d  ape:perspective.
-00000370: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-00000380: 3a74 7970 653d 2269 6e6b 7363 6170 653a  :type="inkscape:
-00000390: 7065 7273 7033 6422 0d0a 2020 2020 2020  persp3d"..      
-000003a0: 2069 6e6b 7363 6170 653a 7670 5f78 3d22   inkscape:vp_x="
-000003b0: 3020 3a20 3530 203a 2031 220d 0a20 2020  0 : 50 : 1"..   
-000003c0: 2020 2020 696e 6b73 6361 7065 3a76 705f      inkscape:vp_
-000003d0: 793d 2230 203a 2031 3030 3020 3a20 3022  y="0 : 1000 : 0"
-000003e0: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
-000003f0: 653a 7670 5f7a 3d22 3530 3020 3a20 3530  e:vp_z="500 : 50
-00000400: 203a 2031 220d 0a20 2020 2020 2020 696e   : 1"..       in
-00000410: 6b73 6361 7065 3a70 6572 7370 3364 2d6f  kscape:persp3d-o
-00000420: 7269 6769 6e3d 2232 3530 203a 2033 332e  rigin="250 : 33.
-00000430: 3333 3333 3333 203a 2031 220d 0a20 2020  333333 : 1"..   
-00000440: 2020 2020 6964 3d22 7065 7273 7065 6374      id="perspect
-00000450: 6976 6533 3833 3222 202f 3e0d 0a20 2020  ive3832" />..   
-00000460: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
-00000470: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
-00000480: 6561 7247 7261 6469 656e 7433 3735 3522  earGradient3755"
-00000490: 3e0d 0a20 2020 2020 203c 7374 6f70 0d0a  >..      <stop..
-000004a0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-000004b0: 7374 6f70 2d63 6f6c 6f72 3a23 6666 6361  stop-color:#ffca
-000004c0: 6361 3b73 746f 702d 6f70 6163 6974 793a  ca;stop-opacity:
-000004d0: 313b 220d 0a20 2020 2020 2020 2020 6f66  1;"..         of
-000004e0: 6673 6574 3d22 3022 0d0a 2020 2020 2020  fset="0"..      
-000004f0: 2020 2069 643d 2273 746f 7033 3735 3722     id="stop3757"
-00000500: 202f 3e0d 0a20 2020 2020 203c 7374 6f70   />..      <stop
-00000510: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
-00000520: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6664  ="stop-color:#fd
-00000530: 3030 3030 3b73 746f 702d 6f70 6163 6974  0000;stop-opacit
-00000540: 793a 313b 220d 0a20 2020 2020 2020 2020  y:1;"..         
-00000550: 6f66 6673 6574 3d22 3122 0d0a 2020 2020  offset="1"..    
-00000560: 2020 2020 2069 643d 2273 746f 7033 3735       id="stop375
-00000570: 3922 202f 3e0d 0a20 2020 203c 2f6c 696e  9" />..    </lin
-00000580: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
-00000590: 2020 3c72 6164 6961 6c47 7261 6469 656e    <radialGradien
-000005a0: 740d 0a20 2020 2020 2020 696e 6b73 6361  t..       inksca
-000005b0: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
-000005c0: 7973 220d 0a20 2020 2020 2020 786c 696e  ys"..       xlin
-000005d0: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-000005e0: 7261 6469 656e 7433 3735 3522 0d0a 2020  radient3755"..  
-000005f0: 2020 2020 2069 643d 2272 6164 6961 6c47       id="radialG
-00000600: 7261 6469 656e 7433 3836 3622 0d0a 2020  radient3866"..  
-00000610: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
-00000620: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
-00000630: 7365 220d 0a20 2020 2020 2020 6378 3d22  se"..       cx="
-00000640: 3436 2e35 3338 3833 220d 0a20 2020 2020  46.53883"..     
-00000650: 2020 6379 3d22 3333 2e32 3239 3332 3822    cy="33.229328"
-00000660: 0d0a 2020 2020 2020 2066 783d 2234 362e  ..       fx="46.
-00000670: 3533 3838 3322 0d0a 2020 2020 2020 2066  53883"..       f
-00000680: 793d 2233 332e 3232 3933 3238 220d 0a20  y="33.229328".. 
-00000690: 2020 2020 2020 723d 2236 2e34 3539 3437        r="6.45947
-000006a0: 3535 2220 2f3e 0d0a 2020 2020 3c72 6164  55" />..    <rad
-000006b0: 6961 6c47 7261 6469 656e 740d 0a20 2020  ialGradient..   
-000006c0: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
-000006d0: 6c65 6374 3d22 616c 7761 7973 220d 0a20  lect="always".. 
-000006e0: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
-000006f0: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
-00000700: 7433 3735 3522 0d0a 2020 2020 2020 2069  t3755"..       i
-00000710: 643d 2272 6164 6961 6c47 7261 6469 656e  d="radialGradien
-00000720: 7433 3836 3822 0d0a 2020 2020 2020 2067  t3868"..       g
-00000730: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
-00000740: 6572 5370 6163 654f 6e55 7365 220d 0a20  erSpaceOnUse".. 
-00000750: 2020 2020 2020 6378 3d22 3436 2e35 3338        cx="46.538
-00000760: 3833 220d 0a20 2020 2020 2020 6379 3d22  83"..       cy="
-00000770: 3333 2e32 3239 3332 3822 0d0a 2020 2020  33.229328"..    
-00000780: 2020 2066 783d 2234 362e 3533 3838 3322     fx="46.53883"
-00000790: 0d0a 2020 2020 2020 2066 793d 2233 332e  ..       fy="33.
-000007a0: 3232 3933 3238 220d 0a20 2020 2020 2020  229328"..       
-000007b0: 723d 2236 2e34 3539 3437 3535 2220 2f3e  r="6.4594755" />
-000007c0: 0d0a 2020 2020 3c72 6164 6961 6c47 7261  ..    <radialGra
-000007d0: 6469 656e 740d 0a20 2020 2020 2020 696e  dient..       in
-000007e0: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
-000007f0: 616c 7761 7973 220d 0a20 2020 2020 2020  always"..       
-00000800: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
-00000810: 6561 7247 7261 6469 656e 7433 3735 3522  earGradient3755"
-00000820: 0d0a 2020 2020 2020 2069 643d 2272 6164  ..       id="rad
-00000830: 6961 6c47 7261 6469 656e 7433 3837 3022  ialGradient3870"
-00000840: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
-00000850: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
-00000860: 654f 6e55 7365 220d 0a20 2020 2020 2020  eOnUse"..       
-00000870: 6378 3d22 3436 2e35 3338 3833 220d 0a20  cx="46.53883".. 
-00000880: 2020 2020 2020 6379 3d22 3333 2e32 3239        cy="33.229
-00000890: 3332 3822 0d0a 2020 2020 2020 2066 783d  328"..       fx=
-000008a0: 2234 362e 3533 3838 3322 0d0a 2020 2020  "46.53883"..    
-000008b0: 2020 2066 793d 2233 332e 3232 3933 3238     fy="33.229328
-000008c0: 220d 0a20 2020 2020 2020 723d 2236 2e34  "..       r="6.4
-000008d0: 3539 3437 3535 2220 2f3e 0d0a 2020 2020  594755" />..    
-000008e0: 3c72 6164 6961 6c47 7261 6469 656e 740d  <radialGradient.
-000008f0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000900: 3a63 6f6c 6c65 6374 3d22 616c 7761 7973  :collect="always
-00000910: 220d 0a20 2020 2020 2020 786c 696e 6b3a  "..       xlink:
-00000920: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
-00000930: 6469 656e 7433 3735 3522 0d0a 2020 2020  dient3755"..    
-00000940: 2020 2069 643d 2272 6164 6961 6c47 7261     id="radialGra
-00000950: 6469 656e 7433 3837 3222 0d0a 2020 2020  dient3872"..    
-00000960: 2020 2067 7261 6469 656e 7455 6e69 7473     gradientUnits
-00000970: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
-00000980: 220d 0a20 2020 2020 2020 6378 3d22 3436  "..       cx="46
-00000990: 2e35 3338 3833 220d 0a20 2020 2020 2020  .53883"..       
-000009a0: 6379 3d22 3333 2e32 3239 3332 3822 0d0a  cy="33.229328"..
-000009b0: 2020 2020 2020 2066 783d 2234 362e 3533         fx="46.53
-000009c0: 3838 3322 0d0a 2020 2020 2020 2066 793d  883"..       fy=
-000009d0: 2233 332e 3232 3933 3238 220d 0a20 2020  "33.229328"..   
-000009e0: 2020 2020 723d 2236 2e34 3539 3437 3535      r="6.4594755
-000009f0: 2220 2f3e 0d0a 2020 3c2f 6465 6673 3e0d  " />..  </defs>.
-00000a00: 0a20 203c 736f 6469 706f 6469 3a6e 616d  .  <sodipodi:nam
-00000a10: 6564 7669 6577 0d0a 2020 2020 2069 643d  edview..     id=
-00000a20: 2262 6173 6522 0d0a 2020 2020 2070 6167  "base"..     pag
-00000a30: 6563 6f6c 6f72 3d22 2366 6666 6666 6622  ecolor="#ffffff"
-00000a40: 0d0a 2020 2020 2062 6f72 6465 7263 6f6c  ..     bordercol
-00000a50: 6f72 3d22 2336 3636 3636 3622 0d0a 2020  or="#666666"..  
-00000a60: 2020 2062 6f72 6465 726f 7061 6369 7479     borderopacity
-00000a70: 3d22 312e 3022 0d0a 2020 2020 2069 6e6b  ="1.0"..     ink
-00000a80: 7363 6170 653a 7061 6765 6f70 6163 6974  scape:pageopacit
-00000a90: 793d 2230 2e30 220d 0a20 2020 2020 696e  y="0.0"..     in
-00000aa0: 6b73 6361 7065 3a70 6167 6573 6861 646f  kscape:pageshado
-00000ab0: 773d 2232 220d 0a20 2020 2020 696e 6b73  w="2"..     inks
-00000ac0: 6361 7065 3a7a 6f6f 6d3d 2232 2e32 3222  cape:zoom="2.22"
-00000ad0: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
-00000ae0: 6378 3d22 3235 3022 0d0a 2020 2020 2069  cx="250"..     i
-00000af0: 6e6b 7363 6170 653a 6379 3d22 3530 220d  nkscape:cy="50".
-00000b00: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-00000b10: 6f63 756d 656e 742d 756e 6974 733d 2270  ocument-units="p
-00000b20: 7822 0d0a 2020 2020 2069 6e6b 7363 6170  x"..     inkscap
-00000b30: 653a 6375 7272 656e 742d 6c61 7965 723d  e:current-layer=
-00000b40: 226c 6179 6572 3122 0d0a 2020 2020 2073  "layer1"..     s
-00000b50: 686f 7767 7269 643d 2266 616c 7365 220d  howgrid="false".
-00000b60: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-00000b70: 696e 646f 772d 7769 6474 683d 2231 3537  indow-width="157
-00000b80: 3522 0d0a 2020 2020 2069 6e6b 7363 6170  5"..     inkscap
-00000b90: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
-00000ba0: 2238 3830 220d 0a20 2020 2020 696e 6b73  "880"..     inks
-00000bb0: 6361 7065 3a77 696e 646f 772d 783d 2232  cape:window-x="2
-00000bc0: 3322 0d0a 2020 2020 2069 6e6b 7363 6170  3"..     inkscap
-00000bd0: 653a 7769 6e64 6f77 2d79 3d22 2d33 220d  e:window-y="-3".
-00000be0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-00000bf0: 696e 646f 772d 6d61 7869 6d69 7a65 643d  indow-maximized=
-00000c00: 2231 2220 2f3e 0d0a 2020 3c6d 6574 6164  "1" />..  <metad
-00000c10: 6174 610d 0a20 2020 2020 6964 3d22 6d65  ata..     id="me
-00000c20: 7461 6461 7461 3722 3e0d 0a20 2020 203c  tadata7">..    <
-00000c30: 7264 663a 5244 463e 0d0a 2020 2020 2020  rdf:RDF>..      
-00000c40: 3c63 633a 576f 726b 0d0a 2020 2020 2020  <cc:Work..      
-00000c50: 2020 2072 6466 3a61 626f 7574 3d22 223e     rdf:about="">
-00000c60: 0d0a 2020 2020 2020 2020 3c64 633a 666f  ..        <dc:fo
-00000c70: 726d 6174 3e69 6d61 6765 2f73 7667 2b78  rmat>image/svg+x
-00000c80: 6d6c 3c2f 6463 3a66 6f72 6d61 743e 0d0a  ml</dc:format>..
-00000c90: 2020 2020 2020 2020 3c64 633a 7479 7065          <dc:type
-00000ca0: 0d0a 2020 2020 2020 2020 2020 2072 6466  ..           rdf
-00000cb0: 3a72 6573 6f75 7263 653d 2268 7474 703a  :resource="http:
-00000cc0: 2f2f 7075 726c 2e6f 7267 2f64 632f 6463  //purl.org/dc/dc
-00000cd0: 6d69 7479 7065 2f53 7469 6c6c 496d 6167  mitype/StillImag
-00000ce0: 6522 202f 3e0d 0a20 2020 2020 2020 203c  e" />..        <
-00000cf0: 6463 3a74 6974 6c65 3e3c 2f64 633a 7469  dc:title></dc:ti
-00000d00: 746c 653e 0d0a 2020 2020 2020 3c2f 6363  tle>..      </cc
-00000d10: 3a57 6f72 6b3e 0d0a 2020 2020 3c2f 7264  :Work>..    </rd
-00000d20: 663a 5244 463e 0d0a 2020 3c2f 6d65 7461  f:RDF>..  </meta
-00000d30: 6461 7461 3e0d 0a20 203c 670d 0a20 2020  data>..  <g..   
-00000d40: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00000d50: 3d22 4c61 7965 7220 3122 0d0a 2020 2020  ="Layer 1"..    
-00000d60: 2069 6e6b 7363 6170 653a 6772 6f75 706d   inkscape:groupm
-00000d70: 6f64 653d 226c 6179 6572 220d 0a20 2020  ode="layer"..   
-00000d80: 2020 6964 3d22 6c61 7965 7231 220d 0a20    id="layer1".. 
-00000d90: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-00000da0: 7261 6e73 6c61 7465 2830 2c2d 3935 322e  ranslate(0,-952.
-00000db0: 3336 3231 3829 223e 0d0a 2020 2020 3c67  36218)">..    <g
-00000dc0: 0d0a 2020 2020 2020 2069 643d 2267 3338  ..       id="g38
-00000dd0: 3438 220d 0a20 2020 2020 2020 7472 616e  48"..       tran
-00000de0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00000df0: 282d 3136 2c30 2922 3e0d 0a20 2020 2020  (-16,0)">..     
-00000e00: 203c 7061 7468 0d0a 2020 2020 2020 2020   <path..        
-00000e10: 2073 7479 6c65 3d22 6f70 6163 6974 793a   style="opacity:
-00000e20: 302e 353b 6669 6c6c 3a6e 6f6e 653b 7374  0.5;fill:none;st
-00000e30: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00000e40: 6f6b 652d 7769 6474 683a 3170 783b 7374  oke-width:1px;st
-00000e50: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00000e60: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00000e70: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
-00000e80: 7061 6369 7479 3a31 220d 0a20 2020 2020  pacity:1"..     
-00000e90: 2020 2020 643d 226d 2037 322e 3933 3439      d="m 72.9349
-00000ea0: 3738 2c39 3732 2e30 3033 3635 202d 312e  78,972.00365 -1.
-00000eb0: 3937 3731 362c 3334 2e37 3130 3035 220d  97716,34.71005".
-00000ec0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00000ed0: 7468 3337 3831 220d 0a20 2020 2020 2020  th3781"..       
-00000ee0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00000ef0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00000f00: 3022 202f 3e0d 0a20 2020 2020 203c 7061  0" />..      <pa
-00000f10: 7468 0d0a 2020 2020 2020 2020 2074 7261  th..         tra
-00000f20: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00000f30: 6528 302c 3935 322e 3336 3231 3829 220d  e(0,952.36218)".
-00000f40: 0a20 2020 2020 2020 2020 643d 226d 2035  .         d="m 5
-00000f50: 322e 3434 3333 3835 2c33 352e 3034 3137  2.443385,35.0417
-00000f60: 3138 2063 2030 2c33 2e32 3931 3332 3720  18 c 0,3.291327 
-00000f70: 2d32 2e36 3638 3134 382c 352e 3935 3934  -2.668148,5.9594
-00000f80: 3735 202d 352e 3935 3934 3735 2c35 2e39  75 -5.959475,5.9
-00000f90: 3539 3437 3520 2d33 2e32 3931 3332 382c  59475 -3.291328,
-00000fa0: 3020 2d35 2e39 3539 3437 362c 2d32 2e36  0 -5.959476,-2.6
-00000fb0: 3638 3134 3820 2d35 2e39 3539 3437 362c  68148 -5.959476,
-00000fc0: 2d35 2e39 3539 3437 3520 302c 2d33 2e32  -5.959475 0,-3.2
-00000fd0: 3931 3332 3820 322e 3636 3831 3438 2c2d  91328 2.668148,-
-00000fe0: 352e 3935 3934 3736 2035 2e39 3539 3437  5.959476 5.95947
-00000ff0: 362c 2d35 2e39 3539 3437 3620 332e 3239  6,-5.959476 3.29
-00001000: 3133 3237 2c30 2035 2e39 3539 3437 352c  1327,0 5.959475,
-00001010: 322e 3636 3831 3438 2035 2e39 3539 3437  2.668148 5.95947
-00001020: 352c 352e 3935 3934 3736 207a 220d 0a20  5,5.959476 z".. 
-00001030: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-00001040: 3a72 793d 2235 2e39 3539 3437 3535 220d  :ry="5.9594755".
-00001050: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-00001060: 6469 3a72 783d 2235 2e39 3539 3437 3535  di:rx="5.9594755
-00001070: 220d 0a20 2020 2020 2020 2020 736f 6469  "..         sodi
-00001080: 706f 6469 3a63 793d 2233 352e 3034 3137  podi:cy="35.0417
-00001090: 3138 220d 0a20 2020 2020 2020 2020 736f  18"..         so
-000010a0: 6469 706f 6469 3a63 783d 2234 362e 3438  dipodi:cx="46.48
-000010b0: 3339 3122 0d0a 2020 2020 2020 2020 2069  391"..         i
-000010c0: 643d 2270 6174 6832 3938 3522 0d0a 2020  d="path2985"..  
-000010d0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000010e0: 6c6c 3a75 726c 2823 7261 6469 616c 4772  ll:url(#radialGr
-000010f0: 6164 6965 6e74 3338 3636 293b 6669 6c6c  adient3866);fill
-00001100: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00001110: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00001120: 2d77 6964 7468 3a31 3b73 7472 6f6b 652d  -width:1;stroke-
-00001130: 6c69 6e65 6a6f 696e 3a72 6f75 6e64 3b73  linejoin:round;s
-00001140: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00001150: 3a34 3b73 7472 6f6b 652d 6f70 6163 6974  :4;stroke-opacit
-00001160: 793a 313b 7374 726f 6b65 2d64 6173 6861  y:1;stroke-dasha
-00001170: 7272 6179 3a6e 6f6e 6522 0d0a 2020 2020  rray:none"..    
-00001180: 2020 2020 2073 6f64 6970 6f64 693a 7479       sodipodi:ty
-00001190: 7065 3d22 6172 6322 202f 3e0d 0a20 2020  pe="arc" />..   
-000011a0: 2020 203c 7061 7468 0d0a 2020 2020 2020     <path..      
-000011b0: 2020 2073 6f64 6970 6f64 693a 7479 7065     sodipodi:type
-000011c0: 3d22 6172 6322 0d0a 2020 2020 2020 2020  ="arc"..        
-000011d0: 2073 7479 6c65 3d22 6669 6c6c 3a75 726c   style="fill:url
-000011e0: 2823 7261 6469 616c 4772 6164 6965 6e74  (#radialGradient
-000011f0: 3338 3638 293b 6669 6c6c 2d6f 7061 6369  3868);fill-opaci
-00001200: 7479 3a31 3b73 7472 6f6b 653a 2330 3030  ty:1;stroke:#000
-00001210: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-00001220: 3a31 3b73 7472 6f6b 652d 6c69 6e65 6a6f  :1;stroke-linejo
-00001230: 696e 3a72 6f75 6e64 3b73 7472 6f6b 652d  in:round;stroke-
-00001240: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00001250: 6f6b 652d 6f70 6163 6974 793a 313b 7374  oke-opacity:1;st
-00001260: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00001270: 6f6e 6522 0d0a 2020 2020 2020 2020 2069  one"..         i
-00001280: 643d 2270 6174 6833 3736 3322 0d0a 2020  d="path3763"..  
-00001290: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-000012a0: 6378 3d22 3436 2e34 3833 3931 220d 0a20  cx="46.48391".. 
-000012b0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-000012c0: 3a63 793d 2233 352e 3034 3137 3138 220d  :cy="35.041718".
-000012d0: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-000012e0: 6469 3a72 783d 2235 2e39 3539 3437 3535  di:rx="5.9594755
-000012f0: 220d 0a20 2020 2020 2020 2020 736f 6469  "..         sodi
-00001300: 706f 6469 3a72 793d 2235 2e39 3539 3437  podi:ry="5.95947
-00001310: 3535 220d 0a20 2020 2020 2020 2020 643d  55"..         d=
-00001320: 226d 2035 322e 3434 3333 3835 2c33 352e  "m 52.443385,35.
-00001330: 3034 3137 3138 2063 2030 2c33 2e32 3931  041718 c 0,3.291
-00001340: 3332 3720 2d32 2e36 3638 3134 382c 352e  327 -2.668148,5.
-00001350: 3935 3934 3735 202d 352e 3935 3934 3735  959475 -5.959475
-00001360: 2c35 2e39 3539 3437 3520 2d33 2e32 3931  ,5.959475 -3.291
-00001370: 3332 382c 3020 2d35 2e39 3539 3437 362c  328,0 -5.959476,
-00001380: 2d32 2e36 3638 3134 3820 2d35 2e39 3539  -2.668148 -5.959
-00001390: 3437 362c 2d35 2e39 3539 3437 3520 302c  476,-5.959475 0,
-000013a0: 2d33 2e32 3931 3332 3820 322e 3636 3831  -3.291328 2.6681
-000013b0: 3438 2c2d 352e 3935 3934 3736 2035 2e39  48,-5.959476 5.9
-000013c0: 3539 3437 362c 2d35 2e39 3539 3437 3620  59476,-5.959476 
-000013d0: 332e 3239 3133 3237 2c30 2035 2e39 3539  3.291327,0 5.959
-000013e0: 3437 352c 322e 3636 3831 3438 2035 2e39  475,2.668148 5.9
-000013f0: 3539 3437 352c 352e 3935 3934 3736 207a  59475,5.959476 z
-00001400: 220d 0a20 2020 2020 2020 2020 7472 616e  "..         tran
-00001410: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00001420: 2837 362e 3031 3035 3435 2c39 3432 2e30  (76.010545,942.0
-00001430: 3337 3035 2922 202f 3e0d 0a20 2020 2020  3705)" />..     
-00001440: 203c 7061 7468 0d0a 2020 2020 2020 2020   <path..        
-00001450: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-00001460: 736c 6174 6528 3437 2e34 3531 3637 2c39  slate(47.45167,9
-00001470: 3936 2e37 3833 3937 2922 0d0a 2020 2020  96.78397)"..    
-00001480: 2020 2020 2064 3d22 6d20 3532 2e34 3433       d="m 52.443
-00001490: 3338 352c 3335 2e30 3431 3731 3820 6320  385,35.041718 c 
-000014a0: 302c 332e 3239 3133 3237 202d 322e 3636  0,3.291327 -2.66
-000014b0: 3831 3438 2c35 2e39 3539 3437 3520 2d35  8148,5.959475 -5
-000014c0: 2e39 3539 3437 352c 352e 3935 3934 3735  .959475,5.959475
-000014d0: 202d 332e 3239 3133 3238 2c30 202d 352e   -3.291328,0 -5.
-000014e0: 3935 3934 3736 2c2d 322e 3636 3831 3438  959476,-2.668148
-000014f0: 202d 352e 3935 3934 3736 2c2d 352e 3935   -5.959476,-5.95
-00001500: 3934 3735 2030 2c2d 332e 3239 3133 3238  9475 0,-3.291328
-00001510: 2032 2e36 3638 3134 382c 2d35 2e39 3539   2.668148,-5.959
-00001520: 3437 3620 352e 3935 3934 3736 2c2d 352e  476 5.959476,-5.
-00001530: 3935 3934 3736 2033 2e32 3931 3332 372c  959476 3.291327,
-00001540: 3020 352e 3935 3934 3735 2c32 2e36 3638  0 5.959475,2.668
-00001550: 3134 3820 352e 3935 3934 3735 2c35 2e39  148 5.959475,5.9
-00001560: 3539 3437 3620 7a22 0d0a 2020 2020 2020  59476 z"..      
-00001570: 2020 2073 6f64 6970 6f64 693a 7279 3d22     sodipodi:ry="
-00001580: 352e 3935 3934 3735 3522 0d0a 2020 2020  5.9594755"..    
-00001590: 2020 2020 2073 6f64 6970 6f64 693a 7278       sodipodi:rx
-000015a0: 3d22 352e 3935 3934 3735 3522 0d0a 2020  ="5.9594755"..  
-000015b0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-000015c0: 6379 3d22 3335 2e30 3431 3731 3822 0d0a  cy="35.041718"..
-000015d0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-000015e0: 693a 6378 3d22 3436 2e34 3833 3931 220d  i:cx="46.48391".
-000015f0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00001600: 7468 3337 3637 220d 0a20 2020 2020 2020  th3767"..       
-00001610: 2020 7374 796c 653d 2266 696c 6c3a 7572    style="fill:ur
-00001620: 6c28 2372 6164 6961 6c47 7261 6469 656e  l(#radialGradien
-00001630: 7433 3837 3029 3b66 696c 6c2d 6f70 6163  t3870);fill-opac
-00001640: 6974 793a 313b 7374 726f 6b65 3a23 3030  ity:1;stroke:#00
-00001650: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-00001660: 683a 313b 7374 726f 6b65 2d6c 696e 656a  h:1;stroke-linej
-00001670: 6f69 6e3a 726f 756e 643b 7374 726f 6b65  oin:round;stroke
-00001680: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00001690: 726f 6b65 2d6f 7061 6369 7479 3a31 3b73  roke-opacity:1;s
-000016a0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-000016b0: 6e6f 6e65 220d 0a20 2020 2020 2020 2020  none"..         
-000016c0: 736f 6469 706f 6469 3a74 7970 653d 2261  sodipodi:type="a
-000016d0: 7263 2220 2f3e 0d0a 2020 2020 2020 3c70  rc" />..      <p
-000016e0: 6174 680d 0a20 2020 2020 2020 2020 736f  ath..         so
-000016f0: 6469 706f 6469 3a74 7970 653d 2261 7263  dipodi:type="arc
-00001700: 220d 0a20 2020 2020 2020 2020 7374 796c  "..         styl
-00001710: 653d 226f 7061 6369 7479 3a30 2e35 3b66  e="opacity:0.5;f
-00001720: 696c 6c3a 7572 6c28 2372 6164 6961 6c47  ill:url(#radialG
-00001730: 7261 6469 656e 7433 3837 3229 3b66 696c  radient3872);fil
-00001740: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00001750: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
-00001760: 652d 7769 6474 683a 313b 7374 726f 6b65  e-width:1;stroke
-00001770: 2d6c 696e 656a 6f69 6e3a 726f 756e 643b  -linejoin:round;
-00001780: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00001790: 743a 343b 7374 726f 6b65 2d6f 7061 6369  t:4;stroke-opaci
-000017a0: 7479 3a31 3b73 7472 6f6b 652d 6461 7368  ty:1;stroke-dash
-000017b0: 6172 7261 793a 6e6f 6e65 220d 0a20 2020  array:none"..   
-000017c0: 2020 2020 2020 6964 3d22 7061 7468 3337        id="path37
-000017d0: 3731 220d 0a20 2020 2020 2020 2020 736f  71"..         so
-000017e0: 6469 706f 6469 3a63 783d 2234 362e 3438  dipodi:cx="46.48
-000017f0: 3339 3122 0d0a 2020 2020 2020 2020 2073  391"..         s
-00001800: 6f64 6970 6f64 693a 6379 3d22 3335 2e30  odipodi:cy="35.0
-00001810: 3431 3731 3822 0d0a 2020 2020 2020 2020  41718"..        
-00001820: 2073 6f64 6970 6f64 693a 7278 3d22 352e   sodipodi:rx="5.
-00001830: 3935 3934 3735 3522 0d0a 2020 2020 2020  9594755"..      
-00001840: 2020 2073 6f64 6970 6f64 693a 7279 3d22     sodipodi:ry="
-00001850: 352e 3935 3934 3735 3522 0d0a 2020 2020  5.9594755"..    
-00001860: 2020 2020 2064 3d22 6d20 3532 2e34 3433       d="m 52.443
-00001870: 3338 352c 3335 2e30 3431 3731 3820 6320  385,35.041718 c 
-00001880: 302c 332e 3239 3133 3237 202d 322e 3636  0,3.291327 -2.66
-00001890: 3831 3438 2c35 2e39 3539 3437 3520 2d35  8148,5.959475 -5
-000018a0: 2e39 3539 3437 352c 352e 3935 3934 3735  .959475,5.959475
-000018b0: 202d 332e 3239 3133 3238 2c30 202d 352e   -3.291328,0 -5.
-000018c0: 3935 3934 3736 2c2d 322e 3636 3831 3438  959476,-2.668148
-000018d0: 202d 352e 3935 3934 3736 2c2d 352e 3935   -5.959476,-5.95
-000018e0: 3934 3735 2030 2c2d 332e 3239 3133 3238  9475 0,-3.291328
-000018f0: 2032 2e36 3638 3134 382c 2d35 2e39 3539   2.668148,-5.959
-00001900: 3437 3620 352e 3935 3934 3736 2c2d 352e  476 5.959476,-5.
-00001910: 3935 3934 3736 2033 2e32 3931 3332 372c  959476 3.291327,
-00001920: 3020 352e 3935 3934 3735 2c32 2e36 3638  0 5.959475,2.668
-00001930: 3134 3820 352e 3935 3934 3735 2c35 2e39  148 5.959475,5.9
-00001940: 3539 3437 3620 7a22 0d0a 2020 2020 2020  59476 z"..      
-00001950: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-00001960: 616e 736c 6174 6528 3233 2e39 3435 3531  anslate(23.94551
-00001970: 392c 3937 372e 3233 3231 3229 2220 2f3e  9,977.23212)" />
-00001980: 0d0a 2020 2020 2020 3c70 6174 680d 0a20  ..      <path.. 
-00001990: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000019a0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-000019b0: 7475 7265 3d22 3022 0d0a 2020 2020 2020  ture="0"..      
-000019c0: 2020 2069 643d 2270 6174 6833 3737 3522     id="path3775"
-000019d0: 0d0a 2020 2020 2020 2020 2064 3d22 4d20  ..         d="M 
-000019e0: 3435 2e39 3133 3838 342c 3939 332e 3438  45.913884,993.48
-000019f0: 3639 3620 3433 2e39 3336 3733 312c 3130  696 43.936731,10
-00001a00: 3238 2e31 3937 220d 0a20 2020 2020 2020  28.197"..       
-00001a10: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
-00001a20: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
-00001a30: 303b 7374 726f 6b65 2d77 6964 7468 3a31  0;stroke-width:1
-00001a40: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
-00001a50: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00001a60: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00001a70: 6f6b 652d 6f70 6163 6974 793a 3122 202f  oke-opacity:1" /
-00001a80: 3e0d 0a20 2020 2020 203c 7061 7468 0d0a  >..      <path..
-00001a90: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00001aa0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
-00001ab0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-00001ac0: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
-00001ad0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00001ae0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00001af0: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
-00001b00: 7479 3a31 220d 0a20 2020 2020 2020 2020  ty:1"..         
-00001b10: 643d 226d 2039 362e 3232 3134 3431 2c39  d="m 96.221441,9
-00001b20: 3931 2e35 3535 3520 2d31 2e39 3737 3135  91.5555 -1.97715
-00001b30: 332c 3334 2e37 3122 0d0a 2020 2020 2020  3,34.71"..      
-00001b40: 2020 2069 643d 2270 6174 6833 3737 3722     id="path3777"
-00001b50: 0d0a 2020 2020 2020 2020 2069 6e6b 7363  ..         inksc
-00001b60: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00001b70: 7276 6174 7572 653d 2230 2220 2f3e 0d0a  rvature="0" />..
-00001b80: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
-00001b90: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00001ba0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00001bb0: 7265 3d22 3022 0d0a 2020 2020 2020 2020  re="0"..        
-00001bc0: 2069 643d 2270 6174 6833 3737 3922 0d0a   id="path3779"..
-00001bd0: 2020 2020 2020 2020 2064 3d22 6d20 3132           d="m 12
-00001be0: 322e 3336 3338 2c39 3833 2e33 3831 3531  2.3638,983.38151
-00001bf0: 202d 312e 3937 3731 362c 3334 2e37 3039   -1.97716,34.709
-00001c00: 3939 220d 0a20 2020 2020 2020 2020 7374  99"..         st
-00001c10: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
-00001c20: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
-00001c30: 726f 6b65 2d77 6964 7468 3a31 7078 3b73  roke-width:1px;s
-00001c40: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00001c50: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00001c60: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00001c70: 6f70 6163 6974 793a 3122 202f 3e0d 0a20  opacity:1" />.. 
-00001c80: 2020 2020 203c 7061 7468 0d0a 2020 2020       <path..    
-00001c90: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
-00001ca0: 7472 616e 736c 6174 6528 302c 3935 322e  translate(0,952.
-00001cb0: 3336 3231 3829 220d 0a20 2020 2020 2020  36218)"..       
-00001cc0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00001cd0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00001ce0: 3022 0d0a 2020 2020 2020 2020 2069 643d  0"..         id=
-00001cf0: 2270 6174 6833 3738 3322 0d0a 2020 2020  "path3783"..    
-00001d00: 2020 2020 2064 3d22 6d20 3434 2e31 3536       d="m 44.156
-00001d10: 3431 352c 3735 2e33 3935 3433 3120 3433  415,75.395431 43
-00001d20: 2e34 3937 3336 342c 332e 3935 3433 3035  .497364,3.954305
-00001d30: 220d 0a20 2020 2020 2020 2020 7374 796c  "..         styl
-00001d40: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
-00001d50: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00001d60: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
-00001d70: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00001d80: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00001d90: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
-00001da0: 6163 6974 793a 3122 202f 3e0d 0a20 2020  acity:1" />..   
-00001db0: 2020 203c 7061 7468 0d0a 2020 2020 2020     <path..      
-00001dc0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a6e     style="fill:n
-00001dd0: 6f6e 653b 7374 726f 6b65 3a23 3030 3030  one;stroke:#0000
-00001de0: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-00001df0: 3170 783b 7374 726f 6b65 2d6c 696e 6563  1px;stroke-linec
-00001e00: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00001e10: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00001e20: 726f 6b65 2d6f 7061 6369 7479 3a31 220d  roke-opacity:1".
-00001e30: 0a20 2020 2020 2020 2020 643d 226d 2037  .         d="m 7
-00001e40: 322e 3731 3532 392c 3937 322e 3339 3733  2.71529,972.3973
-00001e50: 3320 3433 2e34 3937 3336 2c33 2e39 3534  3 43.49736,3.954
-00001e60: 3322 0d0a 2020 2020 2020 2020 2069 643d  3"..         id=
-00001e70: 2270 6174 6833 3738 3522 0d0a 2020 2020  "path3785"..    
-00001e80: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00001e90: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-00001ea0: 653d 2230 2220 2f3e 0d0a 2020 2020 2020  e="0" />..      
-00001eb0: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
-00001ec0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00001ed0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00001ee0: 0d0a 2020 2020 2020 2020 2069 643d 2270  ..         id="p
-00001ef0: 6174 6833 3738 3722 0d0a 2020 2020 2020  ath3787"..      
-00001f00: 2020 2064 3d22 6d20 3736 2e34 3439 3931     d="m 76.44991
-00001f10: 322c 3130 3133 2e34 3738 3220 3433 2e34  2,1013.4782 43.4
-00001f20: 3937 3335 382c 332e 3935 3433 220d 0a20  97358,3.9543".. 
-00001f30: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00001f40: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
-00001f50: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-00001f60: 6964 7468 3a31 7078 3b73 7472 6f6b 652d  idth:1px;stroke-
-00001f70: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00001f80: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00001f90: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-00001fa0: 793a 3122 202f 3e0d 0a20 2020 2020 203c  y:1" />..      <
-00001fb0: 7061 7468 0d0a 2020 2020 2020 2020 2073  path..         s
-00001fc0: 7479 6c65 3d22 6669 6c6c 3a6e 6f6e 653b  tyle="fill:none;
-00001fd0: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
-00001fe0: 7472 6f6b 652d 7769 6474 683a 3170 783b  troke-width:1px;
-00001ff0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00002000: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00002010: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00002020: 2d6f 7061 6369 7479 3a31 220d 0a20 2020  -opacity:1"..   
-00002030: 2020 2020 2020 643d 226d 2035 322e 3530        d="m 52.50
-00002040: 3433 3934 2c39 3837 2e39 3934 3837 2034  4394,987.99487 4
-00002050: 332e 3439 3733 3634 2c33 2e39 3534 3322  3.497364,3.9543"
-00002060: 0d0a 2020 2020 2020 2020 2069 643d 2270  ..         id="p
-00002070: 6174 6833 3738 3922 0d0a 2020 2020 2020  ath3789"..      
-00002080: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00002090: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-000020a0: 2230 2220 2f3e 0d0a 2020 2020 2020 3c70  "0" />..      <p
-000020b0: 6174 680d 0a20 2020 2020 2020 2020 7472  ath..         tr
-000020c0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-000020d0: 7465 2830 2c39 3532 2e33 3632 3138 2922  te(0,952.36218)"
-000020e0: 0d0a 2020 2020 2020 2020 2069 6e6b 7363  ..         inksc
-000020f0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00002100: 7276 6174 7572 653d 2230 220d 0a20 2020  rvature="0"..   
-00002110: 2020 2020 2020 6964 3d22 7061 7468 3337        id="path37
-00002120: 3931 220d 0a20 2020 2020 2020 2020 643d  91"..         d=
-00002130: 224d 2034 342e 3135 3634 3135 2c37 352e  "M 44.156415,75.
-00002140: 3137 3537 3437 2036 352e 3436 3537 3239  175747 65.465729
-00002150: 2c36 332e 3533 3235 3133 220d 0a20 2020  ,63.532513"..   
-00002160: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00002170: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
-00002180: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-00002190: 7468 3a31 7078 3b73 7472 6f6b 652d 6c69  th:1px;stroke-li
-000021a0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-000021b0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-000021c0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-000021d0: 3122 202f 3e0d 0a20 2020 2020 203c 7061  1" />..      <pa
-000021e0: 7468 0d0a 2020 2020 2020 2020 2073 7479  th..         sty
-000021f0: 6c65 3d22 6669 6c6c 3a6e 6f6e 653b 7374  le="fill:none;st
-00002200: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00002210: 6f6b 652d 7769 6474 683a 3170 783b 7374  oke-width:1px;st
-00002220: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00002230: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00002240: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
-00002250: 7061 6369 7479 3a31 220d 0a20 2020 2020  pacity:1"..     
-00002260: 2020 2020 643d 224d 2035 312e 3430 3539      d="M 51.4059
-00002270: 3736 2c39 3834 2e30 3430 3536 2037 322e  76,984.04056 72.
-00002280: 3731 3532 392c 3937 322e 3339 3733 3322  71529,972.39733"
-00002290: 0d0a 2020 2020 2020 2020 2069 643d 2270  ..         id="p
-000022a0: 6174 6833 3739 3322 0d0a 2020 2020 2020  ath3793"..      
-000022b0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-000022c0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-000022d0: 2230 2220 2f3e 0d0a 2020 2020 2020 3c70  "0" />..      <p
-000022e0: 6174 680d 0a20 2020 2020 2020 2020 696e  ath..         in
-000022f0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00002300: 2d63 7572 7661 7475 7265 3d22 3022 0d0a  -curvature="0"..
-00002310: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00002320: 6833 3739 3522 0d0a 2020 2020 2020 2020  h3795"..        
-00002330: 2064 3d22 4d20 3936 2e32 3231 3434 322c   d="M 96.221442,
-00002340: 3939 322e 3136 3838 3620 3131 372e 3533  992.16886 117.53
-00002350: 3037 362c 3938 302e 3532 3536 3322 0d0a  076,980.52563"..
-00002360: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00002370: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
-00002380: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-00002390: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
-000023a0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-000023b0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-000023c0: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
-000023d0: 7479 3a31 2220 2f3e 0d0a 2020 2020 2020  ty:1" />..      
-000023e0: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
-000023f0: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
-00002400: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00002410: 7374 726f 6b65 2d77 6964 7468 3a31 7078  stroke-width:1px
-00002420: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00002430: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00002440: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00002450: 652d 6f70 6163 6974 793a 3122 0d0a 2020  e-opacity:1"..  
-00002460: 2020 2020 2020 2064 3d22 6d20 3939 2e30         d="m 99.0
-00002470: 3737 3333 2c31 3032 392e 3037 3537 2032  7733,1029.0757 2
-00002480: 312e 3330 3933 322c 2d31 312e 3634 3332  1.30932,-11.6432
-00002490: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
-000024a0: 7061 7468 3337 3937 220d 0a20 2020 2020  path3797"..     
-000024b0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-000024c0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-000024d0: 3d22 3022 202f 3e0d 0a20 2020 203c 2f67  ="0" />..    </g
-000024e0: 3e0d 0a20 2020 203c 7465 7874 0d0a 2020  >..    <text..  
-000024f0: 2020 2020 2078 6d6c 3a73 7061 6365 3d22       xml:space="
-00002500: 7072 6573 6572 7665 220d 0a20 2020 2020  preserve"..     
-00002510: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
-00002520: 7a65 3a34 3070 783b 666f 6e74 2d73 7479  ze:40px;font-sty
-00002530: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
-00002540: 6569 6768 743a 6e6f 726d 616c 3b6c 696e  eight:normal;lin
-00002550: 652d 6865 6967 6874 3a31 3235 253b 6c65  e-height:125%;le
-00002560: 7474 6572 2d73 7061 6369 6e67 3a30 7078  tter-spacing:0px
-00002570: 3b77 6f72 642d 7370 6163 696e 673a 3070  ;word-spacing:0p
-00002580: 783b 6669 6c6c 3a23 3030 3030 3030 3b66  x;fill:#000000;f
-00002590: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-000025a0: 726f 6b65 3a6e 6f6e 653b 666f 6e74 2d66  roke:none;font-f
-000025b0: 616d 696c 793a 5361 6e73 220d 0a20 2020  amily:Sans"..   
-000025c0: 2020 2020 783d 2231 3538 2e39 3834 3338      x="158.98438
-000025d0: 220d 0a20 2020 2020 2020 793d 2231 3031  "..       y="101
-000025e0: 302e 3631 3232 220d 0a20 2020 2020 2020  0.6122"..       
-000025f0: 6964 3d22 7465 7874 3337 3939 220d 0a20  id="text3799".. 
-00002600: 2020 2020 2020 736f 6469 706f 6469 3a6c        sodipodi:l
-00002610: 696e 6573 7061 6369 6e67 3d22 3132 3525  inespacing="125%
-00002620: 223e 3c74 7370 616e 0d0a 2020 2020 2020  "><tspan..      
-00002630: 2020 2073 6f64 6970 6f64 693a 726f 6c65     sodipodi:role
-00002640: 3d22 6c69 6e65 220d 0a20 2020 2020 2020  ="line"..       
-00002650: 2020 6964 3d22 7473 7061 6e33 3830 3122    id="tspan3801"
-00002660: 0d0a 2020 2020 2020 2020 2078 3d22 3135  ..         x="15
-00002670: 382e 3938 3433 3822 0d0a 2020 2020 2020  8.98438"..      
-00002680: 2020 2079 3d22 3130 3130 2e36 3132 3222     y="1010.6122"
-00002690: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
-000026a0: 3d22 666f 6e74 2d73 697a 653a 3634 7078  ="font-size:64px
-000026b0: 3b66 6f6e 742d 7374 796c 653a 6974 616c  ;font-style:ital
-000026c0: 6963 3b66 6f6e 742d 7661 7269 616e 743a  ic;font-variant:
-000026d0: 6e6f 726d 616c 3b66 6f6e 742d 7765 6967  normal;font-weig
-000026e0: 6874 3a6e 6f72 6d61 6c3b 666f 6e74 2d73  ht:normal;font-s
-000026f0: 7472 6574 6368 3a6e 6f72 6d61 6c3b 666f  tretch:normal;fo
-00002700: 6e74 2d66 616d 696c 793a 526f 626f 746f  nt-family:Roboto
-00002710: 3b2d 696e 6b73 6361 7065 2d66 6f6e 742d  ;-inkscape-font-
-00002720: 7370 6563 6966 6963 6174 696f 6e3a 526f  specification:Ro
-00002730: 626f 746f 2049 7461 6c69 6322 3e70 7944  boto Italic">pyD
-00002740: 4f45 3c2f 7473 7061 6e3e 3c2f 7465 7874  OE</tspan></text
-00002750: 3e0d 0a20 2020 203c 670d 0a20 2020 2020  >..    <g..     
-00002760: 2020 6964 3d22 6733 3831 3922 0d0a 2020    id="g3819"..  
-00002770: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
-00002780: 6d61 7472 6978 2831 2e30 3832 3230 3131  matrix(1.0822011
-00002790: 2c2d 302e 3231 3936 3134 3037 2c30 2e32  ,-0.21961407,0.2
-000027a0: 3139 3631 3430 372c 312e 3038 3232 3031  1961407,1.082201
-000027b0: 312c 2d32 3431 2e30 3832 3836 2c31 322e  1,-241.08286,12.
-000027c0: 3430 3636 3036 2922 0d0a 2020 2020 2020  406606)"..      
-000027d0: 2073 7479 6c65 3d22 6f70 6163 6974 793a   style="opacity:
-000027e0: 302e 3735 3b66 696c 6c3a 2330 3030 3030  0.75;fill:#00000
-000027f0: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
-00002800: 223e 0d0a 2020 2020 2020 3c74 6578 740d  ">..      <text.
-00002810: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-00002820: 6469 3a6c 696e 6573 7061 6369 6e67 3d22  di:linespacing="
-00002830: 3132 3525 220d 0a20 2020 2020 2020 2020  125%"..         
-00002840: 6964 3d22 7465 7874 3338 3033 220d 0a20  id="text3803".. 
-00002850: 2020 2020 2020 2020 793d 2239 3636 2e39          y="966.9
-00002860: 3839 3522 0d0a 2020 2020 2020 2020 2078  895"..         x
-00002870: 3d22 3430 312e 3030 3731 3722 0d0a 2020  ="401.00717"..  
-00002880: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
-00002890: 6e74 2d73 697a 653a 3230 2e30 3434 3535  nt-size:20.04455
-000028a0: 3536 3670 783b 666f 6e74 2d73 7479 6c65  566px;font-style
-000028b0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d77 6569  :normal;font-wei
-000028c0: 6768 743a 6e6f 726d 616c 3b6c 696e 652d  ght:normal;line-
-000028d0: 6865 6967 6874 3a31 3235 253b 6c65 7474  height:125%;lett
-000028e0: 6572 2d73 7061 6369 6e67 3a30 7078 3b77  er-spacing:0px;w
-000028f0: 6f72 642d 7370 6163 696e 673a 3070 783b  ord-spacing:0px;
-00002900: 6669 6c6c 3a23 3030 3030 3030 3b66 696c  fill:#000000;fil
-00002910: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00002920: 6b65 3a6e 6f6e 653b 666f 6e74 2d66 616d  ke:none;font-fam
-00002930: 696c 793a 5361 6e73 220d 0a20 2020 2020  ily:Sans"..     
-00002940: 2020 2020 786d 6c3a 7370 6163 653d 2270      xml:space="p
-00002950: 7265 7365 7276 6522 3e3c 7473 7061 6e0d  reserve"><tspan.
-00002960: 0a20 2020 2020 2020 2020 2020 7374 796c  .           styl
-00002970: 653d 2266 6f6e 742d 7369 7a65 3a31 3670  e="font-size:16p
-00002980: 783b 666f 6e74 2d73 7479 6c65 3a6e 6f72  x;font-style:nor
-00002990: 6d61 6c3b 666f 6e74 2d76 6172 6961 6e74  mal;font-variant
-000029a0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d77 6569  :normal;font-wei
-000029b0: 6768 743a 626f 6c64 3b66 6f6e 742d 7374  ght:bold;font-st
-000029c0: 7265 7463 683a 6e6f 726d 616c 3b66 696c  retch:normal;fil
-000029d0: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
-000029e0: 7061 6369 7479 3a31 3b66 6f6e 742d 6661  pacity:1;font-fa
-000029f0: 6d69 6c79 3a54 6558 2047 7972 6520 4375  mily:TeX Gyre Cu
-00002a00: 7273 6f72 3b2d 696e 6b73 6361 7065 2d66  rsor;-inkscape-f
-00002a10: 6f6e 742d 7370 6563 6966 6963 6174 696f  ont-specificatio
-00002a20: 6e3a 5465 5820 4779 7265 2043 7572 736f  n:TeX Gyre Curso
-00002a30: 7220 426f 6c64 220d 0a20 2020 2020 2020  r Bold"..       
-00002a40: 2020 2020 793d 2239 3636 2e39 3839 3522      y="966.9895"
-00002a50: 0d0a 2020 2020 2020 2020 2020 2078 3d22  ..           x="
-00002a60: 3430 312e 3030 3731 3722 0d0a 2020 2020  401.00717"..    
-00002a70: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
-00002a80: 3338 3035 220d 0a20 2020 2020 2020 2020  3805"..         
-00002a90: 2020 736f 6469 706f 6469 3a72 6f6c 653d    sodipodi:role=
-00002aa0: 226c 696e 6522 3e41 2042 2043 3c2f 7473  "line">A B C</ts
-00002ab0: 7061 6e3e 3c74 7370 616e 0d0a 2020 2020  pan><tspan..    
-00002ac0: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
-00002ad0: 6e74 2d73 697a 653a 3136 7078 3b66 6f6e  nt-size:16px;fon
-00002ae0: 742d 7374 796c 653a 6e6f 726d 616c 3b66  t-style:normal;f
-00002af0: 6f6e 742d 7661 7269 616e 743a 6e6f 726d  ont-variant:norm
-00002b00: 616c 3b66 6f6e 742d 7765 6967 6874 3a62  al;font-weight:b
-00002b10: 6f6c 643b 666f 6e74 2d73 7472 6574 6368  old;font-stretch
-00002b20: 3a6e 6f72 6d61 6c3b 6669 6c6c 3a23 3030  :normal;fill:#00
-00002b30: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
-00002b40: 793a 313b 666f 6e74 2d66 616d 696c 793a  y:1;font-family:
-00002b50: 5465 5820 4779 7265 2043 7572 736f 723b  TeX Gyre Cursor;
-00002b60: 2d69 6e6b 7363 6170 652d 666f 6e74 2d73  -inkscape-font-s
-00002b70: 7065 6369 6669 6361 7469 6f6e 3a54 6558  pecification:TeX
-00002b80: 2047 7972 6520 4375 7273 6f72 2042 6f6c   Gyre Cursor Bol
-00002b90: 6422 0d0a 2020 2020 2020 2020 2020 2069  d"..           i
-00002ba0: 643d 2274 7370 616e 3338 3037 220d 0a20  d="tspan3807".. 
-00002bb0: 2020 2020 2020 2020 2020 793d 2239 3836            y="986
-00002bc0: 2e39 3839 3522 0d0a 2020 2020 2020 2020  .9895"..        
-00002bd0: 2020 2078 3d22 3430 312e 3030 3731 3722     x="401.00717"
-00002be0: 0d0a 2020 2020 2020 2020 2020 2073 6f64  ..           sod
-00002bf0: 6970 6f64 693a 726f 6c65 3d22 6c69 6e65  ipodi:role="line
-00002c00: 223e 3020 3020 313c 2f74 7370 616e 3e3c  ">0 0 1</tspan><
-00002c10: 7473 7061 6e0d 0a20 2020 2020 2020 2020  tspan..         
-00002c20: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
-00002c30: 7a65 3a31 3670 783b 666f 6e74 2d73 7479  ze:16px;font-sty
-00002c40: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
-00002c50: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
-00002c60: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
-00002c70: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
-00002c80: 616c 3b66 696c 6c3a 2330 3030 3030 303b  al;fill:#000000;
-00002c90: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
-00002ca0: 6f6e 742d 6661 6d69 6c79 3a54 6558 2047  ont-family:TeX G
-00002cb0: 7972 6520 4375 7273 6f72 3b2d 696e 6b73  yre Cursor;-inks
-00002cc0: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
-00002cd0: 6963 6174 696f 6e3a 5465 5820 4779 7265  ication:TeX Gyre
-00002ce0: 2043 7572 736f 7220 426f 6c64 220d 0a20   Cursor Bold".. 
-00002cf0: 2020 2020 2020 2020 2020 6964 3d22 7473            id="ts
-00002d00: 7061 6e33 3830 3922 0d0a 2020 2020 2020  pan3809"..      
-00002d10: 2020 2020 2079 3d22 3130 3036 2e39 3839       y="1006.989
-00002d20: 3522 0d0a 2020 2020 2020 2020 2020 2078  5"..           x
-00002d30: 3d22 3430 312e 3030 3731 3722 0d0a 2020  ="401.00717"..  
-00002d40: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00002d50: 693a 726f 6c65 3d22 6c69 6e65 223e 3120  i:role="line">1 
-00002d60: 3020 303c 2f74 7370 616e 3e3c 7473 7061  0 0</tspan><tspa
-00002d70: 6e0d 0a20 2020 2020 2020 2020 2020 7374  n..           st
-00002d80: 796c 653d 2266 6f6e 742d 7369 7a65 3a31  yle="font-size:1
-00002d90: 3670 783b 666f 6e74 2d73 7479 6c65 3a6e  6px;font-style:n
-00002da0: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
-00002db0: 6e74 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  nt:normal;font-w
-00002dc0: 6569 6768 743a 626f 6c64 3b66 6f6e 742d  eight:bold;font-
-00002dd0: 7374 7265 7463 683a 6e6f 726d 616c 3b66  stretch:normal;f
-00002de0: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
-00002df0: 2d6f 7061 6369 7479 3a31 3b66 6f6e 742d  -opacity:1;font-
-00002e00: 6661 6d69 6c79 3a54 6558 2047 7972 6520  family:TeX Gyre 
-00002e10: 4375 7273 6f72 3b2d 696e 6b73 6361 7065  Cursor;-inkscape
-00002e20: 2d66 6f6e 742d 7370 6563 6966 6963 6174  -font-specificat
-00002e30: 696f 6e3a 5465 5820 4779 7265 2043 7572  ion:TeX Gyre Cur
-00002e40: 736f 7220 426f 6c64 220d 0a20 2020 2020  sor Bold"..     
-00002e50: 2020 2020 2020 6964 3d22 7473 7061 6e33        id="tspan3
-00002e60: 3831 3122 0d0a 2020 2020 2020 2020 2020  811"..          
-00002e70: 2079 3d22 3130 3236 2e39 3839 3522 0d0a   y="1026.9895"..
-00002e80: 2020 2020 2020 2020 2020 2078 3d22 3430             x="40
-00002e90: 312e 3030 3731 3722 0d0a 2020 2020 2020  1.00717"..      
-00002ea0: 2020 2020 2073 6f64 6970 6f64 693a 726f       sodipodi:ro
-00002eb0: 6c65 3d22 6c69 6e65 223e 3020 3120 303c  le="line">0 1 0<
-00002ec0: 2f74 7370 616e 3e3c 7473 7061 6e0d 0a20  /tspan><tspan.. 
-00002ed0: 2020 2020 2020 2020 2020 7374 796c 653d            style=
-00002ee0: 2266 6f6e 742d 7369 7a65 3a31 3670 783b  "font-size:16px;
-00002ef0: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
-00002f00: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
-00002f10: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
-00002f20: 743a 626f 6c64 3b66 6f6e 742d 7374 7265  t:bold;font-stre
-00002f30: 7463 683a 6e6f 726d 616c 3b66 696c 6c3a  tch:normal;fill:
-00002f40: 2330 3030 3030 303b 6669 6c6c 2d6f 7061  #000000;fill-opa
-00002f50: 6369 7479 3a31 3b66 6f6e 742d 6661 6d69  city:1;font-fami
-00002f60: 6c79 3a54 6558 2047 7972 6520 4375 7273  ly:TeX Gyre Curs
-00002f70: 6f72 3b2d 696e 6b73 6361 7065 2d66 6f6e  or;-inkscape-fon
-00002f80: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
-00002f90: 5465 5820 4779 7265 2043 7572 736f 7220  TeX Gyre Cursor 
-00002fa0: 426f 6c64 220d 0a20 2020 2020 2020 2020  Bold"..         
-00002fb0: 2020 6964 3d22 7473 7061 6e33 3831 3322    id="tspan3813"
-00002fc0: 0d0a 2020 2020 2020 2020 2020 2079 3d22  ..           y="
-00002fd0: 3130 3436 2e39 3839 3522 0d0a 2020 2020  1046.9895"..    
-00002fe0: 2020 2020 2020 2078 3d22 3430 312e 3030         x="401.00
-00002ff0: 3731 3722 0d0a 2020 2020 2020 2020 2020  717"..          
-00003000: 2073 6f64 6970 6f64 693a 726f 6c65 3d22   sodipodi:role="
-00003010: 6c69 6e65 223e 3120 3120 313c 2f74 7370  line">1 1 1</tsp
-00003020: 616e 3e3c 2f74 6578 743e 0d0a 2020 2020  an></text>..    
-00003030: 2020 3c70 6174 680d 0a20 2020 2020 2020    <path..       
-00003040: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00003050: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00003060: 3022 0d0a 2020 2020 2020 2020 2069 643d  0"..         id=
-00003070: 2270 6174 6833 3831 3722 0d0a 2020 2020  "path3817"..    
-00003080: 2020 2020 2064 3d22 6d20 3339 362e 3936       d="m 396.96
-00003090: 3833 362c 3937 312e 3037 3932 3320 3535  836,971.07923 55
-000030a0: 2e31 3430 362c 3022 0d0a 2020 2020 2020  .1406,0"..      
-000030b0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-000030c0: 3030 3030 3030 3b66 696c 6c2d 6f70 6163  000000;fill-opac
-000030d0: 6974 793a 313b 7374 726f 6b65 3a23 3030  ity:1;stroke:#00
-000030e0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-000030f0: 683a 302e 3930 3535 3833 3938 7078 3b73  h:0.90558398px;s
-00003100: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00003110: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00003120: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00003130: 6f70 6163 6974 793a 3122 202f 3e0d 0a20  opacity:1" />.. 
-00003140: 2020 203c 2f67 3e0d 0a20 2020 203c 7465     </g>..    <te
-00003150: 7874 0d0a 2020 2020 2020 2073 6f64 6970  xt..       sodip
-00003160: 6f64 693a 6c69 6e65 7370 6163 696e 673d  odi:linespacing=
-00003170: 2231 3235 2522 0d0a 2020 2020 2020 2069  "125%"..       i
-00003180: 643d 2274 6578 7433 3832 3822 0d0a 2020  d="text3828"..  
-00003190: 2020 2020 2079 3d22 3130 3434 2e33 3032       y="1044.302
-000031a0: 3722 0d0a 2020 2020 2020 2078 3d22 3131  7"..       x="11
-000031b0: 362e 3839 3637 3122 0d0a 2020 2020 2020  6.89671"..      
-000031c0: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
-000031d0: 653a 3338 2e31 3731 3431 3334 3270 783b  e:38.17141342px;
-000031e0: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
-000031f0: 6c3b 666f 6e74 2d77 6569 6768 743a 6e6f  l;font-weight:no
-00003200: 726d 616c 3b6c 696e 652d 6865 6967 6874  rmal;line-height
-00003210: 3a31 3235 253b 6c65 7474 6572 2d73 7061  :125%;letter-spa
-00003220: 6369 6e67 3a30 7078 3b77 6f72 642d 7370  cing:0px;word-sp
-00003230: 6163 696e 673a 3070 783b 6669 6c6c 3a23  acing:0px;fill:#
-00003240: 3030 3030 3030 3b66 696c 6c2d 6f70 6163  000000;fill-opac
-00003250: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
-00003260: 653b 666f 6e74 2d66 616d 696c 793a 5361  e;font-family:Sa
-00003270: 6e73 220d 0a20 2020 2020 2020 786d 6c3a  ns"..       xml:
-00003280: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
-00003290: 3e3c 7473 7061 6e0d 0a20 2020 2020 2020  ><tspan..       
-000032a0: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
-000032b0: 7a65 3a31 392e 3038 3537 3036 3731 7078  ze:19.08570671px
-000032c0: 3b66 6f6e 742d 7374 796c 653a 6974 616c  ;font-style:ital
-000032d0: 6963 3b66 6f6e 742d 7661 7269 616e 743a  ic;font-variant:
-000032e0: 6e6f 726d 616c 3b66 6f6e 742d 7765 6967  normal;font-weig
-000032f0: 6874 3a6e 6f72 6d61 6c3b 666f 6e74 2d73  ht:normal;font-s
-00003300: 7472 6574 6368 3a6e 6f72 6d61 6c3b 666f  tretch:normal;fo
-00003310: 6e74 2d66 616d 696c 793a 526f 626f 746f  nt-family:Roboto
-00003320: 3b2d 696e 6b73 6361 7065 2d66 6f6e 742d  ;-inkscape-font-
-00003330: 7370 6563 6966 6963 6174 696f 6e3a 526f  specification:Ro
-00003340: 626f 746f 2049 7461 6c69 6322 0d0a 2020  boto Italic"..  
-00003350: 2020 2020 2020 2079 3d22 3130 3434 2e33         y="1044.3
-00003360: 3032 3722 0d0a 2020 2020 2020 2020 2078  027"..         x
-00003370: 3d22 3131 362e 3839 3637 3122 0d0a 2020  ="116.89671"..  
-00003380: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
-00003390: 3338 3330 220d 0a20 2020 2020 2020 2020  3830"..         
-000033a0: 736f 6469 706f 6469 3a72 6f6c 653d 226c  sodipodi:role="l
-000033b0: 696e 6522 3e44 6573 6967 6e20 6f66 2045  ine">Design of E
-000033c0: 7870 6572 696d 656e 7473 2066 6f72 2050  xperiments for P
-000033d0: 7974 686f 6e3c 2f74 7370 616e 3e3c 2f74  ython</tspan></t
-000033e0: 6578 743e 0d0a 2020 2020 3c67 0d0a 2020  ext>..    <g..  
-000033f0: 2020 2020 2069 643d 2267 3339 3231 220d       id="g3921".
-00003400: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-00003410: 6d3d 2274 7261 6e73 6c61 7465 2830 2c2d  m="translate(0,-
-00003420: 302e 3930 3039 3030 3929 223e 0d0a 2020  0.9009009)">..  
-00003430: 2020 2020 3c70 6174 680d 0a20 2020 2020      <path..     
-00003440: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-00003450: 6574 7970 6573 3d22 6373 6322 0d0a 2020  etypes="csc"..  
-00003460: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00003470: 3d22 7472 616e 736c 6174 6528 302c 3935  ="translate(0,95
-00003480: 322e 3336 3231 3829 220d 0a20 2020 2020  2.36218)"..     
-00003490: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-000034a0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-000034b0: 3d22 3022 0d0a 2020 2020 2020 2020 2069  ="0"..         i
-000034c0: 643d 2270 6174 6833 3839 3322 0d0a 2020  d="path3893"..  
-000034d0: 2020 2020 2020 2064 3d22 4d20 3232 2e30         d="M 22.0
-000034e0: 3732 3037 322c 3837 2e38 3337 3833 3820  72072,87.837838 
-000034f0: 4320 3632 2e31 3632 3136 322c 3831 2e39  C 62.162162,81.9
-00003500: 3831 3938 3220 3733 2e38 3733 3837 332c  81982 73.873873,
-00003510: 3638 2e30 3138 3031 3820 3635 2e33 3135  68.018018 65.315
-00003520: 3331 352c 3531 2e33 3531 3335 3120 3536  315,51.351351 56
-00003530: 2e37 3536 3735 382c 3334 2e36 3834 3638  .756758,34.68468
-00003540: 3420 3739 2e37 3239 3733 2c31 382e 3931  4 79.72973,18.91
-00003550: 3839 3139 2031 3032 2e32 3532 3235 2c31  8919 102.25225,1
-00003560: 312e 3731 3137 3132 220d 0a20 2020 2020  1.711712"..     
-00003570: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00003580: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
-00003590: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-000035a0: 3a34 3b73 7472 6f6b 652d 6c69 6e65 6361  :4;stroke-lineca
-000035b0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-000035c0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-000035d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000035e0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-000035f0: 313b 7374 726f 6b65 2d64 6173 6861 7272  1;stroke-dasharr
-00003600: 6179 3a6e 6f6e 6522 202f 3e0d 0a20 2020  ay:none" />..   
-00003610: 2020 203c 7061 7468 0d0a 2020 2020 2020     <path..      
-00003620: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00003630: 7479 7065 733d 2263 7373 7373 6363 220d  types="csssscc".
-00003640: 0a20 2020 2020 2020 2020 7472 616e 7366  .         transf
-00003650: 6f72 6d3d 2274 7261 6e73 6c61 7465 2830  orm="translate(0
-00003660: 2c39 3532 2e33 3632 3138 2922 0d0a 2020  ,952.36218)"..  
-00003670: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00003680: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00003690: 7572 653d 2230 220d 0a20 2020 2020 2020  ure="0"..       
-000036a0: 2020 6964 3d22 7061 7468 3338 3935 220d    id="path3895".
-000036b0: 0a20 2020 2020 2020 2020 643d 226d 2031  .         d="m 1
-000036c0: 3032 2e35 3137 3335 2c39 2e33 3234 3037  02.51735,9.32407
-000036d0: 3235 2063 2030 2c30 202d 3130 2e31 3633  25 c 0,0 -10.163
-000036e0: 3535 312c 2d31 2e33 3338 3337 3537 202d  551,-1.3383757 -
-000036f0: 3133 2e36 3637 3233 332c 302e 3431 3334  13.667233,0.4134
-00003700: 3635 202d 332e 3530 3336 3833 2c31 2e37  65 -3.503683,1.7
-00003710: 3531 3834 3135 202d 322e 3830 3732 3536  518415 -2.807256
-00003720: 2c33 2e35 3935 3236 3935 202d 332e 3433  ,3.5952695 -3.43
-00003730: 3933 3733 2c36 2e35 3139 3932 3935 202d  9373,6.5199295 -
-00003740: 302e 3533 3337 3231 2c32 2e34 3639 3430  0.533721,2.46940
-00003750: 3320 302e 3335 3535 3235 2c33 2e36 3130  3 0.355525,3.610
-00003760: 3730 3320 322e 3037 3033 3537 2c33 2e39  703 2.070357,3.9
-00003770: 3831 3435 3720 312e 3339 3232 3831 2c30  81457 1.392281,0
-00003780: 2e33 3031 3031 3720 332e 3338 3636 3833  .301017 3.386683
-00003790: 2c32 2e35 3134 3837 2036 2e36 3531 3836  ,2.51487 6.65186
-000037a0: 332c 312e 3236 3434 3036 2033 2e32 3531  3,1.264406 3.251
-000037b0: 3133 322c 2d31 2e32 3435 3038 3520 342e  132,-1.245085 4.
-000037c0: 3933 3634 3336 2c2d 322e 3831 3032 3920  936436,-2.81029 
-000037d0: 392e 3732 3434 3236 2c2d 382e 3038 3335  9.724426,-8.0835
-000037e0: 3331 207a 220d 0a20 2020 2020 2020 2020  31 z"..         
-000037f0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00003800: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
-00003810: 3a31 3b73 7472 6f6b 653a 2330 3030 3030  :1;stroke:#00000
-00003820: 303b 7374 726f 6b65 2d77 6964 7468 3a31  0;stroke-width:1
-00003830: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
-00003840: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00003850: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00003860: 6f6b 652d 6f70 6163 6974 793a 3122 202f  oke-opacity:1" /
-00003870: 3e0d 0a20 2020 2020 203c 7061 7468 0d0a  >..      <path..
-00003880: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00003890: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-000038a0: 220d 0a20 2020 2020 2020 2020 7472 616e  "..         tran
-000038b0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-000038c0: 2830 2c39 3532 2e33 3632 3138 2922 0d0a  (0,952.36218)"..
-000038d0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-000038e0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-000038f0: 6174 7572 653d 2230 220d 0a20 2020 2020  ature="0"..     
-00003900: 2020 2020 6964 3d22 7061 7468 3338 3937      id="path3897
-00003910: 220d 0a20 2020 2020 2020 2020 643d 226d  "..         d="m
-00003920: 2031 3038 2e33 3735 3236 2c37 2e39 3438   108.37526,7.948
-00003930: 3731 3137 2063 202d 302e 3731 3636 362c  7117 c -0.71666,
-00003940: 312e 3433 3333 3235 202d 352e 3031 3636  1.433325 -5.0166
-00003950: 342c 332e 3334 3434 3234 3320 2d35 2e30  4,3.3444243 -5.0
-00003960: 3136 3634 2c33 2e33 3434 3432 3433 2030  1664,3.3444243 0
-00003970: 2c30 2034 2e35 3338 3836 2c2d 312e 3139  ,0 4.53886,-1.19
-00003980: 3434 3338 2036 2e33 3730 3333 2c2d 302e  4438 6.37033,-0.
-00003990: 3437 3737 3735 220d 0a20 2020 2020 2020  477775"..       
-000039a0: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
-000039b0: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
-000039c0: 303b 7374 726f 6b65 2d77 6964 7468 3a31  0;stroke-width:1
-000039d0: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
-000039e0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-000039f0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00003a00: 6f6b 652d 6f70 6163 6974 793a 3122 202f  oke-opacity:1" /
-00003a10: 3e0d 0a20 2020 203c 2f67 3e0d 0a20 203c  >..    </g>..  <
-00003a20: 2f67 3e0d 0a3c 2f73 7667 3e0d 0a         /g>..</svg>..
+00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
+00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
+00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
+00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
+00000070: 0a0a 3c73 7667 0a20 2020 786d 6c6e 733a  ..<svg.   xmlns:
+00000080: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
+00000090: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
+000000a0: 312e 312f 220a 2020 2078 6d6c 6e73 3a63  1.1/".   xmlns:c
+000000b0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
+000000c0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
+000000d0: 2322 0a20 2020 786d 6c6e 733a 7264 663d  #".   xmlns:rdf=
+000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000000f0: 7267 2f31 3939 392f 3032 2f32 322d 7264  rg/1999/02/22-rd
+00000100: 662d 7379 6e74 6178 2d6e 7323 220a 2020  f-syntax-ns#".  
+00000110: 2078 6d6c 6e73 3a73 7667 3d22 6874 7470   xmlns:svg="http
+00000120: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000130: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
+00000140: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+00000150: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
+00000160: 2078 6d6c 6e73 3a78 6c69 6e6b 3d22 6874   xmlns:xlink="ht
+00000170: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000180: 3139 3939 2f78 6c69 6e6b 220a 2020 2078  1999/xlink".   x
+00000190: 6d6c 6e73 3a73 6f64 6970 6f64 693d 2268  mlns:sodipodi="h
+000001a0: 7474 703a 2f2f 736f 6469 706f 6469 2e73  ttp://sodipodi.s
+000001b0: 6f75 7263 6566 6f72 6765 2e6e 6574 2f44  ourceforge.net/D
+000001c0: 5444 2f73 6f64 6970 6f64 692d 302e 6474  TD/sodipodi-0.dt
+000001d0: 6422 0a20 2020 786d 6c6e 733a 696e 6b73  d".   xmlns:inks
+000001e0: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
+000001f0: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
+00000200: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
+00000210: 6522 0a20 2020 7769 6474 683d 2235 3030  e".   width="500
+00000220: 220a 2020 2068 6569 6768 743d 2231 3030  ".   height="100
+00000230: 220a 2020 2069 643d 2273 7667 3222 0a20  ".   id="svg2". 
+00000240: 2020 7665 7273 696f 6e3d 2231 2e31 220a    version="1.1".
+00000250: 2020 2069 6e6b 7363 6170 653a 7665 7273     inkscape:vers
+00000260: 696f 6e3d 2230 2e34 382e 3420 7239 3933  ion="0.48.4 r993
+00000270: 3922 0a20 2020 736f 6469 706f 6469 3a64  9".   sodipodi:d
+00000280: 6f63 6e61 6d65 3d22 6472 6177 696e 672e  ocname="drawing.
+00000290: 7376 6722 0a20 2020 696e 6b73 6361 7065  svg".   inkscape
+000002a0: 3a65 7870 6f72 742d 6669 6c65 6e61 6d65  :export-filename
+000002b0: 3d22 2f6d 6564 6961 2f4c 696d 626f 2f70  ="/media/Limbo/p
+000002c0: 7974 686f 6e2f 7079 7468 6f6e 3237 2f70  ython/python27/p
+000002d0: 7944 4f45 332f 646f 632f 5f73 7461 7469  yDOE3/doc/_stati
+000002e0: 632f 6c6f 676f 2e70 6e67 220a 2020 2069  c/logo.png".   i
+000002f0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00000300: 6470 693d 2239 3022 0a20 2020 696e 6b73  dpi="90".   inks
+00000310: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00000320: 3d22 3930 223e 0a20 203c 6465 6673 0a20  ="90">.  <defs. 
+00000330: 2020 2020 6964 3d22 6465 6673 3422 3e0a      id="defs4">.
+00000340: 2020 2020 3c69 6e6b 7363 6170 653a 7065      <inkscape:pe
+00000350: 7273 7065 6374 6976 650a 2020 2020 2020  rspective.      
+00000360: 2073 6f64 6970 6f64 693a 7479 7065 3d22   sodipodi:type="
+00000370: 696e 6b73 6361 7065 3a70 6572 7370 3364  inkscape:persp3d
+00000380: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00000390: 653a 7670 5f78 3d22 3020 3a20 3530 203a  e:vp_x="0 : 50 :
+000003a0: 2031 220a 2020 2020 2020 2069 6e6b 7363   1".       inksc
+000003b0: 6170 653a 7670 5f79 3d22 3020 3a20 3130  ape:vp_y="0 : 10
+000003c0: 3030 203a 2030 220a 2020 2020 2020 2069  00 : 0".       i
+000003d0: 6e6b 7363 6170 653a 7670 5f7a 3d22 3530  nkscape:vp_z="50
+000003e0: 3020 3a20 3530 203a 2031 220a 2020 2020  0 : 50 : 1".    
+000003f0: 2020 2069 6e6b 7363 6170 653a 7065 7273     inkscape:pers
+00000400: 7033 642d 6f72 6967 696e 3d22 3235 3020  p3d-origin="250 
+00000410: 3a20 3333 2e33 3333 3333 3320 3a20 3122  : 33.333333 : 1"
+00000420: 0a20 2020 2020 2020 6964 3d22 7065 7273  .       id="pers
+00000430: 7065 6374 6976 6533 3833 3222 202f 3e0a  pective3832" />.
+00000440: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00000450: 656e 740a 2020 2020 2020 2069 643d 226c  ent.       id="l
+00000460: 696e 6561 7247 7261 6469 656e 7433 3735  inearGradient375
+00000470: 3522 3e0a 2020 2020 2020 3c73 746f 700a  5">.      <stop.
+00000480: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000490: 7374 6f70 2d63 6f6c 6f72 3a23 6666 6361  stop-color:#ffca
+000004a0: 6361 3b73 746f 702d 6f70 6163 6974 793a  ca;stop-opacity:
+000004b0: 313b 220a 2020 2020 2020 2020 206f 6666  1;".         off
+000004c0: 7365 743d 2230 220a 2020 2020 2020 2020  set="0".        
+000004d0: 2069 643d 2273 746f 7033 3735 3722 202f   id="stop3757" /
+000004e0: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
+000004f0: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
+00000500: 6f70 2d63 6f6c 6f72 3a23 6664 3030 3030  op-color:#fd0000
+00000510: 3b73 746f 702d 6f70 6163 6974 793a 313b  ;stop-opacity:1;
+00000520: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
+00000530: 743d 2231 220a 2020 2020 2020 2020 2069  t="1".         i
+00000540: 643d 2273 746f 7033 3735 3922 202f 3e0a  d="stop3759" />.
+00000550: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
+00000560: 6965 6e74 3e0a 2020 2020 3c72 6164 6961  ient>.    <radia
+00000570: 6c47 7261 6469 656e 740a 2020 2020 2020  lGradient.      
+00000580: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
+00000590: 743d 2261 6c77 6179 7322 0a20 2020 2020  t="always".     
+000005a0: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+000005b0: 696e 6561 7247 7261 6469 656e 7433 3735  inearGradient375
+000005c0: 3522 0a20 2020 2020 2020 6964 3d22 7261  5".       id="ra
+000005d0: 6469 616c 4772 6164 6965 6e74 3338 3636  dialGradient3866
+000005e0: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
+000005f0: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00000600: 654f 6e55 7365 220a 2020 2020 2020 2063  eOnUse".       c
+00000610: 783d 2234 362e 3533 3838 3322 0a20 2020  x="46.53883".   
+00000620: 2020 2020 6379 3d22 3333 2e32 3239 3332      cy="33.22932
+00000630: 3822 0a20 2020 2020 2020 6678 3d22 3436  8".       fx="46
+00000640: 2e35 3338 3833 220a 2020 2020 2020 2066  .53883".       f
+00000650: 793d 2233 332e 3232 3933 3238 220a 2020  y="33.229328".  
+00000660: 2020 2020 2072 3d22 362e 3435 3934 3735       r="6.459475
+00000670: 3522 202f 3e0a 2020 2020 3c72 6164 6961  5" />.    <radia
+00000680: 6c47 7261 6469 656e 740a 2020 2020 2020  lGradient.      
+00000690: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
+000006a0: 743d 2261 6c77 6179 7322 0a20 2020 2020  t="always".     
+000006b0: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+000006c0: 696e 6561 7247 7261 6469 656e 7433 3735  inearGradient375
+000006d0: 3522 0a20 2020 2020 2020 6964 3d22 7261  5".       id="ra
+000006e0: 6469 616c 4772 6164 6965 6e74 3338 3638  dialGradient3868
+000006f0: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
+00000700: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00000710: 654f 6e55 7365 220a 2020 2020 2020 2063  eOnUse".       c
+00000720: 783d 2234 362e 3533 3838 3322 0a20 2020  x="46.53883".   
+00000730: 2020 2020 6379 3d22 3333 2e32 3239 3332      cy="33.22932
+00000740: 3822 0a20 2020 2020 2020 6678 3d22 3436  8".       fx="46
+00000750: 2e35 3338 3833 220a 2020 2020 2020 2066  .53883".       f
+00000760: 793d 2233 332e 3232 3933 3238 220a 2020  y="33.229328".  
+00000770: 2020 2020 2072 3d22 362e 3435 3934 3735       r="6.459475
+00000780: 3522 202f 3e0a 2020 2020 3c72 6164 6961  5" />.    <radia
+00000790: 6c47 7261 6469 656e 740a 2020 2020 2020  lGradient.      
+000007a0: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
+000007b0: 743d 2261 6c77 6179 7322 0a20 2020 2020  t="always".     
+000007c0: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+000007d0: 696e 6561 7247 7261 6469 656e 7433 3735  inearGradient375
+000007e0: 3522 0a20 2020 2020 2020 6964 3d22 7261  5".       id="ra
+000007f0: 6469 616c 4772 6164 6965 6e74 3338 3730  dialGradient3870
+00000800: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
+00000810: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00000820: 654f 6e55 7365 220a 2020 2020 2020 2063  eOnUse".       c
+00000830: 783d 2234 362e 3533 3838 3322 0a20 2020  x="46.53883".   
+00000840: 2020 2020 6379 3d22 3333 2e32 3239 3332      cy="33.22932
+00000850: 3822 0a20 2020 2020 2020 6678 3d22 3436  8".       fx="46
+00000860: 2e35 3338 3833 220a 2020 2020 2020 2066  .53883".       f
+00000870: 793d 2233 332e 3232 3933 3238 220a 2020  y="33.229328".  
+00000880: 2020 2020 2072 3d22 362e 3435 3934 3735       r="6.459475
+00000890: 3522 202f 3e0a 2020 2020 3c72 6164 6961  5" />.    <radia
+000008a0: 6c47 7261 6469 656e 740a 2020 2020 2020  lGradient.      
+000008b0: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
+000008c0: 743d 2261 6c77 6179 7322 0a20 2020 2020  t="always".     
+000008d0: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+000008e0: 696e 6561 7247 7261 6469 656e 7433 3735  inearGradient375
+000008f0: 3522 0a20 2020 2020 2020 6964 3d22 7261  5".       id="ra
+00000900: 6469 616c 4772 6164 6965 6e74 3338 3732  dialGradient3872
+00000910: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
+00000920: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00000930: 654f 6e55 7365 220a 2020 2020 2020 2063  eOnUse".       c
+00000940: 783d 2234 362e 3533 3838 3322 0a20 2020  x="46.53883".   
+00000950: 2020 2020 6379 3d22 3333 2e32 3239 3332      cy="33.22932
+00000960: 3822 0a20 2020 2020 2020 6678 3d22 3436  8".       fx="46
+00000970: 2e35 3338 3833 220a 2020 2020 2020 2066  .53883".       f
+00000980: 793d 2233 332e 3232 3933 3238 220a 2020  y="33.229328".  
+00000990: 2020 2020 2072 3d22 362e 3435 3934 3735       r="6.459475
+000009a0: 3522 202f 3e0a 2020 3c2f 6465 6673 3e0a  5" />.  </defs>.
+000009b0: 2020 3c73 6f64 6970 6f64 693a 6e61 6d65    <sodipodi:name
+000009c0: 6476 6965 770a 2020 2020 2069 643d 2262  dview.     id="b
+000009d0: 6173 6522 0a20 2020 2020 7061 6765 636f  ase".     pageco
+000009e0: 6c6f 723d 2223 6666 6666 6666 220a 2020  lor="#ffffff".  
+000009f0: 2020 2062 6f72 6465 7263 6f6c 6f72 3d22     bordercolor="
+00000a00: 2336 3636 3636 3622 0a20 2020 2020 626f  #666666".     bo
+00000a10: 7264 6572 6f70 6163 6974 793d 2231 2e30  rderopacity="1.0
+00000a20: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000a30: 7061 6765 6f70 6163 6974 793d 2230 2e30  pageopacity="0.0
+00000a40: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000a50: 7061 6765 7368 6164 6f77 3d22 3222 0a20  pageshadow="2". 
+00000a60: 2020 2020 696e 6b73 6361 7065 3a7a 6f6f      inkscape:zoo
+00000a70: 6d3d 2232 2e32 3222 0a20 2020 2020 696e  m="2.22".     in
+00000a80: 6b73 6361 7065 3a63 783d 2232 3530 220a  kscape:cx="250".
+00000a90: 2020 2020 2069 6e6b 7363 6170 653a 6379       inkscape:cy
+00000aa0: 3d22 3530 220a 2020 2020 2069 6e6b 7363  ="50".     inksc
+00000ab0: 6170 653a 646f 6375 6d65 6e74 2d75 6e69  ape:document-uni
+00000ac0: 7473 3d22 7078 220a 2020 2020 2069 6e6b  ts="px".     ink
+00000ad0: 7363 6170 653a 6375 7272 656e 742d 6c61  scape:current-la
+00000ae0: 7965 723d 226c 6179 6572 3122 0a20 2020  yer="layer1".   
+00000af0: 2020 7368 6f77 6772 6964 3d22 6661 6c73    showgrid="fals
+00000b00: 6522 0a20 2020 2020 696e 6b73 6361 7065  e".     inkscape
+00000b10: 3a77 696e 646f 772d 7769 6474 683d 2231  :window-width="1
+00000b20: 3537 3522 0a20 2020 2020 696e 6b73 6361  575".     inksca
+00000b30: 7065 3a77 696e 646f 772d 6865 6967 6874  pe:window-height
+00000b40: 3d22 3838 3022 0a20 2020 2020 696e 6b73  ="880".     inks
+00000b50: 6361 7065 3a77 696e 646f 772d 783d 2232  cape:window-x="2
+00000b60: 3322 0a20 2020 2020 696e 6b73 6361 7065  3".     inkscape
+00000b70: 3a77 696e 646f 772d 793d 222d 3322 0a20  :window-y="-3". 
+00000b80: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+00000b90: 646f 772d 6d61 7869 6d69 7a65 643d 2231  dow-maximized="1
+00000ba0: 2220 2f3e 0a20 203c 6d65 7461 6461 7461  " />.  <metadata
+00000bb0: 0a20 2020 2020 6964 3d22 6d65 7461 6461  .     id="metada
+00000bc0: 7461 3722 3e0a 2020 2020 3c72 6466 3a52  ta7">.    <rdf:R
+00000bd0: 4446 3e0a 2020 2020 2020 3c63 633a 576f  DF>.      <cc:Wo
+00000be0: 726b 0a20 2020 2020 2020 2020 7264 663a  rk.         rdf:
+00000bf0: 6162 6f75 743d 2222 3e0a 2020 2020 2020  about="">.      
+00000c00: 2020 3c64 633a 666f 726d 6174 3e69 6d61    <dc:format>ima
+00000c10: 6765 2f73 7667 2b78 6d6c 3c2f 6463 3a66  ge/svg+xml</dc:f
+00000c20: 6f72 6d61 743e 0a20 2020 2020 2020 203c  ormat>.        <
+00000c30: 6463 3a74 7970 650a 2020 2020 2020 2020  dc:type.        
+00000c40: 2020 2072 6466 3a72 6573 6f75 7263 653d     rdf:resource=
+00000c50: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
+00000c60: 2f64 632f 6463 6d69 7479 7065 2f53 7469  /dc/dcmitype/Sti
+00000c70: 6c6c 496d 6167 6522 202f 3e0a 2020 2020  llImage" />.    
+00000c80: 2020 2020 3c64 633a 7469 746c 653e 3c2f      <dc:title></
+00000c90: 6463 3a74 6974 6c65 3e0a 2020 2020 2020  dc:title>.      
+00000ca0: 3c2f 6363 3a57 6f72 6b3e 0a20 2020 203c  </cc:Work>.    <
+00000cb0: 2f72 6466 3a52 4446 3e0a 2020 3c2f 6d65  /rdf:RDF>.  </me
+00000cc0: 7461 6461 7461 3e0a 2020 3c67 0a20 2020  tadata>.  <g.   
+00000cd0: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
+00000ce0: 3d22 4c61 7965 7220 3122 0a20 2020 2020  ="Layer 1".     
+00000cf0: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
+00000d00: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
+00000d10: 6964 3d22 6c61 7965 7231 220a 2020 2020  id="layer1".    
+00000d20: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00000d30: 736c 6174 6528 302c 2d39 3532 2e33 3632  slate(0,-952.362
+00000d40: 3138 2922 3e0a 2020 2020 3c67 0a20 2020  18)">.    <g.   
+00000d50: 2020 2020 6964 3d22 6733 3834 3822 0a20      id="g3848". 
+00000d60: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+00000d70: 2274 7261 6e73 6c61 7465 282d 3136 2c30  "translate(-16,0
+00000d80: 2922 3e0a 2020 2020 2020 3c70 6174 680a  )">.      <path.
+00000d90: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000da0: 6f70 6163 6974 793a 302e 353b 6669 6c6c  opacity:0.5;fill
+00000db0: 3a6e 6f6e 653b 7374 726f 6b65 3a23 3030  :none;stroke:#00
+00000dc0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+00000dd0: 683a 3170 783b 7374 726f 6b65 2d6c 696e  h:1px;stroke-lin
+00000de0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00000df0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00000e00: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00000e10: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
+00000e20: 3732 2e39 3334 3937 382c 3937 322e 3030  72.934978,972.00
+00000e30: 3336 3520 2d31 2e39 3737 3136 2c33 342e  365 -1.97716,34.
+00000e40: 3731 3030 3522 0a20 2020 2020 2020 2020  71005".         
+00000e50: 6964 3d22 7061 7468 3337 3831 220a 2020  id="path3781".  
+00000e60: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00000e70: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00000e80: 7572 653d 2230 2220 2f3e 0a20 2020 2020  ure="0" />.     
+00000e90: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+00000ea0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00000eb0: 6c61 7465 2830 2c39 3532 2e33 3632 3138  late(0,952.36218
+00000ec0: 2922 0a20 2020 2020 2020 2020 643d 226d  )".         d="m
+00000ed0: 2035 322e 3434 3333 3835 2c33 352e 3034   52.443385,35.04
+00000ee0: 3137 3138 2063 2030 2c33 2e32 3931 3332  1718 c 0,3.29132
+00000ef0: 3720 2d32 2e36 3638 3134 382c 352e 3935  7 -2.668148,5.95
+00000f00: 3934 3735 202d 352e 3935 3934 3735 2c35  9475 -5.959475,5
+00000f10: 2e39 3539 3437 3520 2d33 2e32 3931 3332  .959475 -3.29132
+00000f20: 382c 3020 2d35 2e39 3539 3437 362c 2d32  8,0 -5.959476,-2
+00000f30: 2e36 3638 3134 3820 2d35 2e39 3539 3437  .668148 -5.95947
+00000f40: 362c 2d35 2e39 3539 3437 3520 302c 2d33  6,-5.959475 0,-3
+00000f50: 2e32 3931 3332 3820 322e 3636 3831 3438  .291328 2.668148
+00000f60: 2c2d 352e 3935 3934 3736 2035 2e39 3539  ,-5.959476 5.959
+00000f70: 3437 362c 2d35 2e39 3539 3437 3620 332e  476,-5.959476 3.
+00000f80: 3239 3133 3237 2c30 2035 2e39 3539 3437  291327,0 5.95947
+00000f90: 352c 322e 3636 3831 3438 2035 2e39 3539  5,2.668148 5.959
+00000fa0: 3437 352c 352e 3935 3934 3736 207a 220a  475,5.959476 z".
+00000fb0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00000fc0: 693a 7279 3d22 352e 3935 3934 3735 3522  i:ry="5.9594755"
+00000fd0: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
+00000fe0: 6469 3a72 783d 2235 2e39 3539 3437 3535  di:rx="5.9594755
+00000ff0: 220a 2020 2020 2020 2020 2073 6f64 6970  ".         sodip
+00001000: 6f64 693a 6379 3d22 3335 2e30 3431 3731  odi:cy="35.04171
+00001010: 3822 0a20 2020 2020 2020 2020 736f 6469  8".         sodi
+00001020: 706f 6469 3a63 783d 2234 362e 3438 3339  podi:cx="46.4839
+00001030: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
+00001040: 7061 7468 3239 3835 220a 2020 2020 2020  path2985".      
+00001050: 2020 2073 7479 6c65 3d22 6669 6c6c 3a75     style="fill:u
+00001060: 726c 2823 7261 6469 616c 4772 6164 6965  rl(#radialGradie
+00001070: 6e74 3338 3636 293b 6669 6c6c 2d6f 7061  nt3866);fill-opa
+00001080: 6369 7479 3a31 3b73 7472 6f6b 653a 2330  city:1;stroke:#0
+00001090: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+000010a0: 7468 3a31 3b73 7472 6f6b 652d 6c69 6e65  th:1;stroke-line
+000010b0: 6a6f 696e 3a72 6f75 6e64 3b73 7472 6f6b  join:round;strok
+000010c0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+000010d0: 7472 6f6b 652d 6f70 6163 6974 793a 313b  troke-opacity:1;
+000010e0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000010f0: 3a6e 6f6e 6522 0a20 2020 2020 2020 2020  :none".         
+00001100: 736f 6469 706f 6469 3a74 7970 653d 2261  sodipodi:type="a
+00001110: 7263 2220 2f3e 0a20 2020 2020 203c 7061  rc" />.      <pa
+00001120: 7468 0a20 2020 2020 2020 2020 736f 6469  th.         sodi
+00001130: 706f 6469 3a74 7970 653d 2261 7263 220a  podi:type="arc".
+00001140: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001150: 6669 6c6c 3a75 726c 2823 7261 6469 616c  fill:url(#radial
+00001160: 4772 6164 6965 6e74 3338 3638 293b 6669  Gradient3868);fi
+00001170: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00001180: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00001190: 6b65 2d77 6964 7468 3a31 3b73 7472 6f6b  ke-width:1;strok
+000011a0: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
+000011b0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+000011c0: 6974 3a34 3b73 7472 6f6b 652d 6f70 6163  it:4;stroke-opac
+000011d0: 6974 793a 313b 7374 726f 6b65 2d64 6173  ity:1;stroke-das
+000011e0: 6861 7272 6179 3a6e 6f6e 6522 0a20 2020  harray:none".   
+000011f0: 2020 2020 2020 6964 3d22 7061 7468 3337        id="path37
+00001200: 3633 220a 2020 2020 2020 2020 2073 6f64  63".         sod
+00001210: 6970 6f64 693a 6378 3d22 3436 2e34 3833  ipodi:cx="46.483
+00001220: 3931 220a 2020 2020 2020 2020 2073 6f64  91".         sod
+00001230: 6970 6f64 693a 6379 3d22 3335 2e30 3431  ipodi:cy="35.041
+00001240: 3731 3822 0a20 2020 2020 2020 2020 736f  718".         so
+00001250: 6469 706f 6469 3a72 783d 2235 2e39 3539  dipodi:rx="5.959
+00001260: 3437 3535 220a 2020 2020 2020 2020 2073  4755".         s
+00001270: 6f64 6970 6f64 693a 7279 3d22 352e 3935  odipodi:ry="5.95
+00001280: 3934 3735 3522 0a20 2020 2020 2020 2020  94755".         
+00001290: 643d 226d 2035 322e 3434 3333 3835 2c33  d="m 52.443385,3
+000012a0: 352e 3034 3137 3138 2063 2030 2c33 2e32  5.041718 c 0,3.2
+000012b0: 3931 3332 3720 2d32 2e36 3638 3134 382c  91327 -2.668148,
+000012c0: 352e 3935 3934 3735 202d 352e 3935 3934  5.959475 -5.9594
+000012d0: 3735 2c35 2e39 3539 3437 3520 2d33 2e32  75,5.959475 -3.2
+000012e0: 3931 3332 382c 3020 2d35 2e39 3539 3437  91328,0 -5.95947
+000012f0: 362c 2d32 2e36 3638 3134 3820 2d35 2e39  6,-2.668148 -5.9
+00001300: 3539 3437 362c 2d35 2e39 3539 3437 3520  59476,-5.959475 
+00001310: 302c 2d33 2e32 3931 3332 3820 322e 3636  0,-3.291328 2.66
+00001320: 3831 3438 2c2d 352e 3935 3934 3736 2035  8148,-5.959476 5
+00001330: 2e39 3539 3437 362c 2d35 2e39 3539 3437  .959476,-5.95947
+00001340: 3620 332e 3239 3133 3237 2c30 2035 2e39  6 3.291327,0 5.9
+00001350: 3539 3437 352c 322e 3636 3831 3438 2035  59475,2.668148 5
+00001360: 2e39 3539 3437 352c 352e 3935 3934 3736  .959475,5.959476
+00001370: 207a 220a 2020 2020 2020 2020 2074 7261   z".         tra
+00001380: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00001390: 6528 3736 2e30 3130 3534 352c 3934 322e  e(76.010545,942.
+000013a0: 3033 3730 3529 2220 2f3e 0a20 2020 2020  03705)" />.     
+000013b0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+000013c0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+000013d0: 6c61 7465 2834 372e 3435 3136 372c 3939  late(47.45167,99
+000013e0: 362e 3738 3339 3729 220a 2020 2020 2020  6.78397)".      
+000013f0: 2020 2064 3d22 6d20 3532 2e34 3433 3338     d="m 52.44338
+00001400: 352c 3335 2e30 3431 3731 3820 6320 302c  5,35.041718 c 0,
+00001410: 332e 3239 3133 3237 202d 322e 3636 3831  3.291327 -2.6681
+00001420: 3438 2c35 2e39 3539 3437 3520 2d35 2e39  48,5.959475 -5.9
+00001430: 3539 3437 352c 352e 3935 3934 3735 202d  59475,5.959475 -
+00001440: 332e 3239 3133 3238 2c30 202d 352e 3935  3.291328,0 -5.95
+00001450: 3934 3736 2c2d 322e 3636 3831 3438 202d  9476,-2.668148 -
+00001460: 352e 3935 3934 3736 2c2d 352e 3935 3934  5.959476,-5.9594
+00001470: 3735 2030 2c2d 332e 3239 3133 3238 2032  75 0,-3.291328 2
+00001480: 2e36 3638 3134 382c 2d35 2e39 3539 3437  .668148,-5.95947
+00001490: 3620 352e 3935 3934 3736 2c2d 352e 3935  6 5.959476,-5.95
+000014a0: 3934 3736 2033 2e32 3931 3332 372c 3020  9476 3.291327,0 
+000014b0: 352e 3935 3934 3735 2c32 2e36 3638 3134  5.959475,2.66814
+000014c0: 3820 352e 3935 3934 3735 2c35 2e39 3539  8 5.959475,5.959
+000014d0: 3437 3620 7a22 0a20 2020 2020 2020 2020  476 z".         
+000014e0: 736f 6469 706f 6469 3a72 793d 2235 2e39  sodipodi:ry="5.9
+000014f0: 3539 3437 3535 220a 2020 2020 2020 2020  594755".        
+00001500: 2073 6f64 6970 6f64 693a 7278 3d22 352e   sodipodi:rx="5.
+00001510: 3935 3934 3735 3522 0a20 2020 2020 2020  9594755".       
+00001520: 2020 736f 6469 706f 6469 3a63 793d 2233    sodipodi:cy="3
+00001530: 352e 3034 3137 3138 220a 2020 2020 2020  5.041718".      
+00001540: 2020 2073 6f64 6970 6f64 693a 6378 3d22     sodipodi:cx="
+00001550: 3436 2e34 3833 3931 220a 2020 2020 2020  46.48391".      
+00001560: 2020 2069 643d 2270 6174 6833 3736 3722     id="path3767"
+00001570: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00001580: 2266 696c 6c3a 7572 6c28 2372 6164 6961  "fill:url(#radia
+00001590: 6c47 7261 6469 656e 7433 3837 3029 3b66  lGradient3870);f
+000015a0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+000015b0: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
+000015c0: 6f6b 652d 7769 6474 683a 313b 7374 726f  oke-width:1;stro
+000015d0: 6b65 2d6c 696e 656a 6f69 6e3a 726f 756e  ke-linejoin:roun
+000015e0: 643b 7374 726f 6b65 2d6d 6974 6572 6c69  d;stroke-miterli
+000015f0: 6d69 743a 343b 7374 726f 6b65 2d6f 7061  mit:4;stroke-opa
+00001600: 6369 7479 3a31 3b73 7472 6f6b 652d 6461  city:1;stroke-da
+00001610: 7368 6172 7261 793a 6e6f 6e65 220a 2020  sharray:none".  
+00001620: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00001630: 7479 7065 3d22 6172 6322 202f 3e0a 2020  type="arc" />.  
+00001640: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00001650: 2020 2073 6f64 6970 6f64 693a 7479 7065     sodipodi:type
+00001660: 3d22 6172 6322 0a20 2020 2020 2020 2020  ="arc".         
+00001670: 7374 796c 653d 226f 7061 6369 7479 3a30  style="opacity:0
+00001680: 2e35 3b66 696c 6c3a 7572 6c28 2372 6164  .5;fill:url(#rad
+00001690: 6961 6c47 7261 6469 656e 7433 3837 3229  ialGradient3872)
+000016a0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+000016b0: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+000016c0: 7472 6f6b 652d 7769 6474 683a 313b 7374  troke-width:1;st
+000016d0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
+000016e0: 756e 643b 7374 726f 6b65 2d6d 6974 6572  und;stroke-miter
+000016f0: 6c69 6d69 743a 343b 7374 726f 6b65 2d6f  limit:4;stroke-o
+00001700: 7061 6369 7479 3a31 3b73 7472 6f6b 652d  pacity:1;stroke-
+00001710: 6461 7368 6172 7261 793a 6e6f 6e65 220a  dasharray:none".
+00001720: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00001730: 6833 3737 3122 0a20 2020 2020 2020 2020  h3771".         
+00001740: 736f 6469 706f 6469 3a63 783d 2234 362e  sodipodi:cx="46.
+00001750: 3438 3339 3122 0a20 2020 2020 2020 2020  48391".         
+00001760: 736f 6469 706f 6469 3a63 793d 2233 352e  sodipodi:cy="35.
+00001770: 3034 3137 3138 220a 2020 2020 2020 2020  041718".        
+00001780: 2073 6f64 6970 6f64 693a 7278 3d22 352e   sodipodi:rx="5.
+00001790: 3935 3934 3735 3522 0a20 2020 2020 2020  9594755".       
+000017a0: 2020 736f 6469 706f 6469 3a72 793d 2235    sodipodi:ry="5
+000017b0: 2e39 3539 3437 3535 220a 2020 2020 2020  .9594755".      
+000017c0: 2020 2064 3d22 6d20 3532 2e34 3433 3338     d="m 52.44338
+000017d0: 352c 3335 2e30 3431 3731 3820 6320 302c  5,35.041718 c 0,
+000017e0: 332e 3239 3133 3237 202d 322e 3636 3831  3.291327 -2.6681
+000017f0: 3438 2c35 2e39 3539 3437 3520 2d35 2e39  48,5.959475 -5.9
+00001800: 3539 3437 352c 352e 3935 3934 3735 202d  59475,5.959475 -
+00001810: 332e 3239 3133 3238 2c30 202d 352e 3935  3.291328,0 -5.95
+00001820: 3934 3736 2c2d 322e 3636 3831 3438 202d  9476,-2.668148 -
+00001830: 352e 3935 3934 3736 2c2d 352e 3935 3934  5.959476,-5.9594
+00001840: 3735 2030 2c2d 332e 3239 3133 3238 2032  75 0,-3.291328 2
+00001850: 2e36 3638 3134 382c 2d35 2e39 3539 3437  .668148,-5.95947
+00001860: 3620 352e 3935 3934 3736 2c2d 352e 3935  6 5.959476,-5.95
+00001870: 3934 3736 2033 2e32 3931 3332 372c 3020  9476 3.291327,0 
+00001880: 352e 3935 3934 3735 2c32 2e36 3638 3134  5.959475,2.66814
+00001890: 3820 352e 3935 3934 3735 2c35 2e39 3539  8 5.959475,5.959
+000018a0: 3437 3620 7a22 0a20 2020 2020 2020 2020  476 z".         
+000018b0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+000018c0: 6c61 7465 2832 332e 3934 3535 3139 2c39  late(23.945519,9
+000018d0: 3737 2e32 3332 3132 2922 202f 3e0a 2020  77.23212)" />.  
+000018e0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+000018f0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00001900: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00001910: 2230 220a 2020 2020 2020 2020 2069 643d  "0".         id=
+00001920: 2270 6174 6833 3737 3522 0a20 2020 2020  "path3775".     
+00001930: 2020 2020 643d 224d 2034 352e 3931 3338      d="M 45.9138
+00001940: 3834 2c39 3933 2e34 3836 3936 2034 332e  84,993.48696 43.
+00001950: 3933 3637 3331 2c31 3032 382e 3139 3722  936731,1028.197"
+00001960: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00001970: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
+00001980: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
+00001990: 2d77 6964 7468 3a31 7078 3b73 7472 6f6b  -width:1px;strok
+000019a0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+000019b0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+000019c0: 6974 6572 3b73 7472 6f6b 652d 6f70 6163  iter;stroke-opac
+000019d0: 6974 793a 3122 202f 3e0a 2020 2020 2020  ity:1" />.      
+000019e0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+000019f0: 7479 6c65 3d22 6669 6c6c 3a6e 6f6e 653b  tyle="fill:none;
+00001a00: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+00001a10: 7472 6f6b 652d 7769 6474 683a 3170 783b  troke-width:1px;
+00001a20: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00001a30: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00001a40: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00001a50: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001a60: 2020 2020 2064 3d22 6d20 3936 2e32 3231       d="m 96.221
+00001a70: 3434 312c 3939 312e 3535 3535 202d 312e  441,991.5555 -1.
+00001a80: 3937 3731 3533 2c33 342e 3731 220a 2020  977153,34.71".  
+00001a90: 2020 2020 2020 2069 643d 2270 6174 6833         id="path3
+00001aa0: 3737 3722 0a20 2020 2020 2020 2020 696e  777".         in
+00001ab0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00001ac0: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00001ad0: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+00001ae0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00001af0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00001b00: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+00001b10: 2069 643d 2270 6174 6833 3737 3922 0a20   id="path3779". 
+00001b20: 2020 2020 2020 2020 643d 226d 2031 3232          d="m 122
+00001b30: 2e33 3633 382c 3938 332e 3338 3135 3120  .3638,983.38151 
+00001b40: 2d31 2e39 3737 3136 2c33 342e 3730 3939  -1.97716,34.7099
+00001b50: 3922 0a20 2020 2020 2020 2020 7374 796c  9".         styl
+00001b60: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
+00001b70: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00001b80: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
+00001b90: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00001ba0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00001bb0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+00001bc0: 6163 6974 793a 3122 202f 3e0a 2020 2020  acity:1" />.    
+00001bd0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00001be0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00001bf0: 736c 6174 6528 302c 3935 322e 3336 3231  slate(0,952.3621
+00001c00: 3829 220a 2020 2020 2020 2020 2069 6e6b  8)".         ink
+00001c10: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00001c20: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00001c30: 2020 2020 2020 2069 643d 2270 6174 6833         id="path3
+00001c40: 3738 3322 0a20 2020 2020 2020 2020 643d  783".         d=
+00001c50: 226d 2034 342e 3135 3634 3135 2c37 352e  "m 44.156415,75.
+00001c60: 3339 3534 3331 2034 332e 3439 3733 3634  395431 43.497364
+00001c70: 2c33 2e39 3534 3330 3522 0a20 2020 2020  ,3.954305".     
+00001c80: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00001c90: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
+00001ca0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00001cb0: 3a31 7078 3b73 7472 6f6b 652d 6c69 6e65  :1px;stroke-line
+00001cc0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00001cd0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00001ce0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00001cf0: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00001d00: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001d10: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+00001d20: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00001d30: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
+00001d40: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00001d50: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00001d60: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+00001d70: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00001d80: 3d22 6d20 3732 2e37 3135 3239 2c39 3732  ="m 72.71529,972
+00001d90: 2e33 3937 3333 2034 332e 3439 3733 362c  .39733 43.49736,
+00001da0: 332e 3935 3433 220a 2020 2020 2020 2020  3.9543".        
+00001db0: 2069 643d 2270 6174 6833 3738 3522 0a20   id="path3785". 
+00001dc0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00001dd0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00001de0: 7475 7265 3d22 3022 202f 3e0a 2020 2020  ture="0" />.    
+00001df0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00001e00: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+00001e10: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00001e20: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00001e30: 6174 6833 3738 3722 0a20 2020 2020 2020  ath3787".       
+00001e40: 2020 643d 226d 2037 362e 3434 3939 3132    d="m 76.449912
+00001e50: 2c31 3031 332e 3437 3832 2034 332e 3439  ,1013.4782 43.49
+00001e60: 3733 3538 2c33 2e39 3534 3322 0a20 2020  7358,3.9543".   
+00001e70: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00001e80: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
+00001e90: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00001ea0: 7468 3a31 7078 3b73 7472 6f6b 652d 6c69  th:1px;stroke-li
+00001eb0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00001ec0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00001ed0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00001ee0: 3122 202f 3e0a 2020 2020 2020 3c70 6174  1" />.      <pat
+00001ef0: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00001f00: 3d22 6669 6c6c 3a6e 6f6e 653b 7374 726f  ="fill:none;stro
+00001f10: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+00001f20: 652d 7769 6474 683a 3170 783b 7374 726f  e-width:1px;stro
+00001f30: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00001f40: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00001f50: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+00001f60: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00001f70: 2064 3d22 6d20 3532 2e35 3034 3339 342c   d="m 52.504394,
+00001f80: 3938 372e 3939 3438 3720 3433 2e34 3937  987.99487 43.497
+00001f90: 3336 342c 332e 3935 3433 220a 2020 2020  364,3.9543".    
+00001fa0: 2020 2020 2069 643d 2270 6174 6833 3738       id="path378
+00001fb0: 3922 0a20 2020 2020 2020 2020 696e 6b73  9".         inks
+00001fc0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00001fd0: 7572 7661 7475 7265 3d22 3022 202f 3e0a  urvature="0" />.
+00001fe0: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00001ff0: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+00002000: 7472 616e 736c 6174 6528 302c 3935 322e  translate(0,952.
+00002010: 3336 3231 3829 220a 2020 2020 2020 2020  36218)".        
+00002020: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+00002030: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00002040: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00002050: 6174 6833 3739 3122 0a20 2020 2020 2020  ath3791".       
+00002060: 2020 643d 224d 2034 342e 3135 3634 3135    d="M 44.156415
+00002070: 2c37 352e 3137 3537 3437 2036 352e 3436  ,75.175747 65.46
+00002080: 3537 3239 2c36 332e 3533 3235 3133 220a  5729,63.532513".
+00002090: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+000020a0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+000020b0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+000020c0: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
+000020d0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+000020e0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+000020f0: 7465 723b 7374 726f 6b65 2d6f 7061 6369  ter;stroke-opaci
+00002100: 7479 3a31 2220 2f3e 0a20 2020 2020 203c  ty:1" />.      <
+00002110: 7061 7468 0a20 2020 2020 2020 2020 7374  path.         st
+00002120: 796c 653d 2266 696c 6c3a 6e6f 6e65 3b73  yle="fill:none;s
+00002130: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+00002140: 726f 6b65 2d77 6964 7468 3a31 7078 3b73  roke-width:1px;s
+00002150: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00002160: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00002170: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00002180: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00002190: 2020 2020 643d 224d 2035 312e 3430 3539      d="M 51.4059
+000021a0: 3736 2c39 3834 2e30 3430 3536 2037 322e  76,984.04056 72.
+000021b0: 3731 3532 392c 3937 322e 3339 3733 3322  71529,972.39733"
+000021c0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+000021d0: 7468 3337 3933 220a 2020 2020 2020 2020  th3793".        
+000021e0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+000021f0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00002200: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+00002210: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00002220: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00002230: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+00002240: 2020 2020 6964 3d22 7061 7468 3337 3935      id="path3795
+00002250: 220a 2020 2020 2020 2020 2064 3d22 4d20  ".         d="M 
+00002260: 3936 2e32 3231 3434 322c 3939 322e 3136  96.221442,992.16
+00002270: 3838 3620 3131 372e 3533 3037 362c 3938  886 117.53076,98
+00002280: 302e 3532 3536 3322 0a20 2020 2020 2020  0.52563".       
+00002290: 2020 7374 796c 653d 2266 696c 6c3a 6e6f    style="fill:no
+000022a0: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
+000022b0: 303b 7374 726f 6b65 2d77 6964 7468 3a31  0;stroke-width:1
+000022c0: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
+000022d0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+000022e0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+000022f0: 6f6b 652d 6f70 6163 6974 793a 3122 202f  oke-opacity:1" /
+00002300: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+00002310: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00002320: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
+00002330: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
+00002340: 6474 683a 3170 783b 7374 726f 6b65 2d6c  dth:1px;stroke-l
+00002350: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00002360: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00002370: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
+00002380: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+00002390: 6d20 3939 2e30 3737 3333 2c31 3032 392e  m 99.07733,1029.
+000023a0: 3037 3537 2032 312e 3330 3933 322c 2d31  0757 21.30932,-1
+000023b0: 312e 3634 3332 220a 2020 2020 2020 2020  1.6432".        
+000023c0: 2069 643d 2270 6174 6833 3739 3722 0a20   id="path3797". 
+000023d0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+000023e0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+000023f0: 7475 7265 3d22 3022 202f 3e0a 2020 2020  ture="0" />.    
+00002400: 3c2f 673e 0a20 2020 203c 7465 7874 0a20  </g>.    <text. 
+00002410: 2020 2020 2020 786d 6c3a 7370 6163 653d        xml:space=
+00002420: 2270 7265 7365 7276 6522 0a20 2020 2020  "preserve".     
+00002430: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
+00002440: 7a65 3a34 3070 783b 666f 6e74 2d73 7479  ze:40px;font-sty
+00002450: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
+00002460: 6569 6768 743a 6e6f 726d 616c 3b6c 696e  eight:normal;lin
+00002470: 652d 6865 6967 6874 3a31 3235 253b 6c65  e-height:125%;le
+00002480: 7474 6572 2d73 7061 6369 6e67 3a30 7078  tter-spacing:0px
+00002490: 3b77 6f72 642d 7370 6163 696e 673a 3070  ;word-spacing:0p
+000024a0: 783b 6669 6c6c 3a23 3030 3030 3030 3b66  x;fill:#000000;f
+000024b0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+000024c0: 726f 6b65 3a6e 6f6e 653b 666f 6e74 2d66  roke:none;font-f
+000024d0: 616d 696c 793a 5361 6e73 220a 2020 2020  amily:Sans".    
+000024e0: 2020 2078 3d22 3135 382e 3938 3433 3822     x="158.98438"
+000024f0: 0a20 2020 2020 2020 793d 2231 3031 302e  .       y="1010.
+00002500: 3631 3232 220a 2020 2020 2020 2069 643d  6122".       id=
+00002510: 2274 6578 7433 3739 3922 0a20 2020 2020  "text3799".     
+00002520: 2020 736f 6469 706f 6469 3a6c 696e 6573    sodipodi:lines
+00002530: 7061 6369 6e67 3d22 3132 3525 223e 3c74  pacing="125%"><t
+00002540: 7370 616e 0a20 2020 2020 2020 2020 736f  span.         so
+00002550: 6469 706f 6469 3a72 6f6c 653d 226c 696e  dipodi:role="lin
+00002560: 6522 0a20 2020 2020 2020 2020 6964 3d22  e".         id="
+00002570: 7473 7061 6e33 3830 3122 0a20 2020 2020  tspan3801".     
+00002580: 2020 2020 783d 2231 3538 2e39 3834 3338      x="158.98438
+00002590: 220a 2020 2020 2020 2020 2079 3d22 3130  ".         y="10
+000025a0: 3130 2e36 3132 3222 0a20 2020 2020 2020  10.6122".       
+000025b0: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
+000025c0: 7a65 3a36 3470 783b 666f 6e74 2d73 7479  ze:64px;font-sty
+000025d0: 6c65 3a69 7461 6c69 633b 666f 6e74 2d76  le:italic;font-v
+000025e0: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
+000025f0: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
+00002600: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
+00002610: 726d 616c 3b66 6f6e 742d 6661 6d69 6c79  rmal;font-family
+00002620: 3a52 6f62 6f74 6f3b 2d69 6e6b 7363 6170  :Roboto;-inkscap
+00002630: 652d 666f 6e74 2d73 7065 6369 6669 6361  e-font-specifica
+00002640: 7469 6f6e 3a52 6f62 6f74 6f20 4974 616c  tion:Roboto Ital
+00002650: 6963 223e 7079 444f 4533 3c2f 7473 7061  ic">pyDOE3</tspa
+00002660: 6e3e 3c2f 7465 7874 3e0a 2020 2020 3c67  n></text>.    <g
+00002670: 0a20 2020 2020 2020 6964 3d22 6733 3831  .       id="g381
+00002680: 3922 0a20 2020 2020 2020 7472 616e 7366  9".       transf
+00002690: 6f72 6d3d 226d 6174 7269 7828 312e 3038  orm="matrix(1.08
+000026a0: 3232 3031 312c 2d30 2e32 3139 3631 3430  22011,-0.2196140
+000026b0: 372c 302e 3231 3936 3134 3037 2c31 2e30  7,0.21961407,1.0
+000026c0: 3832 3230 3131 2c2d 3234 312e 3038 3238  822011,-241.0828
+000026d0: 362c 3132 2e34 3036 3630 3629 220a 2020  6,12.406606)".  
+000026e0: 2020 2020 2073 7479 6c65 3d22 6f70 6163       style="opac
+000026f0: 6974 793a 302e 3735 3b66 696c 6c3a 2330  ity:0.75;fill:#0
+00002700: 3030 3030 303b 6669 6c6c 2d6f 7061 6369  00000;fill-opaci
+00002710: 7479 3a31 223e 0a20 2020 2020 203c 7465  ty:1">.      <te
+00002720: 7874 0a20 2020 2020 2020 2020 736f 6469  xt.         sodi
+00002730: 706f 6469 3a6c 696e 6573 7061 6369 6e67  podi:linespacing
+00002740: 3d22 3132 3525 220a 2020 2020 2020 2020  ="125%".        
+00002750: 2069 643d 2274 6578 7433 3830 3322 0a20   id="text3803". 
+00002760: 2020 2020 2020 2020 793d 2239 3636 2e39          y="966.9
+00002770: 3839 3522 0a20 2020 2020 2020 2020 783d  895".         x=
+00002780: 2234 3031 2e30 3037 3137 220a 2020 2020  "401.00717".    
+00002790: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
+000027a0: 2d73 697a 653a 3230 2e30 3434 3535 3536  -size:20.0445556
+000027b0: 3670 783b 666f 6e74 2d73 7479 6c65 3a6e  6px;font-style:n
+000027c0: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
+000027d0: 743a 6e6f 726d 616c 3b6c 696e 652d 6865  t:normal;line-he
+000027e0: 6967 6874 3a31 3235 253b 6c65 7474 6572  ight:125%;letter
+000027f0: 2d73 7061 6369 6e67 3a30 7078 3b77 6f72  -spacing:0px;wor
+00002800: 642d 7370 6163 696e 673a 3070 783b 6669  d-spacing:0px;fi
+00002810: 6c6c 3a23 3030 3030 3030 3b66 696c 6c2d  ll:#000000;fill-
+00002820: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00002830: 3a6e 6f6e 653b 666f 6e74 2d66 616d 696c  :none;font-famil
+00002840: 793a 5361 6e73 220a 2020 2020 2020 2020  y:Sans".        
+00002850: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
+00002860: 6572 7665 223e 3c74 7370 616e 0a20 2020  erve"><tspan.   
+00002870: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00002880: 6f6e 742d 7369 7a65 3a31 3670 783b 666f  ont-size:16px;fo
+00002890: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
+000028a0: 666f 6e74 2d76 6172 6961 6e74 3a6e 6f72  font-variant:nor
+000028b0: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
+000028c0: 626f 6c64 3b66 6f6e 742d 7374 7265 7463  bold;font-stretc
+000028d0: 683a 6e6f 726d 616c 3b66 696c 6c3a 2330  h:normal;fill:#0
+000028e0: 3030 3030 303b 6669 6c6c 2d6f 7061 6369  00000;fill-opaci
+000028f0: 7479 3a31 3b66 6f6e 742d 6661 6d69 6c79  ty:1;font-family
+00002900: 3a54 6558 2047 7972 6520 4375 7273 6f72  :TeX Gyre Cursor
+00002910: 3b2d 696e 6b73 6361 7065 2d66 6f6e 742d  ;-inkscape-font-
+00002920: 7370 6563 6966 6963 6174 696f 6e3a 5465  specification:Te
+00002930: 5820 4779 7265 2043 7572 736f 7220 426f  X Gyre Cursor Bo
+00002940: 6c64 220a 2020 2020 2020 2020 2020 2079  ld".           y
+00002950: 3d22 3936 362e 3938 3935 220a 2020 2020  ="966.9895".    
+00002960: 2020 2020 2020 2078 3d22 3430 312e 3030         x="401.00
+00002970: 3731 3722 0a20 2020 2020 2020 2020 2020  717".           
+00002980: 6964 3d22 7473 7061 6e33 3830 3522 0a20  id="tspan3805". 
+00002990: 2020 2020 2020 2020 2020 736f 6469 706f            sodipo
+000029a0: 6469 3a72 6f6c 653d 226c 696e 6522 3e41  di:role="line">A
+000029b0: 2042 2043 3c2f 7473 7061 6e3e 3c74 7370   B C</tspan><tsp
+000029c0: 616e 0a20 2020 2020 2020 2020 2020 7374  an.           st
+000029d0: 796c 653d 2266 6f6e 742d 7369 7a65 3a31  yle="font-size:1
+000029e0: 3670 783b 666f 6e74 2d73 7479 6c65 3a6e  6px;font-style:n
+000029f0: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
+00002a00: 6e74 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  nt:normal;font-w
+00002a10: 6569 6768 743a 626f 6c64 3b66 6f6e 742d  eight:bold;font-
+00002a20: 7374 7265 7463 683a 6e6f 726d 616c 3b66  stretch:normal;f
+00002a30: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
+00002a40: 2d6f 7061 6369 7479 3a31 3b66 6f6e 742d  -opacity:1;font-
+00002a50: 6661 6d69 6c79 3a54 6558 2047 7972 6520  family:TeX Gyre 
+00002a60: 4375 7273 6f72 3b2d 696e 6b73 6361 7065  Cursor;-inkscape
+00002a70: 2d66 6f6e 742d 7370 6563 6966 6963 6174  -font-specificat
+00002a80: 696f 6e3a 5465 5820 4779 7265 2043 7572  ion:TeX Gyre Cur
+00002a90: 736f 7220 426f 6c64 220a 2020 2020 2020  sor Bold".      
+00002aa0: 2020 2020 2069 643d 2274 7370 616e 3338       id="tspan38
+00002ab0: 3037 220a 2020 2020 2020 2020 2020 2079  07".           y
+00002ac0: 3d22 3938 362e 3938 3935 220a 2020 2020  ="986.9895".    
+00002ad0: 2020 2020 2020 2078 3d22 3430 312e 3030         x="401.00
+00002ae0: 3731 3722 0a20 2020 2020 2020 2020 2020  717".           
+00002af0: 736f 6469 706f 6469 3a72 6f6c 653d 226c  sodipodi:role="l
+00002b00: 696e 6522 3e30 2030 2031 3c2f 7473 7061  ine">0 0 1</tspa
+00002b10: 6e3e 3c74 7370 616e 0a20 2020 2020 2020  n><tspan.       
+00002b20: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
+00002b30: 7369 7a65 3a31 3670 783b 666f 6e74 2d73  size:16px;font-s
+00002b40: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
+00002b50: 2d76 6172 6961 6e74 3a6e 6f72 6d61 6c3b  -variant:normal;
+00002b60: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00002b70: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
+00002b80: 726d 616c 3b66 696c 6c3a 2330 3030 3030  rmal;fill:#00000
+00002b90: 303b 6669 6c6c 2d6f 7061 6369 7479 3a31  0;fill-opacity:1
+00002ba0: 3b66 6f6e 742d 6661 6d69 6c79 3a54 6558  ;font-family:TeX
+00002bb0: 2047 7972 6520 4375 7273 6f72 3b2d 696e   Gyre Cursor;-in
+00002bc0: 6b73 6361 7065 2d66 6f6e 742d 7370 6563  kscape-font-spec
+00002bd0: 6966 6963 6174 696f 6e3a 5465 5820 4779  ification:TeX Gy
+00002be0: 7265 2043 7572 736f 7220 426f 6c64 220a  re Cursor Bold".
+00002bf0: 2020 2020 2020 2020 2020 2069 643d 2274             id="t
+00002c00: 7370 616e 3338 3039 220a 2020 2020 2020  span3809".      
+00002c10: 2020 2020 2079 3d22 3130 3036 2e39 3839       y="1006.989
+00002c20: 3522 0a20 2020 2020 2020 2020 2020 783d  5".           x=
+00002c30: 2234 3031 2e30 3037 3137 220a 2020 2020  "401.00717".    
+00002c40: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00002c50: 726f 6c65 3d22 6c69 6e65 223e 3120 3020  role="line">1 0 
+00002c60: 303c 2f74 7370 616e 3e3c 7473 7061 6e0a  0</tspan><tspan.
+00002c70: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00002c80: 3d22 666f 6e74 2d73 697a 653a 3136 7078  ="font-size:16px
+00002c90: 3b66 6f6e 742d 7374 796c 653a 6e6f 726d  ;font-style:norm
+00002ca0: 616c 3b66 6f6e 742d 7661 7269 616e 743a  al;font-variant:
+00002cb0: 6e6f 726d 616c 3b66 6f6e 742d 7765 6967  normal;font-weig
+00002cc0: 6874 3a62 6f6c 643b 666f 6e74 2d73 7472  ht:bold;font-str
+00002cd0: 6574 6368 3a6e 6f72 6d61 6c3b 6669 6c6c  etch:normal;fill
+00002ce0: 3a23 3030 3030 3030 3b66 696c 6c2d 6f70  :#000000;fill-op
+00002cf0: 6163 6974 793a 313b 666f 6e74 2d66 616d  acity:1;font-fam
+00002d00: 696c 793a 5465 5820 4779 7265 2043 7572  ily:TeX Gyre Cur
+00002d10: 736f 723b 2d69 6e6b 7363 6170 652d 666f  sor;-inkscape-fo
+00002d20: 6e74 2d73 7065 6369 6669 6361 7469 6f6e  nt-specification
+00002d30: 3a54 6558 2047 7972 6520 4375 7273 6f72  :TeX Gyre Cursor
+00002d40: 2042 6f6c 6422 0a20 2020 2020 2020 2020   Bold".         
+00002d50: 2020 6964 3d22 7473 7061 6e33 3831 3122    id="tspan3811"
+00002d60: 0a20 2020 2020 2020 2020 2020 793d 2231  .           y="1
+00002d70: 3032 362e 3938 3935 220a 2020 2020 2020  026.9895".      
+00002d80: 2020 2020 2078 3d22 3430 312e 3030 3731       x="401.0071
+00002d90: 3722 0a20 2020 2020 2020 2020 2020 736f  7".           so
+00002da0: 6469 706f 6469 3a72 6f6c 653d 226c 696e  dipodi:role="lin
+00002db0: 6522 3e30 2031 2030 3c2f 7473 7061 6e3e  e">0 1 0</tspan>
+00002dc0: 3c74 7370 616e 0a20 2020 2020 2020 2020  <tspan.         
+00002dd0: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
+00002de0: 7a65 3a31 3670 783b 666f 6e74 2d73 7479  ze:16px;font-sty
+00002df0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
+00002e00: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
+00002e10: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
+00002e20: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
+00002e30: 616c 3b66 696c 6c3a 2330 3030 3030 303b  al;fill:#000000;
+00002e40: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b66  fill-opacity:1;f
+00002e50: 6f6e 742d 6661 6d69 6c79 3a54 6558 2047  ont-family:TeX G
+00002e60: 7972 6520 4375 7273 6f72 3b2d 696e 6b73  yre Cursor;-inks
+00002e70: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
+00002e80: 6963 6174 696f 6e3a 5465 5820 4779 7265  ication:TeX Gyre
+00002e90: 2043 7572 736f 7220 426f 6c64 220a 2020   Cursor Bold".  
+00002ea0: 2020 2020 2020 2020 2069 643d 2274 7370           id="tsp
+00002eb0: 616e 3338 3133 220a 2020 2020 2020 2020  an3813".        
+00002ec0: 2020 2079 3d22 3130 3436 2e39 3839 3522     y="1046.9895"
+00002ed0: 0a20 2020 2020 2020 2020 2020 783d 2234  .           x="4
+00002ee0: 3031 2e30 3037 3137 220a 2020 2020 2020  01.00717".      
+00002ef0: 2020 2020 2073 6f64 6970 6f64 693a 726f       sodipodi:ro
+00002f00: 6c65 3d22 6c69 6e65 223e 3120 3120 313c  le="line">1 1 1<
+00002f10: 2f74 7370 616e 3e3c 2f74 6578 743e 0a20  /tspan></text>. 
+00002f20: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
+00002f30: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+00002f40: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+00002f50: 3d22 3022 0a20 2020 2020 2020 2020 6964  ="0".         id
+00002f60: 3d22 7061 7468 3338 3137 220a 2020 2020  ="path3817".    
+00002f70: 2020 2020 2064 3d22 6d20 3339 362e 3936       d="m 396.96
+00002f80: 3833 362c 3937 312e 3037 3932 3320 3535  836,971.07923 55
+00002f90: 2e31 3430 362c 3022 0a20 2020 2020 2020  .1406,0".       
+00002fa0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
+00002fb0: 3030 3030 303b 6669 6c6c 2d6f 7061 6369  00000;fill-opaci
+00002fc0: 7479 3a31 3b73 7472 6f6b 653a 2330 3030  ty:1;stroke:#000
+00002fd0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00002fe0: 3a30 2e39 3035 3538 3339 3870 783b 7374  :0.90558398px;st
+00002ff0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00003000: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00003010: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6f  n:miter;stroke-o
+00003020: 7061 6369 7479 3a31 2220 2f3e 0a20 2020  pacity:1" />.   
+00003030: 203c 2f67 3e0a 2020 2020 3c74 6578 740a   </g>.    <text.
+00003040: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00003050: 6c69 6e65 7370 6163 696e 673d 2231 3235  linespacing="125
+00003060: 2522 0a20 2020 2020 2020 6964 3d22 7465  %".       id="te
+00003070: 7874 3338 3238 220a 2020 2020 2020 2079  xt3828".       y
+00003080: 3d22 3130 3434 2e33 3032 3722 0a20 2020  ="1044.3027".   
+00003090: 2020 2020 783d 2231 3136 2e38 3936 3731      x="116.89671
+000030a0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+000030b0: 666f 6e74 2d73 697a 653a 3338 2e31 3731  font-size:38.171
+000030c0: 3431 3334 3270 783b 666f 6e74 2d73 7479  41342px;font-sty
+000030d0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
+000030e0: 6569 6768 743a 6e6f 726d 616c 3b6c 696e  eight:normal;lin
+000030f0: 652d 6865 6967 6874 3a31 3235 253b 6c65  e-height:125%;le
+00003100: 7474 6572 2d73 7061 6369 6e67 3a30 7078  tter-spacing:0px
+00003110: 3b77 6f72 642d 7370 6163 696e 673a 3070  ;word-spacing:0p
+00003120: 783b 6669 6c6c 3a23 3030 3030 3030 3b66  x;fill:#000000;f
+00003130: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00003140: 726f 6b65 3a6e 6f6e 653b 666f 6e74 2d66  roke:none;font-f
+00003150: 616d 696c 793a 5361 6e73 220a 2020 2020  amily:Sans".    
+00003160: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
+00003170: 6573 6572 7665 223e 3c74 7370 616e 0a20  eserve"><tspan. 
+00003180: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00003190: 6f6e 742d 7369 7a65 3a31 392e 3038 3537  ont-size:19.0857
+000031a0: 3036 3731 7078 3b66 6f6e 742d 7374 796c  0671px;font-styl
+000031b0: 653a 6974 616c 6963 3b66 6f6e 742d 7661  e:italic;font-va
+000031c0: 7269 616e 743a 6e6f 726d 616c 3b66 6f6e  riant:normal;fon
+000031d0: 742d 7765 6967 6874 3a6e 6f72 6d61 6c3b  t-weight:normal;
+000031e0: 666f 6e74 2d73 7472 6574 6368 3a6e 6f72  font-stretch:nor
+000031f0: 6d61 6c3b 666f 6e74 2d66 616d 696c 793a  mal;font-family:
+00003200: 526f 626f 746f 3b2d 696e 6b73 6361 7065  Roboto;-inkscape
+00003210: 2d66 6f6e 742d 7370 6563 6966 6963 6174  -font-specificat
+00003220: 696f 6e3a 526f 626f 746f 2049 7461 6c69  ion:Roboto Itali
+00003230: 6322 0a20 2020 2020 2020 2020 793d 2231  c".         y="1
+00003240: 3034 342e 3330 3237 220a 2020 2020 2020  044.3027".      
+00003250: 2020 2078 3d22 3131 362e 3839 3637 3122     x="116.89671"
+00003260: 0a20 2020 2020 2020 2020 6964 3d22 7473  .         id="ts
+00003270: 7061 6e33 3833 3022 0a20 2020 2020 2020  pan3830".       
+00003280: 2020 736f 6469 706f 6469 3a72 6f6c 653d    sodipodi:role=
+00003290: 226c 696e 6522 3e44 6573 6967 6e20 6f66  "line">Design of
+000032a0: 2045 7870 6572 696d 656e 7473 2066 6f72   Experiments for
+000032b0: 2050 7974 686f 6e3c 2f74 7370 616e 3e3c   Python</tspan><
+000032c0: 2f74 6578 743e 0a20 2020 203c 670a 2020  /text>.    <g.  
+000032d0: 2020 2020 2069 643d 2267 3339 3231 220a       id="g3921".
+000032e0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000032f0: 3d22 7472 616e 736c 6174 6528 302c 2d30  ="translate(0,-0
+00003300: 2e39 3030 3930 3039 2922 3e0a 2020 2020  .9009009)">.    
+00003310: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00003320: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+00003330: 7065 733d 2263 7363 220a 2020 2020 2020  pes="csc".      
+00003340: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
+00003350: 616e 736c 6174 6528 302c 3935 322e 3336  anslate(0,952.36
+00003360: 3231 3829 220a 2020 2020 2020 2020 2069  218)".         i
+00003370: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00003380: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+00003390: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+000033a0: 6833 3839 3322 0a20 2020 2020 2020 2020  h3893".         
+000033b0: 643d 224d 2032 322e 3037 3230 3732 2c38  d="M 22.072072,8
+000033c0: 372e 3833 3738 3338 2043 2036 322e 3136  7.837838 C 62.16
+000033d0: 3231 3632 2c38 312e 3938 3139 3832 2037  2162,81.981982 7
+000033e0: 332e 3837 3338 3733 2c36 382e 3031 3830  3.873873,68.0180
+000033f0: 3138 2036 352e 3331 3533 3135 2c35 312e  18 65.315315,51.
+00003400: 3335 3133 3531 2035 362e 3735 3637 3538  351351 56.756758
+00003410: 2c33 342e 3638 3436 3834 2037 392e 3732  ,34.684684 79.72
+00003420: 3937 332c 3138 2e39 3138 3931 3920 3130  973,18.918919 10
+00003430: 322e 3235 3232 352c 3131 2e37 3131 3731  2.25225,11.71171
+00003440: 3222 0a20 2020 2020 2020 2020 7374 796c  2".         styl
+00003450: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
+00003460: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00003470: 6b65 2d77 6964 7468 3a34 3b73 7472 6f6b  ke-width:4;strok
+00003480: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00003490: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+000034a0: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+000034b0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+000034c0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+000034d0: 2d64 6173 6861 7272 6179 3a6e 6f6e 6522  -dasharray:none"
+000034e0: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+000034f0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00003500: 693a 6e6f 6465 7479 7065 733d 2263 7373  i:nodetypes="css
+00003510: 7373 6363 220a 2020 2020 2020 2020 2074  sscc".         t
+00003520: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00003530: 6174 6528 302c 3935 322e 3336 3231 3829  ate(0,952.36218)
+00003540: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00003550: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00003560: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00003570: 2020 2020 2069 643d 2270 6174 6833 3839       id="path389
+00003580: 3522 0a20 2020 2020 2020 2020 643d 226d  5".         d="m
+00003590: 2031 3032 2e35 3137 3335 2c39 2e33 3234   102.51735,9.324
+000035a0: 3037 3235 2063 2030 2c30 202d 3130 2e31  0725 c 0,0 -10.1
+000035b0: 3633 3535 312c 2d31 2e33 3338 3337 3537  63551,-1.3383757
+000035c0: 202d 3133 2e36 3637 3233 332c 302e 3431   -13.667233,0.41
+000035d0: 3334 3635 202d 332e 3530 3336 3833 2c31  3465 -3.503683,1
+000035e0: 2e37 3531 3834 3135 202d 322e 3830 3732  .7518415 -2.8072
+000035f0: 3536 2c33 2e35 3935 3236 3935 202d 332e  56,3.5952695 -3.
+00003600: 3433 3933 3733 2c36 2e35 3139 3932 3935  439373,6.5199295
+00003610: 202d 302e 3533 3337 3231 2c32 2e34 3639   -0.533721,2.469
+00003620: 3430 3320 302e 3335 3535 3235 2c33 2e36  403 0.355525,3.6
+00003630: 3130 3730 3320 322e 3037 3033 3537 2c33  10703 2.070357,3
+00003640: 2e39 3831 3435 3720 312e 3339 3232 3831  .981457 1.392281
+00003650: 2c30 2e33 3031 3031 3720 332e 3338 3636  ,0.301017 3.3866
+00003660: 3833 2c32 2e35 3134 3837 2036 2e36 3531  83,2.51487 6.651
+00003670: 3836 332c 312e 3236 3434 3036 2033 2e32  863,1.264406 3.2
+00003680: 3531 3133 322c 2d31 2e32 3435 3038 3520  51132,-1.245085 
+00003690: 342e 3933 3634 3336 2c2d 322e 3831 3032  4.936436,-2.8102
+000036a0: 3920 392e 3732 3434 3236 2c2d 382e 3038  9 9.724426,-8.08
+000036b0: 3335 3331 207a 220a 2020 2020 2020 2020  3531 z".        
+000036c0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+000036d0: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
+000036e0: 793a 313b 7374 726f 6b65 3a23 3030 3030  y:1;stroke:#0000
+000036f0: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
+00003700: 3170 783b 7374 726f 6b65 2d6c 696e 6563  1px;stroke-linec
+00003710: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00003720: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00003730: 726f 6b65 2d6f 7061 6369 7479 3a31 2220  roke-opacity:1" 
+00003740: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+00003750: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+00003760: 3a6e 6f64 6574 7970 6573 3d22 6363 6322  :nodetypes="ccc"
+00003770: 0a20 2020 2020 2020 2020 7472 616e 7366  .         transf
+00003780: 6f72 6d3d 2274 7261 6e73 6c61 7465 2830  orm="translate(0
+00003790: 2c39 3532 2e33 3632 3138 2922 0a20 2020  ,952.36218)".   
+000037a0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+000037b0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+000037c0: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
+000037d0: 6964 3d22 7061 7468 3338 3937 220a 2020  id="path3897".  
+000037e0: 2020 2020 2020 2064 3d22 6d20 3130 382e         d="m 108.
+000037f0: 3337 3532 362c 372e 3934 3837 3131 3720  37526,7.9487117 
+00003800: 6320 2d30 2e37 3136 3636 2c31 2e34 3333  c -0.71666,1.433
+00003810: 3332 3520 2d35 2e30 3136 3634 2c33 2e33  325 -5.01664,3.3
+00003820: 3434 3432 3433 202d 352e 3031 3636 342c  444243 -5.01664,
+00003830: 332e 3334 3434 3234 3320 302c 3020 342e  3.3444243 0,0 4.
+00003840: 3533 3838 362c 2d31 2e31 3934 3433 3820  53886,-1.194438 
+00003850: 362e 3337 3033 332c 2d30 2e34 3737 3737  6.37033,-0.47777
+00003860: 3522 0a20 2020 2020 2020 2020 7374 796c  5".         styl
+00003870: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
+00003880: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00003890: 6b65 2d77 6964 7468 3a31 7078 3b73 7472  ke-width:1px;str
+000038a0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+000038b0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+000038c0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+000038d0: 6163 6974 793a 3122 202f 3e0a 2020 2020  acity:1" />.    
+000038e0: 3c2f 673e 0a20 203c 2f67 3e0a 3c2f 7376  </g>.  </g>.</sv
+000038f0: 673e 0a                                  g>.
```

### Comparing `pydoe3-1.0.0/doc/_templates/layout.html` & `pydoe3-1.0.1/doc/_templates/layout.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,88 @@
-{% extends "!layout.html" %}
-
-{% block rootrellink %}
-        {{ toctree() }}
-{% endblock %}
-
-
-{% block relbar1 %}
-
-<div style="background-color: white; text-align: left; padding: 10px 10px 15px 15px">
-<a href="{{ pathto('index') }}"><img src="{{
-pathto("_static/logo.png", 1) }}" border="0" alt="ad"/></a>
-</div>
-{{ super() }}
-{% endblock %}
-
-
-{#############################################################################}
-{# Sidebar customization #)
-
-{# put the sidebar before the body #}
-{% block sidebar1 %}
-
-{%- macro sidebar() %}
-      {%- if not embedded %}{% if not theme_nosidebar|tobool %}
-<div class="sphinxsidebar">
-        <div class="sphinxsidebarwrapper">
-          {%- block sidebarlogo %}
-          {%- if logo %}
-            <p class="logo"><a href="{{ pathto(master_doc) }}">
-              <img class="logo" src="{{ pathto('_static/' + logo, 1) }}" alt="Logo"/>
-            </a></p>
-          {%- endif %}
-          {%- endblock %}
-          {%- block sidebartoc %}
-          {%- block sidebarglobaltoc %}
-            <h3>{{ _('Table of contents') }}</h3>
-            {{ toctree() }}
-          {%- endblock %}
-          {%- endblock %}
-          {%- block sidebarrel %}
-          {%- endblock %}
-          {%- block sidebarsourcelink %}
-          {%- if show_source and has_source and sourcename %}
-            <h3>{{ _('This Page') }}</h3>
-            <ul class="this-page-menu">
-              <li><a href="{{ pathto('_sources/' + sourcename, true)|e }}"
-                     rel="nofollow">{{ _('Show Source') }}</a></li>
-            </ul>
-          {%- endif %}
-          {%- endblock %}
-          {%- if customsidebar %}
-          {% include customsidebar %}
-          {%- endif %}
-          {%- if display_toc %}
-            <h3>{{ _('Section contents') }}</h3>
-            {{ toc }}
-          {%- endif %}
-          {%- block sidebarsearch %}
-          {%- if pagename != "search" %}
-          <div id="searchbox" style="display: none">
-            <h3>{{ _('Quick search') }}</h3>
-              <form class="search" action="{{ pathto('search') }}" method="get">
-                <input type="text" name="q" size="18" />
-                <input type="submit" value="{{ _('Go') }}" />
-                <input type="hidden" name="check_keywords" value="yes" />
-                <input type="hidden" name="area" value="default" />
-              </form>
-              <p class="searchtip" style="font-size: 90%">
-              {{ _('Search the documentation.') }}
-              </p>
-          </div>
-          <script type="text/javascript">$('#searchbox').show(0);</script>
-          {%- endif %}
-          {%- endblock %}
-          {%- block copyright %}
-          <h3>Documentation license</h3>
-<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-nd/3.0/88x31.png" /></a>
-          {%- endblock %}
-        </div>
-      </div>
-      {%- endif %}{% endif %}
-{%- endmacro %}
-
-{{ sidebar() }}{% endblock %}
-
-
-{% block sidebar2 %}{% endblock %}
-
+{% extends "!layout.html" %}
+
+{% block rootrellink %}
+{{ toctree() }}
+{% endblock %}
+
+
+{% block relbar1 %}
+
+<div style="background-color: white; text-align: left; padding: 10px 10px 15px 15px">
+  <a href="{{ pathto('index') }}"><img src="{{
+pathto(" _static/logo_pydoe3.png", 1) }}" border="0" alt="ad" /></a>
+</div>
+{{ super() }}
+{% endblock %}
+
+
+{#############################################################################}
+{# Sidebar customization #)
+
+{# put the sidebar before the body #}
+{% block sidebar1 %}
+
+{%- macro sidebar() %}
+{%- if not embedded %}{% if not theme_nosidebar|tobool %}
+<div class="sphinxsidebar">
+  <div class="sphinxsidebarwrapper">
+    {%- block sidebarlogo %}
+    {%- if logo %}
+    <p class="logo"><a href="{{ pathto(master_doc) }}">
+        <img class="logo" src="{{ pathto('_static/' + logo, 1) }}" alt="Logo" />
+      </a></p>
+    {%- endif %}
+    {%- endblock %}
+    {%- block sidebartoc %}
+    {%- block sidebarglobaltoc %}
+    <h3>{{ _('Table of contents') }}</h3>
+    {{ toctree() }}
+    {%- endblock %}
+    {%- endblock %}
+    {%- block sidebarrel %}
+    {%- endblock %}
+    {%- block sidebarsourcelink %}
+    {%- if show_source and has_source and sourcename %}
+    <h3>{{ _('This Page') }}</h3>
+    <ul class="this-page-menu">
+      <li><a href="{{ pathto('_sources/' + sourcename, true)|e }}" rel="nofollow">{{ _('Show Source') }}</a></li>
+    </ul>
+    {%- endif %}
+    {%- endblock %}
+    {%- if customsidebar %}
+    {% include customsidebar %}
+    {%- endif %}
+    {%- if display_toc %}
+    <h3>{{ _('Section contents') }}</h3>
+    {{ toc }}
+    {%- endif %}
+    {%- block sidebarsearch %}
+    {%- if pagename != "search" %}
+    <div id="searchbox" style="display: none">
+      <h3>{{ _('Quick search') }}</h3>
+      <form class="search" action="{{ pathto('search') }}" method="get">
+        <input type="text" name="q" size="18" />
+        <input type="submit" value="{{ _('Go') }}" />
+        <input type="hidden" name="check_keywords" value="yes" />
+        <input type="hidden" name="area" value="default" />
+      </form>
+      <p class="searchtip" style="font-size: 90%">
+        {{ _('Search the documentation.') }}
+      </p>
+    </div>
+    <script type="text/javascript">$('#searchbox').show(0);</script>
+    {%- endif %}
+    {%- endblock %}
+    {%- block copyright %}
+    <h3>Documentation license</h3>
+    <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/3.0/"><img alt="Creative Commons License"
+        style="border-width:0" src="http://i.creativecommons.org/l/by-nc-nd/3.0/88x31.png" /></a>
+    {%- endblock %}
+  </div>
+</div>
+{%- endif %}{% endif %}
+{%- endmacro %}
+
+{{ sidebar() }}{% endblock %}
+
+
+{% block sidebar2 %}{% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "!layout.html" %} {% block rootrellink %} {{ toctree() }} {%
 endblock %} {% block relbar1 %}
-) }}" border="0" alt="ad"/>
+) }}" border="0" alt="ad" />
 {{ super() }} {% endblock %}
 {#############################################################################}
 {# Sidebar customization #) {# put the sidebar before the body #} {% block
 sidebar1 %} {%- macro sidebar() %} {%- if not embedded %}{% if not
 theme_nosidebar|tobool %}
 {%- block sidebarlogo %} {%- if logo %}
 _[_L_o_g_o_]
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_box_behnken.py` & `pydoe3-1.0.1/pyDOE3/doe_box_behnken.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,96 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-from pyDOE3.doe_factorial import ff2n
-from pyDOE3.doe_repeat_center import repeat_center
-
-__all__ = ['bbdesign']
-
-def bbdesign(n, center=None):
-    """
-    Create a Box-Behnken design
-    
-    Parameters
-    ----------
-    n : int
-        The number of factors in the design
-    
-    Optional
-    --------
-    center : int
-        The number of center points to include (default = 1).
-    
-    Returns
-    -------
-    mat : 2d-array
-        The design matrix
-    
-    Example
-    -------
-    ::
-    
-        >>> bbdesign(3)
-        array([[-1., -1.,  0.],
-               [ 1., -1.,  0.],
-               [-1.,  1.,  0.],
-               [ 1.,  1.,  0.],
-               [-1.,  0., -1.],
-               [ 1.,  0., -1.],
-               [-1.,  0.,  1.],
-               [ 1.,  0.,  1.],
-               [ 0., -1., -1.],
-               [ 0.,  1., -1.],
-               [ 0., -1.,  1.],
-               [ 0.,  1.,  1.],
-               [ 0.,  0.,  0.],
-               [ 0.,  0.,  0.],
-               [ 0.,  0.,  0.]])
-        
-    """
-    assert n>=3, 'Number of variables must be at least 3'
-    
-    # First, compute a factorial DOE with 2 parameters
-    H_fact = ff2n(2)
-    # Now we populate the real DOE with this DOE
-    
-    # We made a factorial design on each pair of dimensions
-    # - So, we created a factorial design with two factors
-    # - Make two loops
-    Index = 0
-    nb_lines = int((0.5*n*(n-1))*H_fact.shape[0])
-    H = repeat_center(n, nb_lines)
-    
-    for i in range(n - 1):
-        for j in range(i + 1, n):
-            Index = Index + 1
-            H[max([0, (Index - 1)*H_fact.shape[0]]):Index*H_fact.shape[0], i] = H_fact[:, 0]
-            H[max([0, (Index - 1)*H_fact.shape[0]]):Index*H_fact.shape[0], j] = H_fact[:, 1]
-
-    if center is None:
-        if n<=16:
-            points= [0, 0, 0, 3, 3, 6, 6, 6, 8, 9, 10, 12, 12, 13, 14, 15, 16]
-            center = points[n]
-        else:
-            center = n
-        
-    H = np.c_[H.T, repeat_center(n, center).T].T
-    
-    return H
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+from pyDOE3.doe_factorial import ff2n
+from pyDOE3.doe_repeat_center import repeat_center
+
+__all__ = ["bbdesign"]
+
+
+def bbdesign(n, center=None):
+    """
+    Create a Box-Behnken design
+
+    Parameters
+    ----------
+    n : int
+        The number of factors in the design
+
+    Optional
+    --------
+    center : int
+        The number of center points to include (default = 1).
+
+    Returns
+    -------
+    mat : 2d-array
+        The design matrix
+
+    Example
+    -------
+    ::
+
+        >>> bbdesign(3)
+        array([[-1., -1.,  0.],
+               [ 1., -1.,  0.],
+               [-1.,  1.,  0.],
+               [ 1.,  1.,  0.],
+               [-1.,  0., -1.],
+               [ 1.,  0., -1.],
+               [-1.,  0.,  1.],
+               [ 1.,  0.,  1.],
+               [ 0., -1., -1.],
+               [ 0.,  1., -1.],
+               [ 0., -1.,  1.],
+               [ 0.,  1.,  1.],
+               [ 0.,  0.,  0.],
+               [ 0.,  0.,  0.],
+               [ 0.,  0.,  0.]])
+
+    """
+    assert n >= 3, "Number of variables must be at least 3"
+
+    # First, compute a factorial DOE with 2 parameters
+    H_fact = ff2n(2)
+    # Now we populate the real DOE with this DOE
+
+    # We made a factorial design on each pair of dimensions
+    # - So, we created a factorial design with two factors
+    # - Make two loops
+    Index = 0
+    nb_lines = int((0.5 * n * (n - 1)) * H_fact.shape[0])
+    H = repeat_center(n, nb_lines)
+
+    for i in range(n - 1):
+        for j in range(i + 1, n):
+            Index = Index + 1
+            H[
+                max([0, (Index - 1) * H_fact.shape[0]]) : Index * H_fact.shape[0], i
+            ] = H_fact[:, 0]
+            H[
+                max([0, (Index - 1) * H_fact.shape[0]]) : Index * H_fact.shape[0], j
+            ] = H_fact[:, 1]
+
+    if center is None:
+        if n <= 16:
+            points = [0, 0, 0, 3, 3, 6, 6, 6, 8, 9, 10, 12, 12, 13, 14, 15, 16]
+            center = points[n]
+        else:
+            center = n
+
+    H = np.c_[H.T, repeat_center(n, center).T].T
+
+    return H
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_composite.py` & `pydoe3-1.0.1/pyDOE3/doe_composite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,160 +1,177 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-from pyDOE3.doe_factorial import ff2n
-from pyDOE3.doe_star import star
-from pyDOE3.doe_union import union
-from pyDOE3.doe_repeat_center import repeat_center
-
-__all__ = ['ccdesign']
-
-def ccdesign(n, center=(4, 4), alpha='orthogonal', face='circumscribed'):
-    """
-    Central composite design
-    
-    Parameters
-    ----------
-    n : int
-        The number of factors in the design.
-    
-    Optional
-    --------
-    center : int array
-        A 1-by-2 array of integers, the number of center points in each block
-        of the design. (Default: (4, 4)).
-    alpha : str
-        A string describing the effect of alpha has on the variance. ``alpha``
-        can take on the following values:
-        
-        1. 'orthogonal' or 'o' (Default)
-        
-        2. 'rotatable' or 'r'
-        
-    face : str
-        The relation between the start points and the corner (factorial) points.
-        There are three options for this input:
-        
-        1. 'circumscribed' or 'ccc': This is the original form of the central
-           composite design. The star points are at some distance ``alpha``
-           from the center, based on the properties desired for the design.
-           The start points establish new extremes for the low and high
-           settings for all factors. These designs have circular, spherical,
-           or hyperspherical symmetry and require 5 levels for each factor.
-           Augmenting an existing factorial or resolution V fractional 
-           factorial design with star points can produce this design.
-        
-        2. 'inscribed' or 'cci': For those situations in which the limits
-           specified for factor settings are truly limits, the CCI design
-           uses the factors settings as the star points and creates a factorial
-           or fractional factorial design within those limits (in other words,
-           a CCI design is a scaled down CCC design with each factor level of
-           the CCC design divided by ``alpha`` to generate the CCI design).
-           This design also requires 5 levels of each factor.
-        
-        3. 'faced' or 'ccf': In this design, the star points are at the center
-           of each face of the factorial space, so ``alpha`` = 1. This 
-           variety requires 3 levels of each factor. Augmenting an existing 
-           factorial or resolution V design with appropriate star points can 
-           also produce this design.
-    
-    Notes
-    -----
-    - Fractional factorial designs are not (yet) available here.
-    - 'ccc' and 'cci' can be rotatable design, but 'ccf' cannot.
-    - If ``face`` is specified, while ``alpha`` is not, then the default value
-      of ``alpha`` is 'orthogonal'.
-        
-    Returns
-    -------
-    mat : 2d-array
-        The design matrix with coded levels -1 and 1
-    
-    Example
-    -------
-    ::
-    
-        >>> ccdesign(3)
-        array([[-1.        , -1.        , -1.        ],
-               [ 1.        , -1.        , -1.        ],
-               [-1.        ,  1.        , -1.        ],
-               [ 1.        ,  1.        , -1.        ],
-               [-1.        , -1.        ,  1.        ],
-               [ 1.        , -1.        ,  1.        ],
-               [-1.        ,  1.        ,  1.        ],
-               [ 1.        ,  1.        ,  1.        ],
-               [ 0.        ,  0.        ,  0.        ],
-               [ 0.        ,  0.        ,  0.        ],
-               [ 0.        ,  0.        ,  0.        ],
-               [ 0.        ,  0.        ,  0.        ],
-               [-1.82574186,  0.        ,  0.        ],
-               [ 1.82574186,  0.        ,  0.        ],
-               [ 0.        , -1.82574186,  0.        ],
-               [ 0.        ,  1.82574186,  0.        ],
-               [ 0.        ,  0.        , -1.82574186],
-               [ 0.        ,  0.        ,  1.82574186],
-               [ 0.        ,  0.        ,  0.        ],
-               [ 0.        ,  0.        ,  0.        ],
-               [ 0.        ,  0.        ,  0.        ],
-               [ 0.        ,  0.        ,  0.        ]])
-        
-       
-    """
-    # Check inputs
-    assert isinstance(n, int) and n>1, '"n" must be an integer greater than 1.'
-    assert alpha.lower() in ('orthogonal', 'o', 'rotatable', 
-        'r'), 'Invalid value for "alpha": {:}'.format(alpha)
-    assert face.lower() in ('circumscribed', 'ccc', 'inscribed', 'cci',
-        'faced', 'ccf'), 'Invalid value for "face": {:}'.format(face)
-    
-    try:
-        nc = len(center)
-    except:
-        raise TypeError('Invalid value for "center": {:}. Expected a 1-by-2 array.'.format(center))
-    else:
-        if nc!=2:
-            raise ValueError('Invalid number of values for "center" (expected 2, but got {:})'.format(nc))
-
-    # Orthogonal Design
-    if alpha.lower() in ('orthogonal', 'o'):
-        H2, a = star(n, alpha='orthogonal', center=center)
-    
-    # Rotatable Design
-    if alpha.lower() in ('rotatable', 'r'):
-        H2, a = star(n, alpha='rotatable')
-    
-    # Inscribed CCD
-    if face.lower() in ('inscribed', 'cci'):
-        H1 = ff2n(n)
-        H1 = H1/a  # Scale down the factorial points
-        H2, a = star(n)
-    
-    # Faced CCD
-    if face.lower() in ('faced', 'ccf'):
-        H2, a = star(n)  # Value of alpha is always 1 in Faced CCD
-        H1 = ff2n(n)
-    
-    # Circumscribed CCD
-    if face.lower() in ('circumscribed', 'ccc'):
-        H1 = ff2n(n)
-    
-    C1 = repeat_center(n, center[0])
-    C2 = repeat_center(n, center[1])
-
-    H1 = union(H1, C1)
-    H2 = union(H2, C2)
-    H = union(H1, H2)
-
-    return H
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+from pyDOE3.doe_factorial import ff2n
+from pyDOE3.doe_star import star
+from pyDOE3.doe_union import union
+from pyDOE3.doe_repeat_center import repeat_center
+
+__all__ = ["ccdesign"]
+
+
+def ccdesign(n, center=(4, 4), alpha="orthogonal", face="circumscribed"):
+    """
+    Central composite design
+
+    Parameters
+    ----------
+    n : int
+        The number of factors in the design.
+
+    Optional
+    --------
+    center : int array
+        A 1-by-2 array of integers, the number of center points in each block
+        of the design. (Default: (4, 4)).
+    alpha : str
+        A string describing the effect of alpha has on the variance. ``alpha``
+        can take on the following values:
+
+        1. 'orthogonal' or 'o' (Default)
+
+        2. 'rotatable' or 'r'
+
+    face : str
+        The relation between the start points and the corner (factorial) points.
+        There are three options for this input:
+
+        1. 'circumscribed' or 'ccc': This is the original form of the central
+           composite design. The star points are at some distance ``alpha``
+           from the center, based on the properties desired for the design.
+           The start points establish new extremes for the low and high
+           settings for all factors. These designs have circular, spherical,
+           or hyperspherical symmetry and require 5 levels for each factor.
+           Augmenting an existing factorial or resolution V fractional
+           factorial design with star points can produce this design.
+
+        2. 'inscribed' or 'cci': For those situations in which the limits
+           specified for factor settings are truly limits, the CCI design
+           uses the factors settings as the star points and creates a factorial
+           or fractional factorial design within those limits (in other words,
+           a CCI design is a scaled down CCC design with each factor level of
+           the CCC design divided by ``alpha`` to generate the CCI design).
+           This design also requires 5 levels of each factor.
+
+        3. 'faced' or 'ccf': In this design, the star points are at the center
+           of each face of the factorial space, so ``alpha`` = 1. This
+           variety requires 3 levels of each factor. Augmenting an existing
+           factorial or resolution V design with appropriate star points can
+           also produce this design.
+
+    Notes
+    -----
+    - Fractional factorial designs are not (yet) available here.
+    - 'ccc' and 'cci' can be rotatable design, but 'ccf' cannot.
+    - If ``face`` is specified, while ``alpha`` is not, then the default value
+      of ``alpha`` is 'orthogonal'.
+
+    Returns
+    -------
+    mat : 2d-array
+        The design matrix with coded levels -1 and 1
+
+    Example
+    -------
+    ::
+
+        >>> ccdesign(3)
+        array([[-1.        , -1.        , -1.        ],
+               [ 1.        , -1.        , -1.        ],
+               [-1.        ,  1.        , -1.        ],
+               [ 1.        ,  1.        , -1.        ],
+               [-1.        , -1.        ,  1.        ],
+               [ 1.        , -1.        ,  1.        ],
+               [-1.        ,  1.        ,  1.        ],
+               [ 1.        ,  1.        ,  1.        ],
+               [ 0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ],
+               [-1.82574186,  0.        ,  0.        ],
+               [ 1.82574186,  0.        ,  0.        ],
+               [ 0.        , -1.82574186,  0.        ],
+               [ 0.        ,  1.82574186,  0.        ],
+               [ 0.        ,  0.        , -1.82574186],
+               [ 0.        ,  0.        ,  1.82574186],
+               [ 0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ]])
+
+
+    """
+    # Check inputs
+    assert isinstance(n, int) and n > 1, '"n" must be an integer greater than 1.'
+    assert alpha.lower() in (
+        "orthogonal",
+        "o",
+        "rotatable",
+        "r",
+    ), 'Invalid value for "alpha": {:}'.format(alpha)
+    assert face.lower() in (
+        "circumscribed",
+        "ccc",
+        "inscribed",
+        "cci",
+        "faced",
+        "ccf",
+    ), 'Invalid value for "face": {:}'.format(face)
+
+    try:
+        nc = len(center)
+    except:
+        raise TypeError(
+            'Invalid value for "center": {:}. Expected a 1-by-2 array.'.format(center)
+        )
+    else:
+        if nc != 2:
+            raise ValueError(
+                'Invalid number of values for "center" (expected 2, but got {:})'.format(
+                    nc
+                )
+            )
+
+    # Orthogonal Design
+    if alpha.lower() in ("orthogonal", "o"):
+        H2, a = star(n, alpha="orthogonal", center=center)
+
+    # Rotatable Design
+    if alpha.lower() in ("rotatable", "r"):
+        H2, a = star(n, alpha="rotatable")
+
+    # Inscribed CCD
+    if face.lower() in ("inscribed", "cci"):
+        H1 = ff2n(n)
+        H1 = H1 / a  # Scale down the factorial points
+        H2, a = star(n)
+
+    # Faced CCD
+    if face.lower() in ("faced", "ccf"):
+        H2, a = star(n)  # Value of alpha is always 1 in Faced CCD
+        H1 = ff2n(n)
+
+    # Circumscribed CCD
+    if face.lower() in ("circumscribed", "ccc"):
+        H1 = ff2n(n)
+
+    C1 = repeat_center(n, center[0])
+    C2 = repeat_center(n, center[1])
+
+    H1 = union(H1, C1)
+    H2 = union(H2, C2)
+    H = union(H1, H2)
+
+    return H
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_factorial.py` & `pydoe3-1.0.1/pyDOE3/doe_factorial.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,535 +1,564 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import itertools
-import math
-import re
-import string
-
-import numpy as np
-from scipy.special import binom
-
-
-__all__ = ['np', 'fullfact', 'ff2n', 'fracfact', 'fracfact_by_res', 'fracfact_opt',
-    'fracfact_aliasing', 'alias_vector_indices']
-
-def fullfact(levels):
-    """
-    Create a general full-factorial design
-    
-    Parameters
-    ----------
-    levels : array-like
-        An array of integers that indicate the number of levels of each input
-        design factor.
-    
-    Returns
-    -------
-    mat : 2d-array
-        The design matrix with coded levels 0 to k-1 for a k-level factor
-    
-    Example
-    -------
-    ::
-    
-        >>> fullfact([2, 4, 3])
-        array([[ 0.,  0.,  0.],
-               [ 1.,  0.,  0.],
-               [ 0.,  1.,  0.],
-               [ 1.,  1.,  0.],
-               [ 0.,  2.,  0.],
-               [ 1.,  2.,  0.],
-               [ 0.,  3.,  0.],
-               [ 1.,  3.,  0.],
-               [ 0.,  0.,  1.],
-               [ 1.,  0.,  1.],
-               [ 0.,  1.,  1.],
-               [ 1.,  1.,  1.],
-               [ 0.,  2.,  1.],
-               [ 1.,  2.,  1.],
-               [ 0.,  3.,  1.],
-               [ 1.,  3.,  1.],
-               [ 0.,  0.,  2.],
-               [ 1.,  0.,  2.],
-               [ 0.,  1.,  2.],
-               [ 1.,  1.,  2.],
-               [ 0.,  2.,  2.],
-               [ 1.,  2.,  2.],
-               [ 0.,  3.,  2.],
-               [ 1.,  3.,  2.]])
-               
-    """
-    n = len(levels)  # number of factors
-    nb_lines = np.prod(levels)  # number of trial conditions
-    H = np.zeros((nb_lines, n))
-    
-    level_repeat = 1
-    range_repeat = np.prod(levels)
-    for i in range(n):
-        range_repeat //= levels[i]
-        lvl = []
-        for j in range(levels[i]):
-            lvl += [j]*level_repeat
-        rng = lvl*range_repeat
-        level_repeat *= levels[i]
-        H[:, i] = rng
-     
-    return H
-    
-################################################################################
-
-def ff2n(n):
-    """
-    Create a 2-Level full-factorial design
-    
-    Parameters
-    ----------
-    n : int
-        The number of factors in the design.
-    
-    Returns
-    -------
-    mat : 2d-array
-        The design matrix with coded levels -1 and 1
-    
-    Example
-    -------
-    ::
-
-        >>> ff2n(3)
-        array([[-1., -1., -1.],
-               [ 1., -1., -1.],
-               [-1.,  1., -1.],
-               [ 1.,  1., -1.],
-               [-1., -1.,  1.],
-               [ 1., -1.,  1.],
-               [-1.,  1.,  1.],
-               [ 1.,  1.,  1.]])
-
-    """
-    return 2*fullfact([2]*n) - 1
-
-################################################################################
-
-def fracfact(gen):
-    """
-    Create a 2-level fractional-factorial design with a generator string.
-
-    Parameters
-    ----------
-    gen : str
-        A string, consisting of lowercase, uppercase letters or operators "-"
-        and "+", indicating the factors of the experiment
-
-    Returns
-    -------
-    H : 2d-array
-        A m-by-n matrix, the fractional factorial design. m is 2^k, where k
-        is the number of letters in ``gen``, and n is the total number of
-        entries in ``gen``.
-
-    Notes
-    -----
-    In ``gen`` we define the main factors of the experiment and the factors
-    whose levels are the products of the main factors. For example, if
-
-        gen = "a b ab"
-
-    then "a" and "b" are the main factors, while the 3rd factor is the product
-    of the first two. If we input uppercase letters in ``gen``, we get the same
-    result. We can also use the operators "+" and "-" in ``gen``.
-
-    For example, if
-
-        gen = "a b -ab"
-
-    then the 3rd factor is the opposite of the product of "a" and "b".
-
-    The output matrix includes the two level full factorial design, built by
-    the main factors of ``gen``, and the products of the main factors. The
-    columns of ``H`` follow the sequence of ``gen``.
-
-    For example, if
-
-        gen = "a b ab c"
-
-    then columns H[:, 0], H[:, 1], and H[:, 3] include the two level full
-    factorial design and H[:, 2] includes the products of the main factors.
-
-    Examples
-    --------
-    ::
-
-        >>> fracfact("a b ab")
-        array([[-1., -1.,  1.],
-               [ 1., -1., -1.],
-               [-1.,  1., -1.],
-               [ 1.,  1.,  1.]])
-
-        >>> fracfact("A B AB")
-        array([[-1., -1.,  1.],
-               [ 1., -1., -1.],
-               [-1.,  1., -1.],
-               [ 1.,  1.,  1.]])
-
-        >>> fracfact("a b -ab c +abc")
-        array([[-1., -1., -1., -1., -1.],
-               [ 1., -1.,  1., -1.,  1.],
-               [-1.,  1.,  1., -1.,  1.],
-               [ 1.,  1., -1., -1., -1.],
-               [-1., -1., -1.,  1.,  1.],
-               [ 1., -1.,  1.,  1., -1.],
-               [-1.,  1.,  1.,  1., -1.],
-               [ 1.,  1., -1.,  1.,  1.]])
-
-    """
-    # Recognize letters and combinations
-    A = [item for item in re.split('\-|\s|\+', gen) if item]  # remove empty strings
-    C = [len(item) for item in A]
-
-    # Indices of single letters (main factors)
-    I = [i for i, item in enumerate(C) if item==1]
-
-    # Indices of letter combinations (we need them to fill out H2 properly).
-    J = [i for i, item in enumerate(C) if item!=1]
-
-    # Check if there are "-" or "+" operators in gen
-    U = [item for item in gen.split(' ') if item]  # remove empty strings
-
-    # If R1 is either None or not, the result is not changed, since it is a
-    # multiplication of 1.
-    R1 = _grep(U, '+')
-    R2 = _grep(U, '-')
-
-    # Fill in design with two level factorial design
-    H1 = ff2n(len(I))
-    H = np.zeros((H1.shape[0], len(C)))
-    H[:, I] = H1
-
-    # Recognize combinations and fill in the rest of matrix H2 with the proper
-    # products
-    for k in J:
-        # For lowercase letters
-        xx = np.array([ord(c) for c in A[k]]) - 97
-
-        # For uppercase letters
-        if np.any(xx<0):
-            xx = np.array([ord(c) for c in A[k]]) - 65
-
-        H[:, k] = np.prod(H1[:, xx], axis=1)
-
-    # Update design if gen includes "-" operator
-    if R2:
-        H[:, R2] *= -1
-
-    # Return the fractional factorial design
-    return H
-
-
-def fracfact_by_res(n, res):
-    """
-    Create a 2-level fractional factorial design with `n` factors
-    and resolution `res`.
-
-    Parameters
-    ----------
-    n : int
-        The number of factors in the design.
-    res : int
-        Desired design resolution
-
-    Returns
-    -------
-    H : 2d-array
-        A m-by-`n` matrix, the fractional factorial design. m is the
-        minimal amount of rows possible for creating a fractional
-        factorial design matrix at resolution `res`
-
-    Raises
-    ------
-    ValueError
-        If the current design is not possible to construct.
-
-    Notes
-    -----
-    The resolution of a design is defined as the length of the shortest
-    word in the defining relation. The resolution describes the level of
-    confounding between factors and interaction effects, where higher
-    resolution indicates lower degree of confounding.
-
-    For example, consider the 2^4-1-design defined by
-
-        gen = "a b c ab"
-
-    The factor "d" is defined by "ab" with defining relation I="abd", where
-    I is the unit vector. In this simple example the shortest word is "abd"
-    meaning that this is a resolution III-design.
-
-    In practice resolution III-, IV- and V-designs are most commonly applied.
-
-    * III: Main effects may be confounded with two-factor interactions.
-    * IV: Main effects are unconfounded by two-factor interactions, but
-          two-factor interactions may be confounded with each other.
-    * V: Main effects unconfounded with up to four-factor interactions,
-         two-factor interactions unconfounded with up to three-factor
-         interactions. Three-factor interactions may be confounded with
-         each other.
-
-    Examples
-    --------
-    ::
-        >>> fracfact_by_res(6, 3)
-        array([[-1., -1., -1.,  1.,  1.,  1.],
-               [ 1., -1., -1., -1., -1.,  1.],
-               [-1.,  1., -1., -1.,  1., -1.],
-               [ 1.,  1., -1.,  1., -1., -1.],
-               [-1., -1.,  1.,  1., -1., -1.],
-               [ 1., -1.,  1., -1.,  1., -1.],
-               [-1.,  1.,  1., -1., -1.,  1.],
-               [ 1.,  1.,  1.,  1.,  1.,  1.]])
-
-        >>> fracfact_by_res(5, 5)
-        Traceback (most recent call last):
-        ...
-        ValueError: design not possible
-    """
-    # Determine minimum required number of base-factors.
-    min_fac = next(itertools.dropwhile(lambda n_: _n_fac_at_res(n_, res) < n,
-                             range(res - 1, n)), None)
-
-    if min_fac is None:
-        raise ValueError('design not possible')
-    elif min_fac > len(string.ascii_lowercase):
-        # This check needs to be done to make sure that the number
-        # of available are enough since `fracfact` parses design generator
-        # characters. In practice, this is highly theoretical and it is
-        # much more likely to run into memory-issues.
-        raise ValueError('design requires too many base-factors.')
-
-    # Get base factors.
-    factors = list(string.ascii_lowercase[:min_fac])
-
-    # Fill out with factor combinations until `n` factors.
-    factor_combs = (''.join(c) for r in range(res - 1, len(factors))
-                    for c in itertools.combinations(factors, r))
-    extra_factors = list(itertools.islice(factor_combs, n - len(factors)))
-
-    # Concatenate `gen` string for `fracfact`.
-    gen = ' '.join(factors + extra_factors)
-    return fracfact(gen)
-
-
-def _grep(haystack, needle):
-    try:
-        haystack[0]
-    except (TypeError, AttributeError):
-        return [0] if needle in haystack else []
-    else:
-        locs = []
-        for idx, item in enumerate(haystack):
-            if needle in item:
-                locs += [idx]
-        return locs
-
-def _n_fac_at_res(n, res):
-    """ Calculate number of possible factors for fractional factorial
-    design with `n` base factors at resolution `res`.
-    """
-    return sum(binom(n, r) for r in range(res - 1, n)) + n
-
-################################################################################
-
-
-def fracfact_opt(n_factors, n_erased, max_attempts=0) :
-    """
-    Find the optimal generator string for a 2-level fractional-factorial design
-    with the specified number of factors and erased factors.
-
-    Parameters
-    ----------
-    n_factors : int
-        The number of factors in the full factorial design
-    n_erased : int
-        The number of factors to "remove" to create the fractional design
-    max_attempts : int
-        The design is searched by exhaustive search, with the most "promising"
-        combinations attempted first. For large designs it might be unfeasible
-        to attempt all combinations.
-        Posite values give the number of models to attemps. Zero or negative
-        values indicate all combinations should be attempted.
-
-    Returns
-    -------
-    gen : str
-        A generator string in the format expected by fracfact() with the 2^k-p
-        design, where k=n_factors and p=n_erased. The design disallows aliasing
-        of main factors, and minimizes aliasing of low-order interactions.
-    alias_map : list of str
-        The map of aliases that the design inflicts.
-        More details in fracfact_aliasing().
-    alias_vector : 1d numpy.array
-        The vector with the cost of the design in term of aliasings.
-        More details in fracfact_aliasing().
-    """
-    def n_comb(n, k):
-        if k<=0 or n<=0 or k>n: return 0
-        return math.factorial(n) / (math.factorial(k) * math.factorial(n-k))
-
-    if n_factors > 20:
-        raise ValueError('Design too big, use 20 factors or less')
-
-    if n_factors<2:
-        raise ValueError('Design too small')
-
-    if n_erased<0:
-        raise ValueError('Number of erased factors must be non-negative')
-
-    n_main_factors = n_factors-n_erased
-    n_aliases = sum(( n_comb(n_main_factors, n)
-                      for n in range(2, n_main_factors+1) ))
-
-    if n_erased>n_comb(n_aliases, n_erased):
-        raise ValueError('Too many erased factors to create aliasing')
-
-    all_names = string.ascii_lowercase
-    factors = range(n_factors)
-    main_factors = range(n_main_factors)
-    main_design = ' '.join([ all_names[f] for f in main_factors ])
-    aliases = itertools.chain.from_iterable((
-            itertools.combinations(main_factors, n)
-            for n in range(2, n_main_factors+1) ))
-
-    aliases = sorted(list(aliases), key=lambda a : (len(a), a), reverse=True)
-    best_design = None
-    best_map = []
-    best_vector = np.repeat(n_factors, n_factors)
-    design_shape = (2**n_main_factors, n_factors)
-    all_combinations = itertools.combinations(aliases, n_erased)
-    all_combinations = (all_combinations if max_attempts<=0 else
-            itertools.islice(all_combinations, 0, max_attempts))
-
-    for aliasing in all_combinations :
-        aliasing_design = ' '.join([
-                ''.join([ all_names[f] for f in a ]) for a in aliasing ])
-        complete_design = main_design+' '+aliasing_design
-        design = fracfact(complete_design)
-        assert design.shape == design_shape
-        alias_map, alias_vector = fracfact_aliasing(design)
-        if list(alias_vector) < list(best_vector):
-            best_design = complete_design
-            best_map = alias_map
-            best_vector = alias_vector
-
-    return best_design, best_map, best_vector
-
-
-def fracfact_aliasing(design):
-    """
-    Find the aliasings in a design, given the contrasts.
-
-    Parameters
-    ----------
-    design : numpy 2d array
-        A design like those returned by fracfact()
-
-    Returns
-    -------
-    alias_map : list of str
-        The map of aliases that the design inflicts. Each string in the list is
-        a set of factors and interactions that are aliased among themselves, in
-        the format a = bcd = def etc. If there is no aliasing (n_erased=0) the
-        map simply lists all factors and interactions.
-    alias_vector : 1d numpy.array
-        The vector with the cost of the design in term of aliasings. Each cell
-        in the array counts the number of aliasing between factors/interactions
-        of size i and of size j, as given by alias_vector_indices().
-
-        The alias cost vector can be turned into a more explicit upper
-        triangular cost matrix with the idiom:
-        alias_matrix = np.zeros((n_factors, n_factors,))
-        alias_matrix[alias_vector_indices(n_factors)] = alias_vector
-
-        The entry in alias_matrix[i,j] (i<=j) shows how many aliasings where
-        created among i-th order interactions and j-th order interactions.
-    """
-    n_rounds, n_factors = design.shape
-
-    if n_factors > 20:
-        raise ValueError('Design too big, use 20 factors or less')
-
-    all_names = string.ascii_lowercase
-    factors = range(n_factors)
-    all_combinations = itertools.chain.from_iterable((
-            itertools.combinations(factors, n) for n in range(1, n_factors+1) ))
-    aliases = {}
-
-    for combination in all_combinations:
-        contrast = np.prod(design[:,combination], axis=1)
-        contrast.flags.writeable = False
-        aliases[contrast.data] = aliases.get(contrast.data, [])
-        aliases[contrast.data].append(combination)
-
-    aliases_list = []
-    for alias in aliases.values():
-        aliases_list.append(sorted(alias, key=lambda a : (len(a), a)))
-    aliases_list = sorted(aliases_list,
-            key=lambda list : ([len(a) for a in list], list))
-
-    aliases_readable = []
-    alias_matrix = np.zeros((n_factors, n_factors, ))
-
-    for alias in aliases_list:
-        alias_readable = ' = '.join([
-                ''.join([ all_names[f] for f in a ]) for a in alias ])
-        aliases_readable.append(alias_readable)
-        for sizes in itertools.combinations([ len(a) for a in alias], 2):
-            assert sizes[0]>=0 and sizes[1]>=0
-            assert sizes[0] <= sizes[1]
-            alias_matrix[sizes[0]-1, sizes[1]-1] += 1
-
-    alias_vector = alias_matrix[alias_vector_indices(n_factors)]
-
-    return aliases_readable, alias_vector
-
-
-def alias_vector_indices(n_factors):
-    """
-    Find the indexes to convert the alias_vector into a square matrix and
-    vice-versa.
-
-    Parameters
-    ----------
-    n_factors : int
-        The number of factors in the full factorial design
-
-    Returns
-    -------
-    rows : 1d numpy array
-    cols : 1d numpy.array
-        Rows and columns of the indices of the upper triangular square matrix
-        with n_factor rows/columns. This function returns a different indice
-        order than numpy.triu_indices, as it puts the indices representing the
-        most serious aliasings first, to help in the optimization procedure.
-    """
-    if n_factors > 20:
-        raise ValueError('Design too big, use 20 factors or less')
-
-    indices = list(itertools.combinations_with_replacement(range(n_factors), 2))
-    indices = sorted(indices, key=lambda i: max(i))
-
-    rows = np.asarray([ i[0] for i in indices ])
-    cols = np.asarray([ i[1] for i in indices ])
-
-    return rows, cols
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import itertools
+import math
+import re
+import string
+
+import numpy as np
+from scipy.special import binom
+
+
+__all__ = [
+    "np",
+    "fullfact",
+    "ff2n",
+    "fracfact",
+    "fracfact_by_res",
+    "fracfact_opt",
+    "fracfact_aliasing",
+    "alias_vector_indices",
+]
+
+
+def fullfact(levels):
+    """
+    Create a general full-factorial design
+
+    Parameters
+    ----------
+    levels : array-like
+        An array of integers that indicate the number of levels of each input
+        design factor.
+
+    Returns
+    -------
+    mat : 2d-array
+        The design matrix with coded levels 0 to k-1 for a k-level factor
+
+    Example
+    -------
+    ::
+
+        >>> fullfact([2, 4, 3])
+        array([[0., 0., 0.],
+               [1., 0., 0.],
+               [0., 1., 0.],
+               [1., 1., 0.],
+               [0., 2., 0.],
+               [1., 2., 0.],
+               [0., 3., 0.],
+               [1., 3., 0.],
+               [0., 0., 1.],
+               [1., 0., 1.],
+               [0., 1., 1.],
+               [1., 1., 1.],
+               [0., 2., 1.],
+               [1., 2., 1.],
+               [0., 3., 1.],
+               [1., 3., 1.],
+               [0., 0., 2.],
+               [1., 0., 2.],
+               [0., 1., 2.],
+               [1., 1., 2.],
+               [0., 2., 2.],
+               [1., 2., 2.],
+               [0., 3., 2.],
+               [1., 3., 2.]])
+
+    """
+    n = len(levels)  # number of factors
+    nb_lines = np.prod(levels)  # number of trial conditions
+    H = np.zeros((nb_lines, n))
+
+    level_repeat = 1
+    range_repeat = np.prod(levels)
+    for i in range(n):
+        range_repeat //= levels[i]
+        lvl = []
+        for j in range(levels[i]):
+            lvl += [j] * level_repeat
+        rng = lvl * range_repeat
+        level_repeat *= levels[i]
+        H[:, i] = rng
+
+    return H
+
+
+################################################################################
+
+
+def ff2n(n):
+    """
+    Create a 2-Level full-factorial design
+
+    Parameters
+    ----------
+    n : int
+        The number of factors in the design.
+
+    Returns
+    -------
+    mat : 2d-array
+        The design matrix with coded levels -1 and 1
+
+    Example
+    -------
+    ::
+
+        >>> ff2n(3)
+        array([[-1., -1., -1.],
+               [ 1., -1., -1.],
+               [-1.,  1., -1.],
+               [ 1.,  1., -1.],
+               [-1., -1.,  1.],
+               [ 1., -1.,  1.],
+               [-1.,  1.,  1.],
+               [ 1.,  1.,  1.]])
+
+    """
+    return 2 * fullfact([2] * n) - 1
+
+
+################################################################################
+
+
+def fracfact(gen):
+    """
+    Create a 2-level fractional-factorial design with a generator string.
+
+    Parameters
+    ----------
+    gen : str
+        A string, consisting of lowercase, uppercase letters or operators "-"
+        and "+", indicating the factors of the experiment
+
+    Returns
+    -------
+    H : 2d-array
+        A m-by-n matrix, the fractional factorial design. m is 2^k, where k
+        is the number of letters in ``gen``, and n is the total number of
+        entries in ``gen``.
+
+    Notes
+    -----
+    In ``gen`` we define the main factors of the experiment and the factors
+    whose levels are the products of the main factors. For example, if
+
+        gen = "a b ab"
+
+    then "a" and "b" are the main factors, while the 3rd factor is the product
+    of the first two. If we input uppercase letters in ``gen``, we get the same
+    result. We can also use the operators "+" and "-" in ``gen``.
+
+    For example, if
+
+        gen = "a b -ab"
+
+    then the 3rd factor is the opposite of the product of "a" and "b".
+
+    The output matrix includes the two level full factorial design, built by
+    the main factors of ``gen``, and the products of the main factors. The
+    columns of ``H`` follow the sequence of ``gen``.
+
+    For example, if
+
+        gen = "a b ab c"
+
+    then columns H[:, 0], H[:, 1], and H[:, 3] include the two level full
+    factorial design and H[:, 2] includes the products of the main factors.
+
+    Examples
+    --------
+    ::
+
+        >>> fracfact("a b ab")
+        array([[-1., -1.,  1.],
+               [ 1., -1., -1.],
+               [-1.,  1., -1.],
+               [ 1.,  1.,  1.]])
+
+        >>> fracfact("A B AB")
+        array([[-1., -1.,  1.],
+               [ 1., -1., -1.],
+               [-1.,  1., -1.],
+               [ 1.,  1.,  1.]])
+
+        >>> fracfact("a b -ab c +abc")
+        array([[-1., -1., -1., -1., -1.],
+               [ 1., -1.,  1., -1.,  1.],
+               [-1.,  1.,  1., -1.,  1.],
+               [ 1.,  1., -1., -1., -1.],
+               [-1., -1., -1.,  1.,  1.],
+               [ 1., -1.,  1.,  1., -1.],
+               [-1.,  1.,  1.,  1., -1.],
+               [ 1.,  1., -1.,  1.,  1.]])
+
+    """
+    # Recognize letters and combinations
+    A = [item for item in re.split(r"\-|\s|\+", gen) if item]  # remove empty strings
+    C = [len(item) for item in A]
+
+    # Indices of single letters (main factors)
+    I = [i for i, item in enumerate(C) if item == 1]
+
+    # Indices of letter combinations (we need them to fill out H2 properly).
+    J = [i for i, item in enumerate(C) if item != 1]
+
+    # Check if there are "-" or "+" operators in gen
+    U = [item for item in gen.split(" ") if item]  # remove empty strings
+
+    # If R1 is either None or not, the result is not changed, since it is a
+    # multiplication of 1.
+    R1 = _grep(U, "+")
+    R2 = _grep(U, "-")
+
+    # Fill in design with two level factorial design
+    H1 = ff2n(len(I))
+    H = np.zeros((H1.shape[0], len(C)))
+    H[:, I] = H1
+
+    # Recognize combinations and fill in the rest of matrix H2 with the proper
+    # products
+    for k in J:
+        # For lowercase letters
+        xx = np.array([ord(c) for c in A[k]]) - 97
+
+        # For uppercase letters
+        if np.any(xx < 0):
+            xx = np.array([ord(c) for c in A[k]]) - 65
+
+        H[:, k] = np.prod(H1[:, xx], axis=1)
+
+    # Update design if gen includes "-" operator
+    if R2:
+        H[:, R2] *= -1
+
+    # Return the fractional factorial design
+    return H
+
+
+def fracfact_by_res(n, res):
+    """
+    Create a 2-level fractional factorial design with `n` factors
+    and resolution `res`.
+
+    Parameters
+    ----------
+    n : int
+        The number of factors in the design.
+    res : int
+        Desired design resolution
+
+    Returns
+    -------
+    H : 2d-array
+        A m-by-`n` matrix, the fractional factorial design. m is the
+        minimal amount of rows possible for creating a fractional
+        factorial design matrix at resolution `res`
+
+    Raises
+    ------
+    ValueError
+        If the current design is not possible to construct.
+
+    Notes
+    -----
+    The resolution of a design is defined as the length of the shortest
+    word in the defining relation. The resolution describes the level of
+    confounding between factors and interaction effects, where higher
+    resolution indicates lower degree of confounding.
+
+    For example, consider the 2^4-1-design defined by
+
+        gen = "a b c ab"
+
+    The factor "d" is defined by "ab" with defining relation I="abd", where
+    I is the unit vector. In this simple example the shortest word is "abd"
+    meaning that this is a resolution III-design.
+
+    In practice resolution III-, IV- and V-designs are most commonly applied.
+
+    * III: Main effects may be confounded with two-factor interactions.
+    * IV: Main effects are unconfounded by two-factor interactions, but
+          two-factor interactions may be confounded with each other.
+    * V: Main effects unconfounded with up to four-factor interactions,
+         two-factor interactions unconfounded with up to three-factor
+         interactions. Three-factor interactions may be confounded with
+         each other.
+
+    Examples
+    --------
+    ::
+        >>> fracfact_by_res(6, 3)
+        array([[-1., -1., -1.,  1.,  1.,  1.],
+               [ 1., -1., -1., -1., -1.,  1.],
+               [-1.,  1., -1., -1.,  1., -1.],
+               [ 1.,  1., -1.,  1., -1., -1.],
+               [-1., -1.,  1.,  1., -1., -1.],
+               [ 1., -1.,  1., -1.,  1., -1.],
+               [-1.,  1.,  1., -1., -1.,  1.],
+               [ 1.,  1.,  1.,  1.,  1.,  1.]])
+
+        >>> fracfact_by_res(5, 5)
+        Traceback (most recent call last):
+        ...
+        ValueError: design not possible
+    """
+    # Determine minimum required number of base-factors.
+    min_fac = next(
+        itertools.dropwhile(lambda n_: _n_fac_at_res(n_, res) < n, range(res - 1, n)),
+        None,
+    )
+
+    if min_fac is None:
+        raise ValueError("design not possible")
+    elif min_fac > len(string.ascii_lowercase):
+        # This check needs to be done to make sure that the number
+        # of available are enough since `fracfact` parses design generator
+        # characters. In practice, this is highly theoretical and it is
+        # much more likely to run into memory-issues.
+        raise ValueError("design requires too many base-factors.")
+
+    # Get base factors.
+    factors = list(string.ascii_lowercase[:min_fac])
+
+    # Fill out with factor combinations until `n` factors.
+    factor_combs = (
+        "".join(c)
+        for r in range(res - 1, len(factors))
+        for c in itertools.combinations(factors, r)
+    )
+    extra_factors = list(itertools.islice(factor_combs, n - len(factors)))
+
+    # Concatenate `gen` string for `fracfact`.
+    gen = " ".join(factors + extra_factors)
+    return fracfact(gen)
+
+
+def _grep(haystack, needle):
+    try:
+        haystack[0]
+    except (TypeError, AttributeError):
+        return [0] if needle in haystack else []
+    else:
+        locs = []
+        for idx, item in enumerate(haystack):
+            if needle in item:
+                locs += [idx]
+        return locs
+
+
+def _n_fac_at_res(n, res):
+    """Calculate number of possible factors for fractional factorial
+    design with `n` base factors at resolution `res`.
+    """
+    return sum(binom(n, r) for r in range(res - 1, n)) + n
+
+
+################################################################################
+
+
+def fracfact_opt(n_factors, n_erased, max_attempts=0):
+    """
+    Find the optimal generator string for a 2-level fractional-factorial design
+    with the specified number of factors and erased factors.
+
+    Parameters
+    ----------
+    n_factors : int
+        The number of factors in the full factorial design
+    n_erased : int
+        The number of factors to "remove" to create the fractional design
+    max_attempts : int
+        The design is searched by exhaustive search, with the most "promising"
+        combinations attempted first. For large designs it might be unfeasible
+        to attempt all combinations.
+        Posite values give the number of models to attemps. Zero or negative
+        values indicate all combinations should be attempted.
+
+    Returns
+    -------
+    gen : str
+        A generator string in the format expected by fracfact() with the 2^k-p
+        design, where k=n_factors and p=n_erased. The design disallows aliasing
+        of main factors, and minimizes aliasing of low-order interactions.
+    alias_map : list of str
+        The map of aliases that the design inflicts.
+        More details in fracfact_aliasing().
+    alias_vector : 1d numpy.array
+        The vector with the cost of the design in term of aliasings.
+        More details in fracfact_aliasing().
+    """
+
+    def n_comb(n, k):
+        if k <= 0 or n <= 0 or k > n:
+            return 0
+        return math.factorial(n) / (math.factorial(k) * math.factorial(n - k))
+
+    if n_factors > 20:
+        raise ValueError("Design too big, use 20 factors or less")
+
+    if n_factors < 2:
+        raise ValueError("Design too small")
+
+    if n_erased < 0:
+        raise ValueError("Number of erased factors must be non-negative")
+
+    n_main_factors = n_factors - n_erased
+    n_aliases = sum((n_comb(n_main_factors, n) for n in range(2, n_main_factors + 1)))
+
+    if n_erased > n_comb(n_aliases, n_erased):
+        raise ValueError("Too many erased factors to create aliasing")
+
+    all_names = string.ascii_lowercase
+    factors = range(n_factors)
+    main_factors = range(n_main_factors)
+    main_design = " ".join([all_names[f] for f in main_factors])
+    aliases = itertools.chain.from_iterable(
+        (itertools.combinations(main_factors, n) for n in range(2, n_main_factors + 1))
+    )
+
+    aliases = sorted(list(aliases), key=lambda a: (len(a), a), reverse=True)
+    best_design = None
+    best_map = []
+    best_vector = np.repeat(n_factors, n_factors)
+    design_shape = (2**n_main_factors, n_factors)
+    all_combinations = itertools.combinations(aliases, n_erased)
+    all_combinations = (
+        all_combinations
+        if max_attempts <= 0
+        else itertools.islice(all_combinations, 0, max_attempts)
+    )
+
+    for aliasing in all_combinations:
+        aliasing_design = " ".join(
+            ["".join([all_names[f] for f in a]) for a in aliasing]
+        )
+        complete_design = main_design + " " + aliasing_design
+        design = fracfact(complete_design)
+        assert design.shape == design_shape
+        alias_map, alias_vector = fracfact_aliasing(design)
+        if list(alias_vector) < list(best_vector):
+            best_design = complete_design
+            best_map = alias_map
+            best_vector = alias_vector
+
+    return best_design, best_map, best_vector
+
+
+def fracfact_aliasing(design):
+    """
+    Find the aliasings in a design, given the contrasts.
+
+    Parameters
+    ----------
+    design : numpy 2d array
+        A design like those returned by fracfact()
+
+    Returns
+    -------
+    alias_map : list of str
+        The map of aliases that the design inflicts. Each string in the list is
+        a set of factors and interactions that are aliased among themselves, in
+        the format a = bcd = def etc. If there is no aliasing (n_erased=0) the
+        map simply lists all factors and interactions.
+    alias_vector : 1d numpy.array
+        The vector with the cost of the design in term of aliasings. Each cell
+        in the array counts the number of aliasing between factors/interactions
+        of size i and of size j, as given by alias_vector_indices().
+
+        The alias cost vector can be turned into a more explicit upper
+        triangular cost matrix with the idiom:
+        alias_matrix = np.zeros((n_factors, n_factors,))
+        alias_matrix[alias_vector_indices(n_factors)] = alias_vector
+
+        The entry in alias_matrix[i,j] (i<=j) shows how many aliasings where
+        created among i-th order interactions and j-th order interactions.
+    """
+    n_rounds, n_factors = design.shape
+
+    if n_factors > 20:
+        raise ValueError("Design too big, use 20 factors or less")
+
+    all_names = string.ascii_lowercase
+    factors = range(n_factors)
+    all_combinations = itertools.chain.from_iterable(
+        (itertools.combinations(factors, n) for n in range(1, n_factors + 1))
+    )
+    aliases = {}
+
+    for combination in all_combinations:
+        contrast = np.prod(design[:, combination], axis=1)
+        contrast.flags.writeable = False
+        aliases[contrast.data] = aliases.get(contrast.data, [])
+        aliases[contrast.data].append(combination)
+
+    aliases_list = []
+    for alias in aliases.values():
+        aliases_list.append(sorted(alias, key=lambda a: (len(a), a)))
+    aliases_list = sorted(aliases_list, key=lambda list: ([len(a) for a in list], list))
+
+    aliases_readable = []
+    alias_matrix = np.zeros(
+        (
+            n_factors,
+            n_factors,
+        )
+    )
+
+    for alias in aliases_list:
+        alias_readable = " = ".join(["".join([all_names[f] for f in a]) for a in alias])
+        aliases_readable.append(alias_readable)
+        for sizes in itertools.combinations([len(a) for a in alias], 2):
+            assert sizes[0] >= 0 and sizes[1] >= 0
+            assert sizes[0] <= sizes[1]
+            alias_matrix[sizes[0] - 1, sizes[1] - 1] += 1
+
+    alias_vector = alias_matrix[alias_vector_indices(n_factors)]
+
+    return aliases_readable, alias_vector
+
+
+def alias_vector_indices(n_factors):
+    """
+    Find the indexes to convert the alias_vector into a square matrix and
+    vice-versa.
+
+    Parameters
+    ----------
+    n_factors : int
+        The number of factors in the full factorial design
+
+    Returns
+    -------
+    rows : 1d numpy array
+    cols : 1d numpy.array
+        Rows and columns of the indices of the upper triangular square matrix
+        with n_factor rows/columns. This function returns a different indice
+        order than numpy.triu_indices, as it puts the indices representing the
+        most serious aliasings first, to help in the optimization procedure.
+    """
+    if n_factors > 20:
+        raise ValueError("Design too big, use 20 factors or less")
+
+    indices = list(itertools.combinations_with_replacement(range(n_factors), 2))
+    indices = sorted(indices, key=lambda i: max(i))
+
+    rows = np.asarray([i[0] for i in indices])
+    cols = np.asarray([i[1] for i in indices])
+
+    return rows, cols
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_fold.py` & `pydoe3-1.0.1/pyDOE3/doe_fold.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-
-__all__ = ['fold']
-
-def fold(H, columns=None):
-    """
-    Fold a design to reduce confounding effects.
-    
-    Parameters
-    ----------
-    H : 2d-array
-        The design matrix to be folded.
-    columns : array
-        Indices of of columns to fold (Default: None). If ``columns=None`` is
-        used, then all columns will be folded.
-    
-    Returns
-    -------
-    Hf : 2d-array
-        The folded design matrix.
-    
-    Examples
-    --------
-    ::
-    
-    """
-    H = np.array(H)
-    assert len(H.shape)==2, 'Input design matrix must be 2d.'
-    
-    if columns is None:
-        columns = range(H.shape[1])
-    
-    Hf = H.copy()
-    
-    for col in columns:
-        vals = np.unique(H[:, col])
-        assert len(vals)==2, 'Input design matrix must be 2-level factors only.'
-        
-        for i in range(H.shape[0]):
-            Hf[i, col] = vals[0] if H[i, col]==vals[1] else vals[1]
-    
-    Hf = np.vstack((H, Hf))
-    
-    return Hf
-        
-    
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+
+__all__ = ["fold"]
+
+
+def fold(H, columns=None):
+    """
+    Fold a design to reduce confounding effects.
+
+    Parameters
+    ----------
+    H : 2d-array
+        The design matrix to be folded.
+    columns : array
+        Indices of of columns to fold (Default: None). If ``columns=None`` is
+        used, then all columns will be folded.
+
+    Returns
+    -------
+    Hf : 2d-array
+        The folded design matrix.
+
+    Examples
+    --------
+    ::
+
+    """
+    H = np.array(H)
+    assert len(H.shape) == 2, "Input design matrix must be 2d."
+
+    if columns is None:
+        columns = range(H.shape[1])
+
+    Hf = H.copy()
+
+    for col in columns:
+        vals = np.unique(H[:, col])
+        assert len(vals) == 2, "Input design matrix must be 2-level factors only."
+
+        for i in range(H.shape[0]):
+            Hf[i, col] = vals[0] if H[i, col] == vals[1] else vals[1]
+
+    Hf = np.vstack((H, Hf))
+
+    return Hf
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_gsd.py` & `pydoe3-1.0.1/pyDOE3/doe_gsd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,220 +1,223 @@
-"""
-Copyright (C) 2018 - Rickard Sjoegren
-"""
-import itertools
-
-import numpy as np
-
-
-def gsd(levels, reduction, n=1):
-    """
-    Create a Generalized Subset Design (GSD).
-
-    Parameters
-    ----------
-    levels : array-like
-        Number of factor levels per factor in design.
-    reduction : int
-        Reduction factor (bigger than 1). Larger `reduction` means fewer
-        experiments in the design and more possible complementary designs.
-    n : int
-        Number of complementary GSD-designs (default 1). The complementary
-        designs are balanced analogous to fold-over in two-level fractional
-        factorial designs.
-
-    Returns
-    -------
-    H : 2d-array | list of 2d-arrays
-        `n` m-by-k matrices where k is the number of factors (equal
-        to the length of `factor_levels`. The number of rows, m, will
-        be approximately equal to the grand product of the factor levels
-        divided by `reduction`.
-
-    Raises
-    ------
-    ValueError
-        If input is valid or if design construction fails. Design can fail
-        if `reduction` is too large compared to values of `levels`.
-
-    Notes
-    -----
-    The Generalized Subset Design (GSD) [1]_ or generalized factorial design is
-    a generalization of traditional fractional factorial designs to problems
-    where factors can have more than two levels.
-
-    In many application problems factors can have categorical or quantitative
-    factors on more than two levels. Previous reduced designs have not been
-    able to deal with such types of problems. Full multi-level factorial
-    designs can handle such problems but are however not economical regarding
-    the number of experiments.
-
-    Note for commercial users, the application of GSD to testing of product
-    characteristics in a processing facility is patented [2]_
-
-    Examples
-    --------
-    An example with three factors using three, four and
-    six levels respectively reduced with a factor 4 ::
-
-        >>> gsd([3, 4, 6], 4)
-        array([[0, 0, 0],
-               [0, 0, 4],
-               [0, 1, 1],
-               [0, 1, 5],
-               [0, 2, 2],
-               [0, 3, 3],
-               [1, 0, 1],
-               [1, 0, 5],
-               [1, 1, 2],
-               [1, 2, 3],
-               [1, 3, 0],
-               [1, 3, 4],
-               [2, 0, 2],
-               [2, 1, 3],
-               [2, 2, 0],
-               [2, 2, 4],
-               [2, 3, 1],
-               [2, 3, 5]])
-
-    Two complementary designs with two factors using three and
-    four levels reduced with a factor 2 ::
-
-        >>> gsd([3, 4], 2, n=2)[0]
-        array([[0, 0],
-               [0, 2],
-               [2, 0],
-               [2, 2],
-               [1, 1],
-               [1, 3]])
-        >>> gsd([3, 4], 2, n=2)[1]
-        array([[0, 1],
-               [0, 3],
-               [2, 1],
-               [2, 3],
-               [1, 0],
-               [1, 2]])
-
-    If design fails ValueError is raised ::
-
-        >>> gsd([2, 3], 5)
-        Traceback (most recent call last):
-         ...
-        ValueError: reduction too large compared to factor levels
-
-    References
-    ----------
-    .. [1] Surowiec, Izabella, Ludvig Vikstrom, Gustaf Hector, Erik Johansson,
-       Conny Vikstrom, and Johan Trygg. "Generalized Subset Designs in
-       Analytical Chemistry." Analytical Chemistry 89, no. 12 (June 20, 2017):
-       6491-97. https://doi.org/10.1021/acs.analchem.7b00506.
-
-    .. [2] Vikstrom, Ludvig, Conny Vikstrom, Erik Johansson, and Gustaf Hector.
-       Computer-implemented systems and methods for generating
-       generalized fractional designs. US9746850 B2, filed May 9,
-       2014, and issued August 29, 2017. http://www.google.se/patents/US9746850.
-
-    """
-    try:
-        assert all(isinstance(v, int) for v in levels), \
-            'levels has to be sequence of integers'
-        assert isinstance(reduction, int) and reduction > 1, \
-            'reduction has to be integer larger than 1'
-        assert isinstance(n, int) and n > 0, \
-            'n has to be positive integer'
-    except AssertionError as e:
-        raise ValueError(e)
-
-    partitions = _make_partitions(levels, reduction)
-    latin_square = _make_latin_square(reduction)
-    ortogonal_arrays = _make_orthogonal_arrays(latin_square, len(levels))
-
-    try:
-        designs = [_map_partitions_to_design(partitions, oa) - 1 for oa in
-                   ortogonal_arrays]
-    except ValueError:
-        raise ValueError('reduction too large compared to factor levels')
-
-    if n == 1:
-        return designs[0]
-    else:
-        return designs[:n]
-
-
-def _make_orthogonal_arrays(latin_square, n_cols):
-    """
-    Augment latin-square to the specified number of columns to produce
-    an orthogonal array.
-    """
-    p = len(latin_square)
-
-    first_row = latin_square[0]
-    A_matrices = [np.array([[v]]) for v in first_row]
-
-    while A_matrices[0].shape[1] < n_cols:
-        new_A_matrices = list()
-
-        for i, A_matrix in enumerate(A_matrices):
-            sub_a = list()
-            for constant, other_A in zip(first_row,
-                                         np.array(A_matrices)[latin_square[i]]):
-                constant_vec = np.repeat(constant, len(other_A))[:, np.newaxis]
-                combined = np.hstack([constant_vec, other_A])
-                sub_a.append(combined)
-
-            new_A_matrices.append(np.vstack(sub_a))
-
-        A_matrices = new_A_matrices
-
-        if A_matrices[0].shape[1] == n_cols:
-            break
-
-    return A_matrices
-
-
-def _map_partitions_to_design(partitions, ortogonal_array):
-    """
-    Map partitioned factor to final design using orthogonal-array produced
-    by augmenting latin square.
-    """
-    assert len(
-        partitions) == ortogonal_array.max() + 1 and ortogonal_array.min() == 0, \
-        'Orthogonal array indexing does not match partition structure'
-
-    mappings = list()
-    for row in ortogonal_array:
-        if any(not partitions[p][factor] for factor, p in enumerate(row)):
-            continue
-
-        partition_sets = [partitions[p][factor] for factor, p in enumerate(row)]
-        mapping = list(itertools.product(*partition_sets))
-        mappings.append(mapping)
-
-    return np.vstack(mappings)
-
-
-def _make_partitions(factor_levels, num_partitions):
-    """
-    Balanced partitioning of factors.
-    """
-    partitions = list()
-    for partition_i in range(1, num_partitions + 1):
-        partition = list()
-
-        for num_levels in factor_levels:
-            part = list()
-            for level_i in range(1, num_levels):
-                index = partition_i + (level_i - 1) * num_partitions
-                if index <= num_levels:
-                    part.append(index)
-
-            partition.append(part)
-
-        partitions.append(partition)
-
-    return partitions
-
-
-def _make_latin_square(n):
-    numbers = np.arange(n)
-    latin_square = np.vstack([np.roll(numbers, -i) for i in range(n)])
-    return latin_square
+"""
+Copyright (C) 2018 - Rickard Sjoegren
+"""
+import itertools
+
+import numpy as np
+
+
+def gsd(levels, reduction, n=1):
+    """
+    Create a Generalized Subset Design (GSD).
+
+    Parameters
+    ----------
+    levels : array-like
+        Number of factor levels per factor in design.
+    reduction : int
+        Reduction factor (bigger than 1). Larger `reduction` means fewer
+        experiments in the design and more possible complementary designs.
+    n : int
+        Number of complementary GSD-designs (default 1). The complementary
+        designs are balanced analogous to fold-over in two-level fractional
+        factorial designs.
+
+    Returns
+    -------
+    H : 2d-array | list of 2d-arrays
+        `n` m-by-k matrices where k is the number of factors (equal
+        to the length of `factor_levels`. The number of rows, m, will
+        be approximately equal to the grand product of the factor levels
+        divided by `reduction`.
+
+    Raises
+    ------
+    ValueError
+        If input is valid or if design construction fails. Design can fail
+        if `reduction` is too large compared to values of `levels`.
+
+    Notes
+    -----
+    The Generalized Subset Design (GSD) [1]_ or generalized factorial design is
+    a generalization of traditional fractional factorial designs to problems
+    where factors can have more than two levels.
+
+    In many application problems factors can have categorical or quantitative
+    factors on more than two levels. Previous reduced designs have not been
+    able to deal with such types of problems. Full multi-level factorial
+    designs can handle such problems but are however not economical regarding
+    the number of experiments.
+
+    Note for commercial users, the application of GSD to testing of product
+    characteristics in a processing facility is patented [2]_
+
+    Examples
+    --------
+    An example with three factors using three, four and
+    six levels respectively reduced with a factor 4 ::
+
+        >>> gsd([3, 4, 6], 4)
+        array([[0, 0, 0],
+               [0, 0, 4],
+               [0, 1, 1],
+               [0, 1, 5],
+               [0, 2, 2],
+               [0, 3, 3],
+               [1, 0, 1],
+               [1, 0, 5],
+               [1, 1, 2],
+               [1, 2, 3],
+               [1, 3, 0],
+               [1, 3, 4],
+               [2, 0, 2],
+               [2, 1, 3],
+               [2, 2, 0],
+               [2, 2, 4],
+               [2, 3, 1],
+               [2, 3, 5]])
+
+    Two complementary designs with two factors using three and
+    four levels reduced with a factor 2 ::
+
+        >>> gsd([3, 4], 2, n=2)[0]
+        array([[0, 0],
+               [0, 2],
+               [2, 0],
+               [2, 2],
+               [1, 1],
+               [1, 3]])
+        >>> gsd([3, 4], 2, n=2)[1]
+        array([[0, 1],
+               [0, 3],
+               [2, 1],
+               [2, 3],
+               [1, 0],
+               [1, 2]])
+
+    If design fails ValueError is raised ::
+
+        >>> gsd([2, 3], 5)
+        Traceback (most recent call last):
+         ...
+        ValueError: reduction too large compared to factor levels
+
+    References
+    ----------
+    .. [1] Surowiec, Izabella, Ludvig Vikstrom, Gustaf Hector, Erik Johansson,
+       Conny Vikstrom, and Johan Trygg. "Generalized Subset Designs in
+       Analytical Chemistry." Analytical Chemistry 89, no. 12 (June 20, 2017):
+       6491-97. https://doi.org/10.1021/acs.analchem.7b00506.
+
+    .. [2] Vikstrom, Ludvig, Conny Vikstrom, Erik Johansson, and Gustaf Hector.
+       Computer-implemented systems and methods for generating
+       generalized fractional designs. US9746850 B2, filed May 9,
+       2014, and issued August 29, 2017. http://www.google.se/patents/US9746850.
+
+    """
+    try:
+        assert all(
+            isinstance(v, int) for v in levels
+        ), "levels has to be sequence of integers"
+        assert (
+            isinstance(reduction, int) and reduction > 1
+        ), "reduction has to be integer larger than 1"
+        assert isinstance(n, int) and n > 0, "n has to be positive integer"
+    except AssertionError as e:
+        raise ValueError(e)
+
+    partitions = _make_partitions(levels, reduction)
+    latin_square = _make_latin_square(reduction)
+    ortogonal_arrays = _make_orthogonal_arrays(latin_square, len(levels))
+
+    try:
+        designs = [
+            _map_partitions_to_design(partitions, oa) - 1 for oa in ortogonal_arrays
+        ]
+    except ValueError:
+        raise ValueError("reduction too large compared to factor levels")
+
+    if n == 1:
+        return designs[0]
+    else:
+        return designs[:n]
+
+
+def _make_orthogonal_arrays(latin_square, n_cols):
+    """
+    Augment latin-square to the specified number of columns to produce
+    an orthogonal array.
+    """
+    p = len(latin_square)
+
+    first_row = latin_square[0]
+    A_matrices = [np.array([[v]]) for v in first_row]
+
+    while A_matrices[0].shape[1] < n_cols:
+        new_A_matrices = list()
+
+        for i, A_matrix in enumerate(A_matrices):
+            sub_a = list()
+            for constant, other_A in zip(
+                first_row, np.array(A_matrices)[latin_square[i]]
+            ):
+                constant_vec = np.repeat(constant, len(other_A))[:, np.newaxis]
+                combined = np.hstack([constant_vec, other_A])
+                sub_a.append(combined)
+
+            new_A_matrices.append(np.vstack(sub_a))
+
+        A_matrices = new_A_matrices
+
+        if A_matrices[0].shape[1] == n_cols:
+            break
+
+    return A_matrices
+
+
+def _map_partitions_to_design(partitions, ortogonal_array):
+    """
+    Map partitioned factor to final design using orthogonal-array produced
+    by augmenting latin square.
+    """
+    assert (
+        len(partitions) == ortogonal_array.max() + 1 and ortogonal_array.min() == 0
+    ), "Orthogonal array indexing does not match partition structure"
+
+    mappings = list()
+    for row in ortogonal_array:
+        if any(not partitions[p][factor] for factor, p in enumerate(row)):
+            continue
+
+        partition_sets = [partitions[p][factor] for factor, p in enumerate(row)]
+        mapping = list(itertools.product(*partition_sets))
+        mappings.append(mapping)
+
+    return np.vstack(mappings)
+
+
+def _make_partitions(factor_levels, num_partitions):
+    """
+    Balanced partitioning of factors.
+    """
+    partitions = list()
+    for partition_i in range(1, num_partitions + 1):
+        partition = list()
+
+        for num_levels in factor_levels:
+            part = list()
+            for level_i in range(1, num_levels):
+                index = partition_i + (level_i - 1) * num_partitions
+                if index <= num_levels:
+                    part.append(index)
+
+            partition.append(part)
+
+        partitions.append(partition)
+
+    return partitions
+
+
+def _make_latin_square(n):
+    numbers = np.arange(n)
+    latin_square = np.vstack([np.roll(numbers, -i) for i in range(n)])
+    return latin_square
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_lhs.py` & `pydoe3-1.0.1/pyDOE3/doe_lhs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,277 +1,301 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-from scipy import spatial
-from scipy import stats
-from scipy import linalg
-from numpy import ma
-
-__all__ = ['lhs']
-
-
-def lhs(n, samples=None, criterion=None, iterations=None, random_state=None, correlation_matrix = None):
-    """
-    Generate a latin-hypercube design
-
-    Parameters
-    ----------
-    n : int
-        The number of factors to generate samples for
-
-    Optional
-    --------
-    samples : int
-        The number of samples to generate for each factor (Default: n)
-    criterion : str
-        Allowable values are "center" or "c", "maximin" or "m",
-        "centermaximin" or "cm", and "correlation" or "corr". If no value
-        given, the design is simply randomized.
-    iterations : int
-        The number of iterations in the maximin and correlations algorithms
-        (Default: 5).
-    randomstate : np.random.RandomState, int
-         Random state (or seed-number) which controls the seed and random draws
-    correlation_matrix : ndarray
-         Enforce correlation between factors (only used in lhsmu)
-
-    Returns
-    -------
-    H : 2d-array
-        An n-by-samples design matrix that has been normalized so factor values
-        are uniformly spaced between zero and one.
-
-    Example
-    -------
-    A 3-factor design (defaults to 3 samples)::
-
-        >>> lhs(3, random_state=42)
-        array([[ 0.12484671,  0.95539205,  0.24399798],
-               [ 0.53288616,  0.38533955,  0.86703834],
-               [ 0.68602787,  0.31690477,  0.38533151]])
-
-    A 4-factor design with 6 samples::
-
-        >>> lhs(4, samples=6, random_state=42)
-        array([[ 0.06242335,  0.19266575,  0.88202411,  0.89439364],
-               [ 0.19266977,  0.53538985,  0.53030416,  0.49498498],
-               [ 0.71737371,  0.75412607,  0.17634727,  0.71520486],
-               [ 0.63874044,  0.85658231,  0.33676408,  0.31102936],
-               [ 0.43351917,  0.45134543,  0.12199899,  0.53056742],
-               [ 0.93530882,  0.15845238,  0.7386575 ,  0.09977641]])
-
-    A 2-factor design with 5 centered samples::
-
-        >>> lhs(2, samples=5, criterion='center', random_state=42)
-        array([[ 0.1,  0.9],
-               [ 0.5,  0.5],
-               [ 0.7,  0.1],
-               [ 0.3,  0.7],
-               [ 0.9,  0.3]])
-
-    A 3-factor design with 4 samples where the minimum distance between
-    all samples has been maximized::
-
-        >>> lhs(3, samples=4, criterion='maximin', random_state=42)
-        array([[ 0.69754389,  0.2997106 ,  0.96250964],
-               [ 0.10585037,  0.09872038,  0.73157522],
-               [ 0.25351996,  0.65148999,  0.07337204],
-               [ 0.91276926,  0.97873992,  0.42783549]])
-
-    A 4-factor design with 5 samples where the samples are as uncorrelated
-    as possible (within 10 iterations)::
-
-        >>> lhs(4, samples=5, criterion='correlation', iterations=10, random_state=42)
-        array([[ 0.72088348,  0.05121366,  0.97609357,  0.92487081],
-               [ 0.49507404,  0.51265511,  0.00808672,  0.37915272],
-               [ 0.22217816,  0.2878673 ,  0.24034384,  0.42786629],
-               [ 0.91977309,  0.93895699,  0.64061224,  0.14213258],
-               [ 0.04719698,  0.70796822,  0.53910322,  0.78857071]])
-
-    """
-    H = None
-
-    if random_state is None:
-        random_state = np.random.RandomState()
-    elif not isinstance(random_state, np.random.RandomState):
-        random_state = np.random.RandomState(random_state)
-
-    if samples is None:
-        samples = n
-
-    if criterion is not None:
-        if not criterion.lower() in ('center', 'c', 'maximin', 'm',
-                                     'centermaximin', 'cm', 'correlation',
-                                     'corr','lhsmu'):
-            raise ValueError('Invalid value for "criterion": {}'.format(criterion))
-
-    else:
-        H = _lhsclassic(n, samples, random_state)
-
-    if criterion is None:
-        criterion = 'center'
-    if iterations is None:
-        iterations = 5
-
-    if H is None:
-        if criterion.lower() in ('center', 'c'):
-            H = _lhscentered(n, samples, random_state)
-        elif criterion.lower() in ('maximin', 'm'):
-            H = _lhsmaximin(n, samples, iterations, 'maximin', random_state)
-        elif criterion.lower() in ('centermaximin', 'cm'):
-            H = _lhsmaximin(n, samples, iterations, 'centermaximin', random_state)
-        elif criterion.lower() in ('correlation', 'corr'):
-            H = _lhscorrelate(n, samples, iterations, random_state)
-        elif criterion.lower() in ('lhsmu'):
-            # as specified by the paper. M is set to 5
-            H = _lhsmu(n, samples, correlation_matrix, random_state, M=5)
-
-    return H
-
-################################################################################
-
-def _lhsclassic(n, samples, randomstate):
-    # Generate the intervals
-    cut = np.linspace(0, 1, samples + 1)    
-    
-    # Fill points uniformly in each interval
-    u = randomstate.rand(samples, n)
-    a = cut[:samples]
-    b = cut[1:samples + 1]
-    rdpoints = np.zeros_like(u)
-    for j in range(n):
-        rdpoints[:, j] = u[:, j]*(b-a) + a
-    
-    # Make the random pairings
-    H = np.zeros_like(rdpoints)
-    for j in range(n):
-        order = randomstate.permutation(range(samples))
-        H[:, j] = rdpoints[order, j]
-    
-    return H
-    
-################################################################################
-
-def _lhscentered(n, samples, randomstate):
-    # Generate the intervals
-    cut = np.linspace(0, 1, samples + 1)    
-    
-    # Fill points uniformly in each interval
-    u = randomstate.rand(samples, n)
-    a = cut[:samples]
-    b = cut[1:samples + 1]
-    _center = (a + b)/2
-    
-    # Make the random pairings
-    H = np.zeros_like(u)
-    for j in range(n):
-        H[:, j] = randomstate.permutation(_center)
-    
-    return H
-    
-################################################################################
-
-def _lhsmaximin(n, samples, iterations, lhstype, randomstate):
-    maxdist = 0
-    
-    # Maximize the minimum distance between points
-    for i in range(iterations):
-        if lhstype=='maximin':
-            Hcandidate = _lhsclassic(n, samples, randomstate)
-        else:
-            Hcandidate = _lhscentered(n, samples, randomstate)
-        
-        d = spatial.distance.pdist(Hcandidate, 'euclidean')
-        if maxdist<np.min(d):
-            maxdist = np.min(d)
-            H = Hcandidate.copy()
-    
-    return H
-
-################################################################################
-
-def _lhscorrelate(n, samples, iterations, randomstate):
-    mincorr = np.inf
-    
-    # Minimize the components correlation coefficients
-    for i in range(iterations):
-        # Generate a random LHS
-        Hcandidate = _lhsclassic(n, samples, randomstate)
-        R = np.corrcoef(Hcandidate.T)
-        if np.max(np.abs(R[R!=1]))<mincorr:
-            mincorr = np.max(np.abs(R-np.eye(R.shape[0])))
-            H = Hcandidate.copy()
-    
-    return H
- 
- ################################################################################
-
-def _lhsmu(N, samples=None, corr=None, random_state=None, M=5):
-
-    if random_state is None:
-        random_state = np.random.RandomState()
-    elif not isinstance(random_state, np.random.RandomState):
-        random_state = np.random.RandomState(random_state)
-
-    if samples is None:
-        samples = N
-
-    I = M*samples
-
-    rdpoints = random_state.uniform(size=(I, N))
-
-    dist = spatial.distance.cdist(rdpoints, rdpoints, metric='euclidean')
-    D_ij = ma.masked_array(dist, mask=np.identity(I))
-
-    index_rm = np.zeros(I-samples, dtype=int)
-    i = 0
-    while i < I-samples:
-        order = ma.sort(D_ij, axis=1)
-
-        avg_dist = ma.mean(order[:, 0:2], axis=1)
-        min_l = ma.argmin(avg_dist)
-
-        D_ij[min_l, :] = ma.masked
-        D_ij[:, min_l] = ma.masked
-
-        index_rm[i] = min_l
-        i += 1
-
-    rdpoints = np.delete(rdpoints, index_rm, axis=0)
-
-    if(corr is not None):
-        #check if covariance matrix is valid
-        assert type(corr) == np.ndarray
-        assert corr.ndim == 2
-        assert corr.shape[0] == corr.shape[1]
-        assert corr.shape[0] == N
-
-        norm_u = stats.norm().ppf(rdpoints)
-        L = linalg.cholesky(corr, lower=True)
-
-        norm_u = np.matmul(norm_u, L)
-
-        H = stats.norm().cdf(norm_u)
-    else:
-        H = np.zeros_like(rdpoints, dtype=float)
-        rank = np.argsort(rdpoints, axis=0)
-
-        for l in range(samples):
-            low = float(l)/samples
-            high = float(l+1)/samples
-
-            l_pos = rank == l
-            H[l_pos] = random_state.uniform(low, high, size=N)
-    return H
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+from scipy import spatial
+from scipy import stats
+from scipy import linalg
+from numpy import ma
+
+__all__ = ["lhs"]
+
+
+def lhs(
+    n,
+    samples=None,
+    criterion=None,
+    iterations=None,
+    random_state=None,
+    correlation_matrix=None,
+):
+    """
+    Generate a latin-hypercube design
+
+    Parameters
+    ----------
+    n : int
+        The number of factors to generate samples for
+
+    Optional
+    --------
+    samples : int
+        The number of samples to generate for each factor (Default: n)
+    criterion : str
+        Allowable values are "center" or "c", "maximin" or "m",
+        "centermaximin" or "cm", and "correlation" or "corr". If no value
+        given, the design is simply randomized.
+    iterations : int
+        The number of iterations in the maximin and correlations algorithms
+        (Default: 5).
+    randomstate : np.random.RandomState, int
+         Random state (or seed-number) which controls the seed and random draws
+    correlation_matrix : ndarray
+         Enforce correlation between factors (only used in lhsmu)
+
+    Returns
+    -------
+    H : 2d-array
+        An n-by-samples design matrix that has been normalized so factor values
+        are uniformly spaced between zero and one.
+
+    Example
+    -------
+    A 3-factor design (defaults to 3 samples)::
+
+        >>> lhs(3, random_state=42)
+        array([[0.12484671, 0.95539205, 0.24399798],
+               [0.53288616, 0.38533955, 0.86703834],
+               [0.68602787, 0.31690477, 0.38533151]])
+
+    A 4-factor design with 6 samples::
+
+        >>> lhs(4, samples=6, random_state=42)
+        array([[0.06242335, 0.19266575, 0.88202411, 0.89439364],
+               [0.19266977, 0.53538985, 0.53030416, 0.49498498],
+               [0.71737371, 0.75412607, 0.17634727, 0.71520486],
+               [0.63874044, 0.85658231, 0.33676408, 0.31102936],
+               [0.43351917, 0.45134543, 0.12199899, 0.53056742],
+               [0.93530882, 0.15845238, 0.7386575 , 0.09977641]])
+
+    A 2-factor design with 5 centered samples::
+
+        >>> lhs(2, samples=5, criterion='center', random_state=42)
+        array([[0.1, 0.9],
+               [0.5, 0.5],
+               [0.7, 0.1],
+               [0.3, 0.7],
+               [0.9, 0.3]])
+
+    A 3-factor design with 4 samples where the minimum distance between
+    all samples has been maximized::
+
+        >>> lhs(3, samples=4, criterion='maximin', random_state=42)
+        array([[0.69754389, 0.2997106 , 0.96250964],
+               [0.10585037, 0.09872038, 0.73157522],
+               [0.25351996, 0.65148999, 0.07337204],
+               [0.91276926, 0.97873992, 0.42783549]])
+
+    A 4-factor design with 5 samples where the samples are as uncorrelated
+    as possible (within 10 iterations)::
+
+        >>> lhs(4, samples=5, criterion='correlation', iterations=10, random_state=42)
+        array([[0.4846803 , 0.74226839, 0.23305339, 0.97000772],
+               [0.98526018, 0.11735023, 0.75803511, 0.20312728],
+               [0.10793843, 0.2592547 , 0.98299194, 0.72119199],
+               [0.25519984, 0.4789763 , 0.19305106, 0.12140685],
+               [0.63976848, 0.93021541, 0.45869763, 0.40281596]])
+
+    """
+    H = None
+
+    if random_state is None:
+        random_state = np.random.RandomState()
+    elif not isinstance(random_state, np.random.RandomState):
+        random_state = np.random.RandomState(random_state)
+
+    if samples is None:
+        samples = n
+
+    if criterion is not None:
+        if not criterion.lower() in (
+            "center",
+            "c",
+            "maximin",
+            "m",
+            "centermaximin",
+            "cm",
+            "correlation",
+            "corr",
+            "lhsmu",
+        ):
+            raise ValueError('Invalid value for "criterion": {}'.format(criterion))
+
+    else:
+        H = _lhsclassic(n, samples, random_state)
+
+    if criterion is None:
+        criterion = "center"
+    if iterations is None:
+        iterations = 5
+
+    if H is None:
+        if criterion.lower() in ("center", "c"):
+            H = _lhscentered(n, samples, random_state)
+        elif criterion.lower() in ("maximin", "m"):
+            H = _lhsmaximin(n, samples, iterations, "maximin", random_state)
+        elif criterion.lower() in ("centermaximin", "cm"):
+            H = _lhsmaximin(n, samples, iterations, "centermaximin", random_state)
+        elif criterion.lower() in ("correlation", "corr"):
+            H = _lhscorrelate(n, samples, iterations, random_state)
+        elif criterion.lower() in ("lhsmu"):
+            # as specified by the paper. M is set to 5
+            H = _lhsmu(n, samples, correlation_matrix, random_state, M=5)
+
+    return H
+
+
+################################################################################
+
+
+def _lhsclassic(n, samples, randomstate):
+    # Generate the intervals
+    cut = np.linspace(0, 1, samples + 1)
+
+    # Fill points uniformly in each interval
+    u = randomstate.rand(samples, n)
+    a = cut[:samples]
+    b = cut[1 : samples + 1]
+    rdpoints = np.zeros_like(u)
+    for j in range(n):
+        rdpoints[:, j] = u[:, j] * (b - a) + a
+
+    # Make the random pairings
+    H = np.zeros_like(rdpoints)
+    for j in range(n):
+        order = randomstate.permutation(range(samples))
+        H[:, j] = rdpoints[order, j]
+
+    return H
+
+
+################################################################################
+
+
+def _lhscentered(n, samples, randomstate):
+    # Generate the intervals
+    cut = np.linspace(0, 1, samples + 1)
+
+    # Fill points uniformly in each interval
+    u = randomstate.rand(samples, n)
+    a = cut[:samples]
+    b = cut[1 : samples + 1]
+    _center = (a + b) / 2
+
+    # Make the random pairings
+    H = np.zeros_like(u)
+    for j in range(n):
+        H[:, j] = randomstate.permutation(_center)
+
+    return H
+
+
+################################################################################
+
+
+def _lhsmaximin(n, samples, iterations, lhstype, randomstate):
+    maxdist = 0
+
+    # Maximize the minimum distance between points
+    for i in range(iterations):
+        if lhstype == "maximin":
+            Hcandidate = _lhsclassic(n, samples, randomstate)
+        else:
+            Hcandidate = _lhscentered(n, samples, randomstate)
+
+        d = spatial.distance.pdist(Hcandidate, "euclidean")
+        if maxdist < np.min(d):
+            maxdist = np.min(d)
+            H = Hcandidate.copy()
+
+    return H
+
+
+################################################################################
+
+
+def _lhscorrelate(n, samples, iterations, randomstate):
+    mincorr = np.inf
+
+    # Minimize the components correlation coefficients
+    for i in range(iterations):
+        # Generate a random LHS
+        Hcandidate = _lhsclassic(n, samples, randomstate)
+        R = np.corrcoef(Hcandidate.T)
+        if np.max(np.abs(R[R != 1])) < mincorr:
+            mincorr = np.max(np.abs(R - np.eye(R.shape[0])))
+            H = Hcandidate.copy()
+
+    return H
+
+
+################################################################################
+
+
+def _lhsmu(N, samples=None, corr=None, random_state=None, M=5):
+    if random_state is None:
+        random_state = np.random.RandomState()
+    elif not isinstance(random_state, np.random.RandomState):
+        random_state = np.random.RandomState(random_state)
+
+    if samples is None:
+        samples = N
+
+    I = M * samples
+
+    rdpoints = random_state.uniform(size=(I, N))
+
+    dist = spatial.distance.cdist(rdpoints, rdpoints, metric="euclidean")
+    D_ij = ma.masked_array(dist, mask=np.identity(I))
+
+    index_rm = np.zeros(I - samples, dtype=int)
+    i = 0
+    while i < I - samples:
+        order = ma.sort(D_ij, axis=1)
+
+        avg_dist = ma.mean(order[:, 0:2], axis=1)
+        min_l = ma.argmin(avg_dist)
+
+        D_ij[min_l, :] = ma.masked
+        D_ij[:, min_l] = ma.masked
+
+        index_rm[i] = min_l
+        i += 1
+
+    rdpoints = np.delete(rdpoints, index_rm, axis=0)
+
+    if corr is not None:
+        # check if covariance matrix is valid
+        assert type(corr) == np.ndarray
+        assert corr.ndim == 2
+        assert corr.shape[0] == corr.shape[1]
+        assert corr.shape[0] == N
+
+        norm_u = stats.norm().ppf(rdpoints)
+        L = linalg.cholesky(corr, lower=True)
+
+        norm_u = np.matmul(norm_u, L)
+
+        H = stats.norm().cdf(norm_u)
+    else:
+        H = np.zeros_like(rdpoints, dtype=float)
+        rank = np.argsort(rdpoints, axis=0)
+
+        for l in range(samples):
+            low = float(l) / samples
+            high = float(l + 1) / samples
+
+            l_pos = rank == l
+            H[l_pos] = random_state.uniform(low, high, size=N)
+    return H
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_repeat_center.py` & `pydoe3-1.0.1/pyDOE3/doe_repeat_center.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-
-def repeat_center(n, repeat):
-    """
-    Create the center-point portion of a design matrix
-    
-    Parameters
-    ----------
-    n : int
-        The number of factors in the original design
-    repeat : int
-        The number of center points to repeat
-    
-    Returns
-    -------
-    mat : 2d-array
-        The center-point portion of a design matrix (elements all zero).
-    
-    Example
-    -------
-    ::
-    
-        >>> repeat_center(3, 2)
-        array([[ 0.,  0.,  0.],
-               [ 0.,  0.,  0.]])
-       
-    """
-    return np.zeros((repeat, n))
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+
+
+def repeat_center(n, repeat):
+    """
+    Create the center-point portion of a design matrix
+
+    Parameters
+    ----------
+    n : int
+        The number of factors in the original design
+    repeat : int
+        The number of center points to repeat
+
+    Returns
+    -------
+    mat : 2d-array
+        The center-point portion of a design matrix (elements all zero).
+
+    Example
+    -------
+    ::
+
+        >>> repeat_center(3, 2)
+        array([[0., 0., 0.],
+               [0., 0., 0.]])
+
+    """
+    return np.zeros((repeat, n))
```

### Comparing `pydoe3-1.0.0/pyDOE3/doe_union.py` & `pydoe3-1.0.1/pyDOE3/doe_union.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-
-def union(H1, H2):
-    """
-    Join two matrices by stacking them on top of each other.
-    
-    Parameters
-    ----------
-    H1 : 2d-array
-        The matrix that goes on top of the new matrix
-    H2 : 2d-array
-        The matrix that goes on bottom of the new matrix
-    
-    Returns
-    -------
-    mat : 2d-array
-        The new matrix that contains the rows of ``H1`` on top of the rows of
-        ``H2``.
-    
-    Example
-    -------
-    ::
-    
-        >>> union(np.eye(2), -np.eye(2))
-        array([[ 1.,  0.],
-               [ 0.,  1.],
-               [-1.,  0.],
-               [ 0., -1.]])
-               
-    """
-    H = np.r_[H1, H2]
-    return H
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+
+
+def union(H1, H2):
+    """
+    Join two matrices by stacking them on top of each other.
+
+    Parameters
+    ----------
+    H1 : 2d-array
+        The matrix that goes on top of the new matrix
+    H2 : 2d-array
+        The matrix that goes on bottom of the new matrix
+
+    Returns
+    -------
+    mat : 2d-array
+        The new matrix that contains the rows of ``H1`` on top of the rows of
+        ``H2``.
+
+    Example
+    -------
+    ::
+
+        >>> union(np.eye(2), 2 * np.eye(2))
+        array([[1., 0.],
+               [0., 1.],
+               [2., 0.],
+               [0., 2.]])
+
+    """
+    H = np.r_[H1, H2]
+    return H
```

### Comparing `pydoe3-1.0.0/pyDOE3/var_regression_matrix.py` & `pydoe3-1.0.1/pyDOE3/var_regression_matrix.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-"""
-This code was originally published by the following individuals for use with
-Scilab:
-    Copyright (C) 2012 - 2013 - Michael Baudin
-    Copyright (C) 2012 - Maria Christopoulou
-    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-    Copyright (C) 2009 - Yann Collette
-    Copyright (C) 2009 - CEA - Jean-Marc Martinez
-    
-    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-Much thanks goes to these individuals. It has been converted to Python by 
-Abraham Lee.
-"""
-
-import numpy as np
-
-def var_regression_matrix(H, x, model, sigma=1):
-    """
-    Compute the variance of the 'regression error'.
-    
-    Parameters
-    ----------
-    H : 2d-array
-        The regression matrix
-    x : 2d-array
-        The coordinates to calculate the regression error variance at.
-    model : str
-        A string of tokens that define the regression model (e.g. 
-        '1 x1 x2 x1*x2')
-    sigma : scalar
-        An estimate of the variance (default: 1).
-    
-    Returns
-    -------
-    var : scalar
-        The variance of the regression error, evaluated at ``x``.
-        
-    """
-    x = np.atleast_2d(x)
-    H = np.atleast_2d(H)
-    
-    if x.shape[0]==1:
-        x = x.T
-    
-    if np.rank(H)<(np.dot(H.T, H)).shape[0]:
-        raise ValueError("model and DOE don't suit together")
-    
-    x_mod = build_regression_matrix(x, model)
-    var = sigma**2*np.dot(np.dot(x_mod.T, np.linalg.inv(np.dot(H.T, H))), x_mod)
-    return var
+"""
+This code was originally published by the following individuals for use with
+Scilab:
+    Copyright (C) 2012 - 2013 - Michael Baudin
+    Copyright (C) 2012 - Maria Christopoulou
+    Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+    Copyright (C) 2009 - Yann Collette
+    Copyright (C) 2009 - CEA - Jean-Marc Martinez
+    
+    website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+Much thanks goes to these individuals. It has been converted to Python by 
+Abraham Lee.
+"""
+
+import numpy as np
+
+
+def var_regression_matrix(H, x, model, sigma=1):
+    """
+    Compute the variance of the 'regression error'.
+
+    Parameters
+    ----------
+    H : 2d-array
+        The regression matrix
+    x : 2d-array
+        The coordinates to calculate the regression error variance at.
+    model : str
+        A string of tokens that define the regression model (e.g.
+        '1 x1 x2 x1*x2')
+    sigma : scalar
+        An estimate of the variance (default: 1).
+
+    Returns
+    -------
+    var : scalar
+        The variance of the regression error, evaluated at ``x``.
+
+    """
+    x = np.atleast_2d(x)
+    H = np.atleast_2d(H)
+
+    if x.shape[0] == 1:
+        x = x.T
+
+    if np.rank(H) < (np.dot(H.T, H)).shape[0]:
+        raise ValueError("model and DOE don't suit together")
+
+    x_mod = build_regression_matrix(x, model)
+    var = sigma**2 * np.dot(np.dot(x_mod.T, np.linalg.inv(np.dot(H.T, H))), x_mod)
+    return var
```

### Comparing `pydoe3-1.0.0/LICENSE` & `pydoe3-1.0.1/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-Copyright (c) 2014, Abraham D. Lee
-Copyright (c) 2018, Rickard Sjögren & Daniel Svensson
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice,
-this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-this list of conditions and the following disclaimer in the documentation
-and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors
-may be used to endorse or promote products derived from this software without
-specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS
-BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY,
-OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
-THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2014, Abraham D. Lee
+Copyright (c) 2018, Rickard Sjögren & Daniel Svensson
+Copyright (c) 2023, Rémi Lafage
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice,
+this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+this list of conditions and the following disclaimer in the documentation
+and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors
+may be used to endorse or promote products derived from this software without
+specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS
+BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY,
+OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
+THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pydoe3-1.0.0/README.md` & `pydoe3-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,90 @@
-pyDOE3: An experimental design package for python
-=====================================================
-
-`pyDOE3` is a fork of the [`pyDOE2`](https://github.com/clicumu/pyDOE2) package 
-that is designed to help the scientist, engineer, statistician, etc., to 
-construct appropriate experimental designs.
-
-This fork came to life to solve bugs and issues that remained unsolved in the
-original package.
-
-Capabilities
-------------
-
-The package currently includes functions for creating designs for any 
-number of factors:
-
-- Factorial Designs
-    - General Full-Factorial (``fullfact``)
-    - 2-level Full-Factorial (``ff2n``)
-    - 2-level Fractional Factorial (``fracfact``)
-    - Plackett-Burman (``pbdesign``)
-    - Generalized Subset Designs (``gsd``)
-- Response-Surface Designs 
-    - Box-Behnken (``bbdesign``)
-    - Central-Composite (``ccdesign``)
-- Randomized Designs
-    - Latin-Hypercube (``lhs``)
-  
-See the original [pyDOE homepage](http://pythonhosted.org/pyDOE) for details
-on usage and other notes.
-
-Requirements
-------------
-
-- NumPy
-- SciPy
-
-Installation and download
--------------------------
-
-Through pip:
-
-```
-pip install pyDOE3
-```
-
-
-Credits
--------
-
-`pyDOE` original code was originally converted from code by the following 
-individuals for use with Scilab:
-    
-- Copyright (C) 2012 - 2013 - Michael Baudin
-- Copyright (C) 2012 - Maria Christopoulou
-- Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
-- Copyright (C) 2009 - Yann Collette
-- Copyright (C) 2009 - CEA - Jean-Marc Martinez
-
-- Website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
-
-`pyDOE` was converted to Python by the following individual:
-
-- Copyright (c) 2014, Abraham D. Lee
-
-The following individuals forked and work on `pyDOE2`:
-
-- Copyright (C) 2018 - Rickard Sjögren and Daniel Svensson
-
-
-License
--------
-
-This package is provided under the *BSD License* (3-clause)
-
-References
-----------
-
-- [Factorial designs](http://en.wikipedia.org/wiki/Factorial_experiment)
-- [Plackett-Burman designs](http://en.wikipedia.org/wiki/Plackett-Burman_design)
-- [Box-Behnken designs](http://en.wikipedia.org/wiki/Box-Behnken_design)
-- [Central composite designs](http://en.wikipedia.org/wiki/Central_composite_design)
-- [Latin-Hypercube designs](http://en.wikipedia.org/wiki/Latin_hypercube_sampling)
-- Surowiec, Izabella, Ludvig Vikström, Gustaf Hector, Erik Johansson,
-Conny Vikström, and Johan Trygg. “Generalized Subset Designs in Analytical
-Chemistry.” Analytical Chemistry 89, no. 12 (June 20, 2017): 6491–97.
-https://doi.org/10.1021/acs.analchem.7b00506.
+[![Tests](https://github.com/relf/pyDOE3/actions/workflows/tests.yml/badge.svg)](https://github.com/relf/pyDOE3/actions/workflows/tests.yml)
+[![Documentation](https://readthedocs.org/projects/pydoe3/badge/?version=latest)](https://pydoe3.readthedocs.io/en/latest/?badge=latest)
+
+
+pyDOE3: An experimental design package for python
+=====================================================
+
+`pyDOE3` is a fork of the [`pyDOE2`](https://github.com/clicumu/pyDOE2) package 
+that is designed to help the scientist, engineer, statistician, etc., to 
+construct appropriate experimental designs.
+
+This fork came to life to solve bugs and issues that remained unsolved in the
+original package.
+
+
+Capabilities
+------------
+
+The package currently includes functions for creating designs for any 
+number of factors:
+
+- Factorial Designs
+    - General Full-Factorial (``fullfact``)
+    - 2-level Full-Factorial (``ff2n``)
+    - 2-level Fractional Factorial (``fracfact``)
+    - Plackett-Burman (``pbdesign``)
+    - Generalized Subset Designs (``gsd``)
+- Response-Surface Designs 
+    - Box-Behnken (``bbdesign``)
+    - Central-Composite (``ccdesign``)
+- Randomized Designs
+    - Latin-Hypercube (``lhs``)
+  
+See [Documentation](https://pydoe3.readthedocs.io).
+
+Requirements
+------------
+
+- NumPy
+- SciPy
+
+
+Installation
+------------
+
+```
+pip install pyDOE3
+```
+
+
+Credits
+-------
+
+`pyDOE` original code was originally converted from code by the following 
+individuals for use with Scilab:
+    
+- Copyright (C) 2012 - 2013 - Michael Baudin
+- Copyright (C) 2012 - Maria Christopoulou
+- Copyright (C) 2010 - 2011 - INRIA - Michael Baudin
+- Copyright (C) 2009 - Yann Collette
+- Copyright (C) 2009 - CEA - Jean-Marc Martinez
+
+- Website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
+
+`pyDOE` was converted to Python by the following individual:
+
+- Copyright (c) 2014, Abraham D. Lee & timsimst
+
+The following individuals forked and work on `pyDOE2`:
+
+- Copyright (C) 2018 - Rickard Sjögren and Daniel Svensson
+
+
+License
+-------
+
+This package is provided under the *BSD License* (3-clause)
+
+References
+----------
+
+- [Factorial designs](http://en.wikipedia.org/wiki/Factorial_experiment)
+- [Plackett-Burman designs](http://en.wikipedia.org/wiki/Plackett-Burman_design)
+- [Box-Behnken designs](http://en.wikipedia.org/wiki/Box-Behnken_design)
+- [Central composite designs](http://en.wikipedia.org/wiki/Central_composite_design)
+- [Latin-Hypercube designs](http://en.wikipedia.org/wiki/Latin_hypercube_sampling)
+- Surowiec, Izabella, Ludvig Vikström, Gustaf Hector, Erik Johansson,
+Conny Vikström, and Johan Trygg. “Generalized Subset Designs in Analytical
+Chemistry.” Analytical Chemistry 89, no. 12 (June 20, 2017): 6491–97.
+https://doi.org/10.1021/acs.analchem.7b00506.
```

### Comparing `pydoe3-1.0.0/PKG-INFO` & `pydoe3-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: pyDOE3
-Version: 1.0.0
+Version: 1.0.1
 Summary: Design of experiments for Python
 Project-URL: source, https://github.com/relf/pyDOE3
 Author-email: Rémi Lafage <remi.lafage@onera.fr>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: DOE,design of experiments,experimental design,optimization,python,statistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: numpy
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
+[![Tests](https://github.com/relf/pyDOE3/actions/workflows/tests.yml/badge.svg)](https://github.com/relf/pyDOE3/actions/workflows/tests.yml)
+[![Documentation](https://readthedocs.org/projects/pydoe3/badge/?version=latest)](https://pydoe3.readthedocs.io/en/latest/?badge=latest)
+
+
 pyDOE3: An experimental design package for python
 =====================================================
 
 `pyDOE3` is a fork of the [`pyDOE2`](https://github.com/clicumu/pyDOE2) package 
 that is designed to help the scientist, engineer, statistician, etc., to 
 construct appropriate experimental designs.
 
 This fork came to life to solve bugs and issues that remained unsolved in the
 original package.
 
+
 Capabilities
 ------------
 
 The package currently includes functions for creating designs for any 
 number of factors:
 
 - Factorial Designs
@@ -55,27 +58,25 @@
     - Generalized Subset Designs (``gsd``)
 - Response-Surface Designs 
     - Box-Behnken (``bbdesign``)
     - Central-Composite (``ccdesign``)
 - Randomized Designs
     - Latin-Hypercube (``lhs``)
   
-See the original [pyDOE homepage](http://pythonhosted.org/pyDOE) for details
-on usage and other notes.
+See [Documentation](https://pydoe3.readthedocs.io).
 
 Requirements
 ------------
 
 - NumPy
 - SciPy
 
-Installation and download
--------------------------
 
-Through pip:
+Installation
+------------
 
 ```
 pip install pyDOE3
 ```
 
 
 Credits
@@ -90,15 +91,15 @@
 - Copyright (C) 2009 - Yann Collette
 - Copyright (C) 2009 - CEA - Jean-Marc Martinez
 
 - Website: forge.scilab.org/index.php/p/scidoe/sourcetree/master/macros
 
 `pyDOE` was converted to Python by the following individual:
 
-- Copyright (c) 2014, Abraham D. Lee
+- Copyright (c) 2014, Abraham D. Lee & timsimst
 
 The following individuals forked and work on `pyDOE2`:
 
 - Copyright (C) 2018 - Rickard Sjögren and Daniel Svensson
 
 
 License
```

