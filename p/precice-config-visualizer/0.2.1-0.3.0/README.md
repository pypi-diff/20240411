# Comparing `tmp/precice-config-visualizer-0.2.1.tar.gz` & `tmp/precice-config-visualizer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precice-config-visualizer-0.2.1.tar", last modified: Tue Apr  9 10:07:45 2024, max compression
+gzip compressed data, was "precice-config-visualizer-0.3.0.tar", last modified: Thu Apr 11 13:13:24 2024, max compression
```

## Comparing `precice-config-visualizer-0.2.1.tar` & `precice-config-visualizer-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/preciceconfigvisualizer/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15928 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13494 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:13:24.000000 precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/preciceconfigvisualizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2473 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13491 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/preciceconfigvisualizer/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:13:24.327786 precice-config-visualizer-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:13:14.000000 precice-config-visualizer-0.3.0/setup.py
```

### Comparing `precice-config-visualizer-0.2.1/LICENSE` & `precice-config-visualizer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.1/PKG-INFO` & `precice-config-visualizer-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 0.2.1
+Version: 0.3.0
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
@@ -19,14 +19,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pydot
 Requires-Dist: xdot
 Requires-Dist: PyGObject
+Requires-Dist: typing_extensions
 
 # preCICE Config-Visualizer
 
 The `config-visualizer` is a tool meant to help visualize and debug precice configuration xml files. This tool produces a dot file as output, which visualizes the various participants, communicators and meshes defined in the configuration file and the movement of data between them.
 
 ## Installation options
 
@@ -53,30 +54,42 @@
 ### CLI
 
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
 
-The command line version of the tool transforms the XML configuration file into a dot graph file.
-This is especially useful if the output needs to be altered for various reasons.
-To edit the actual graph, displaying it using a dot viewer such as [xdot](https://pypi.org/project/xdot/) can be helpful.
+The command line version of the tool transforms the XML configuration file into a dot graph and either outputs it to the terminal or writes it to a file.
+If the extension of the output file is `.png`, `.pdf`, `.svg`, or `.jpg`, then the tool will render the output using `graghviz`.
+The dot output is especially useful if the output needs to be altered for various reasons.
+To edit the dot version of the graph, displaying it using a dot viewer such as [xdot](https://pypi.org/project/xdot/) can be helpful.
 
 The tool reads from stdin if no configuration file is given as an argument and the output is printed to stdout if no output filename if specified using the `-o` option.
 
 To generate `graph.dot` from `precice-config.xml` use:
 
 ```
+precice-config-visualizer precice-config.xml > graph.dot
 precice-config-visualizer -o graph.dot precice-config.xml
 ```
 
-To `precice-config.xml` as PDF use:
+To generate an image from `precice-config.xml` use:
 
 ```
-precice-config-visualizer precice-config.xml | dot -Tpdf -o graph.pdf
+precice-config-visualizer -o graph.png precice-config.xml
+precice-config-visualizer -o graph.pdf precice-config.xml
+precice-config-visualizer -o graph.svg precice-config.xml
+```
+
+To modify the dot graph from `precice-config.xml` yourself use:
+
+```
+precice-config-visualizer precice-config.xml > graph.dot
+# Edit graph.dot here
+dot -Tpdf -o graph.pdf graph.dot
 ```
 
 Further options can be used to control the output appearance. Some information can be turned off or merged.
 For a full list of options, run:
 
 ```
 precice-config-visualizer --help
```

### Comparing `precice-config-visualizer-0.2.1/README.md` & `precice-config-visualizer-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,30 +27,42 @@
 ### CLI
 
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
 
-The command line version of the tool transforms the XML configuration file into a dot graph file.
-This is especially useful if the output needs to be altered for various reasons.
-To edit the actual graph, displaying it using a dot viewer such as [xdot](https://pypi.org/project/xdot/) can be helpful.
+The command line version of the tool transforms the XML configuration file into a dot graph and either outputs it to the terminal or writes it to a file.
+If the extension of the output file is `.png`, `.pdf`, `.svg`, or `.jpg`, then the tool will render the output using `graghviz`.
+The dot output is especially useful if the output needs to be altered for various reasons.
+To edit the dot version of the graph, displaying it using a dot viewer such as [xdot](https://pypi.org/project/xdot/) can be helpful.
 
 The tool reads from stdin if no configuration file is given as an argument and the output is printed to stdout if no output filename if specified using the `-o` option.
 
 To generate `graph.dot` from `precice-config.xml` use:
 
 ```
+precice-config-visualizer precice-config.xml > graph.dot
 precice-config-visualizer -o graph.dot precice-config.xml
 ```
 
-To `precice-config.xml` as PDF use:
+To generate an image from `precice-config.xml` use:
 
 ```
-precice-config-visualizer precice-config.xml | dot -Tpdf -o graph.pdf
+precice-config-visualizer -o graph.png precice-config.xml
+precice-config-visualizer -o graph.pdf precice-config.xml
+precice-config-visualizer -o graph.svg precice-config.xml
+```
+
+To modify the dot graph from `precice-config.xml` yourself use:
+
+```
+precice-config-visualizer precice-config.xml > graph.dot
+# Edit graph.dot here
+dot -Tpdf -o graph.pdf graph.dot
 ```
 
 Further options can be used to control the output appearance. Some information can be turned off or merged.
 For a full list of options, run:
 
 ```
 precice-config-visualizer --help
```

### Comparing `precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.metainfo.xml` & `precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.metainfo.xml`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.svg` & `precice-config-visualizer-0.3.0/data/org.precice.config_visualizer.svg`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/PKG-INFO` & `precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 0.2.1
+Version: 0.3.0
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
@@ -19,14 +19,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pydot
 Requires-Dist: xdot
 Requires-Dist: PyGObject
+Requires-Dist: typing_extensions
 
 # preCICE Config-Visualizer
 
 The `config-visualizer` is a tool meant to help visualize and debug precice configuration xml files. This tool produces a dot file as output, which visualizes the various participants, communicators and meshes defined in the configuration file and the movement of data between them.
 
 ## Installation options
 
@@ -53,30 +54,42 @@
 ### CLI
 
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
 
-The command line version of the tool transforms the XML configuration file into a dot graph file.
-This is especially useful if the output needs to be altered for various reasons.
-To edit the actual graph, displaying it using a dot viewer such as [xdot](https://pypi.org/project/xdot/) can be helpful.
+The command line version of the tool transforms the XML configuration file into a dot graph and either outputs it to the terminal or writes it to a file.
+If the extension of the output file is `.png`, `.pdf`, `.svg`, or `.jpg`, then the tool will render the output using `graghviz`.
+The dot output is especially useful if the output needs to be altered for various reasons.
+To edit the dot version of the graph, displaying it using a dot viewer such as [xdot](https://pypi.org/project/xdot/) can be helpful.
 
 The tool reads from stdin if no configuration file is given as an argument and the output is printed to stdout if no output filename if specified using the `-o` option.
 
 To generate `graph.dot` from `precice-config.xml` use:
 
 ```
+precice-config-visualizer precice-config.xml > graph.dot
 precice-config-visualizer -o graph.dot precice-config.xml
 ```
 
-To `precice-config.xml` as PDF use:
+To generate an image from `precice-config.xml` use:
 
 ```
-precice-config-visualizer precice-config.xml | dot -Tpdf -o graph.pdf
+precice-config-visualizer -o graph.png precice-config.xml
+precice-config-visualizer -o graph.pdf precice-config.xml
+precice-config-visualizer -o graph.svg precice-config.xml
+```
+
+To modify the dot graph from `precice-config.xml` yourself use:
+
+```
+precice-config-visualizer precice-config.xml > graph.dot
+# Edit graph.dot here
+dot -Tpdf -o graph.pdf graph.dot
 ```
 
 Further options can be used to control the output appearance. Some information can be turned off or merged.
 For a full list of options, run:
 
 ```
 precice-config-visualizer --help
```

### Comparing `precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/SOURCES.txt` & `precice-config-visualizer-0.3.0/precice_config_visualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.1/preciceconfigvisualizer/cli.py` & `precice-config-visualizer-0.3.0/preciceconfigvisualizer/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 #! /usr/bin/env python
 
 import argparse
 import sys
+import pydot
+import os
 
 from preciceconfigvisualizer.common import configFileToDotCode
 
 
+SUPPORTED_FORMATS = [
+    "dot",
+    "jpeg",
+    "jpg",
+    "pdf",
+    "png",
+    "svg",
+]
+
+
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-o",
         "--outfile",
         nargs="?",
-        type=argparse.FileType("w"),
+        type=argparse.FileType("wb"),
         default=sys.stdout,
-        help="The resulting dot file. Omit to output to stdout.",
+        help=f"The output file. Files with extensions {', '.join(SUPPORTED_FORMATS)} will be rendered using graphviz. Omit to output dot to stdout.",
     )
     displayChoices = ["full", "merged", "hide"]
     parser.add_argument(
         "--data-access",
         choices=displayChoices,
         default="full",
         help="Verbosity of the displayed read/write access between mesh and participant.",
@@ -44,27 +56,39 @@
     parser.add_argument(
         "--mappings",
         choices=displayChoices,
         default="full",
         help="Verbosity of the displayed of mappings.",
     )
     parser.add_argument(
-        "--no-watchpoints", action="store_true", help="Do not display watchpoints."
+        "--no-watchpoints",
+        action="store_false",
+        dest="watchpoints",
+        help="Do not display watchpoints.",
     )
     parser.add_argument(
-        "--no-colors", action="store_true", help="Disable colors in the output."
+        "--no-colors",
+        action="store_false",
+        dest="colors",
+        help="Disable colors in the output.",
     )
     parser.add_argument(
         "--margin", default=0, type=int, help="Margin around cluster borders in points."
     )
     parser.add_argument("infile", type=str, help="The XML configuration file.")
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
-    dot = configFileToDotCode(args.infile, args)
-    args.outfile.write(dot)
+    dot = configFileToDotCode(args.infile, **vars(args))
+
+    ext = os.path.splitext(args.outfile.name)[1].lower().lstrip(".")
+    if ext in SUPPORTED_FORMATS:
+        g = pydot.graph_from_dot_data(dot)[0]
+        args.outfile.write(g.create(format=ext))
+    else:
+        args.outfile.write(dot.encode())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `precice-config-visualizer-0.2.1/preciceconfigvisualizer/common.py` & `precice-config-visualizer-0.3.0/preciceconfigvisualizer/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 import sys
-import types
 from collections import defaultdict
 from itertools import cycle
 
 import pydot
 from lxml import etree
 
+
+from typing import Literal, TypedDict
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Unpack
+else:
+    from typing import Unpack
+
+
 if sys.version_info < (3, 6):
     raise RuntimeError(
         "This program requires python 3.6 or later but you attempted to run it"
         " with python {}.{}".format(sys.version_info.major.sys.version_info.minor)
     )
 
+VISIBILITY_TYPE = Literal["full", "merged", "hide"]
+
+
+class VisualizationParameters(TypedDict):
+    data_access: VISIBILITY_TYPE
+    data_exchange: VISIBILITY_TYPE
+    communicators: VISIBILITY_TYPE
+    cplschemes: VISIBILITY_TYPE
+    mappings: VISIBILITY_TYPE
+    watchpoints: bool
+    colors: bool
+    margin: int
+
 
 def isTrue(text: str) -> bool:
     return text.lower() in ["yes", "1", "true", "on"]
 
 
 def quote(text: str) -> str:
     return f'"{text}"'
@@ -61,19 +82,19 @@
 
 
 def getParticipantNames(solverinterface: etree._Element) -> list[str]:
     return [p.attrib["name"] for p in solverinterface.findall("participant")]
 
 
 def getParticipantColor(
-    solverinterface: str, blackOnly: bool = False
+    solverinterface: str, use_colors: bool = False
 ) -> dict[str, str]:
     names = getParticipantNames(solverinterface)
     colors = None
-    if blackOnly:
+    if not use_colors:
         colors = cycle(["black"])
     else:
         colorblind = [
             "#0173B2",
             "#DE8F05",
             "#029E73",
             "#D55E00",
@@ -84,15 +105,34 @@
             "#ECE133",
             "#56B4E9",
         ]
         colors = cycle(colorblind)
     return dict(zip(names, colors))
 
 
-def configToGraph(ast: etree._Element, args) -> pydot.Graph:
+def findAllWithPrefix(e: etree._Element, prefix: str):
+    for child in e.iterchildren():
+        if child.tag.startswith(prefix):
+            yield child
+
+
+def configToGraph(
+    ast: etree._Element, **kwargs: Unpack[VisualizationParameters]
+) -> pydot.Graph:
+    data_access = kwargs.get("data_access", "full")
+    data_exchange = kwargs.get("data_exchange", "full")
+    communicators = kwargs.get("communicators", "full")
+    cplschemes = kwargs.get("cplschemes", "full")
+    mappings = kwargs.get("mappings", "full")
+
+    watchpoints = kwargs.get("watchpoints", True)
+    colors = kwargs.get("colors", True)
+
+    margin = kwargs.get("margin", 0)
+
     assert ast.tag == "precice-configuration"
 
     solverinterfaces = ast.findall("solver-interface")
     precice_version = -1
     si_dims = None  # precice v2
 
     assert len(solverinterfaces) in [0, 1]
@@ -109,330 +149,323 @@
 
     g = pydot.Graph(
         layout="dot",
         splines="true",
         overlap="scale",
         compound=True,
         rankdir="LR",
-        margin=args.margin,
+        margin=margin,
     )
     dataType = {}
     meshes = {}
     meshDims = {}
     participantClusterName = {}
     m2nCluster = pydot.Cluster("m2n", label=quote("Communicators"))
     g.add_subgraph(m2nCluster)
     cplCluster = pydot.Cluster("cpl", label=quote("Coupling Schemes"))
     g.add_subgraph(cplCluster)
 
-    participantColor = getParticipantColor(root, args.no_colors)
+    participantColor = getParticipantColor(root, colors)
 
-    for elem in root.iterchildren():
-        if elem.tag.startswith("data"):
-            kind = elem.tag[elem.tag.find(":") + 1 :]
-            name = elem.attrib["name"]
-            dataType[name] = kind
-        elif "mesh" == elem.tag:
-            name = elem.attrib["name"]
-            meshDims[name] = elem.attrib["dimensions"] if si_dims is None else si_dims
-            meshes[name] = [use.attrib["name"] for use in elem.findall("use-data")]
-        elif "participant" == elem.tag:
-            name = elem.attrib["name"]
-            participant = pydot.Cluster(name, label=quote(name), style="bold")
-            participantClusterName[name] = participant.get_name()
-            color = participantColor[name]
-            addNode(participant, name, color=color, shape="doubleoctagon")
-            # use-mesh
-            for use in elem.findall("use-mesh"):
-                mesh = use.attrib["name"]
-                meshname = f"{name}-{mesh}"
-                provided = "provide" in use.attrib
-                if provided:
-                    label = mesh + (
-                        ""
-                        if mesh not in meshDims
-                        else f"<SUP><I>{meshDims[mesh]}D</I></SUP>"
-                    )
-                    addNode(
-                        participant,
-                        meshname,
-                        shape="cylinder",
-                        label=f"<{label}>",
-                        color=color,
-                    )
-                else:
-                    pfrom = use.attrib["from"]
-                    label = f"<{mesh} from {pfrom}>"
-                    addNode(
-                        participant,
-                        meshname,
-                        shape="cylinder",
-                        label=label,
-                        color=participantColor[pfrom],
-                        style="dashed",
-                    )
-            # provide-mesh
-            for use in elem.findall("provide-mesh"):
-                mesh = use.attrib["name"]
-                meshname = f"{name}-{mesh}"
+    for elem in findAllWithPrefix(root, "data"):
+        kind = elem.tag[elem.tag.find(":") + 1 :]
+        name = elem.attrib["name"]
+        dataType[name] = kind
+
+    for elem in root.findall("mesh"):
+        name = elem.attrib["name"]
+        meshDims[name] = elem.attrib["dimensions"] if si_dims is None else si_dims
+        meshes[name] = [use.attrib["name"] for use in elem.findall("use-data")]
+
+    for elem in root.findall("participant"):
+        name = elem.attrib["name"]
+        participant = pydot.Cluster(name, label=quote(name), style="bold")
+        participantClusterName[name] = participant.get_name()
+        color = participantColor[name]
+        addNode(participant, name, color=color, shape="doubleoctagon")
+        # use-mesh
+        for use in elem.findall("use-mesh"):
+            mesh = use.attrib["name"]
+            meshname = f"{name}-{mesh}"
+            provided = "provide" in use.attrib
+            if provided:
                 label = mesh + (
                     ""
                     if mesh not in meshDims
                     else f"<SUP><I>{meshDims[mesh]}D</I></SUP>"
                 )
-                if isTrue(use.attrib.get("dynamic", "no")):
-                    mesh += "\ndynamic"
                 addNode(
                     participant,
                     meshname,
                     shape="cylinder",
                     label=f"<{label}>",
                     color=color,
                 )
-            # receive-mesh
-            for use in elem.findall("receive-mesh"):
-                mesh = use.attrib["name"]
-                meshname = f"{name}-{mesh}"
+            else:
                 pfrom = use.attrib["from"]
+                label = f"<{mesh} from {pfrom}>"
                 addNode(
                     participant,
                     meshname,
                     shape="cylinder",
-                    label=quote(f"{mesh}\nfrom {pfrom}"),
+                    label=label,
                     color=participantColor[pfrom],
                     style="dashed",
                 )
-            # read-data
-            for read in elem.findall("read-data"):
-                mesh = read.attrib["mesh"]
-                meshNode = f"{name}-{mesh}"
-                data = read.attrib["name"]
-                if args.data_access == "full":
-                    addEdge(
-                        participant,
-                        meshNode,
-                        name,
-                        label=quote(data),
-                        tooltip=dataType[data],
-                        color=color,
-                    )
-                elif args.data_access == "merged":
-                    reversed = getEdge(participant, name, meshNode)
-                    if reversed is None:
-                        addUniqueEdge(participant, meshNode, name)
-                    else:
-                        reversed.set_dir("both")
-            # write-data
-            for write in elem.findall("write-data"):
-                mesh = write.attrib["mesh"]
-                meshNode = f"{name}-{mesh}"
-                data = write.attrib["name"]
-                if args.data_access == "full":
-                    addEdge(
-                        participant,
-                        name,
-                        meshNode,
-                        label=quote(data),
-                        tooltip=dataType[data],
-                        color=color,
-                    )
-                elif args.data_access == "merged":
-                    reversed = getEdge(participant, meshNode, name)
-                    if reversed is None:
-                        addUniqueEdge(participant, name, meshNode, color=color)
+        # provide-mesh
+        for use in elem.findall("provide-mesh"):
+            mesh = use.attrib["name"]
+            meshname = f"{name}-{mesh}"
+            label = mesh + (
+                "" if mesh not in meshDims else f"<SUP><I>{meshDims[mesh]}D</I></SUP>"
+            )
+            if isTrue(use.attrib.get("dynamic", "no")):
+                mesh += "\ndynamic"
+            addNode(
+                participant,
+                meshname,
+                shape="cylinder",
+                label=f"<{label}>",
+                color=color,
+            )
+        # receive-mesh
+        for use in elem.findall("receive-mesh"):
+            mesh = use.attrib["name"]
+            meshname = f"{name}-{mesh}"
+            pfrom = use.attrib["from"]
+            addNode(
+                participant,
+                meshname,
+                shape="cylinder",
+                label=quote(f"{mesh}\nfrom {pfrom}"),
+                color=participantColor[pfrom],
+                style="dashed",
+            )
+        # read-data
+        for read in elem.findall("read-data"):
+            mesh = read.attrib["mesh"]
+            meshNode = f"{name}-{mesh}"
+            data = read.attrib["name"]
+            if data_access == "full":
+                addEdge(
+                    participant,
+                    meshNode,
+                    name,
+                    label=quote(data),
+                    tooltip=dataType[data],
+                    color=color,
+                )
+            elif data_access == "merged":
+                reversed = getEdge(participant, name, meshNode)
+                if reversed is None:
+                    addUniqueEdge(participant, meshNode, name)
+                else:
+                    reversed.set_dir("both")
+        # write-data
+        for write in elem.findall("write-data"):
+            mesh = write.attrib["mesh"]
+            meshNode = f"{name}-{mesh}"
+            data = write.attrib["name"]
+            if data_access == "full":
+                addEdge(
+                    participant,
+                    name,
+                    meshNode,
+                    label=quote(data),
+                    tooltip=dataType[data],
+                    color=color,
+                )
+            elif data_access == "merged":
+                reversed = getEdge(participant, meshNode, name)
+                if reversed is None:
+                    addUniqueEdge(participant, name, meshNode, color=color)
+                else:
+                    reversed.set_dir("both")
+
+        # watchpoint
+        for watchpoint in elem.findall("watch-point"):
+            wpmesh = watchpoint.attrib["mesh"]
+            wpname = watchpoint.attrib["name"]
+            wpcoord = watchpoint.attrib["coordinate"]
+            if watchpoints:
+                wpnode = f"{name}-WP-{wpname}"
+                addNode(
+                    participant,
+                    wpnode,
+                    shape="note",
+                    label=quote(f"{wpname}\nat ({wpcoord})"),
+                    color=color,
+                )
+                addEdge(participant, wpnode, name, color=color)
+
+        # other children
+        for child in elem.iterchildren():
+            # register mappings
+            if child.tag.startswith("mapping:"):
+                mkind = child.tag[child.tag.find(":") + 1 :]
+                mfrom = name + "-" + child.attrib["from"]
+                mto = name + "-" + child.attrib["to"]
+                if mappings == "full":
+                    addEdge(participant, mfrom, mto, label=quote(mkind), color=color)
+                elif mappings == "merged":
+                    e = getEdge(participant, mto, mfrom)
+                    if e is None:
+                        addEdge(participant, mfrom, mto, color=color)
                     else:
-                        reversed.set_dir("both")
+                        e.set_dir("both")
 
-            # watchpoint
-            for watchpoint in elem.findall("watch-point"):
-                wpmesh = watchpoint.attrib["mesh"]
-                wpname = watchpoint.attrib["name"]
-                wpcoord = watchpoint.attrib["coordinate"]
-                if not args.no_watchpoints:
-                    wpnode = f"{name}-WP-{wpname}"
-                    addNode(
-                        participant,
-                        wpnode,
-                        shape="note",
-                        label=quote(f"{wpname}\nat ({wpcoord})"),
-                        color=color,
-                    )
-                    addEdge(participant, wpnode, name, color=color)
+            # master
+            if child.tag.startswith("master:"):
+                kind = child.tag[child.tag.find(":") + 1 :]
+                addNode(participant, name + kind, shape="component", label=quote(kind))
+
+        g.add_subgraph(participant)
+
+    for elem in findAllWithPrefix(root, "m2n"):
+        kind = elem.tag[elem.tag.find(":") + 1 :]
+        pfrom = elem.attrib["from" if "from" in elem.attrib else "connector"]
+        pto = elem.attrib["to" if "to" in elem.attrib else "acceptor"]
+        name = f"m2n-{pto}-{pfrom}"
+        if communicators == "full":
+            addNode(m2nCluster, name, shape="component", label=quote(kind))
+            addEdge(
+                g,
+                name,
+                pto,
+                lhead=participantClusterName[pto],
+                dir="both",
+                color=participantColor[pto],
+            )
+            addEdge(
+                g,
+                name,
+                pfrom,
+                lhead=participantClusterName[pfrom],
+                dir="both",
+                color=participantColor[pfrom],
+            )
+        if communicators == "merged":
+            addEdge(
+                g,
+                pfrom,
+                pto,
+                lhead=participantClusterName[pto],
+                ltail=participantClusterName[pfrom],
+                label=quote(kind),
+                dir="both",
+            )
 
-            # other children
-            for child in elem.iterchildren():
-                # register mappings
-                if child.tag.startswith("mapping:"):
-                    mkind = child.tag[child.tag.find(":") + 1 :]
-                    mfrom = name + "-" + child.attrib["from"]
-                    mto = name + "-" + child.attrib["to"]
-                    if args.mappings == "full":
-                        addEdge(
-                            participant, mfrom, mto, label=quote(mkind), color=color
-                        )
-                    elif args.mappings == "merged":
-                        e = getEdge(participant, mto, mfrom)
-                        if e is None:
-                            addEdge(participant, mfrom, mto, color=color)
-                        else:
-                            e.set_dir("both")
-
-                # master
-                if child.tag.startswith("master:"):
-                    kind = child.tag[child.tag.find(":") + 1 :]
-                    addNode(
-                        participant, name + kind, shape="component", label=quote(kind)
-                    )
+    for elem in findAllWithPrefix(root, "coupling-scheme"):
+        kind = elem.tag[elem.tag.find(":") + 1 :]
+        # Every cplscheme apart from multi
+        name = "-".join(
+            ["cpl", "multi"] + [e.attrib["name"] for e in elem.findall("participant")]
+        )
+
+        if kind == "multi":
+            if cplschemes == "full":
+                addNode(cplCluster, name, shape="component", label=quote(kind))
+                for other in elem.findall("participant"):
+                    thisName = other.attrib["name"]
+                    e = addEdge(
+                        g,
+                        name,
+                        thisName,
+                        lhead=participantClusterName[thisName],
+                        color=participantColor[thisName],
+                    )
+                    if other.get("control"):
+                        e.set_taillabel("Controller")
+            elif cplschemes == "merged":
+                addNode(g, name, shape="circle", tooltip=quote(kind), label=quote(""))
+                for other in elem.findall("participant"):
+                    thisName = other.attrib["name"]
+                    e = addEdge(g, name, thisName)
+                    if other.get("control"):
+                        e.set_style("bold")
+                        e.set_tooltip("Controller")
+
+        else:
+            # Every cplscheme apart from multi
+            first = elem.find("participants").attrib["first"]
+            second = elem.find("participants").attrib["second"]
+            name = f"cpl-{first}-{second}"
 
-            g.add_subgraph(participant)
-        # m2n
-        elif elem.tag.startswith("m2n"):
-            kind = elem.tag[elem.tag.find(":") + 1 :]
-            pfrom = elem.attrib["from" if "from" in elem.attrib else "connector"]
-            pto = elem.attrib["to" if "to" in elem.attrib else "acceptor"]
-            name = f"m2n-{pto}-{pfrom}"
-            if args.communicators == "full":
-                addNode(m2nCluster, name, shape="component", label=quote(kind))
+            if cplschemes == "full":
+                addNode(cplCluster, name, shape="component", label=quote(kind))
                 addEdge(
                     g,
                     name,
-                    pto,
-                    lhead=participantClusterName[pto],
-                    dir="both",
-                    color=participantColor[pto],
+                    first,
+                    lhead=participantClusterName[first],
+                    taillabel=quote("first"),
+                    color=participantColor[first],
                 )
                 addEdge(
                     g,
                     name,
-                    pfrom,
-                    lhead=participantClusterName[pfrom],
-                    dir="both",
-                    color=participantColor[pfrom],
+                    second,
+                    lhead=participantClusterName[second],
+                    taillabel=quote("second"),
+                    color=participantColor[second],
                 )
-            if args.communicators == "merged":
-                addEdge(
+            elif cplschemes == "merged":
+                addUniqueEdge(
                     g,
-                    pfrom,
-                    pto,
-                    lhead=participantClusterName[pto],
-                    ltail=participantClusterName[pfrom],
-                    label=quote(kind),
+                    first,
+                    second,
                     dir="both",
+                    taillabel=quote("first"),
+                    headlabel=quote("second"),
+                    label=quote(kind),
                 )
 
-        # cpl schemes
-        elif elem.tag.startswith("coupling-scheme"):
-            kind = elem.tag[elem.tag.find(":") + 1 :]
-            # Every cplscheme apart from multi
-            name = "-".join(
-                ["cpl", "multi"]
-                + [e.attrib["name"] for e in elem.findall("participant")]
-            )
-
-            if kind == "multi":
-                if args.cplschemes == "full":
-                    addNode(cplCluster, name, shape="component", label=quote(kind))
-                    for other in elem.findall("participant"):
-                        thisName = other.attrib["name"]
-                        e = addEdge(
-                            g,
-                            name,
-                            thisName,
-                            lhead=participantClusterName[thisName],
-                            color=participantColor[thisName],
-                        )
-                        if other.get("control"):
-                            e.set_taillabel("Controller")
-                elif args.cplschemes == "merged":
-                    addNode(
-                        g, name, shape="circle", tooltip=quote(kind), label=quote("")
-                    )
-                    for other in elem.findall("participant"):
-                        thisName = other.attrib["name"]
-                        e = addEdge(g, name, thisName)
-                        if other.get("control"):
-                            e.set_style("bold")
-                            e.set_tooltip("Controller")
-
-            else:
-                # Every cplscheme apart from multi
-                first = elem.find("participants").attrib["first"]
-                second = elem.find("participants").attrib["second"]
-                name = f"cpl-{first}-{second}"
-
-                if args.cplschemes == "full":
-                    addNode(cplCluster, name, shape="component", label=quote(kind))
-                    addEdge(
-                        g,
-                        name,
-                        first,
-                        lhead=participantClusterName[first],
-                        taillabel=quote("first"),
-                        color=participantColor[first],
-                    )
-                    addEdge(
-                        g,
-                        name,
-                        second,
-                        lhead=participantClusterName[second],
-                        taillabel=quote("second"),
-                        color=participantColor[second],
-                    )
-                elif args.cplschemes == "merged":
-                    addUniqueEdge(
-                        g,
-                        first,
-                        second,
-                        dir="both",
-                        taillabel=quote("first"),
-                        headlabel=quote("second"),
-                        label=quote(kind),
-                    )
-
-            # exchange tags
-            # This is indepedant of the above
-            for exchange in elem.findall("exchange"):
-                mesh = exchange.attrib["mesh"]
-                data = exchange.attrib["data"]
-                pfrom = exchange.attrib["from"]
-                pto = exchange.attrib["to"]
-                init = isTrue(exchange.get("initialize", "no"))
-                withSubsteps = isTrue(exchange.get("substeps", "no"))
-                if args.data_exchange == "full":
-                    pcolor = participantColor[pfrom]
-                    style = "bold" if init else ""
-                    tooltip = dataType[data] + (" initialized" if init else "")
-                    color = f"{pcolor}:invis:{pcolor}" if withSubsteps else pcolor
-                    addEdge(
-                        g,
-                        f"{pfrom}-{mesh}",
-                        f"{pto}-{mesh}",
-                        label=quote(data),
-                        tooltip=tooltip,
-                        color=color,
-                        style=style,
-                    )
-                elif args.data_exchange == "merged":
-                    addUniqueEdge(
-                        g,
-                        f"{pfrom}-{mesh}",
-                        f"{pto}-{mesh}",
-                        color=participantColor[pfrom],
-                    )
+        # exchange tags
+        # This is indepedant of the above
+        for exchange in elem.findall("exchange"):
+            mesh = exchange.attrib["mesh"]
+            data = exchange.attrib["data"]
+            pfrom = exchange.attrib["from"]
+            pto = exchange.attrib["to"]
+            init = isTrue(exchange.get("initialize", "no"))
+            withSubsteps = isTrue(exchange.get("substeps", "no"))
+            if data_exchange == "full":
+                pcolor = participantColor[pfrom]
+                style = "bold" if init else ""
+                tooltip = dataType[data] + (" initialized" if init else "")
+                color = f"{pcolor}:invis:{pcolor}" if withSubsteps else pcolor
+                addEdge(
+                    g,
+                    f"{pfrom}-{mesh}",
+                    f"{pto}-{mesh}",
+                    label=quote(data),
+                    tooltip=tooltip,
+                    color=color,
+                    style=style,
+                )
+            elif data_exchange == "merged":
+                addUniqueEdge(
+                    g,
+                    f"{pfrom}-{mesh}",
+                    f"{pto}-{mesh}",
+                    color=participantColor[pfrom],
+                )
 
     return g
 
 
 def readBinary(streamlike):
     """
     Reading binary from sys.stdin requires to use the underlying buffer instead
     """
     try:
         return streamlike.buffer.read()
     except:
         return streamlike.read()
 
 
-def configFileToDotCode(filename: str, args) -> str:
+def configFileToDotCode(
+    filename: str, **kwargs: Unpack[VisualizationParameters]
+) -> str:
     xml = parseXML(readBinary(open(filename, "rb")))
-    g = configToGraph(xml, args)
+    g = configToGraph(xml, **kwargs)
     return g.to_string()
```

### Comparing `precice-config-visualizer-0.2.1/preciceconfigvisualizer/gui.py` & `precice-config-visualizer-0.3.0/preciceconfigvisualizer/gui.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.1/preciceconfigvisualizer/window.py` & `precice-config-visualizer-0.3.0/preciceconfigvisualizer/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,26 +237,26 @@
         def getVisibilty(cb):
             return {
                 "Show": "full",
                 "Merge": "merged",
                 "Hide": "hide",
             }[get_active_value(cb)]
 
-        args = types.SimpleNamespace(
-            data_access=getVisibilty(self.data_access),
-            data_exchange=getVisibilty(self.data_exchange),
-            communicators=getVisibilty(self.communicators),
-            cplschemes=getVisibilty(self.cplschemes),
-            mappings=getVisibilty(self.mappings),
-            no_watchpoints=False,
-            no_colors=False,
-            margin=self.margin.get_value(),
-        )
+        args = {
+            "data_access": getVisibilty(self.data_access),
+            "data_exchange": getVisibilty(self.data_exchange),
+            "communicators": getVisibilty(self.communicators),
+            "cplschemes": getVisibilty(self.cplschemes),
+            "mappings": getVisibilty(self.mappings),
+            "watchpoints": True,
+            "colors": True,
+            "margin": self.margin.get_value(),
+        }
 
-        dot = configFileToDotCode(self._filename, args)
+        dot = configFileToDotCode(self._filename, **args)
         self.error_bar.set_visible(False)
         self.dotcode = dot.encode()
         self.dotwidget.set_dotcode(dot.encode())
 
     def on_open(self, caller):
         dialog = Gtk.FileChooserDialog(
             title="Choose preCICE configuration",
```

### Comparing `precice-config-visualizer-0.2.1/pyproject.toml` & `precice-config-visualizer-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=41", "wheel", "setuptools-git-versioning"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="precice-config-visualizer"
 dynamic = [ "version" ]
 dependencies = [
-    "lxml", "pydot", "xdot", "PyGObject"
+    "lxml", "pydot", "xdot", "PyGObject", "typing_extensions"
 ]
 requires-python = ">=3.8"
 authors = [
     { name = "The preCICE Developers",  email="info@precice.org"}
 ]
 maintainers = [
     { name = "Frédéric Simonis",  email="frederic.simonis@ipvs.uni-stuttgart.de"}
```

