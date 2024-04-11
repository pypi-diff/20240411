# Comparing `tmp/stpyvista-0.0.8.tar.gz` & `tmp/stpyvista-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpyvista-0.0.8.tar", last modified: Tue Apr 11 16:18:51 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `stpyvista-0.0.8.tar` & `stpyvista-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.246677 stpyvista-0.0.8/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)    35129 2022-10-10 23:59:26.000000 stpyvista-0.0.8/LICENSE
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       78 2022-10-10 23:59:26.000000 stpyvista-0.0.8/MANIFEST.in
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     2548 2023-04-11 16:18:51.246677 stpyvista-0.0.8/PKG-INFO
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     1955 2023-04-11 16:18:15.000000 stpyvista-0.0.8/README.md
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      741 2023-04-11 16:18:34.000000 stpyvista-0.0.8/pyproject.toml
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2023-04-11 16:18:51.246677 stpyvista-0.0.8/setup.cfg
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      735 2023-04-11 16:17:19.000000 stpyvista-0.0.8/setup.py
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.242676 stpyvista-0.0.8/src/
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.242676 stpyvista-0.0.8/src/stpyvista/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     3760 2023-03-30 13:25:16.000000 stpyvista-0.0.8/src/stpyvista/__init__.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       74 2022-10-11 00:08:17.000000 stpyvista-0.0.8/src/stpyvista/__main__.py
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.246677 stpyvista-0.0.8/src/stpyvista/frontend/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      631 2022-11-06 19:43:06.000000 stpyvista-0.0.8/src/stpyvista/frontend/index.html
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     2021 2023-03-30 13:18:38.000000 stpyvista-0.0.8/src/stpyvista/frontend/main.js
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     1198 2023-03-10 15:57:04.000000 stpyvista-0.0.8/src/stpyvista/frontend/streamlit-component-lib.js
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      166 2023-03-09 01:49:59.000000 stpyvista-0.0.8/src/stpyvista/frontend/style.css
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.242676 stpyvista-0.0.8/src/stpyvista.egg-info/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     2548 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/PKG-INFO
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      437 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/SOURCES.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)        1 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/dependency_links.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/requires.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       10 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 stpyvista-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 stpyvista-0.0.9/MANIFEST.in
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 stpyvista-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 stpyvista-0.0.9/src/stpyvista/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 stpyvista-0.0.9/src/stpyvista/__main__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 stpyvista-0.0.9/src/stpyvista/frontend/index.html
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 stpyvista-0.0.9/src/stpyvista/frontend/main.js
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 stpyvista-0.0.9/src/stpyvista/frontend/streamlit-component-lib.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 stpyvista-0.0.9/src/stpyvista/frontend/style.css
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 stpyvista-0.0.9/test/cube.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 stpyvista-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35129 2020-02-02 00:00:00.000000 stpyvista-0.0.9/LICENSE
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 stpyvista-0.0.9/README.md
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 stpyvista-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 stpyvista-0.0.9/PKG-INFO
```

### Comparing `stpyvista-0.0.8/LICENSE` & `stpyvista-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stpyvista-0.0.8/pyproject.toml` & `stpyvista-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "stpyvista"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Edwin S", email="esaavedrac@u.northwestern.edu" },
 ]
-description = "Streamlit component that allows you to show PyVista 3d visualizations"
+description = "Streamlit component to render pyvista 3D visualizations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -22,9 +22,10 @@
     "pyvista",
     "bokeh",
     "panel",
     "ipython"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/edsaac/streamlit-PyVista-viewer"
-"Bug Tracker" = "https://github.com/edsaac/streamlit-PyVista-viewer/issues"
+"Homepage" = "https://github.com/edsaac/stpyvista"
+"Bug Tracker" = "https://github.com/edsaac/stpyvista/issues"
+"Examples" = "https://stpyvista.streamlit.app/"
```

### Comparing `stpyvista-0.0.8/src/stpyvista/frontend/index.html` & `stpyvista-0.0.9/src/stpyvista/frontend/index.html`

 * *Files identical despite different names*

### Comparing `stpyvista-0.0.8/src/stpyvista/frontend/main.js` & `stpyvista-0.0.9/src/stpyvista/frontend/main.js`

 * *Files identical despite different names*

### Comparing `stpyvista-0.0.8/src/stpyvista/frontend/streamlit-component-lib.js` & `stpyvista-0.0.9/src/stpyvista/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

