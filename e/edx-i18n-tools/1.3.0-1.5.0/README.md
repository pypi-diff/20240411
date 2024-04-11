# Comparing `tmp/edx-i18n-tools-1.3.0.tar.gz` & `tmp/edx-i18n-tools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-i18n-tools-1.3.0.tar", last modified: Fri Oct  6 06:14:43 2023, max compression
+gzip compressed data, was "edx-i18n-tools-1.5.0.tar", last modified: Thu Apr 11 17:29:25 2024, max compression
```

## Comparing `edx-i18n-tools-1.3.0.tar` & `edx-i18n-tools-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 06:14:43.333198 edx-i18n-tools-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-06 06:14:43.333198 edx-i18n-tools-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 06:14:43.333198 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-06 06:14:43.000000 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-10-06 06:14:43.000000 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 06:14:43.000000 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-06 06:14:43.000000 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-06 06:14:43.000000 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-06 06:14:43.000000 edx-i18n-tools-1.3.0/edx_i18n_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 06:14:43.333198 edx-i18n-tools-1.3.0/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/branch_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/changed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)    12450 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1431 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/transifex.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/i18n/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 06:14:43.333198 edx-i18n-tools-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-06 06:14:43.333198 edx-i18n-tools-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2199 2023-10-06 06:14:39.000000 edx-i18n-tools-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 17:29:25.000000 edx-i18n-tools-1.5.0/edx_i18n_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.062615 edx-i18n-tools-1.5.0/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/branch_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1431 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/i18n/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.062615 edx-i18n-tools-1.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2478 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:29:25.066615 edx-i18n-tools-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_transifex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-11 17:29:21.000000 edx-i18n-tools-1.5.0/tests/test_validate.py
```

### Comparing `edx-i18n-tools-1.3.0/LICENSE.txt` & `edx-i18n-tools-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/NOTICE.txt` & `edx-i18n-tools-1.5.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/README.rst` & `edx-i18n-tools-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/__init__.py` & `edx-i18n-tools-1.5.0/i18n/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Tool to be used by other IDAs for internationalization.
 """
 import argparse
 import sys
 
 from . import config
 
-__version__ = '1.3.0'
+__version__ = '1.5.0'
 
 
 class Runner:
     """
     Runner class for internationalization.
     """
     def __init__(self):
```

### Comparing `edx-i18n-tools-1.3.0/i18n/branch_cleanup.py` & `edx-i18n-tools-1.5.0/i18n/branch_cleanup.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/changed.py` & `edx-i18n-tools-1.5.0/i18n/changed.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/config.py` & `edx-i18n-tools-1.5.0/i18n/config.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/converter.py` & `edx-i18n-tools-1.5.0/i18n/converter.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/dummy.py` & `edx-i18n-tools-1.5.0/i18n/dummy.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/execute.py` & `edx-i18n-tools-1.5.0/i18n/execute.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/extract.py` & `edx-i18n-tools-1.5.0/i18n/extract.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/generate.py` & `edx-i18n-tools-1.5.0/i18n/generate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/main.py` & `edx-i18n-tools-1.5.0/i18n/main.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/segment.py` & `edx-i18n-tools-1.5.0/i18n/segment.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/transifex.py` & `edx-i18n-tools-1.5.0/i18n/transifex.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/i18n/validate.py` & `edx-i18n-tools-1.5.0/i18n/validate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.3.0/setup.py` & `edx-i18n-tools-1.5.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 import os
 import re
+import pathlib
 
 from setuptools import setup
 
 
 def load_requirements(*requirements_paths):
     """
     Load all requirements from the specified requirements files.
@@ -38,19 +39,25 @@
      if version_match:
          return version_match.group(1)
      raise RuntimeError("Unable to find version string.")
 
 
 VERSION = get_version("i18n", "__init__.py")
 
+here = pathlib.Path(__file__).parent.resolve()
+
+# Get the long description from the README file
+long_description = (here / "README.rst").read_text(encoding="utf-8")
 
 setup(
     name='edx-i18n-tools',
     version=VERSION,
     description='edX Internationalization Tools',
+    long_description=long_description,
+    long_description_content_type='text/x-rst',
     author='edX',
     author_email='oscm@edx.org',
     url='https://github.com/openedx/i18n-tools',
     packages=[
         'i18n',
     ],
     install_requires=load_requirements('requirements/base.in'),
@@ -64,12 +71,12 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
     ],
 )
```

