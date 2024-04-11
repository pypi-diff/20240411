# Comparing `tmp/typepigeon-2.0.2.tar.gz` & `tmp/typepigeon-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typepigeon-2.0.2.tar", last modified: Sat Nov 18 17:36:16 2023, max compression
+gzip compressed data, was "typepigeon-2.0.3.tar", last modified: Thu Apr 11 17:56:09 2024, max compression
```

## Comparing `typepigeon-2.0.2.tar` & `typepigeon-2.0.3.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.805139 typepigeon-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.797139 typepigeon-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.801139 typepigeon-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-11-18 17:36:01.000000 typepigeon-2.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-18 17:36:01.000000 typepigeon-2.0.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-11-18 17:36:01.000000 typepigeon-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-11-18 17:36:01.000000 typepigeon-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-18 17:36:01.000000 typepigeon-2.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    35145 2023-11-18 17:36:01.000000 typepigeon-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    45526 2023-11-18 17:36:16.805139 typepigeon-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-11-18 17:36:01.000000 typepigeon-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.801139 typepigeon-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.801139 typepigeon-2.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/source/subscripted_type.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/source/to_json.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-18 17:36:01.000000 typepigeon-2.0.2/docs/source/to_type.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-11-18 17:36:01.000000 typepigeon-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 17:36:16.805139 typepigeon-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.801139 typepigeon-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.797139 typepigeon-2.0.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.797139 typepigeon-2.0.2/tests/data/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.801139 typepigeon-2.0.2/tests/data/reference/test_convert_crs/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/data/reference/test_convert_crs/epsg4326.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/data/reference/test_convert_crs/epsg4326.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/test_subscripted_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/test_to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/test_to_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/test_to_type_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tests/test_to_type_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-11-18 17:36:01.000000 typepigeon-2.0.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.801139 typepigeon-2.0.2/typepigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-18 17:36:01.000000 typepigeon-2.0.2/typepigeon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-11-18 17:36:01.000000 typepigeon-2.0.2/typepigeon/to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2023-11-18 17:36:01.000000 typepigeon-2.0.2/typepigeon/to_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-11-18 17:36:01.000000 typepigeon-2.0.2/typepigeon/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 17:36:16.805139 typepigeon-2.0.2/typepigeon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45526 2023-11-18 17:36:16.000000 typepigeon-2.0.2/typepigeon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-11-18 17:36:16.000000 typepigeon-2.0.2/typepigeon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 17:36:16.000000 typepigeon-2.0.2/typepigeon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-18 17:36:16.000000 typepigeon-2.0.2/typepigeon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-18 17:36:16.000000 typepigeon-2.0.2/typepigeon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.469455 typepigeon-2.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.461455 typepigeon-2.0.3/.builds/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.builds/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.builds/mirror.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.builds/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.461455 typepigeon-2.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.461455 typepigeon-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-11 17:55:56.000000 typepigeon-2.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-04-11 17:55:56.000000 typepigeon-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    45492 2024-04-11 17:56:09.469455 typepigeon-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-11 17:55:56.000000 typepigeon-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.461455 typepigeon-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.465455 typepigeon-2.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/source/subscripted_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/source/to_json.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 17:55:56.000000 typepigeon-2.0.3/docs/source/to_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-11 17:55:56.000000 typepigeon-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:56:09.469455 typepigeon-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.465455 typepigeon-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.461455 typepigeon-2.0.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.461455 typepigeon-2.0.3/tests/data/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.465455 typepigeon-2.0.3/tests/data/reference/test_convert_crs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/data/reference/test_convert_crs/epsg4326.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/data/reference/test_convert_crs/epsg4326.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/test_subscripted_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/test_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/test_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/test_to_type_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tests/test_to_type_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-11 17:55:56.000000 typepigeon-2.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.465455 typepigeon-2.0.3/typepigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-11 17:55:56.000000 typepigeon-2.0.3/typepigeon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-11 17:55:56.000000 typepigeon-2.0.3/typepigeon/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-11 17:55:56.000000 typepigeon-2.0.3/typepigeon/to_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-11 17:55:56.000000 typepigeon-2.0.3/typepigeon/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:56:09.465455 typepigeon-2.0.3/typepigeon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45492 2024-04-11 17:56:09.000000 typepigeon-2.0.3/typepigeon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-11 17:56:09.000000 typepigeon-2.0.3/typepigeon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:56:09.000000 typepigeon-2.0.3/typepigeon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-11 17:56:09.000000 typepigeon-2.0.3/typepigeon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 17:56:09.000000 typepigeon-2.0.3/typepigeon.egg-info/top_level.txt
```

### Comparing `typepigeon-2.0.2/.gitignore` & `typepigeon-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/.pre-commit-config.yaml` & `typepigeon-2.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/LICENSE` & `typepigeon-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/PKG-INFO` & `typepigeon-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typepigeon
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python type converter
 Author-email: Zach Burnett <zachary.r.burnett@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -713,24 +713,24 @@
 
 ```shell
 pip install typepigeon
 ```
 
 ## Features
 
-- convert values directly from one Python type to another with `convert_value()`
-- convert values to JSON format with `convert_to_json()`
+- convert values directly from one Python type to another with `to_type()`
+- convert values to JSON format with `to_json()`
 - convert generic aliases (`List[str]`) to simple collection types (`[str]`)
-  with `guard_generic_alias()`
+  with `subscripted_type()`
 
 ## Usage
 
 With TypePigeon, you can convert simple values from one type to another:
 
-### `convert_value()`
+### `to_type()`
 
 ```python
 import typepigeon
 
 typepigeon.to_type(0.55, str)
 '0.55'
 
@@ -785,15 +785,15 @@
 typepigeon.to_type(CRS.from_epsg(4326), str)
 'GEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],CS[ellipsoidal,2],AXIS["geodetic latitude (Lat)",north,ORDER[1],ANGLEUNIT["degree",0.0174532925199433]],AXIS["geodetic longitude (Lon)",east,ORDER[2],ANGLEUNIT["degree",0.0174532925199433]],USAGE[SCOPE["Horizontal component of 3D system."],AREA["World."],BBOX[-90,-180,90,180]],ID["EPSG",4326]]'
 
 typepigeon.to_type(4326, CRS)
 CRS.from_epsg(4326)
 ```
 
-### `convert_to_json()`
+### `to_json()`
 
 ```python
 from datetime import datetime
 
 import typepigeon
 
 typepigeon.to_json(5)
@@ -808,15 +808,15 @@
 typepigeon.to_json([5, '6', {3: datetime(2021, 3, 27)}])
 [5, '6', {3: '2021-03-27 00:00:00'}]
 
 typepigeon.to_json({'test': [5, '6', {3: datetime(2021, 3, 27)}]})
 {'test': [5, '6', {3: '2021-03-27 00:00:00'}]}
 ```
 
-### `guard_generic_alias()`
+### `subscripted_type()`
 
 ```python
 import typepigeon.types
 from typing import Dict, List, Tuple
 
 import typepigeon
```

### Comparing `typepigeon-2.0.2/README.md` & `typepigeon-2.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 ```shell
 pip install typepigeon
 ```
 
 ## Features
 
-- convert values directly from one Python type to another with `convert_value()`
-- convert values to JSON format with `convert_to_json()`
+- convert values directly from one Python type to another with `to_type()`
+- convert values to JSON format with `to_json()`
 - convert generic aliases (`List[str]`) to simple collection types (`[str]`)
-  with `guard_generic_alias()`
+  with `subscripted_type()`
 
 ## Usage
 
 With TypePigeon, you can convert simple values from one type to another:
 
-### `convert_value()`
+### `to_type()`
 
 ```python
 import typepigeon
 
 typepigeon.to_type(0.55, str)
 '0.55'
 
@@ -85,15 +85,15 @@
 typepigeon.to_type(CRS.from_epsg(4326), str)
 'GEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],CS[ellipsoidal,2],AXIS["geodetic latitude (Lat)",north,ORDER[1],ANGLEUNIT["degree",0.0174532925199433]],AXIS["geodetic longitude (Lon)",east,ORDER[2],ANGLEUNIT["degree",0.0174532925199433]],USAGE[SCOPE["Horizontal component of 3D system."],AREA["World."],BBOX[-90,-180,90,180]],ID["EPSG",4326]]'
 
 typepigeon.to_type(4326, CRS)
 CRS.from_epsg(4326)
 ```
 
-### `convert_to_json()`
+### `to_json()`
 
 ```python
 from datetime import datetime
 
 import typepigeon
 
 typepigeon.to_json(5)
@@ -108,15 +108,15 @@
 typepigeon.to_json([5, '6', {3: datetime(2021, 3, 27)}])
 [5, '6', {3: '2021-03-27 00:00:00'}]
 
 typepigeon.to_json({'test': [5, '6', {3: datetime(2021, 3, 27)}]})
 {'test': [5, '6', {3: '2021-03-27 00:00:00'}]}
 ```
 
-### `guard_generic_alias()`
+### `subscripted_type()`
 
 ```python
 import typepigeon.types
 from typing import Dict, List, Tuple
 
 import typepigeon
```

### Comparing `typepigeon-2.0.2/docs/Makefile` & `typepigeon-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/docs/make.bat` & `typepigeon-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/docs/source/conf.py` & `typepigeon-2.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/pyproject.toml` & `typepigeon-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/data/reference/test_convert_crs/epsg4326.json` & `typepigeon-2.0.3/tests/data/reference/test_convert_crs/epsg4326.json`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/data/reference/test_convert_crs/epsg4326.txt` & `typepigeon-2.0.3/tests/data/reference/test_convert_crs/epsg4326.txt`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/test_subscripted_type.py` & `typepigeon-2.0.3/tests/test_subscripted_type.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/test_to_json.py` & `typepigeon-2.0.3/tests/test_to_json.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/test_to_type.py` & `typepigeon-2.0.3/tests/test_to_type.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/test_to_type_class.py` & `typepigeon-2.0.3/tests/test_to_type_class.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/tests/test_to_type_geometry.py` & `typepigeon-2.0.3/tests/test_to_type_geometry.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/typepigeon/to_json.py` & `typepigeon-2.0.3/typepigeon/to_json.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/typepigeon/to_type.py` & `typepigeon-2.0.3/typepigeon/to_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                         raise ValueError(msg)
                     input_value = collection_type(
                         to_type(input_value[index], current_type) for index, current_type in enumerate(output_type)
                     )
                 else:
                     input_value = collection_type()
             elif isinstance(input_value, str):
-                input_value = json.loads(input_value)
+                input_value = json.loads(input_value.replace("'", '"'))
 
             elif isinstance(input_value, Mapping):
                 converted_items = []
                 key_to_type = next(iter(output_type))
                 value_to_type = output_type[key_to_type]
                 for key, sub_value in input_value.items():
                     key = to_type(key, key_to_type)
```

### Comparing `typepigeon-2.0.2/typepigeon/types.py` & `typepigeon-2.0.3/typepigeon/types.py`

 * *Files identical despite different names*

### Comparing `typepigeon-2.0.2/typepigeon.egg-info/PKG-INFO` & `typepigeon-2.0.3/typepigeon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typepigeon
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python type converter
 Author-email: Zach Burnett <zachary.r.burnett@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -713,24 +713,24 @@
 
 ```shell
 pip install typepigeon
 ```
 
 ## Features
 
-- convert values directly from one Python type to another with `convert_value()`
-- convert values to JSON format with `convert_to_json()`
+- convert values directly from one Python type to another with `to_type()`
+- convert values to JSON format with `to_json()`
 - convert generic aliases (`List[str]`) to simple collection types (`[str]`)
-  with `guard_generic_alias()`
+  with `subscripted_type()`
 
 ## Usage
 
 With TypePigeon, you can convert simple values from one type to another:
 
-### `convert_value()`
+### `to_type()`
 
 ```python
 import typepigeon
 
 typepigeon.to_type(0.55, str)
 '0.55'
 
@@ -785,15 +785,15 @@
 typepigeon.to_type(CRS.from_epsg(4326), str)
 'GEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],CS[ellipsoidal,2],AXIS["geodetic latitude (Lat)",north,ORDER[1],ANGLEUNIT["degree",0.0174532925199433]],AXIS["geodetic longitude (Lon)",east,ORDER[2],ANGLEUNIT["degree",0.0174532925199433]],USAGE[SCOPE["Horizontal component of 3D system."],AREA["World."],BBOX[-90,-180,90,180]],ID["EPSG",4326]]'
 
 typepigeon.to_type(4326, CRS)
 CRS.from_epsg(4326)
 ```
 
-### `convert_to_json()`
+### `to_json()`
 
 ```python
 from datetime import datetime
 
 import typepigeon
 
 typepigeon.to_json(5)
@@ -808,15 +808,15 @@
 typepigeon.to_json([5, '6', {3: datetime(2021, 3, 27)}])
 [5, '6', {3: '2021-03-27 00:00:00'}]
 
 typepigeon.to_json({'test': [5, '6', {3: datetime(2021, 3, 27)}]})
 {'test': [5, '6', {3: '2021-03-27 00:00:00'}]}
 ```
 
-### `guard_generic_alias()`
+### `subscripted_type()`
 
 ```python
 import typepigeon.types
 from typing import Dict, List, Tuple
 
 import typepigeon
```

### Comparing `typepigeon-2.0.2/typepigeon.egg-info/SOURCES.txt` & `typepigeon-2.0.3/typepigeon.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.md
 pyproject.toml
 tox.ini
+.builds/build.yml
+.builds/mirror.yml
+.builds/test.yml
 .github/workflows/build.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 docs/source/readme.rst
```

