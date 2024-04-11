# Comparing `tmp/precice-config-visualizer-0.3.0.tar.gz` & `tmp/precice-config-visualizer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precice-config-visualizer-0.3.0.tar", last modified: Thu Apr 11 13:13:24 2024, max compression
+gzip compressed data, was "precice-config-visualizer-1.0.0.tar", last modified: Thu Apr 11 13:27:21 2024, max compression
```

## Comparing `precice-config-visualizer-0.3.0.tar` & `precice-config-visualizer-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/data/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/preciceconfigvisualizer/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2473 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13491 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:21.987594 precice-config-visualizer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-11 13:27:21.987594 precice-config-visualizer-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:21.983594 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:21.983594 precice-config-visualizer-1.0.0/preciceconfigvisualizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2473 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/preciceconfigvisualizer/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/preciceconfigvisualizer/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:27:21.987594 precice-config-visualizer-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/setup.py
```

### Comparing `precice-config-visualizer-0.3.0/LICENSE` & `precice-config-visualizer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.3.0/PKG-INFO` & `precice-config-visualizer-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 0.3.0
+Version: 1.0.0
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
 Project-URL: Bug Tracker, https://github.com/precice/config-visualizer/issues
-Keywords: preCICE,dot,graphviz,XML,interactive,configuration,visualization
+Keywords: preCICE,dot,graphviz,XML,configuration,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pydot
-Requires-Dist: xdot
-Requires-Dist: PyGObject
 Requires-Dist: typing_extensions
 
 # preCICE Config-Visualizer
 
 The `config-visualizer` is a tool meant to help visualize and debug precice configuration xml files. This tool produces a dot file as output, which visualizes the various participants, communicators and meshes defined in the configuration file and the movement of data between them.
 
 ## Installation options
@@ -35,28 +33,14 @@
 
 ```
 pipx install precice-config-visualizer
 ```
 
 ## Usage
 
-The config visualizer can be use via the CLI or the interactive GUI.
-
-### GUI
-
-```
-precice-config-visualizer-gui [CONFIG-FILE]
-```
-
-You can launch the GUI directly from the command line.
-Passing the path to a configuration file is optional.
-All further adjustments are made directly in the GUI.
-
-### CLI
-
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
 
 The command line version of the tool transforms the XML configuration file into a dot graph and either outputs it to the terminal or writes it to a file.
 If the extension of the output file is `.png`, `.pdf`, `.svg`, or `.jpg`, then the tool will render the output using `graghviz`.
```

### Comparing `precice-config-visualizer-0.3.0/README.md` & `precice-config-visualizer-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,28 +8,14 @@
 
 ```
 pipx install precice-config-visualizer
 ```
 
 ## Usage
 
-The config visualizer can be use via the CLI or the interactive GUI.
-
-### GUI
-
-```
-precice-config-visualizer-gui [CONFIG-FILE]
-```
-
-You can launch the GUI directly from the command line.
-Passing the path to a configuration file is optional.
-All further adjustments are made directly in the GUI.
-
-### CLI
-
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
 
 The command line version of the tool transforms the XML configuration file into a dot graph and either outputs it to the terminal or writes it to a file.
 If the extension of the output file is `.png`, `.pdf`, `.svg`, or `.jpg`, then the tool will render the output using `graghviz`.
```

### Comparing `precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/PKG-INFO` & `precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 0.3.0
+Version: 1.0.0
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
 Project-URL: Bug Tracker, https://github.com/precice/config-visualizer/issues
-Keywords: preCICE,dot,graphviz,XML,interactive,configuration,visualization
+Keywords: preCICE,dot,graphviz,XML,configuration,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pydot
-Requires-Dist: xdot
-Requires-Dist: PyGObject
 Requires-Dist: typing_extensions
 
 # preCICE Config-Visualizer
 
 The `config-visualizer` is a tool meant to help visualize and debug precice configuration xml files. This tool produces a dot file as output, which visualizes the various participants, communicators and meshes defined in the configuration file and the movement of data between them.
 
 ## Installation options
@@ -35,28 +33,14 @@
 
 ```
 pipx install precice-config-visualizer
 ```
 
 ## Usage
 
-The config visualizer can be use via the CLI or the interactive GUI.
-
-### GUI
-
-```
-precice-config-visualizer-gui [CONFIG-FILE]
-```
-
-You can launch the GUI directly from the command line.
-Passing the path to a configuration file is optional.
-All further adjustments are made directly in the GUI.
-
-### CLI
-
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
 
 The command line version of the tool transforms the XML configuration file into a dot graph and either outputs it to the terminal or writes it to a file.
 If the extension of the output file is `.png`, `.pdf`, `.svg`, or `.jpg`, then the tool will render the output using `graghviz`.
```

### Comparing `precice-config-visualizer-0.3.0/preciceconfigvisualizer/cli.py` & `precice-config-visualizer-1.0.0/preciceconfigvisualizer/cli.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.3.0/preciceconfigvisualizer/common.py` & `precice-config-visualizer-1.0.0/preciceconfigvisualizer/common.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.3.0/pyproject.toml` & `precice-config-visualizer-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 requires = ["setuptools>=41", "wheel", "setuptools-git-versioning"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="precice-config-visualizer"
 dynamic = [ "version" ]
 dependencies = [
-    "lxml", "pydot", "xdot", "PyGObject", "typing_extensions"
+    "lxml", "pydot", "typing_extensions"
 ]
 requires-python = ">=3.8"
 authors = [
     { name = "The preCICE Developers",  email="info@precice.org"}
 ]
 maintainers = [
     { name = "Frédéric Simonis",  email="frederic.simonis@ipvs.uni-stuttgart.de"}
 ]
 description="A tool for visualizing a preCICE configuration file as a dot file."
 readme = "README.md"
 license={ text = "GPLv3" }
-keywords = [ "preCICE", "dot", "graphviz", "XML", "interactive", "configuration", "visualization" ]
+keywords = [ "preCICE", "dot", "graphviz", "XML",  "configuration", "visualization" ]
 classifiers=[
 "Development Status :: 4 - Beta",
 "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 "Programming Language :: Python :: 3 :: Only",
 "Programming Language :: Python :: 3.8",
 "Topic :: Scientific/Engineering :: Visualization",
 "Topic :: Utilities",
@@ -33,23 +33,15 @@
 Documentation = "https://precice.org/tooling-config-visualization.html"
 Repository = "https://github.com/precice/config-visualizer.git"
 "Bug Tracker" = "https://github.com/precice/config-visualizer/issues"
 
 [project.scripts]
 precice-config-visualizer = "preciceconfigvisualizer.cli:main"
 
-[project.gui-scripts]
-precice-config-visualizer-gui = "preciceconfigvisualizer.gui:main"
-
 [tool.setuptools]
 packages=["preciceconfigvisualizer"]
 
-[tool.setuptools.data-files]
-"share/applications" = ["data/org.precice.config_visualizer.desktop"]
-"share/metainfo" = ["data/org.precice.config_visualizer.metainfo.xml"]
-"share/icons/hicolor/scalable/apps/" = ["data/org.precice.config_visualizer.svg"]
-
 [tool.setuptools-git-versioning]
 enabled = true
 
 [tool.mypy]
 disable_error_code = "import-untyped"
```

