# Comparing `tmp/rastervision_gdal_vsi-0.21.3.tar.gz` & `tmp/rastervision_gdal_vsi-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_gdal_vsi-0.21.3.tar", last modified: Tue Oct 17 19:14:42 2023, max compression
+gzip compressed data, was "rastervision_gdal_vsi-0.30.0.tar", last modified: Wed Apr 10 22:11:09 2024, max compression
```

## Comparing `rastervision_gdal_vsi-0.21.3.tar` & `rastervision_gdal_vsi-0.30.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.883347 rastervision_gdal_vsi-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      553 2023-10-17 19:14:42.883347 rastervision_gdal_vsi-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.883347 rastervision_gdal_vsi-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.883347 rastervision_gdal_vsi-0.21.3/rastervision/gdal_vsi/
--rw-rw-r--   0 root         (0) root         (0)      358 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.21.3/rastervision/gdal_vsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7698 2023-09-26 14:00:58.000000 rastervision_gdal_vsi-0.21.3/rastervision/gdal_vsi/vsi_file_system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.883347 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      553 2023-10-17 19:14:42.000000 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2023-10-17 19:14:42.000000 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:42.000000 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:42.000000 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-10-17 19:14:42.000000 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:42.000000 rastervision_gdal_vsi-0.21.3/rastervision_gdal_vsi.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       50 2023-10-17 13:37:07.000000 rastervision_gdal_vsi-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:42.883347 rastervision_gdal_vsi-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1132 2023-10-17 13:37:07.000000 rastervision_gdal_vsi-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      553 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.687690 rastervision_gdal_vsi-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      358 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7698 2024-04-07 00:38:15.000000 rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/vsi_file_system.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      553 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      380 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:49.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       27 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       50 2024-04-10 21:55:10.000000 rastervision_gdal_vsi-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1720 2024-04-10 21:55:10.000000 rastervision_gdal_vsi-0.30.0/setup.py
```

### Comparing `rastervision_gdal_vsi-0.21.3/rastervision/gdal_vsi/vsi_file_system.py` & `rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/vsi_file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_gdal_vsi-0.21.3/setup.py` & `rastervision_gdal_vsi-0.30.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 # flake8: noqa
 
-from os import path as op
-import io
-from setuptools import (setup, find_namespace_packages)
-
-here = op.abspath(op.dirname(__file__))
-with io.open(op.join(here, 'requirements.txt'), encoding='utf-8') as f:
-    all_reqs = f.read().split('\n')
-install_requires = [x.strip() for x in all_reqs if 'git+' not in x]
+from os.path import abspath, dirname, join
+from setuptools import setup, find_namespace_packages
+import re
 
 name = 'rastervision_gdal_vsi'
-version = '0.21.3'
+version = '0.30.0'
 description = 'A rastervision plugin that adds a GDAL VSI file system'
+requirement_constraints = {}
+
+here = abspath(dirname(__file__))
+
+
+def parse_requirements(requirements_path: str) -> list[str]:
+    requirements = []
+    with open(requirements_path, 'r', encoding='utf-8') as f:
+        for line in f:
+            if 'git+' in line:
+                continue
+            # match package name, ignoring version constraints
+            match = re.match(r'^\s*([^\s<=>]+)', line)
+            if not match:
+                continue
+            package_name = match.group(1)
+            if package_name in requirement_constraints:
+                constraint = requirement_constraints[package_name]
+                package_name = f'{package_name}{constraint}'
+            requirements.append(package_name)
+    return requirements
+
 
 setup(
     name=name,
     version=version,
     description=description,
     url='https://github.com/azavea/raster-vision',
     author='Azavea',
@@ -26,9 +43,9 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     keywords=
     'raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing',
     packages=find_namespace_packages(exclude=['integration_tests*', 'tests*']),
-    install_requires=install_requires,
+    install_requires=parse_requirements(join(here, 'requirements.txt')),
     zip_safe=False)
```

