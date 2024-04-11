# Comparing `tmp/geocs-0.1.0.tar.gz` & `tmp/geocs-1.0.0.tar.gz`

## Comparing `geocs-0.1.0.tar` & `geocs-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,67 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 geocs-0.1.0/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geocs-0.1.0/src/GeoCS/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 geocs-0.1.0/src/GeoCS/data/BaseData.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 geocs-0.1.0/src/GeoCS/data/TypeData.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geocs-0.1.0/src/GeoCS/operations/__init__.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 geocs-0.1.0/src/GeoCS/operations/plotLib.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 geocs-0.1.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 geocs-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geocs-0.1.0/README.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 geocs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 geocs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 geocs-1.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 geocs-1.0.0/CITATION.cff
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 geocs-1.0.0/noxfile.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/index.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/.buildinfo
+-rw-r--r--   0        0        0    30297 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/genindex.html
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/index.html
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/objects.inv
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/py-modindex.html
+-rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/search.html
+-rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/searchindex.js
+-rw-r--r--   0        0        0  2722108 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/.doctrees/index.doctree
+-rw-r--r--   0        0        0   396838 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/.doctrees/source/GeoCS.doctree
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/.doctrees/source/modules.doctree
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/.doctrees/tutorials/installation.doctree
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_sources/index.md.txt
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_sources/source/GeoCS.rst.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_sources/source/modules.rst.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_sources/tutorials/installation.md.txt
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/basic.css
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/clipboard.min.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/copy-button.svg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/copybutton.css
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/copybutton.js
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/debug.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/doctools.js
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/plus.png
+-rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/searchtools.js
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/skeleton.css
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/scripts/furo-extensions.js
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/scripts/furo.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0        0        0    28551 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/scripts/furo.js.map
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/styles/furo-extensions.css
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/styles/furo-extensions.css.map
+-rw-r--r--   0        0        0    48265 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/styles/furo.css
+-rw-r--r--   0        0        0    72783 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/_static/styles/furo.css.map
+-rw-r--r--   0        0        0   159256 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/source/GeoCS.html
+-rw-r--r--   0        0        0    32207 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/source/modules.html
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/build/tutorials/installation.html
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/source/GeoCS.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/source/modules.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 geocs-1.0.0/docs/tutorials/installation.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 geocs-1.0.0/src/GeoCS/__init__.py
+-rw-r--r--   0        0        0    10378 2020-02-02 00:00:00.000000 geocs-1.0.0/src/GeoCS/calc_lib.py
+-rw-r--r--   0        0        0    26663 2020-02-02 00:00:00.000000 geocs-1.0.0/src/GeoCS/data_lib.py
+-rw-r--r--   0        0        0    17409 2020-02-02 00:00:00.000000 geocs-1.0.0/src/GeoCS/plot_lib.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 geocs-1.0.0/tests/some_code.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 geocs-1.0.0/tests/test_basic.py
+-rw-r--r--   0        0        0   189172 2020-02-02 00:00:00.000000 geocs-1.0.0/tests/DiffMaps/20160502_0050000.0.npz
+-rw-r--r--   0        0        0   897174 2020-02-02 00:00:00.000000 geocs-1.0.0/tests/bounds/20160502_00/concave0.001
+-rw-r--r--   0        0        0   897174 2020-02-02 00:00:00.000000 geocs-1.0.0/tests/bounds/20160502_00/convex
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 geocs-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 geocs-1.0.0/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 geocs-1.0.0/README.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 geocs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 geocs-1.0.0/PKG-INFO
```

### Comparing `geocs-0.1.0/LICENSE` & `geocs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocs-0.1.0/pyproject.toml` & `geocs-1.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # contents of pyproject.toml
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "GeoCS"
-version = "0.1.0"
+version = "1.0.0"
 description = "Coherent sets for Geophysical trajectories."
 readme = "README.md"
 license.file = "LICENSE"
 authors = [
   { name = "Henry Schoeller", email = "h.schoeller@posteo.de" },
 ]
 maintainers = [
   { name = "Henry Schoeller", email = "h.schoeller@posteo.de" },
 ]
 requires-python = ">=3.8"
 
 dependencies = [
   "numpy",
+  "matplotlib",
+  "seaborn",
+  "scikit-learn",
+  "alphashape",
   "cartopy",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
@@ -35,8 +39,17 @@
   "Topic :: Scientific/Engineering :: Atmospheric Science",
   "Topic :: Scientific/Engineering :: Oceanography",
   "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 [tool.hatch.version]
 scheme = "pep440"
-source = "tag"
+source = "tag"
+
+[project.optional-dependencies]
+docs = [
+  "furo",
+  "myst_parser >=0.13",
+  "sphinx >=4.0",
+  "sphinx-copybutton",
+  "sphinx-autodoc-typehints",
+]
```

### Comparing `geocs-0.1.0/PKG-INFO` & `geocs-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: GeoCS
-Version: 0.1.0
+Version: 1.0.0
 Summary: Coherent sets for Geophysical trajectories.
 Author-email: Henry Schoeller <h.schoeller@posteo.de>
 Maintainer-email: Henry Schoeller <h.schoeller@posteo.de>
 License: MIT License
         
         Copyright (c) [2024] [Henry Schoeller]
         
@@ -35,9 +35,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Oceanography
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
+Requires-Dist: alphashape
 Requires-Dist: cartopy
+Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: scikit-learn
+Requires-Dist: seaborn
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx>=4.0; extra == 'docs'
+Description-Content-Type: text/markdown
+
+# GeoCS
+
+A package to calculate coherent sets from geospatial trajectory data.
```

