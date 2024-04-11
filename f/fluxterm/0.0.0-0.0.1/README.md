# Comparing `tmp/fluxterm-0.0.0.tar.gz` & `tmp/fluxterm-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxterm-0.0.0.tar", last modified: Thu Apr 11 02:00:03 2024, max compression
+gzip compressed data, was "fluxterm-0.0.1.tar", last modified: Thu Apr 11 02:29:38 2024, max compression
```

## Comparing `fluxterm-0.0.0.tar` & `fluxterm-0.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:00:03.909469 fluxterm-0.0.0/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2024-04-10 03:57:04.000000 fluxterm-0.0.0/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      241 2024-04-11 01:59:14.000000 fluxterm-0.0.0/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2024-04-10 03:57:12.000000 fluxterm-0.0.0/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3657 2024-04-11 02:00:03.909469 fluxterm-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2783 2024-04-11 01:59:14.000000 fluxterm-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:00:03.909469 fluxterm-0.0.0/fluxterm/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       33 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1428 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/app.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:00:03.909469 fluxterm-0.0.0/fluxterm/assets/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/assets/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8823 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/assets/flux-commands.yaml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9184 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/assets/fluxbird-small.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      694 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/assets/fluxterm.tcss
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1614 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/cli.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      683 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/command.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      333 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/defaults.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:00:03.909469 fluxterm-0.0.0/fluxterm/screen/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      134 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/screen/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1796 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/screen/browser.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      991 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/screen/documentation.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2292 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/screen/fortune.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1993 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/screen/jobs.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      165 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/utils.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      865 2024-04-11 01:59:14.000000 fluxterm-0.0.0/fluxterm/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:00:03.909469 fluxterm-0.0.0/fluxterm.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3657 2024-04-11 02:00:03.000000 fluxterm-0.0.0/fluxterm.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      694 2024-04-11 02:00:03.000000 fluxterm-0.0.0/fluxterm.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-04-11 02:00:03.000000 fluxterm-0.0.0/fluxterm.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       55 2024-04-11 02:00:03.000000 fluxterm-0.0.0/fluxterm.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-04-11 01:30:15.000000 fluxterm-0.0.0/fluxterm.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       81 2024-04-11 02:00:03.000000 fluxterm-0.0.0/fluxterm.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        9 2024-04-11 02:00:03.000000 fluxterm-0.0.0/fluxterm.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2024-04-11 01:59:14.000000 fluxterm-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      222 2024-04-11 02:00:03.909469 fluxterm-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3418 2024-04-11 01:59:14.000000 fluxterm-0.0.0/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:29:38.870544 fluxterm-0.0.1/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2024-04-10 03:57:04.000000 fluxterm-0.0.1/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      241 2024-04-11 01:59:14.000000 fluxterm-0.0.1/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2024-04-10 03:57:12.000000 fluxterm-0.0.1/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3713 2024-04-11 02:29:38.870544 fluxterm-0.0.1/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2839 2024-04-11 02:24:11.000000 fluxterm-0.0.1/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:29:38.870544 fluxterm-0.0.1/fluxterm/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       33 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1428 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/app.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:29:38.870544 fluxterm-0.0.1/fluxterm/assets/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/assets/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8823 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/assets/flux-commands.yaml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9184 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/assets/fluxbird-small.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      694 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/assets/fluxterm.tcss
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1614 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/cli.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      683 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/command.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      842 2024-04-11 02:24:11.000000 fluxterm-0.0.1/fluxterm/defaults.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:29:38.870544 fluxterm-0.0.1/fluxterm/screen/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      134 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/screen/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1796 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/screen/browser.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      991 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/screen/documentation.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2292 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/screen/fortune.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1985 2024-04-11 02:24:11.000000 fluxterm-0.0.1/fluxterm/screen/jobs.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      165 2024-04-11 01:59:14.000000 fluxterm-0.0.1/fluxterm/utils.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      865 2024-04-11 02:24:11.000000 fluxterm-0.0.1/fluxterm/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-04-11 02:29:38.870544 fluxterm-0.0.1/fluxterm.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3713 2024-04-11 02:29:38.000000 fluxterm-0.0.1/fluxterm.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      694 2024-04-11 02:29:38.000000 fluxterm-0.0.1/fluxterm.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-04-11 02:29:38.000000 fluxterm-0.0.1/fluxterm.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       55 2024-04-11 02:29:38.000000 fluxterm-0.0.1/fluxterm.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-04-11 01:30:15.000000 fluxterm-0.0.1/fluxterm.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       81 2024-04-11 02:29:38.000000 fluxterm-0.0.1/fluxterm.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        9 2024-04-11 02:29:38.000000 fluxterm-0.0.1/fluxterm.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2024-04-11 01:59:14.000000 fluxterm-0.0.1/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      222 2024-04-11 02:29:38.870544 fluxterm-0.0.1/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3418 2024-04-11 01:59:14.000000 fluxterm-0.0.1/setup.py
```

### Comparing `fluxterm-0.0.0/LICENSE` & `fluxterm-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/NOTICE` & `fluxterm-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/PKG-INFO` & `fluxterm-0.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxterm
-Version: 0.0.0
+Version: 0.0.1
 Summary: Terminal application to interact with Flux jobs, cheat sheets, code, and good fortune
 Home-page: https://github.com/converged-computing/flux-term
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Flux framework,HPC,workload manager,jobs queue,textual
@@ -19,14 +19,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 License-File: NOTICE
 
 # Fluxterm
 
+[![PyPI version](https://badge.fury.io/py/fluxterm.svg)](https://badge.fury.io/py/fluxterm)
+
 > 🦩️ I find this highly ridulous. And highly excellent.
 
 Flux... from a terminal! This is a small terminal application that will provide a handle to interact with Flux, but also other useful UI interactions that are nice to have. We currently have:
 
 - A simple code browser
 - A flux jobs interface to see (and possibly TBA interact) with jobs
 - A flux cheat sheet for quick reference
@@ -62,15 +64,14 @@
 
 
 If you'd like a feature added, please [let us know](https://github.com/converged-computing/fluxterm)!
 It is currently bare bones, and development of this project will happen per user request.
 
 ## TODO
 
-- Add emoji status to the jobs table
 - Job table interactivity
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `fluxterm-0.0.0/README.md` & `fluxterm-0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Fluxterm
 
+[![PyPI version](https://badge.fury.io/py/fluxterm.svg)](https://badge.fury.io/py/fluxterm)
+
 > 🦩️ I find this highly ridulous. And highly excellent.
 
 Flux... from a terminal! This is a small terminal application that will provide a handle to interact with Flux, but also other useful UI interactions that are nice to have. We currently have:
 
 - A simple code browser
 - A flux jobs interface to see (and possibly TBA interact) with jobs
 - A flux cheat sheet for quick reference
@@ -39,15 +41,14 @@
 
 
 If you'd like a feature added, please [let us know](https://github.com/converged-computing/fluxterm)!
 It is currently bare bones, and development of this project will happen per user request.
 
 ## TODO
 
-- Add emoji status to the jobs table
 - Job table interactivity
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `fluxterm-0.0.0/fluxterm/app.py` & `fluxterm-0.0.1/fluxterm/app.py`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/assets/flux-commands.yaml` & `fluxterm-0.0.1/fluxterm/assets/flux-commands.yaml`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/assets/fluxbird-small.png` & `fluxterm-0.0.1/fluxterm/assets/fluxbird-small.png`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/assets/fluxterm.tcss` & `fluxterm-0.0.1/fluxterm/assets/fluxterm.tcss`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/cli.py` & `fluxterm-0.0.1/fluxterm/cli.py`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/command.py` & `fluxterm-0.0.1/fluxterm/command.py`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/screen/browser.py` & `fluxterm-0.0.1/fluxterm/screen/browser.py`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/screen/documentation.py` & `fluxterm-0.0.1/fluxterm/screen/documentation.py`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/screen/fortune.py` & `fluxterm-0.0.1/fluxterm/screen/fortune.py`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/fluxterm/screen/jobs.py` & `fluxterm-0.0.1/fluxterm/screen/jobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from textual.app import ComposeResult
 from textual.screen import Screen
 from textual.widgets import DataTable, Footer, Header, Static
+import fluxterm.defaults as defaults
 
 try:
     import flux
     import flux.job
 
     handle = flux.Flux()
 except ImportError:
@@ -53,18 +54,15 @@
                 "nnodes",
                 "ranks",
                 "expiration",
             )
         ]
         for job in listing.get_jobinfos():
             j = job.to_dict()
-            try:
-                state = job.status_emoji
-            except Exception:
-                state = j["state"]
+            state = defaults.JOB_STATES.get(j["state"].lower()) or j["state"]
             ROWS.append(
                 (
                     j["id"],
                     j["userid"],
                     j["urgency"],
                     j["priority"],
                     state,
```

### Comparing `fluxterm-0.0.0/fluxterm/version.py` & `fluxterm-0.0.1/fluxterm/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright 2024, Vanessa Sochat, HPCIC Developer Tools"
 __license__ = "MIT"
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsoch@users.noreply.github.com"
 NAME = "fluxterm"
 PACKAGE_URL = "https://github.com/converged-computing/flux-term"
 KEYWORDS = "Flux framework, HPC, workload manager, jobs queue, textual"
 DESCRIPTION = "Terminal application to interact with Flux jobs, cheat sheets, code, and good fortune"
 LICENSE = "LICENSE"
```

### Comparing `fluxterm-0.0.0/fluxterm.egg-info/PKG-INFO` & `fluxterm-0.0.1/fluxterm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxterm
-Version: 0.0.0
+Version: 0.0.1
 Summary: Terminal application to interact with Flux jobs, cheat sheets, code, and good fortune
 Home-page: https://github.com/converged-computing/flux-term
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Flux framework,HPC,workload manager,jobs queue,textual
@@ -19,14 +19,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 License-File: NOTICE
 
 # Fluxterm
 
+[![PyPI version](https://badge.fury.io/py/fluxterm.svg)](https://badge.fury.io/py/fluxterm)
+
 > 🦩️ I find this highly ridulous. And highly excellent.
 
 Flux... from a terminal! This is a small terminal application that will provide a handle to interact with Flux, but also other useful UI interactions that are nice to have. We currently have:
 
 - A simple code browser
 - A flux jobs interface to see (and possibly TBA interact) with jobs
 - A flux cheat sheet for quick reference
@@ -62,15 +64,14 @@
 
 
 If you'd like a feature added, please [let us know](https://github.com/converged-computing/fluxterm)!
 It is currently bare bones, and development of this project will happen per user request.
 
 ## TODO
 
-- Add emoji status to the jobs table
 - Job table interactivity
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `fluxterm-0.0.0/fluxterm.egg-info/SOURCES.txt` & `fluxterm-0.0.1/fluxterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluxterm-0.0.0/setup.py` & `fluxterm-0.0.1/setup.py`

 * *Files identical despite different names*

