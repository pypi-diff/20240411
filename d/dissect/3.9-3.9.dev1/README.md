# Comparing `tmp/dissect-3.9.tar.gz` & `tmp/dissect-3.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect-3.9.tar", last modified: Tue Sep 26 14:56:51 2023, max compression
+gzip compressed data, was "dissect-3.9.dev1.tar", last modified: Mon Aug 14 14:39:08 2023, max compression
```

## Comparing `dissect-3.9.tar` & `dissect-3.9.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 14:56:51.648516 dissect-3.9/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-09-26 14:56:38.000000 dissect-3.9/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-09-26 14:56:38.000000 dissect-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-26 14:56:38.000000 dissect-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2023-09-26 14:56:51.644516 dissect-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2023-09-26 14:56:38.000000 dissect-3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 14:56:51.644516 dissect-3.9/dissect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2023-09-26 14:56:51.000000 dissect-3.9/dissect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-09-26 14:56:51.000000 dissect-3.9/dissect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 14:56:51.000000 dissect-3.9/dissect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-09-26 14:56:51.000000 dissect-3.9/dissect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 14:56:51.000000 dissect-3.9/dissect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-09-26 14:56:38.000000 dissect-3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 14:56:51.648516 dissect-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-09-26 14:56:38.000000 dissect-3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:39:08.804600 dissect-3.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-14 14:38:51.000000 dissect-3.9.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-14 14:38:51.000000 dissect-3.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-14 14:38:51.000000 dissect-3.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-08-14 14:39:08.804600 dissect-3.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-14 14:38:51.000000 dissect-3.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 14:39:08.804600 dissect-3.9.dev1/dissect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-08-14 14:39:08.000000 dissect-3.9.dev1/dissect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-14 14:39:08.000000 dissect-3.9.dev1/dissect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 14:39:08.000000 dissect-3.9.dev1/dissect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-14 14:39:08.000000 dissect-3.9.dev1/dissect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 14:39:08.000000 dissect-3.9.dev1/dissect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-14 14:38:57.000000 dissect-3.9.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 14:39:08.804600 dissect-3.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-14 14:38:51.000000 dissect-3.9.dev1/tox.ini
```

### Comparing `dissect-3.9/LICENSE` & `dissect-3.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect-3.9/PKG-INFO` & `dissect-3.9.dev1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.9
+Version: 3.9.dev1
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,38 +18,14 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
-Requires-Dist: dissect.cim==3.7
-Requires-Dist: dissect.clfs==1.6
-Requires-Dist: dissect.cstruct==3.10
-Requires-Dist: dissect.esedb==3.9
-Requires-Dist: dissect.etl==3.7
-Requires-Dist: dissect.eventlog==3.6
-Requires-Dist: dissect.evidence==3.7
-Requires-Dist: dissect.executable==1.4
-Requires-Dist: dissect.extfs==3.6
-Requires-Dist: dissect.fat==3.6
-Requires-Dist: dissect.ffs==3.6
-Requires-Dist: dissect.hypervisor==3.9
-Requires-Dist: dissect.ntfs==3.7
-Requires-Dist: dissect.ole==3.6
-Requires-Dist: dissect.regf==3.7
-Requires-Dist: dissect.shellitem==3.6
-Requires-Dist: dissect.sql==3.6
-Requires-Dist: dissect.squashfs==1.3
-Requires-Dist: dissect.target[full]==3.12
-Requires-Dist: dissect.thumbcache==1.6
-Requires-Dist: dissect.util==3.11
-Requires-Dist: dissect.vmfs==3.6
-Requires-Dist: dissect.volume==3.7
-Requires-Dist: dissect.xfs==3.6
 
 # dissect
 
 Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group).
 
 This project is a meta package, it will install all other Dissect modules with the right combination of versions. For
 more information, please see [the documentation](https://docs.dissect.tools/).
```

### Comparing `dissect-3.9/README.md` & `dissect-3.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect-3.9/dissect.egg-info/PKG-INFO` & `dissect-3.9.dev1/dissect.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect
-Version: 3.9
+Version: 3.9.dev1
 Summary: Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group)
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,38 +18,14 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
-Requires-Dist: dissect.cim==3.7
-Requires-Dist: dissect.clfs==1.6
-Requires-Dist: dissect.cstruct==3.10
-Requires-Dist: dissect.esedb==3.9
-Requires-Dist: dissect.etl==3.7
-Requires-Dist: dissect.eventlog==3.6
-Requires-Dist: dissect.evidence==3.7
-Requires-Dist: dissect.executable==1.4
-Requires-Dist: dissect.extfs==3.6
-Requires-Dist: dissect.fat==3.6
-Requires-Dist: dissect.ffs==3.6
-Requires-Dist: dissect.hypervisor==3.9
-Requires-Dist: dissect.ntfs==3.7
-Requires-Dist: dissect.ole==3.6
-Requires-Dist: dissect.regf==3.7
-Requires-Dist: dissect.shellitem==3.6
-Requires-Dist: dissect.sql==3.6
-Requires-Dist: dissect.squashfs==1.3
-Requires-Dist: dissect.target[full]==3.12
-Requires-Dist: dissect.thumbcache==1.6
-Requires-Dist: dissect.util==3.11
-Requires-Dist: dissect.vmfs==3.6
-Requires-Dist: dissect.volume==3.7
-Requires-Dist: dissect.xfs==3.6
 
 # dissect
 
 Dissect is a digital forensics & incident response framework and toolset that allows you to quickly access and analyse forensic artefacts from various disk and file formats, developed by Fox-IT (part of NCC Group).
 
 This project is a meta package, it will install all other Dissect modules with the right combination of versions. For
 more information, please see [the documentation](https://docs.dissect.tools/).
```

### Comparing `dissect-3.9/pyproject.toml` & `dissect-3.9.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,35 +23,35 @@
   "Topic :: Scientific/Engineering :: Information Analysis",
   "Topic :: Security",
   "Topic :: Utilities",
 ]
 dependencies = [
     "dissect.cim==3.7",
     "dissect.clfs==1.6",
-    "dissect.cstruct==3.10",
-    "dissect.esedb==3.9",
+    "dissect.cstruct==3.9",
+    "dissect.esedb==3.8",
     "dissect.etl==3.7",
     "dissect.eventlog==3.6",
-    "dissect.evidence==3.7",
+    "dissect.evidence==3.6",
     "dissect.executable==1.4",
     "dissect.extfs==3.6",
     "dissect.fat==3.6",
     "dissect.ffs==3.6",
-    "dissect.hypervisor==3.9",
+    "dissect.hypervisor==3.8",
     "dissect.ntfs==3.7",
     "dissect.ole==3.6",
     "dissect.regf==3.7",
     "dissect.shellitem==3.6",
     "dissect.sql==3.6",
     "dissect.squashfs==1.3",
-    "dissect.target[full]==3.12",
-    "dissect.thumbcache==1.6",
-    "dissect.util==3.11",
+    "dissect.target[full]==3.11.1",
+    "dissect.thumbcache==1.5",
+    "dissect.util==3.10",
     "dissect.vmfs==3.6",
-    "dissect.volume==3.7",
+    "dissect.volume==3.6",
     "dissect.xfs==3.6",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://dissect.tools"
 documentation = "https://docs.dissect.tools"
@@ -67,7 +67,8 @@
 [tool.setuptools]
 license-files = ["LICENSE", "COPYRIGHT"]
 
 [tool.setuptools.packages.find]
 include = ["dissect.*"]
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
```

### Comparing `dissect-3.9/tox.ini` & `dissect-3.9.dev1/tox.ini`

 * *Files identical despite different names*

