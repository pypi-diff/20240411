# Comparing `tmp/z3c.dependencychecker-2.8.tar.gz` & `tmp/z3c.dependencychecker-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.dependencychecker-2.8.tar", last modified: Wed Nov 30 09:54:18 2022, max compression
+gzip compressed data, was "z3c.dependencychecker-2.9.tar", last modified: Mon Jan 23 17:06:30 2023, max compression
```

## Comparing `z3c.dependencychecker-2.8.tar` & `z3c.dependencychecker-2.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.452833 z3c.dependencychecker-2.8/
--rw-r--r--   0 reinout    (501) staff       (20)     9097 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/CHANGES.rst
--rw-r--r--   0 reinout    (501) staff       (20)       17 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/COPYRIGHT.rst
--rw-r--r--   0 reinout    (501) staff       (20)     1516 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/LICENSE.rst
--rw-r--r--   0 reinout    (501) staff       (20)      138 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/MANIFEST.in
--rw-r--r--   0 reinout    (501) staff       (20)    18222 2022-11-30 09:54:18.452942 z3c.dependencychecker-2.8/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     5445 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/README.rst
--rw-r--r--   0 reinout    (501) staff       (20)      570 2022-11-30 09:54:18.453235 z3c.dependencychecker-2.8/setup.cfg
--rw-r--r--   0 reinout    (501) staff       (20)     2221 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/setup.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.443731 z3c.dependencychecker-2.8/z3c/
--rw-r--r--   0 reinout    (501) staff       (20)       56 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/__init__.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.446315 z3c.dependencychecker-2.8/z3c/dependencychecker/
--rw-r--r--   0 reinout    (501) staff       (20)     2476 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/USAGE.rst
--rw-r--r--   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)    14192 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/db.py
--rw-r--r--   0 reinout    (501) staff       (20)     2295 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/dotted_name.py
--rw-r--r--   0 reinout    (501) staff       (20)     2025 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/main.py
--rw-r--r--   0 reinout    (501) staff       (20)    15034 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/modules.py
--rw-r--r--   0 reinout    (501) staff       (20)     9033 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/package.py
--rw-r--r--   0 reinout    (501) staff       (20)     2338 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/report.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.449713 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/
--rw-r--r--   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     3523 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/conftest.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.449859 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/
--rw-r--r--   0 reinout    (501) staff       (20)     1227 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/setup.py_in
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.442377 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.451548 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/
--rw-r--r--   0 reinout    (501) staff       (20)        9 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/__init__.py_in
--rw-r--r--   0 reinout    (501) staff       (20)      419 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/configure.zcml_in
--rw-r--r--   0 reinout    (501) staff       (20)      239 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/djangosettings.py_in
--rw-r--r--   0 reinout    (501) staff       (20)      195 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/fromimports.py_in
--rw-r--r--   0 reinout    (501) staff       (20)      437 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/ftesting.zcml_in
--rw-r--r--   0 reinout    (501) staff       (20)       77 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/future_imports.py_in
--rw-r--r--   0 reinout    (501) staff       (20)       63 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/import_as.py_in
--rw-r--r--   0 reinout    (501) staff       (20)       53 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/import_asterisk.py_in
--rw-r--r--   0 reinout    (501) staff       (20)       99 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/missingrequirements.py_in
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.442517 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/profiles/
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.452111 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/
--rw-r--r--   0 reinout    (501) staff       (20)      263 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/metadata.xml_in
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.452254 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/types/
--rw-r--r--   0 reinout    (501) staff       (20)      461 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/types/dummy.xml_in
--rw-r--r--   0 reinout    (501) staff       (20)      272 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/stdlib_imports.py_in
--rw-r--r--   0 reinout    (501) staff       (20)       74 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/test_attributes.py_in
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.452690 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/tests/
--rw-r--r--   0 reinout    (501) staff       (20)        9 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/tests/__init__.py_in
--rw-r--r--   0 reinout    (501) staff       (20)      232 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/tests/doctest.txt_in
--rw-r--r--   0 reinout    (501) staff       (20)      328 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/tests/test_setup.py_in
--rw-r--r--   0 reinout    (501) staff       (20)      165 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1/unusedimports.py_in
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.451963 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/
--rw-r--r--   0 reinout    (501) staff       (20)       54 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)      243 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)        8 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/top_level.txt
--rw-r--r--   0 reinout    (501) staff       (20)     4070 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_dotted_name.py
--rw-r--r--   0 reinout    (501) staff       (20)     2189 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_dotted_name_containment.py
--rw-r--r--   0 reinout    (501) staff       (20)    10458 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_imports_database.py
--rw-r--r--   0 reinout    (501) staff       (20)     2436 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_integration.py
--rw-r--r--   0 reinout    (501) staff       (20)     3310 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_main.py
--rw-r--r--   0 reinout    (501) staff       (20)     2849 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_base.py
--rw-r--r--   0 reinout    (501) staff       (20)     4335 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_django_settings.py
--rw-r--r--   0 reinout    (501) staff       (20)     4683 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_docfiles.py
--rw-r--r--   0 reinout    (501) staff       (20)     4909 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_docstrings.py
--rw-r--r--   0 reinout    (501) staff       (20)     3767 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_fti.py
--rw-r--r--   0 reinout    (501) staff       (20)     3157 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_gs_metadata.py
--rw-r--r--   0 reinout    (501) staff       (20)     6450 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_python.py
--rw-r--r--   0 reinout    (501) staff       (20)     7561 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_zcml.py
--rw-r--r--   0 reinout    (501) staff       (20)     5527 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_package.py
--rw-r--r--   0 reinout    (501) staff       (20)     9768 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_package_metadata.py
--rw-r--r--   0 reinout    (501) staff       (20)    17209 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_report.py
--rw-r--r--   0 reinout    (501) staff       (20)     6647 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_user_mappings.py
--rw-r--r--   0 reinout    (501) staff       (20)      859 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/tests/utils.py
--rw-r--r--   0 reinout    (501) staff       (20)      433 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c/dependencychecker/utils.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2022-11-30 09:54:18.444950 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/
--rw-r--r--   0 reinout    (501) staff       (20)    18222 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     3184 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/SOURCES.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/dependency_links.txt
--rw-r--r--   0 reinout    (501) staff       (20)       70 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/entry_points.txt
--rw-r--r--   0 reinout    (501) staff       (20)        4 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/namespace_packages.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/not-zip-safe
--rw-r--r--   0 reinout    (501) staff       (20)       87 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)        4 2022-11-30 09:54:18.000000 z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/top_level.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.390359 z3c.dependencychecker-2.9/
+-rw-r--r--   0 reinout    (501) staff       (20)     9228 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/CHANGES.rst
+-rw-r--r--   0 reinout    (501) staff       (20)       17 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/COPYRIGHT.rst
+-rw-r--r--   0 reinout    (501) staff       (20)     1516 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/LICENSE.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      138 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)    18218 2023-01-23 17:06:30.390444 z3c.dependencychecker-2.9/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     5310 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      593 2023-01-23 17:06:30.390711 z3c.dependencychecker-2.9/setup.cfg
+-rw-r--r--   0 reinout    (501) staff       (20)     2221 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/setup.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.382030 z3c.dependencychecker-2.9/z3c/
+-rw-r--r--   0 reinout    (501) staff       (20)       56 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/__init__.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.384199 z3c.dependencychecker-2.9/z3c/dependencychecker/
+-rw-r--r--   0 reinout    (501) staff       (20)     2476 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/USAGE.rst
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)    14192 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/db.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2295 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/dotted_name.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2025 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/main.py
+-rw-r--r--   0 reinout    (501) staff       (20)    15034 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/modules.py
+-rw-r--r--   0 reinout    (501) staff       (20)     9215 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/package.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2338 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/report.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.387188 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3523 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/conftest.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.387340 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/
+-rw-r--r--   0 reinout    (501) staff       (20)     1227 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/setup.py_in
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.380831 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.389013 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/
+-rw-r--r--   0 reinout    (501) staff       (20)        9 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/__init__.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)      419 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/configure.zcml_in
+-rw-r--r--   0 reinout    (501) staff       (20)      239 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/djangosettings.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)      195 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/fromimports.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)      437 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/ftesting.zcml_in
+-rw-r--r--   0 reinout    (501) staff       (20)       77 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/future_imports.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)       63 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/import_as.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)       53 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/import_asterisk.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)       99 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/missingrequirements.py_in
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.380962 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/profiles/
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.389588 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/
+-rw-r--r--   0 reinout    (501) staff       (20)      263 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/metadata.xml_in
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.389734 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/types/
+-rw-r--r--   0 reinout    (501) staff       (20)      461 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/profiles/default/types/dummy.xml_in
+-rw-r--r--   0 reinout    (501) staff       (20)      272 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/stdlib_imports.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)       74 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/test_attributes.py_in
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.390184 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        9 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/tests/__init__.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)      232 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/tests/doctest.txt_in
+-rw-r--r--   0 reinout    (501) staff       (20)      328 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/tests/test_setup.py_in
+-rw-r--r--   0 reinout    (501) staff       (20)      165 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1/unusedimports.py_in
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.389434 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/
+-rw-r--r--   0 reinout    (501) staff       (20)       54 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      243 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        8 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/src/sample1.egg-info_in/top_level.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     4070 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_dotted_name.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2189 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_dotted_name_containment.py
+-rw-r--r--   0 reinout    (501) staff       (20)    10458 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_imports_database.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2436 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_integration.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3109 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_main.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2849 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_base.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4335 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_django_settings.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4683 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_docfiles.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4909 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_docstrings.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3767 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_fti.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3157 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_gs_metadata.py
+-rw-r--r--   0 reinout    (501) staff       (20)     6450 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_python.py
+-rw-r--r--   0 reinout    (501) staff       (20)     7561 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_zcml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     5527 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_package.py
+-rw-r--r--   0 reinout    (501) staff       (20)    10816 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_package_metadata.py
+-rw-r--r--   0 reinout    (501) staff       (20)    17209 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_report.py
+-rw-r--r--   0 reinout    (501) staff       (20)     6647 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_user_mappings.py
+-rw-r--r--   0 reinout    (501) staff       (20)      859 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/tests/utils.py
+-rw-r--r--   0 reinout    (501) staff       (20)      433 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c/dependencychecker/utils.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-01-23 17:06:30.382955 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)    18218 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     3184 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       70 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/entry_points.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        4 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/namespace_packages.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/not-zip-safe
+-rw-r--r--   0 reinout    (501) staff       (20)       87 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        4 2023-01-23 17:06:30.000000 z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/top_level.txt
```

### Comparing `z3c.dependencychecker-2.8/CHANGES.rst` & `z3c.dependencychecker-2.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of z3c.dependencychecker
 ==================================
 
+2.9 (2023-01-23)
+----------------
+
+- Ignore `Zope` package, as otherwise it swallows all `zope.` namespace packages.
+  [gforcada]
+
 2.8 (2022-11-30)
 ----------------
 
 - Drop python 2.7 support.
   [gforcada]
 
 - Replace travis for GitHub actions.
```

### Comparing `z3c.dependencychecker-2.8/LICENSE.rst` & `z3c.dependencychecker-2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `z3c.dependencychecker-2.8/PKG-INFO` & `z3c.dependencychecker-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.dependencychecker
-Version: 2.8
+Version: 2.9
 Summary: Reports on missing or unneeded setup.py dependencies
 Home-page: https://github.com/reinout/z3c.dependencychecker
 Author: Reinout van Rees
 Author-email: reinout@vanrees.org
 License: BSD
 Keywords: dependencies requirements missing imports
 Classifier: Development Status :: 5 - Production/Stable
@@ -169,21 +169,18 @@
 
 To run the tests (there's some pytest configuration in ``setup.cfg``)::
 
   $ bin/pytest
 
 Some checks that are run by github actions::
 
-  $ bin/black --skip-string-normalization
+  $ bin/black
   $ bin/codespell setup.py z3c/
   $ bin/flake8 setup.py z3c/
 
-Note that the string quoting style is currently not black-standard, so you'll
-have to manage it yourself.
-
 
 Usage of z3c.dependencychecker
 ==============================
 
 .. :doctest:
 
 
@@ -266,14 +263,20 @@
     setup.py to have effect.
     <BLANKLINE>
 
 
 Changelog of z3c.dependencychecker
 ==================================
 
+2.9 (2023-01-23)
+----------------
+
+- Ignore `Zope` package, as otherwise it swallows all `zope.` namespace packages.
+  [gforcada]
+
 2.8 (2022-11-30)
 ----------------
 
 - Drop python 2.7 support.
   [gforcada]
 
 - Replace travis for GitHub actions.
```

### Comparing `z3c.dependencychecker-2.8/README.rst` & `z3c.dependencychecker-2.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -140,13 +140,10 @@
 
 To run the tests (there's some pytest configuration in ``setup.cfg``)::
 
   $ bin/pytest
 
 Some checks that are run by github actions::
 
-  $ bin/black --skip-string-normalization
+  $ bin/black
   $ bin/codespell setup.py z3c/
   $ bin/flake8 setup.py z3c/
-
-Note that the string quoting style is currently not black-standard, so you'll
-have to manage it yourself.
```

### Comparing `z3c.dependencychecker-2.8/setup.cfg` & `z3c.dependencychecker-2.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 [tool:pytest]
 addopts = --cov --cov-report term-missing --cache-clear z3c/
 
 [flake8]
 max-line-length = 88
 max-complexity = 18
+inline-quotes = double
 ignore = E501,  # black takes care of line length
 	W503,  # black takes care of where to break lines
 	D202,  # black takes care of blank lines
 	E203,  # black takes care of spaces within slicing (list[:])
 	E231,  # black takes care of spaces after commas
 	A003,  # as one has to use self.XX it should not be a problem
```

### Comparing `z3c.dependencychecker-2.8/setup.py` & `z3c.dependencychecker-2.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 import codecs
 import os.path
 
 from setuptools import find_packages, setup
 
-version = '2.8'
+version = "2.9"
 
 
 def read(filename):
     try:
-        with codecs.open(filename, encoding='utf-8') as f:
+        with codecs.open(filename, encoding="utf-8") as f:
             return unicode(f.read())
     except NameError:
-        with open(filename, encoding='utf-8') as f:
+        with open(filename, encoding="utf-8") as f:
             return f.read()
 
 
 long_description = f"""
 {read('README.rst')}
 
 {read(os.path.join('z3c', 'dependencychecker', 'USAGE.rst'))}
 
 {read('CHANGES.rst')}
 """
 
 
 setup(
-    name='z3c.dependencychecker',
+    name="z3c.dependencychecker",
     version=version,
-    description='Reports on missing or unneeded setup.py dependencies',
+    description="Reports on missing or unneeded setup.py dependencies",
     long_description=long_description,
-    long_description_content_type='text/x-rst; charset=UTF-8',
+    long_description_content_type="text/x-rst; charset=UTF-8",
     # Get strings from https://pypi.org/classifiers/
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Topic :: Software Development :: Quality Assurance',
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Topic :: Software Development :: Quality Assurance",
     ],
-    keywords='dependencies requirements missing imports',
-    author='Reinout van Rees',
-    author_email='reinout@vanrees.org',
-    url='https://github.com/reinout/z3c.dependencychecker',
-    license='BSD',
-    packages=find_packages(exclude=['ez_setup']),
-    namespace_packages=['z3c'],
+    keywords="dependencies requirements missing imports",
+    author="Reinout van Rees",
+    author_email="reinout@vanrees.org",
+    url="https://github.com/reinout/z3c.dependencychecker",
+    license="BSD",
+    packages=find_packages(exclude=["ez_setup"]),
+    namespace_packages=["z3c"],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'setuptools',
+        "setuptools",
         'stdlib-list; python_version < "3.10"',
-        'cached-property',
-        'toml',
+        "cached-property",
+        "toml",
     ],
     extras_require={
-        'test': ['pytest'],
+        "test": ["pytest"],
     },
     entry_points={
-        'console_scripts': [
-            'dependencychecker = z3c.dependencychecker.main:main',
+        "console_scripts": [
+            "dependencychecker = z3c.dependencychecker.main:main",
         ]
     },
 )
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/USAGE.rst` & `z3c.dependencychecker-2.9/z3c/dependencychecker/USAGE.rst`

 * *Files identical despite different names*

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/db.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,30 +55,30 @@
     def add_imports(self, imports):
         filters = (
             self._filter_out_known_packages,
             self._filter_out_own_package,
             self._filter_out_python_standard_library,
         )
         for single_import in imports:
-            logger.debug('    Import found: %s', single_import.name)
+            logger.debug("    Import found: %s", single_import.name)
 
             unknown_import = self._apply_filters([single_import], filters)
             if unknown_import:
                 self.imports_used.append(single_import)
             else:
-                logger.debug('    Import ignored: %s', single_import.name)
+                logger.debug("    Import ignored: %s", single_import.name)
 
     def add_user_mapping(self, package_name, provided_names):
         package = DottedName(package_name)
         packages_provided = [DottedName(name) for name in provided_names]
 
         if package not in self._all_requirements():
             logger.info(
-                'Ignoring package %s as is not a dependency of the '
-                'package being analyzed',
+                "Ignoring package %s as is not a dependency of the "
+                "package being analyzed",
                 package,
             )
             return
 
         self.user_mappings[package] = set(packages_provided)
 
         for single_package in packages_provided:
@@ -285,17 +285,17 @@
         return self._discard_if_found_obj_in_list(
             dotted_name,
             self.ignored_packages,
         )
 
     def _filter_out_known_packages(self, dotted_name):
         to_ignore = (
-            DottedName('setuptools'),
-            DottedName('pkg_resources'),
-            DottedName('distribute'),
+            DottedName("setuptools"),
+            DottedName("pkg_resources"),
+            DottedName("distribute"),
         )
         return self._discard_if_found_obj_in_list(dotted_name, to_ignore)
 
     @staticmethod
     def _filter_out_testing_imports(dotted_name):
         return not dotted_name.is_test
 
@@ -357,39 +357,39 @@
                 set(list(sys.stdlib_module_names) + list(sys.builtin_module_names))
             )
         else:
             from stdlib_list import stdlib_list
 
             python_version = sys.version_info
             libraries = stdlib_list(
-                '{}.{}'.format(
+                "{}.{}".format(
                     python_version[0],
                     python_version[1],
                 )
             )
 
         fake_std_libraries = [DottedName(x) for x in libraries]
         return fake_std_libraries
 
     def _get_test_extra(self):
-        candidates = ('test', 'tests')
+        candidates = ("test", "tests")
         for candidate in candidates:
             if candidate in self._extras_requirements:
                 return self._extras_requirements[candidate]
 
         return []
 
     def _filter_user_mappings(self, dotted_names):
         """Remove dotted names that are in user mappings"""
         result = []
         for single_import in dotted_names:
             for provided_package in self.reverse_user_mappings:
                 if single_import in provided_package:
                     logger.debug(
-                        'Skip %s as is part of user mapping %s',
+                        "Skip %s as is part of user mapping %s",
                         single_import,
                         self.reverse_user_mappings[provided_package],
                     )
                     break
             else:
                 result.append(single_import)
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/dotted_name.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/dotted_name.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(
         self,
         name,
         file_path=None,
         is_test=False,
     ):
         self.name = name
-        self.safe_name = name.lower().replace('-', '_')
+        self.safe_name = name.lower().replace("-", "_")
 
         self.file_path = file_path
         self.is_test = is_test
 
     @classmethod
     def from_requirement(cls, requirement, file_path=None):
         """A requirement in this method's context is a
@@ -26,15 +26,15 @@
         return cls(
             requirement.project_name,
             file_path=file_path,
         )
 
     @cached_property
     def namespaces(self):
-        return self.safe_name.split('.')
+        return self.safe_name.split(".")
 
     @cached_property
     def is_namespaced(self):
         return bool(len(self.namespaces) - 1)
 
     def __lt__(self, other):
         if not isinstance(other, DottedName):
@@ -44,15 +44,15 @@
     def __eq__(self, other):
         if not isinstance(other, DottedName):
             return NotImplemented
 
         return self.safe_name == other.safe_name
 
     def __repr__(self):
-        return f'<DottedName {self.name}>'
+        return f"<DottedName {self.name}>"
 
     def __hash__(self):
         digest = hashlib.sha256(self.safe_name.encode()).hexdigest()
         return int(digest, 16) % 10**8
 
     def __contains__(self, item):
         """Check if self is in item or the other way around
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/main.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,60 +28,60 @@
     exit(0)
 
 
 def parse_command_line():
     usage = 'Usage: %prog [path]\n(path defaults to package name, fallback is "src/")'
     parser = optparse.OptionParser(usage=usage, version=_version())
     parser.add_option(
-        '-v',
-        '--verbose',
-        action='store_true',
-        dest='verbose',
+        "-v",
+        "--verbose",
+        action="store_true",
+        dest="verbose",
         default=False,
-        help='Show debug output',
+        help="Show debug output",
     )
     parser.add_option(
-        '--exit-zero',
-        action='store_false',
-        dest='exit_status',
+        "--exit-zero",
+        action="store_false",
+        dest="exit_status",
         default=True,
         help='Exit with status code "0" even if there are errors.',
     )
     options, args = parser.parse_args()
     return options, args
 
 
 def _version():
-    ourselves = pkg_resources.require('z3c.dependencychecker')[0]
+    ourselves = pkg_resources.require("z3c.dependencychecker")[0]
     return ourselves.version
 
 
 def set_log_level(verbose):
     level = logging.INFO
     if verbose:
         level = logging.DEBUG
 
     logging.basicConfig(
-        level=level, stream=sys.stdout, format='%(levelname)s: %(message)s'
+        level=level, stream=sys.stdout, format="%(levelname)s: %(message)s"
     )
 
 
 def get_path(args):
     """Get path to the python source distribution that will be checked for
     dependencies
 
     If no path is given on the command line arguments, the current working
     directory is used instead.
     """
     path = os.getcwd()
 
     if len(args) < 1:
-        logger.debug('path used: %s', path)
+        logger.debug("path used: %s", path)
         return path
 
     path = os.path.abspath(args[0])
     if os.path.isdir(path):
-        logger.debug('path used: %s', path)
+        logger.debug("path used: %s", path)
         return path
 
-    logger.error('Given path is not a folder: %s', args[0])
+    logger.error("Given path is not a folder: %s", args[0])
     sys.exit(1)
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/modules.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,27 +58,27 @@
         which is not always a folder:
         - folder example: z3c.dependencychecker itself
         - file example: flake8-isort or any other single file distribution
 
         Return this very same class, which would allow to call the scan()
         method to get an iterator over all this file's imports.
         """
-        if top_dir.endswith('.py'):
+        if top_dir.endswith(".py"):
             yield cls(top_dir, top_dir)
             return
 
         for path, folders, filenames in os.walk(top_dir):
-            if '__init__.py' not in filenames:
+            if "__init__.py" not in filenames:
                 # Don't descend further into the tree.
                 # Clear folders variable in-place.
                 folders[:] = []
                 continue
 
             for filename in filenames:
-                if filename.endswith('.py'):
+                if filename.endswith(".py"):
                     yield cls(
                         top_dir,
                         os.path.join(path, filename),
                     )
 
     def scan(self):
         for node in ast.walk(self._get_tree()):
@@ -100,18 +100,18 @@
                     is_test=self.testing,
                 )
 
         elif isinstance(node, ast.ImportFrom):
             if self._is_relative_import(node):
                 return
             for name in node.names:
-                if name.name == '*':
+                if name.name == "*":
                     dotted_name = node.module
                 else:
-                    dotted_name = f'{node.module}.{name.name}'
+                    dotted_name = f"{node.module}.{name.name}"
                 yield DottedName(
                     dotted_name,
                     file_path=self.path,
                     is_test=self.testing,
                 )
 
     @staticmethod
@@ -123,36 +123,36 @@
     """Extract imports from .zcml files
 
     These files are in common use in Zope/Plone based projects to define its
     components and more.
     """
 
     ELEMENTS = {
-        'include': ('package',),
-        'adapter': ('for', 'factory', 'provides'),
-        'utility': ('provides', 'component'),
-        'browser:page': ('class', 'for', 'layer'),
-        'subscriber': ('handler', 'for'),
-        'securityPolicy': ('component',),
-        'genericsetup:registerProfile': ('provides',),
+        "include": ("package",),
+        "adapter": ("for", "factory", "provides"),
+        "utility": ("provides", "component"),
+        "browser:page": ("class", "for", "layer"),
+        "subscriber": ("handler", "for"),
+        "securityPolicy": ("component",),
+        "genericsetup:registerProfile": ("provides",),
     }
 
     @classmethod
     def create_from_files(cls, top_dir):
         """Find all ZCML files in the package
 
         Return this very same class, which would allow to call the scan()
         method to get an iterator over all this file's imports.
         """
-        if top_dir.endswith('.py'):
+        if top_dir.endswith(".py"):
             return
 
         for path, _folders, filenames in os.walk(top_dir):
             for filename in filenames:
-                if filename.endswith('.zcml'):
+                if filename.endswith(".zcml"):
                     yield cls(
                         top_dir,
                         os.path.join(path, filename),
                     )
 
     def scan(self):
         tree = ElementTree.parse(self.path).getroot()
@@ -162,81 +162,81 @@
             for node in tree.iter(element_namespaced):
                 for attrib in self.ELEMENTS[element]:
                     yield from self._extract_dotted_name(node, attrib)
 
     def _extract_dotted_name(self, node, attr):
         if attr in node.keys():
             candidate_text = node.get(attr)
-            for dotted_name in candidate_text.split(' '):
-                if not dotted_name or dotted_name.startswith('.'):
+            for dotted_name in candidate_text.split(" "):
+                if not dotted_name or dotted_name.startswith("."):
                     continue
 
-                if dotted_name == '*':
+                if dotted_name == "*":
                     continue
 
                 yield DottedName(
                     dotted_name,
                     file_path=self.path,
                     is_test=self.testing,
                 )
 
     @staticmethod
     def _build_namespaced_element(element):
-        if ':' in element:
-            namespace, name = element.split(':')
-            return '{{http://namespaces.zope.org/{0}}}{1}'.format(
+        if ":" in element:
+            namespace, name = element.split(":")
+            return "{{http://namespaces.zope.org/{0}}}{1}".format(
                 namespace,
                 name,
             )
 
-        return f'{{http://namespaces.zope.org/zope}}{element}'
+        return f"{{http://namespaces.zope.org/zope}}{element}"
 
 
 class FTIFile(BaseModule):
     """Extract imports from Factory Type Information files
 
     These are xml files, usually located inside a types folder and used by
     Zope/Plone based projects to define its content types.
     """
 
-    TYPES_FOLDER = f'{os.sep}types'
+    TYPES_FOLDER = f"{os.sep}types"
 
     @classmethod
     def create_from_files(cls, top_dir):
         """Find all FTI files, which are xml, in the package
 
         Return this very same class, which would allow to call the scan()
         method to get an iterator over all this file's imports.
         """
-        if top_dir.endswith('.py'):
+        if top_dir.endswith(".py"):
             return
 
         for path, _folders, filenames in os.walk(top_dir):
             for filename in filenames:
-                if filename.endswith('.xml') and cls.TYPES_FOLDER in path:
+                if filename.endswith(".xml") and cls.TYPES_FOLDER in path:
                     yield cls(
                         top_dir,
                         os.path.join(path, filename),
                     )
 
     def scan(self):
         tree = ElementTree.parse(self.path).getroot()
 
-        for node in tree.iter('property'):
-            if 'name' in node.keys():
-                name = node.get('name')
-                if name == 'behaviors':
-                    for subnode in node.iter('element'):
-                        if 'value' in subnode.keys():
+        for node in tree.iter("property"):
+            if "name" in node.keys():
+                name = node.get("name")
+                if name == "behaviors":
+                    for subnode in node.iter("element"):
+                        if "value" in subnode.keys():
                             yield DottedName(
-                                subnode.get('value'),
+                                subnode.get("value"),
                                 file_path=self.path,
                                 is_test=self.testing,
                             )
-                elif name in ('klass', 'schema'):
+                elif name in ("klass", "schema"):
                     if node.text:
                         yield DottedName(
                             node.text.strip(),
                             file_path=self.path,
                             is_test=self.testing,
                         )
 
@@ -244,44 +244,44 @@
 class GSMetadata(BaseModule):
     """Extract imports from Generic Setup metadata.xml files
 
     These files are in common use in Zope/Plone to define Generic Setup
     profile dependencies between projects.
     """
 
-    PROFILE_RE = re.compile(r'profile-(?P<dotted_name>[\w.]+):[\w\W]+')
+    PROFILE_RE = re.compile(r"profile-(?P<dotted_name>[\w.]+):[\w\W]+")
 
     @classmethod
     def create_from_files(cls, top_dir):
         """Find all metadata.xml files in the package
 
         Return this very same class, which would allow to call the scan()
         method to get an iterator over all this file's imports.
         """
-        if top_dir.endswith('.py'):
+        if top_dir.endswith(".py"):
             return
 
         for path, _folders, filenames in os.walk(top_dir):
             for filename in filenames:
-                if filename == 'metadata.xml':
+                if filename == "metadata.xml":
                     yield cls(
                         top_dir,
                         os.path.join(path, filename),
                     )
 
     def scan(self):
         tree = ElementTree.parse(self.path).getroot()
 
-        for node in tree.iter('dependency'):
+        for node in tree.iter("dependency"):
             if not node.text:
                 continue
             result = self.PROFILE_RE.search(node.text.strip())
             if result:
                 yield DottedName(
-                    result.group('dotted_name'),
+                    result.group("dotted_name"),
                     file_path=self.path,
                     is_test=self.testing,
                 )
 
 
 class PythonDocstrings(PythonModule):
     """Extract imports from docstrings found inside python modules
@@ -303,15 +303,15 @@
                 docstring = ast.get_docstring(node)
                 yield from self._parse_docstring(docstring)
 
     def _parse_docstring(self, docstring):
         if not docstring:
             return
 
-        for line in docstring.split('\n'):
+        for line in docstring.split("\n"):
             code = self._extract_code(line)
             if code:
                 try:
                     tree = ast.parse(code)
                 except SyntaxError:
                     logger.debug(
                         'Could not parse "%s" in %s',
@@ -323,16 +323,16 @@
                 for node in ast.walk(tree):
                     for dotted_name in self._process_ast_node(node):
                         dotted_name.is_test = True
                         yield dotted_name
 
     @staticmethod
     def _extract_code(line):
-        if '>>>' in line:
-            position = line.find('>>>') + 3
+        if ">>>" in line:
+            position = line.find(">>>") + 3
             return line[position:].strip()
 
 
 class DocFiles(PythonDocstrings):
     """Extract imports from documentation-like documents
 
     One extended testing pattern (at least in Zope/Plone based projects) is to
@@ -348,20 +348,20 @@
         which is not always a folder:
         - folder example: z3c.dependencychecker itself
         - file example: flake8-isort or any other single file distribution
 
         Return this very same class, which would allow to call the scan()
         method to get an iterator over all this file's imports.
         """
-        if top_dir.endswith('.py'):
+        if top_dir.endswith(".py"):
             return
 
         for path, _folders, filenames in os.walk(top_dir):
             for filename in filenames:
-                if filename.endswith('.txt') or filename.endswith('.rst'):
+                if filename.endswith(".txt") or filename.endswith(".rst"):
                     yield cls(
                         top_dir,
                         os.path.join(path, filename),
                     )
 
     def scan(self):
         with open(self.path) as doc_file:
@@ -398,20 +398,20 @@
         which is not always a folder:
         - folder example: z3c.dependencychecker itself
         - file example: flake8-isort or any other single file distribution
 
         Return this very same class, which would allow to call the scan()
         method to get an iterator over all this file's imports.
         """
-        if top_dir.endswith('.py'):
+        if top_dir.endswith(".py"):
             return
 
         for path, _folders, filenames in os.walk(top_dir):
             for filename in filenames:
-                if fnmatch.fnmatch(filename, '*settings.py'):
+                if fnmatch.fnmatch(filename, "*settings.py"):
                     yield cls(
                         top_dir,
                         os.path.join(path, filename),
                     )
 
     def scan(self):
         for node in ast.walk(self._get_tree()):
@@ -435,26 +435,26 @@
                         )
 
     @staticmethod
     def _is_installed_apps_assignment(node):
         if (
             len(node.targets) == 1
             and isinstance(node.targets[0], ast.Name)
-            and node.targets[0].id == 'INSTALLED_APPS'
+            and node.targets[0].id == "INSTALLED_APPS"
         ):
             return True
 
         return False
 
     @staticmethod
     def _is_test_runner_assignment(node):
         if (
             len(node.targets) == 1
             and isinstance(node.targets[0], ast.Name)
-            and node.targets[0].id == 'TEST_RUNNER'
+            and node.targets[0].id == "TEST_RUNNER"
         ):
             return True
 
         return False
 
 
 MODULES = (
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/package.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 class PackageMetadata:
     """Information related to a python source distribution
 
     It relies heavily on setuptools and pkg_resources APIs.
     """
 
     def __init__(self, path):
-        logger.debug('Reading package metadata for %s...', path)
+        logger.debug("Reading package metadata for %s...", path)
         self._path = path
         self._working_set = self._generate_working_set_with_ourselves()
 
     @cached_property
     def distribution_root(self):
-        if 'setup.py' not in os.listdir(self._path):
+        if "setup.py" not in os.listdir(self._path):
             logger.error(
-                'setup.py was not found in %s. '
-                'Without it dependencychecker can not work.',
+                "setup.py was not found in %s. "
+                "Without it dependencychecker can not work.",
                 self._path,
             )
             sys.exit(1)
         return self._path
 
     @cached_property
     def setup_py_path(self):
         return os.path.join(
             self.distribution_root,
-            'setup.py',
+            "setup.py",
         )
 
     @cached_property
     def package_dir(self):
         """Check where the .egg-info is located"""
         try_paths = [self.distribution_root]
         top_level_elements = [
@@ -53,42 +53,42 @@
             for folder in os.listdir(self.distribution_root)
         ]
         try_paths += [folder for folder in top_level_elements if os.path.isdir(folder)]
         for path in try_paths:
             folder_found = self._find_egg_info_in_folder(path)
             if folder_found:
                 logger.debug(
-                    '.egg-info folder found at %s folder',
+                    ".egg-info folder found at %s folder",
                     path,
                 )
                 return path
 
-        logger.error('.egg-info folder could not be found')
+        logger.error(".egg-info folder could not be found")
         sys.exit(1)
 
     @staticmethod
     def _find_egg_info_in_folder(path):
         with change_dir(path):
-            results = glob.glob('*.egg-info')
+            results = glob.glob("*.egg-info")
         return results
 
     @cached_property
     def egg_info_dir(self):
         results = self._find_egg_info_in_folder(self.package_dir)
         return os.path.join(
             self.package_dir,
             results[0],
         )
 
     @cached_property
     def name(self):
         path, filename = os.path.split(self.egg_info_dir)
-        name = filename[: -len('.egg-info')]
+        name = filename[: -len(".egg-info")]
         logger.debug(
-            'Package name is %s',
+            "Package name is %s",
             name,
         )
 
         return name
 
     def _generate_working_set_with_ourselves(self):
         """Use pkg_resources API to enable the package being analyzed
@@ -106,88 +106,92 @@
         """
         ourselves = pkg_resources.Requirement.parse(self.name)
         try:
             package = self._working_set.find(ourselves)
             return package
         except ValueError:
             logger.error(
-                'Package %s could not be found.\n'
-                'You might need to put it in development mode,\n'
-                'i.e. python setup.py develop',
+                "Package %s could not be found.\n"
+                "You might need to put it in development mode,\n"
+                "i.e. python setup.py develop",
                 self.name,
             )
             sys.exit(1)
 
     def get_required_dependencies(self):
         this_package = self._get_ourselves_from_working_set()
         requirements = this_package.requires()
         for requirement in requirements:
+            if requirement.project_name == "Zope":
+                logger.debug("Ignoring 'Zope' requirement")
+                continue
             yield DottedName.from_requirement(
                 requirement,
                 file_path=self.setup_py_path,
             )
 
     def get_extras_dependencies(self):
         """Get this packages' extras dependencies defined in setup.py"""
         this_package = self._get_ourselves_from_working_set()
 
         for extra_name in this_package.extras:
             extra_requirements = this_package.requires(extras=(extra_name,))
             dotted_names = (
                 DottedName.from_requirement(req, file_path=self.setup_py_path)
                 for req in extra_requirements
+                if req.project_name != "Zope"
             )
             yield extra_name, dotted_names
 
     @cached_property
     def top_level(self):
         path = os.path.join(
             self.egg_info_dir,
-            'top_level.txt',
+            "top_level.txt",
         )
         if not os.path.exists(path):
             logger.error(
-                'top_level.txt could not be found on %s.\n'
-                'It is needed for dependencychecker to work properly.',
+                "top_level.txt could not be found on %s.\n"
+                "It is needed for dependencychecker to work properly.",
                 self.egg_info_dir,
             )
             sys.exit(1)
 
         with open(path) as top_level_file:
             content = top_level_file.read().strip()
 
         top_levels = []
-        for candidate in content.split('\n'):
+        for candidate in content.split("\n"):
             possible_top_level = os.path.join(
                 self.package_dir,
                 candidate,
             )
 
             if os.path.exists(possible_top_level):
-                logger.debug('Found top level %s', possible_top_level)
+                logger.debug("Found top level %s", possible_top_level)
                 top_levels.append(possible_top_level)
                 continue
 
-            single_module = f'{possible_top_level}.py'
+            single_module = f"{possible_top_level}.py"
             if os.path.exists(single_module):
-                logger.debug('Found top level %s', single_module)
+                logger.debug("Found top level %s", single_module)
                 top_levels.append(single_module)
                 continue
 
             logger.warning(
-                'Top level %s not found but referenced by top_level.txt',
+                "Top level %s not found but referenced by top_level.txt",
                 possible_top_level,
             )
 
         if top_levels:
             return top_levels
 
         logger.error(
-            'There are paths found in %s%stop_level.txt that do not exist.\n'
-            'Maybe you need to put the package in development again?',
+            "There are paths found in %s%stop_level.txt that do not exist.\n"
+            "Maybe you need to put the package in development again?",
             self.egg_info_dir,
             os.sep,
         )
         sys.exit(1)
 
 
 class Package:
@@ -225,43 +229,43 @@
         They need to be on a pyproject.toml file within the table
         tool.dependencychecker.
 
         See tests/test_user_mappings.py for examples.
         """
         config = self._load_user_config()
         for package, packages_provided in config.items():
-            if package == 'ignore-packages':
+            if package == "ignore-packages":
                 if isinstance(packages_provided, list):
                     self.imports.add_ignored_packages(packages_provided)
                 else:
                     logger.warning(
-                        'ignore-packages key in pyproject.toml needs to '
-                        'be a list, even for a single package to be ignored.'
+                        "ignore-packages key in pyproject.toml needs to "
+                        "be a list, even for a single package to be ignored."
                     )
             elif isinstance(packages_provided, list):
                 self.imports.add_user_mapping(package, packages_provided)
 
     def analyze_package(self):
         for top_folder in self.metadata.top_level:
-            logger.debug('Analyzing package top_level %s...', top_folder)
+            logger.debug("Analyzing package top_level %s...", top_folder)
             for module_obj in MODULES:
                 logger.debug(
-                    'Starting analyzing files using %s...',
+                    "Starting analyzing files using %s...",
                     module_obj,
                 )
                 for source_file in module_obj.create_from_files(top_folder):
                     logger.debug(
-                        'Searching dependencies (with %s) in file %s...',
+                        "Searching dependencies (with %s) in file %s...",
                         module_obj.__name__,
                         source_file.path,
                     )
                     self.imports.add_imports(source_file.scan())
 
     def _load_user_config(self):
         config_file_path = os.sep.join(
-            [self.metadata.distribution_root, 'pyproject.toml']
+            [self.metadata.distribution_root, "pyproject.toml"]
         )
         try:
             config = toml.load(config_file_path)
-            return config['tool']['dependencychecker']
+            return config["tool"]["dependencychecker"]
         except (OSError, KeyError):
             return {}
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/report.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,75 +5,75 @@
 
 class Report:
     def __init__(self, package):
         self._database = package.imports
         self.exit_status = 0
 
     def print_report(self):
-        logger.debug('Package requirements: %s', self._database._requirements)
-        logger.debug('Package extras: %s', self._database._extras_requirements)
+        logger.debug("Package requirements: %s", self._database._requirements)
+        logger.debug("Package extras: %s", self._database._extras_requirements)
         logger.debug(
-            'User defined mappings: %s',
+            "User defined mappings: %s",
             self._database.user_mappings,
         )
         self.missing_requirements()
         self.missing_test_requirements()
         self.unneeded_requirements()
         self.requirements_that_should_be_test_requirements()
         self.unneeded_test_requirements()
         self.print_notice()
 
     def missing_requirements(self):
         self._print_metric(
-            'Missing requirements',
+            "Missing requirements",
             self._database.get_missing_imports,
         )
 
     def missing_test_requirements(self):
         self._print_metric(
-            'Missing test requirements',
+            "Missing test requirements",
             self._database.get_missing_test_imports,
         )
 
     def unneeded_requirements(self):
         self._print_metric(
-            'Unneeded requirements',
+            "Unneeded requirements",
             self._database.get_unneeded_requirements,
         )
 
     def requirements_that_should_be_test_requirements(self):
         self._print_metric(
-            'Requirements that should be test requirements',
+            "Requirements that should be test requirements",
             self._database.requirements_that_should_be_test_requirements,
         )
 
     def unneeded_test_requirements(self):
         self._print_metric(
-            'Unneeded test requirements',
+            "Unneeded test requirements",
             self._database.get_unneeded_test_requirements,
         )
 
     @staticmethod
     def print_notice():
-        print('')
-        print('Note: requirements are taken from the egginfo dir, so you need')
-        print('to re-run buildout (or setup.py or whatever) for changes in')
-        print('setup.py to have effect.')
-        print('')
+        print("")
+        print("Note: requirements are taken from the egginfo dir, so you need")
+        print("to re-run buildout (or setup.py or whatever) for changes in")
+        print("setup.py to have effect.")
+        print("")
 
     def _print_metric(self, title, method):
         missed = method()
         if len(missed) == 0:
             return
 
         self.exit_status = 1
 
         self._print_header(title)
         for dotted_name in missed:
-            print(f'     {dotted_name.name}')
+            print(f"     {dotted_name.name}")
 
     @staticmethod
     def _print_header(message):
         if message:
-            print('')
+            print("")
             print(message)
-            print('=' * len(message))
+            print("=" * len(message))
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/conftest.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 
 from z3c.dependencychecker.dotted_name import DottedName
 from z3c.dependencychecker.package import ImportsDatabase
 
 
 @pytest.fixture
 def fake_project():
-    temp_folder = tempfile.mkdtemp(prefix='depcheck')
+    temp_folder = tempfile.mkdtemp(prefix="depcheck")
     fake_package_files = pkg_resources.resource_filename(
-        'z3c.dependencychecker.tests',
-        'sample1',
+        "z3c.dependencychecker.tests",
+        "sample1",
     )
-    package_folder = os.path.join(temp_folder, 'sample1')
+    package_folder = os.path.join(temp_folder, "sample1")
     shutil.copytree(fake_package_files, package_folder)
     # To prevent the sample .py files to be picked up by ourselves or other
     # tools, I'm postfixing them with ``_in``, now we get to rename them.
     # Same for zcml files.
     for (dirpath, dirnames, filenames) in os.walk(package_folder):
         for filename in filenames + dirnames:
-            if not filename.endswith('_in'):
+            if not filename.endswith("_in"):
                 continue
-            new_filename = filename.replace('_in', '')
-            if new_filename == '_it__.py':
+            new_filename = filename.replace("_in", "")
+            if new_filename == "_it__.py":
                 # Oopsie :-) The replace works too well...
-                new_filename = '__init__.py'
+                new_filename = "__init__.py"
             source = os.path.join(dirpath, filename)
             target = os.path.join(dirpath, new_filename)
             os.rename(source, target)
 
     yield package_folder
     shutil.rmtree(temp_folder)
 
@@ -52,69 +52,69 @@
     """Creates a folder structure that contains the minimal files needed
     to make Package class be able to initialize without errors
     """
     folder = tempfile.mkdtemp()
     _add_setup_py(folder)
     package_name = _add_egg_info(folder)
 
-    src_folder = os.path.join(folder, 'src')
+    src_folder = os.path.join(folder, "src")
     os.makedirs(src_folder)
 
     yield folder, package_name
 
     shutil.rmtree(folder)
 
 
 def _add_setup_py(folder):
-    with open(os.path.join(folder, 'setup.py'), 'w') as setup_py_file:
-        setup_py_file.write('hi')
+    with open(os.path.join(folder, "setup.py"), "w") as setup_py_file:
+        setup_py_file.write("hi")
 
 
 def _add_egg_info(folder):
-    package_name = ''.join(random.choice(string.ascii_lowercase) for _ in range(10))
+    package_name = "".join(random.choice(string.ascii_lowercase) for _ in range(10))
 
     egg_info_folder_path = os.path.join(
         folder,
-        f'{package_name}.egg-info',
+        f"{package_name}.egg-info",
     )
     os.makedirs(egg_info_folder_path)
 
     _write_pkg_info_file(egg_info_folder_path)
     _write_requires_file(egg_info_folder_path)
     _write_top_level_file(egg_info_folder_path, package_name)
 
     return package_name
 
 
 def _write_pkg_info_file(folder):
-    with open(os.path.join(folder, 'PKG-INFO'), 'w') as pkg_info:
-        lines = '\n'.join(
-            ['Metadata-Version: 1.0', 'Name: testpackage', 'Version: 1.0.dev0']
+    with open(os.path.join(folder, "PKG-INFO"), "w") as pkg_info:
+        lines = "\n".join(
+            ["Metadata-Version: 1.0", "Name: testpackage", "Version: 1.0.dev0"]
         )
         pkg_info.write(lines)
 
 
 def _write_requires_file(folder):
-    with open(os.path.join(folder, 'requires.txt'), 'w') as requires_file:
-        lines = '\n'.join(['one', 'two'])
+    with open(os.path.join(folder, "requires.txt"), "w") as requires_file:
+        lines = "\n".join(["one", "two"])
         requires_file.write(lines)
 
 
 def _write_top_level_file(folder_path, package_name):
-    file_path = os.path.join(folder_path, 'top_level.txt')
-    with open(file_path, 'w') as top_level_file:
-        lines = '\n'.join([package_name])
+    file_path = os.path.join(folder_path, "top_level.txt")
+    with open(file_path, "w") as top_level_file:
+        lines = "\n".join([package_name])
         top_level_file.write(lines)
 
     sources_top_folder = os.path.join(
         folder_path,
-        '..',
+        "..",
         package_name,
     )
     os.makedirs(sources_top_folder)
 
 
 @pytest.fixture
 def minimal_database():
     database = ImportsDatabase()
-    database.own_dotted_name = DottedName('fake')
+    database.own_dotted_name = DottedName("fake")
     return database
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/sample1/setup.py_in` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/sample1/setup.py_in`

 * *Files identical despite different names*

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_dotted_name.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_dotted_name.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,166 +2,166 @@
 
 import pytest
 
 from z3c.dependencychecker.dotted_name import DottedName
 
 
 def test_minimal():
-    obj = DottedName('dotted.name')
-    assert obj.name == 'dotted.name'
+    obj = DottedName("dotted.name")
+    assert obj.name == "dotted.name"
 
 
 def test_no_path():
-    obj = DottedName('dotted.name')
+    obj = DottedName("dotted.name")
     assert obj.file_path is None
 
 
 def test_file_path_given():
-    obj = DottedName('dotted.name', file_path='/one/two')
-    assert obj.file_path == '/one/two'
+    obj = DottedName("dotted.name", file_path="/one/two")
+    assert obj.file_path == "/one/two"
 
 
 def test_requirement_constructor():
     mock_object = mock.MagicMock()
-    mock_property = mock.PropertyMock(return_value='my.dotted.name')
+    mock_property = mock.PropertyMock(return_value="my.dotted.name")
     type(mock_object).project_name = mock_property
 
     obj = DottedName.from_requirement(mock_object)
 
     assert obj.file_path is None
-    assert obj.name == 'my.dotted.name'
+    assert obj.name == "my.dotted.name"
 
 
 def test_requirement_constructor_with_path():
     mock_object = mock.MagicMock()
-    mock_property = mock.PropertyMock(return_value='my.dotted.name')
+    mock_property = mock.PropertyMock(return_value="my.dotted.name")
     type(mock_object).project_name = mock_property
 
-    obj = DottedName.from_requirement(mock_object, file_path='/one/two')
+    obj = DottedName.from_requirement(mock_object, file_path="/one/two")
 
-    assert obj.file_path == '/one/two'
+    assert obj.file_path == "/one/two"
 
 
 def test_is_test_import():
-    obj = DottedName('plone.app.dexterity', is_test=True)
+    obj = DottedName("plone.app.dexterity", is_test=True)
     assert obj.is_test
 
 
 def test_not_a_test_import():
-    obj = DottedName('plone.app.dexterity')
+    obj = DottedName("plone.app.dexterity")
     assert not obj.is_test
 
 
 def test_safe_name_no_changes():
-    obj = DottedName('hi.there')
+    obj = DottedName("hi.there")
     assert obj.name == obj.safe_name
 
 
 def test_safe_name_lowercase():
-    original_name = 'Hi.There'
+    original_name = "Hi.There"
     obj = DottedName(original_name)
     assert original_name.lower() == obj.safe_name
 
 
 def test_safe_name_dash_to_underscore():
-    original_name = 'hi-there'
+    original_name = "hi-there"
     obj = DottedName(original_name)
-    assert original_name.replace('-', '_') == obj.safe_name
+    assert original_name.replace("-", "_") == obj.safe_name
 
 
 def test_safe_name_all_at_once():
-    original_name = 'Hi-There'
+    original_name = "Hi-There"
     obj = DottedName(original_name)
-    assert obj.safe_name == 'hi_there'
+    assert obj.safe_name == "hi_there"
 
 
 def test_namespaces_none():
-    obj = DottedName('plain_package_name')
-    assert obj.namespaces == ['plain_package_name']
+    obj = DottedName("plain_package_name")
+    assert obj.namespaces == ["plain_package_name"]
 
 
 def test_namespaces_some():
-    obj = DottedName('plone.app.dexterity')
+    obj = DottedName("plone.app.dexterity")
     assert len(obj.namespaces) == 3
 
 
 def test_namespaces_some_details():
-    obj = DottedName('plone.app.dexterity')
-    assert obj.namespaces == ['plone', 'app', 'dexterity']
+    obj = DottedName("plone.app.dexterity")
+    assert obj.namespaces == ["plone", "app", "dexterity"]
 
 
 def test_namespaces_really_long():
-    obj = DottedName('one.two.three.four.five.six')
+    obj = DottedName("one.two.three.four.five.six")
     assert len(obj.namespaces) == 6
-    assert obj.namespaces == ['one', 'two', 'three', 'four', 'five', 'six']
+    assert obj.namespaces == ["one", "two", "three", "four", "five", "six"]
 
 
 def test_is_namespaced_not():
-    obj = DottedName('nope')
+    obj = DottedName("nope")
     assert obj.is_namespaced is False
 
 
 def test_is_namespaced():
-    obj = DottedName('plone.app.dexterity')
+    obj = DottedName("plone.app.dexterity")
     assert obj.is_namespaced
 
 
 def test_comparison_fallback():
-    obj1 = DottedName('plone.app.dexterity')
+    obj1 = DottedName("plone.app.dexterity")
     with pytest.raises(TypeError):
         obj1 < 33  # noqa: B015
 
 
 def test_comparison_bigger_than():
-    obj1 = DottedName('plone.app.ldap')
-    obj2 = DottedName('plone.app.dexterity')
+    obj1 = DottedName("plone.app.ldap")
+    obj2 = DottedName("plone.app.dexterity")
     assert obj1 > obj2
 
 
 def test_comparison_bigger_or_equal_than():
-    obj1 = DottedName('plone.app.ldap')
-    obj2 = DottedName('plone.app.dexterity')
+    obj1 = DottedName("plone.app.ldap")
+    obj2 = DottedName("plone.app.dexterity")
     assert obj1 >= obj2
     assert obj1 >= obj1
 
 
 def test_comparison_smaller_than():
-    obj1 = DottedName('plone.app.dexterity')
-    obj2 = DottedName('plone.app.ldap')
+    obj1 = DottedName("plone.app.dexterity")
+    obj2 = DottedName("plone.app.ldap")
     assert obj1 < obj2
 
 
 def test_comparison_smaller_or_equal_than():
-    obj1 = DottedName('plone.app.dexterity')
-    obj2 = DottedName('plone.app.ldap')
+    obj1 = DottedName("plone.app.dexterity")
+    obj2 = DottedName("plone.app.ldap")
     assert obj1 <= obj2
     assert obj1 <= obj1
 
 
 def test_comparison_equality():
-    obj1 = DottedName('plone.app.dexterity')
+    obj1 = DottedName("plone.app.dexterity")
     assert obj1 == obj1
 
 
 def test_comparison_equality_fallback():
-    obj1 = DottedName('plone.app.dexterity')
+    obj1 = DottedName("plone.app.dexterity")
     result = obj1 == object()
     assert not result
 
 
 def test_repr():
-    obj = DottedName('z3c.dependencychecker')
-    assert repr(obj) == '<DottedName z3c.dependencychecker>'
+    obj = DottedName("z3c.dependencychecker")
+    assert repr(obj) == "<DottedName z3c.dependencychecker>"
 
 
 def test_hash():
-    obj1 = DottedName('bla')
+    obj1 = DottedName("bla")
     assert isinstance(hash(obj1), int)
 
 
 def test_hash_in_use():
-    obj1 = DottedName('one')
-    obj2 = DottedName('two')
-    obj3 = DottedName('three')
-    obj4 = DottedName('one')
+    obj1 = DottedName("one")
+    obj2 = DottedName("two")
+    obj3 = DottedName("three")
+    obj4 = DottedName("one")
     uniques = {obj1, obj2, obj3, obj4}
     assert len(uniques) == 3
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_dotted_name_containment.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_dotted_name_containment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 from z3c.dependencychecker.dotted_name import DottedName
 
 
 def test_fallback():
     test_import = object()
-    requirement = DottedName('plone.app.dexterity')
+    requirement = DottedName("plone.app.dexterity")
     result = test_import in requirement
     assert not result
 
 
 def test_same_name_no_namespaces():
-    test_import = DottedName('Plone')
-    requirement = DottedName('Plone')
+    test_import = DottedName("Plone")
+    requirement = DottedName("Plone")
     result = test_import in requirement
     assert result
 
 
 def test_different_name_no_namespaces():
-    test_import = DottedName('Plone')
-    requirement = DottedName('Zope')
+    test_import = DottedName("Plone")
+    requirement = DottedName("Zope")
     result = test_import in requirement
     assert not result
 
 
 def test_no_substring_match_beginning():
-    test_import = DottedName('plo')
-    requirement = DottedName('plone.app.imaging')
+    test_import = DottedName("plo")
+    requirement = DottedName("plone.app.imaging")
     result = test_import in requirement
     assert not result
 
 
 def test_no_substring_match_beginning_reverse_check():
-    test_import = DottedName('reinout.happy')
-    requirement = DottedName('re')
+    test_import = DottedName("reinout.happy")
+    requirement = DottedName("re")
     result = test_import in requirement
     assert not result
 
 
 def test_no_substring_match_middle():
-    test_import = DottedName('ima')
-    requirement = DottedName('plone.app.imaging')
+    test_import = DottedName("ima")
+    requirement = DottedName("plone.app.imaging")
     result = test_import in requirement
     assert not result
 
 
 def test_no_substring_match_end():
-    test_import = DottedName('imaging')
-    requirement = DottedName('plone.app.imaging')
+    test_import = DottedName("imaging")
+    requirement = DottedName("plone.app.imaging")
     result = test_import in requirement
     assert not result
 
 
 def test_subpackage():
-    test_import = DottedName('plone.app.imaging.interfaces.IImage')
-    requirement = DottedName('plone.app.imaging')
+    test_import = DottedName("plone.app.imaging.interfaces.IImage")
+    requirement = DottedName("plone.app.imaging")
     result = test_import in requirement
     assert result
 
 
 def test_same_number_of_namespaces_but_different():
-    test_import = DottedName('plone.app.dexterity')
-    requirement = DottedName('plone.app.imaging')
+    test_import = DottedName("plone.app.dexterity")
+    requirement = DottedName("plone.app.imaging")
     result = test_import in requirement
     assert not result
 
 
 def test_share_only_part_of_namespace():
-    test_import = DottedName('plone.app.dexterity.interfaces')
-    requirement = DottedName('plone.app.imaging')
+    test_import = DottedName("plone.app.dexterity.interfaces")
+    requirement = DottedName("plone.app.imaging")
     result = test_import in requirement
     assert not result
 
 
 def test_both_sides_are_tested():
-    test_import = DottedName('plone.app.dexterity')
-    requirement = DottedName('plone.app.imaging.interfaces')
+    test_import = DottedName("plone.app.dexterity")
+    requirement = DottedName("plone.app.imaging.interfaces")
     result = test_import in requirement
     assert not result
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_imports_database.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_imports_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,308 +11,308 @@
     database = ImportsDatabase()
     assert isinstance(database._requirements, set)
     assert len(database._requirements) == 0
 
 
 def test_add_dependencies():
     database = ImportsDatabase()
-    database.add_requirements([DottedName('one'), DottedName('two')])
+    database.add_requirements([DottedName("one"), DottedName("two")])
 
     names = get_requirements_names(database)
     assert len(names) == 2
-    assert 'one' in names
-    assert 'two' in names
+    assert "one" in names
+    assert "two" in names
 
 
 def test_declared_dependencies_no_duplicates():
     """Check that if there are duplicated requirements,
     they are correctly filtered and only one remains
     """
     database = ImportsDatabase()
     database.add_requirements(
-        [DottedName('one'), DottedName('two'), DottedName('three'), DottedName('one')]
+        [DottedName("one"), DottedName("two"), DottedName("three"), DottedName("one")]
     )
 
     requirements = get_requirements_names(database)
     assert len(requirements) == 3
 
 
 def test_no_extras():
     database = ImportsDatabase()
     assert len(get_extras_requirements_names(database)) == 0
 
 
 def test_extras_requirements_key_names():
     database = ImportsDatabase()
-    database.add_extra_requirements('test', [DottedName('one')])
-    database.add_extra_requirements('plone', [DottedName('two')])
+    database.add_extra_requirements("test", [DottedName("one")])
+    database.add_extra_requirements("plone", [DottedName("two")])
 
     extras = get_extras_requirements_names(database)
     assert len(extras) == 2
-    assert 'test' in extras
-    assert 'plone' in extras
+    assert "test" in extras
+    assert "plone" in extras
 
 
 def test_add_extra_dependencies():
     database = ImportsDatabase()
     imports = [
-        DottedName('one'),
-        DottedName('two'),
+        DottedName("one"),
+        DottedName("two"),
     ]
-    database.add_extra_requirements('test', imports)
+    database.add_extra_requirements("test", imports)
 
-    test_extras = get_requirements_names_for_extra(database, extra='test')
+    test_extras = get_requirements_names_for_extra(database, extra="test")
     assert len(test_extras) == 2
-    assert 'one' in test_extras
-    assert 'two' in test_extras
+    assert "one" in test_extras
+    assert "two" in test_extras
 
 
 def test_warning_extra_declared_twice(caplog):
     """Show a warning if an extra is declared twice on setup.py"""
     database = ImportsDatabase()
-    database.add_extra_requirements('test', [DottedName('one')])
-    database.add_extra_requirements('test', [DottedName('two')])
+    database.add_extra_requirements("test", [DottedName("one")])
+    database.add_extra_requirements("test", [DottedName("two")])
 
     last_log = caplog.records[-1]
     message = 'extra requirement "test" is declared twice in setup.py'
     assert message == last_log.message
 
 
 def test_direct_requirements_filtered_on_extras():
     """Check that direct requirements are filtered when added to an extra"""
     database = ImportsDatabase()
-    database.add_requirements([DottedName('one'), DottedName('two')])
-    database.add_extra_requirements('test', [DottedName('one'), DottedName('three')])
+    database.add_requirements([DottedName("one"), DottedName("two")])
+    database.add_extra_requirements("test", [DottedName("one"), DottedName("three")])
 
-    test_extras = get_requirements_names_for_extra(database, extra='test')
+    test_extras = get_requirements_names_for_extra(database, extra="test")
     assert len(test_extras) == 1
-    assert 'three' in test_extras
-    assert 'one' not in test_extras
+    assert "three" in test_extras
+    assert "one" not in test_extras
 
 
 def test_filter_duplicate_extra_requirements():
     """If an extra is declared twice, duplicate requirements are filtered"""
     database = ImportsDatabase()
-    database.add_extra_requirements('test', [DottedName('one'), DottedName('three')])
-    database.add_extra_requirements('test', [DottedName('two'), DottedName('three')])
+    database.add_extra_requirements("test", [DottedName("one"), DottedName("three")])
+    database.add_extra_requirements("test", [DottedName("two"), DottedName("three")])
 
-    test_extras = get_requirements_names_for_extra(database, extra='test')
+    test_extras = get_requirements_names_for_extra(database, extra="test")
     assert len(test_extras) == 3
-    assert 'one' in test_extras
-    assert 'two' in test_extras
-    assert 'three' in test_extras
+    assert "one" in test_extras
+    assert "two" in test_extras
+    assert "three" in test_extras
 
 
 def test_no_used_imports():
     database = ImportsDatabase()
     assert len(database.imports_used) == 0
 
 
 def test_add_used_imports():
     database = ImportsDatabase()
-    database.own_dotted_name = DottedName('something-else')
-    database.add_imports([DottedName('one'), DottedName('two')])
+    database.own_dotted_name = DottedName("something-else")
+    database.add_imports([DottedName("one"), DottedName("two")])
     assert len(database.imports_used) == 2
 
 
 def test_unique_imports(minimal_database):
     minimal_database.add_imports(
         [
-            DottedName('zope.component.ISite'),
-            DottedName('zope.component'),
-            DottedName('zope.component'),
+            DottedName("zope.component.ISite"),
+            DottedName("zope.component"),
+            DottedName("zope.component"),
         ]
     )
 
     dotted_names = minimal_database._get_unique_imports()
     names = [x.name for x in dotted_names]
 
     assert len(dotted_names) == 2
-    assert 'zope.component' in names
-    assert 'zope.component.ISite' in names
+    assert "zope.component" in names
+    assert "zope.component.ISite" in names
 
 
 def test_unique_and_sorted_imports(minimal_database):
     minimal_database.add_imports(
-        [DottedName('zope.c'), DottedName('zope.a'), DottedName('zope.b')]
+        [DottedName("zope.c"), DottedName("zope.a"), DottedName("zope.b")]
     )
 
     dotted_names = minimal_database._get_unique_imports()
 
     assert len(dotted_names) == 3
-    assert dotted_names[0].name == 'zope.a'
-    assert dotted_names[1].name == 'zope.b'
-    assert dotted_names[2].name == 'zope.c'
+    assert dotted_names[0].name == "zope.a"
+    assert dotted_names[1].name == "zope.b"
+    assert dotted_names[2].name == "zope.c"
 
 
 def test_filter_out_known_packages(minimal_database):
-    dotted_name = DottedName('bla')
+    dotted_name = DottedName("bla")
     result = minimal_database._filter_out_known_packages(dotted_name)
     assert result is True
 
 
 def test_filter_out_known_packages_filtered(minimal_database):
-    dotted_name = DottedName('setuptools')
+    dotted_name = DottedName("setuptools")
     result = minimal_database._filter_out_known_packages(dotted_name)
     assert result is False
 
 
 def test_filter_out_known_packages_filtered_nested(minimal_database):
-    dotted_name = DottedName('setuptools.my.package')
+    dotted_name = DottedName("setuptools.my.package")
     result = minimal_database._filter_out_known_packages(dotted_name)
     assert result is False
 
 
 def test_filter_out_known_packages_filtered_nested_other(minimal_database):
-    dotted_name = DottedName('pkg_resources.my.package')
+    dotted_name = DottedName("pkg_resources.my.package")
     result = minimal_database._filter_out_known_packages(dotted_name)
     assert result is False
 
 
 def test_filter_out_testing_imports(minimal_database):
-    dotted_name = DottedName('bla', is_test=True)
+    dotted_name = DottedName("bla", is_test=True)
     result = minimal_database._filter_out_testing_imports(dotted_name)
     assert result is False
 
 
 def test_filter_out_testing_imports_no_testing_import(minimal_database):
-    dotted_name = DottedName('bla', is_test=False)
+    dotted_name = DottedName("bla", is_test=False)
     result = minimal_database._filter_out_testing_imports(dotted_name)
     assert result is True
 
 
 def test_filter_out_own_package(minimal_database):
-    minimal_database.own_dotted_name = DottedName('zope.component')
-    result = minimal_database._filter_out_own_package(DottedName('bla'))
+    minimal_database.own_dotted_name = DottedName("zope.component")
+    result = minimal_database._filter_out_own_package(DottedName("bla"))
     assert result is True
 
 
 def test_filter_out_own_package_filtered(minimal_database):
-    minimal_database.own_dotted_name = DottedName('zope.component')
+    minimal_database.own_dotted_name = DottedName("zope.component")
     result = minimal_database._filter_out_own_package(
-        DottedName('zope.component'),
+        DottedName("zope.component"),
     )
     assert result is False
 
 
 def test_filter_out_own_package_if_subpackage(minimal_database):
-    minimal_database.own_dotted_name = DottedName('zope.component')
-    subpackage = DottedName('zope.component.adapter')
+    minimal_database.own_dotted_name = DottedName("zope.component")
+    subpackage = DottedName("zope.component.adapter")
     result = minimal_database._filter_out_own_package(subpackage)
     assert result is False
 
 
 def test_filter_out_requirements(minimal_database):
-    pkg = DottedName('zope.component')
+    pkg = DottedName("zope.component")
     minimal_database.add_requirements([pkg])
     result = minimal_database._filter_out_requirements(pkg)
     assert result is False
 
 
 def test_filter_out_std_library(minimal_database):
-    pkg = DottedName('os.path.join')
+    pkg = DottedName("os.path.join")
     result = minimal_database._filter_out_python_standard_library(pkg)
     assert result is False
 
 
 def test_filter_out_requirements_keep_other(minimal_database):
-    pkg1 = DottedName('zope.component')
-    pkg2 = DottedName('zope.interface')
+    pkg1 = DottedName("zope.component")
+    pkg2 = DottedName("zope.interface")
 
     minimal_database.add_imports([pkg1, pkg2])
     minimal_database.add_requirements([pkg1])
     dotted_names = minimal_database.get_missing_imports()
 
     assert len(dotted_names) == 1
     assert pkg2 is dotted_names[0]
 
 
 def test_filter_out_test_requirements_in_extra(minimal_database):
-    dotted_name = DottedName('bli.blu.bla')
+    dotted_name = DottedName("bli.blu.bla")
     minimal_database.add_extra_requirements(
-        'test',
-        (DottedName('bla'), DottedName('bli')),
+        "test",
+        (DottedName("bla"), DottedName("bli")),
     )
     result = minimal_database._filter_out_test_requirements(dotted_name)
     assert result is False
 
 
 def test_filter_out_test_requirements_in_extra_variant(minimal_database):
-    dotted_name = DottedName('bli.blu.bla')
+    dotted_name = DottedName("bli.blu.bla")
     minimal_database.add_extra_requirements(
-        'tests',
-        (DottedName('bla'), DottedName('bli')),
+        "tests",
+        (DottedName("bla"), DottedName("bli")),
     )
     result = minimal_database._filter_out_test_requirements(dotted_name)
     assert result is False
 
 
 def test_get_imports_used_filter_subpackage(minimal_database):
-    subpkg1 = DottedName('zope.component.adapter')
-    subpkg2 = DottedName('zope.component.another.one')
+    subpkg1 = DottedName("zope.component.adapter")
+    subpkg2 = DottedName("zope.component.another.one")
 
     minimal_database.add_imports([subpkg1, subpkg2])
-    minimal_database.add_requirements([DottedName('zope.component')])
+    minimal_database.add_requirements([DottedName("zope.component")])
     dotted_names = minimal_database.get_missing_imports()
 
     assert len(dotted_names) == 0
 
 
 def test_get_imports_used_filter_std_library(minimal_database):
     minimal_database.add_imports(
         [
-            DottedName('zope.component'),
-            DottedName('os.path.join'),
-            DottedName('sys.version_info'),
+            DottedName("zope.component"),
+            DottedName("os.path.join"),
+            DottedName("sys.version_info"),
         ]
     )
 
     dotted_names = minimal_database.get_missing_imports()
 
     assert len(dotted_names) == 1
-    assert dotted_names[0].name == 'zope.component'
+    assert dotted_names[0].name == "zope.component"
 
 
 def test_get_missing_testing_imports(minimal_database):
-    test_import = DottedName('zope.component', is_test=True)
-    regular_import = DottedName('zope.interface', is_test=False)
+    test_import = DottedName("zope.component", is_test=True)
+    regular_import = DottedName("zope.interface", is_test=False)
     minimal_database.add_imports([test_import, regular_import])
 
     dotted_names = minimal_database.get_missing_test_imports()
 
     assert len(dotted_names) == 1
     assert dotted_names[0] is test_import
 
 
 def test_get_missing_testing_imports_filter_test_extras(minimal_database):
-    test_import1 = DottedName('zope.component', is_test=True)
-    test_import2 = DottedName('zope.interface', is_test=True)
+    test_import1 = DottedName("zope.component", is_test=True)
+    test_import2 = DottedName("zope.interface", is_test=True)
     minimal_database.add_imports([test_import1, test_import2])
-    minimal_database.add_extra_requirements('test', (test_import1,))
+    minimal_database.add_extra_requirements("test", (test_import1,))
 
     dotted_names = minimal_database.get_missing_test_imports()
 
     assert len(dotted_names) == 1
     assert dotted_names[0] is test_import2
 
 
 def test_get_test_extra(minimal_database):
-    dotted_name = DottedName('bla')
-    minimal_database.add_extra_requirements('test', (dotted_name,))
+    dotted_name = DottedName("bla")
+    minimal_database.add_extra_requirements("test", (dotted_name,))
     result = minimal_database._get_test_extra()
     assert len(result) == 1
     assert dotted_name in result
 
 
 def test_get_test_extra_plural(minimal_database):
-    dotted_name = DottedName('bla')
-    minimal_database.add_extra_requirements('tests', (dotted_name,))
+    dotted_name = DottedName("bla")
+    minimal_database.add_extra_requirements("tests", (dotted_name,))
     result = minimal_database._get_test_extra()
     assert len(result) == 1
     assert dotted_name in result
 
 
 def test_get_test_extra_no_extra(minimal_database):
-    dotted_name = DottedName('bla')
-    minimal_database.add_extra_requirements('other', (dotted_name,))
+    dotted_name = DottedName("bla")
+    minimal_database.add_extra_requirements("other", (dotted_name,))
     result = minimal_database._get_test_extra()
     assert result == []
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_integration.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,42 +48,42 @@
 setup.py to have effect.
 
 """
 
 
 def test_highlevel_integration(capsys, fake_project):
     with change_dir(fake_project):
-        arguments = ['dependencychecker']
+        arguments = ["dependencychecker"]
         try:
-            with mock.patch.object(sys, 'argv', arguments):
+            with mock.patch.object(sys, "argv", arguments):
                 main()
         except SystemExit:
             out, err = capsys.readouterr()
             assert MAIN_OUTPUT in out
         else:
             assert True is False  # pragma: nocover
 
 
 def test_entry_point_installed():
     """Check that pkg_resources can find the entry point defined in setup.py"""
     entry_point = load_entry_point(
-        'z3c.dependencychecker', 'console_scripts', 'dependencychecker'
+        "z3c.dependencychecker", "console_scripts", "dependencychecker"
     )
     assert entry_point
 
 
 def test_entry_point_run():
     """Check that calling the entry point calls a z3c.dependencychecker
     function
     """
 
     def fake_main():
-        return 'All dependencies are fine'
+        return "All dependencies are fine"
 
     import z3c.dependencychecker.main
 
-    with mock.patch.object(z3c.dependencychecker.main, 'main', fake_main):
+    with mock.patch.object(z3c.dependencychecker.main, "main", fake_main):
         entry_point = load_entry_point(
-            'z3c.dependencychecker', 'console_scripts', 'dependencychecker'
+            "z3c.dependencychecker", "console_scripts", "dependencychecker"
         )
 
-    assert entry_point() == 'All dependencies are fine'
+    assert entry_point() == "All dependencies are fine"
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_main.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import logging
 import os
 import sys
 import tempfile
 from unittest import mock
 
+import pytest
+
 from z3c.dependencychecker.main import (
     _version,
     get_path,
     main,
     parse_command_line,
     set_log_level,
 )
 from z3c.dependencychecker.utils import change_dir
 
 
 def test_usage_non_existing_option():
-    arguments = ['dependencychecker', '--non-existing']
-    sys_exit = False
-    try:
-        with mock.patch.object(sys, 'argv', arguments):
+    arguments = ["dependencychecker", "--non-existing"]
+    with pytest.raises(SystemExit):
+        with mock.patch.object(sys, "argv", arguments):
             parse_command_line()
-    except SystemExit:
-        sys_exit = True
-
-    assert sys_exit
 
 
 def test_usage_set_verbose():
-    arguments = ['dependencychecker', '--verbose']
-    with mock.patch.object(sys, 'argv', arguments):
+    arguments = ["dependencychecker", "--verbose"]
+    with mock.patch.object(sys, "argv", arguments):
         options, args = parse_command_line()
 
     assert options.verbose
 
 
 def test_version():
-    assert _version().endswith('.dev0')
+    assert _version().endswith(".dev0")
 
 
 def test_set_debug_logging():
     _cleanup_logging_handlers()
     set_log_level(True)
     assert logging.getLogger().getEffectiveLevel() == logging.DEBUG
 
@@ -99,30 +96,20 @@
 
     assert sys_exit
 
 
 def test_exit_zero_not_set(minimal_structure):
     path, _ = minimal_structure
 
-    arguments = ['dependencychecker', path]
-    exit_code = 0
-    try:
-        with mock.patch.object(sys, 'argv', arguments):
+    arguments = ["dependencychecker", path]
+    with pytest.raises(SystemExit):
+        with mock.patch.object(sys, "argv", arguments):
             main()
-    except SystemExit as exc:
-        exit_code = exc.code
-
-    assert exit_code == 1
 
 
 def test_exit_zero_set(minimal_structure):
     path, _ = minimal_structure
 
-    arguments = ['dependencychecker', '--exit-zero', path]
-    exit_code = 0
-    try:
-        with mock.patch.object(sys, 'argv', arguments):
+    arguments = ["dependencychecker", "--exit-zero", path]
+    with pytest.raises(SystemExit):
+        with mock.patch.object(sys, "argv", arguments):
             main()
-    except SystemExit as exc:
-        exit_code = exc.code
-
-    assert exit_code == 0
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_base.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,74 +4,74 @@
 import pytest
 
 from z3c.dependencychecker.modules import BaseModule
 from z3c.dependencychecker.tests.utils import write_source_file_at
 
 
 def test_module_path():
-    obj = BaseModule('/some/path', '/some/path/random/bla')
-    assert obj.path == '/some/path/random/bla'
+    obj = BaseModule("/some/path", "/some/path/random/bla")
+    assert obj.path == "/some/path/random/bla"
 
 
 def test_scan_raises():
-    obj = BaseModule('/some/path', '/some/path/random/bla')
+    obj = BaseModule("/some/path", "/some/path/random/bla")
     with pytest.raises(NotImplementedError):
         obj.scan()
 
 
 def test_create_from_files_raises():
     with pytest.raises(NotImplementedError):
-        BaseModule.create_from_files('/some/path')
+        BaseModule.create_from_files("/some/path")
 
 
 def test_has_test_with_prefix_in_path():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'blatest'))
+    temporal_file = write_source_file_at((folder, "blatest"))
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing
 
 
 def test_has_test_in_path():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'test'))
+    temporal_file = write_source_file_at((folder, "test"))
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing
 
 
 def test_has_tests_in_path():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'tests'))
+    temporal_file = write_source_file_at((folder, "tests"))
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing
 
 
 def test_has_test_in_filename():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'bla'), filename='test.py')
+    temporal_file = write_source_file_at((folder, "bla"), filename="test.py")
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing
 
 
 def test_has_tests_in_filename():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'bla'), filename='tests.py')
+    temporal_file = write_source_file_at((folder, "bla"), filename="tests.py")
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing
 
 
 def test_has_tests_with_suffix_in_filename():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'bla'), filename='testsohlala.py')
+    temporal_file = write_source_file_at((folder, "bla"), filename="testsohlala.py")
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing
 
 
 def test_is_not_a_test_module():
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'bla'), filename='bla.py')
+    temporal_file = write_source_file_at((folder, "bla"), filename="bla.py")
     python_module = BaseModule(folder, temporal_file)
     assert python_module.testing is False
 
 
 def test_parent_folder_is_test_but_module_not():
     """Be sure to ignore the filesystem part and take into account the
     package part
@@ -80,10 +80,10 @@
     /home/gil/testing/my.package
     And a file within it like:
     /home/gil/testing/my.package/src/my/package/configure.zcml
     Despite having 'test' in the path, as it is not part of the package,
     it should be ignored.
     """
     folder = tempfile.mkdtemp()
-    temporal_file = write_source_file_at((folder, 'test', 'bla'), filename='bla.py')
-    python_module = BaseModule(os.path.join(folder, 'test'), temporal_file)
+    temporal_file = write_source_file_at((folder, "test", "bla"), filename="bla.py")
+    python_module = BaseModule(os.path.join(folder, "test"), temporal_file)
     assert python_module.testing is False
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_django_settings.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_django_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import tempfile
 
 from z3c.dependencychecker.modules import DjangoSettings
 from z3c.dependencychecker.tests.utils import write_source_file_at
 
-RANDOM_CODE = 'from zope.component import adapter'
-RANDOM_ASSIGNMENT = 'a = 3'
+RANDOM_CODE = "from zope.component import adapter"
+RANDOM_ASSIGNMENT = "a = 3"
 APPS_ASSIGNMENT_TO_STRING = 'INSTALLED_APPS = "random"'
 APPS_ASSIGNMENT_TO_TUPLE = 'INSTALLED_APPS = ("random1", "random2", )'
 APPS_ASSIGNMENT_TO_LIST = 'INSTALLED_APPS = ["random3", "random4", ]'
 APPS_ASSIGNMENT_TO_LIST_MIXED = 'INSTALLED_APPS = ["random5", 3, ]'
 TEST_RUNNER_ASSIGNMENT_TO_LIST = 'TEST_RUNNER = ["random6", "random7", ]'
 TEST_RUNNER_ASSIGNMENT_TO_STRING = 'TEST_RUNNER = "random8"'
 
@@ -28,33 +28,33 @@
 def test_create_from_files_nothing(minimal_structure):
     path, package_name = minimal_structure
     modules_found = list(DjangoSettings.create_from_files(path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_single_file_random_name():
-    _, tmp_file = tempfile.mkstemp('.py')
+    _, tmp_file = tempfile.mkstemp(".py")
     modules_found = list(DjangoSettings.create_from_files(tmp_file))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_single_file_settings_name(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
-    write_source_file_at([src_path], filename='some_settings.py')
+    src_path = os.path.join(path, "src")
+    write_source_file_at([src_path], filename="some_settings.py")
     modules_found = list(DjangoSettings.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_create_from_files_deep_nested(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     write_source_file_at(
-        [src_path, 'a', 'b', 'c'],
-        filename='anothersettings.py',
+        [src_path, "a", "b", "c"],
+        filename="anothersettings.py",
     )
     modules_found = list(DjangoSettings.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_random_code(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, RANDOM_CODE)
@@ -83,16 +83,16 @@
 
 
 def test_apps_assignment_to_tuple_details(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         APPS_ASSIGNMENT_TO_TUPLE,
     )
-    assert 'random1' in dotted_names
-    assert 'random2' in dotted_names
+    assert "random1" in dotted_names
+    assert "random2" in dotted_names
 
 
 def test_apps_assignment_to_list(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         APPS_ASSIGNMENT_TO_LIST,
     )
@@ -100,16 +100,16 @@
 
 
 def test_apps_assignment_to_list_details(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         APPS_ASSIGNMENT_TO_LIST,
     )
-    assert 'random3' in dotted_names
-    assert 'random4' in dotted_names
+    assert "random3" in dotted_names
+    assert "random4" in dotted_names
 
 
 def test_apps_assignment_to_list_mixed(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         APPS_ASSIGNMENT_TO_LIST_MIXED,
     )
@@ -117,15 +117,15 @@
 
 
 def test_apps_assignment_to_list_mixed_details(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         APPS_ASSIGNMENT_TO_LIST_MIXED,
     )
-    assert dotted_names[0] == 'random5'
+    assert dotted_names[0] == "random5"
 
 
 def test_runner_assignment_to_list(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         TEST_RUNNER_ASSIGNMENT_TO_LIST,
     )
@@ -141,8 +141,8 @@
 
 
 def test_apps_assignment_to_string_mixed_details(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         TEST_RUNNER_ASSIGNMENT_TO_STRING,
     )
-    assert dotted_names[0] == 'random8'
+    assert dotted_names[0] == "random8"
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_docfiles.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_docfiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,37 +60,37 @@
     doc_file = DocFiles(folder.strpath, temporal_file)
     dotted_names = [x.name for x in doc_file.scan()]
     return dotted_names
 
 
 def test_create_from_files_nothing(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     modules_found = list(DocFiles.create_from_files(src_path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_deep_nested_txt(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     write_source_file_at(
-        [src_path, 'a', 'b', 'c'],
-        filename='bla.txt',
+        [src_path, "a", "b", "c"],
+        filename="bla.txt",
     )
 
     modules_found = list(DocFiles.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_create_from_files_deep_nested_rst(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     write_source_file_at(
-        [src_path, 'a', 'b', 'c'],
-        filename='bla.rst',
+        [src_path, "a", "b", "c"],
+        filename="bla.rst",
     )
 
     modules_found = list(DocFiles.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_no_code(tmpdir):
@@ -106,20 +106,20 @@
 def test_code_found(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, SINGLE_IMPORT)
     assert len(dotted_names) == 1
 
 
 def test_code_found_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, SINGLE_IMPORT)
-    assert dotted_names == ['zope.annotation']
+    assert dotted_names == ["zope.annotation"]
 
 
 def test_always_testing(tmpdir):
     temporal_file = write_source_file_at(
-        (tmpdir.strpath,), source_code='>>> import foo', filename='file.rst'
+        (tmpdir.strpath,), source_code=">>> import foo", filename="file.rst"
     )
 
     doc_file = DocFiles(tmpdir.strpath, temporal_file)
     dotted_names = list(doc_file.scan())
     assert len(dotted_names) == 1
     assert dotted_names[0].is_test
 
@@ -133,16 +133,16 @@
 
 
 def test_multiple_imports_same_line_details(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_SAME_LINE,
     )
-    assert 'zope.interface.Interface' in dotted_names
-    assert 'zope.interface.Attribute' in dotted_names
+    assert "zope.interface.Interface" in dotted_names
+    assert "zope.interface.Attribute" in dotted_names
 
 
 def test_multiple_imports_different_lines(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES,
     )
@@ -151,16 +151,16 @@
 
 def test_multiple_imports_different_lines_details(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES,
     )
 
-    assert 'zope.component.adapter' in dotted_names
-    assert 'zope.component.utility' in dotted_names
+    assert "zope.component.adapter" in dotted_names
+    assert "zope.component.utility" in dotted_names
 
 
 def test_multiple_imports_with_invalid_lines(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES_WITH_INVALID_CODE_LINES_BETWEEN,
     )
@@ -169,9 +169,9 @@
 
 def test_multiple_imports_with_invalid_lines_details(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES_WITH_INVALID_CODE_LINES_BETWEEN,
     )
 
-    assert 'zope.component.adapter' in dotted_names
-    assert 'zope.component.utility' in dotted_names
+    assert "zope.component.adapter" in dotted_names
+    assert "zope.component.utility" in dotted_names
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_docstrings.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_docstrings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from z3c.dependencychecker.modules import PythonDocstrings
 from z3c.dependencychecker.tests.utils import write_source_file_at
 
-NO_DOC = 'class MyClass(object): ...'
+NO_DOC = "class MyClass(object): ..."
 INVALID_PYTHON = '''
 """
 >>> and some text here that breaks the parser
 """
 '''
 DOC_IN_MODULE = '''
 """
@@ -89,45 +89,45 @@
 def test_docstring_in_module(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_MODULE)
     assert len(dotted_names) == 1
 
 
 def test_docstring_in_module_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_MODULE)
-    assert dotted_names == ['zope.component']
+    assert dotted_names == ["zope.component"]
 
 
 def test_docstring_in_function(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_FUNCTION)
     assert len(dotted_names) == 1
 
 
 def test_docstring_in_function_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_FUNCTION)
-    assert dotted_names == ['zope.component.adapter']
+    assert dotted_names == ["zope.component.adapter"]
 
 
 def test_docstring_in_class(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_CLASS)
     assert len(dotted_names) == 1
 
 
 def test_docstring_in_class_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_CLASS)
-    assert dotted_names == ['zope.component.utility']
+    assert dotted_names == ["zope.component.utility"]
 
 
 def test_docstring_in_method(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_METHOD)
     assert len(dotted_names) == 1
 
 
 def test_docstring_in_method_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, DOC_IN_METHOD)
-    assert dotted_names == ['zope.interface']
+    assert dotted_names == ["zope.interface"]
 
 
 def test_docstring_multiple_imports_same_line(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_SAME_LINE,
     )
@@ -135,16 +135,16 @@
 
 
 def test_docstring_multiple_imports_same_line_details(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_SAME_LINE,
     )
-    assert 'zope.interface.Interface' in dotted_names
-    assert 'zope.interface.Attribute' in dotted_names
+    assert "zope.interface.Interface" in dotted_names
+    assert "zope.interface.Attribute" in dotted_names
 
 
 def test_docstring_multiple_imports_different_line(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES,
     )
@@ -152,16 +152,16 @@
 
 
 def test_docstring_multiple_imports_same_different_line_details(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES,
     )
-    assert 'zope.component.adapter' in dotted_names
-    assert 'zope.component.utility' in dotted_names
+    assert "zope.component.adapter" in dotted_names
+    assert "zope.component.utility" in dotted_names
 
 
 def test_docstring_multiple_imports_with_invalid_lines(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES_WITH_INVALID_CODE_LINES_BETWEEN,
     )
@@ -169,9 +169,9 @@
 
 
 def test_docstring_multiple_imports_with_invalid_lines_details(tmpdir):
     dotted_names = _get_dependencies_on_file(
         tmpdir,
         MULTIPLE_IMPORTS_DIFFERENT_LINES_WITH_INVALID_CODE_LINES_BETWEEN,
     )
-    assert 'zope.component.adapter' in dotted_names
-    assert 'zope.component.utility' in dotted_names
+    assert "zope.component.adapter" in dotted_names
+    assert "zope.component.utility" in dotted_names
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_fti.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_fti.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 def _get_fti_imports_on_file(folder, source):
     full_content = XML_TEMPLATE.format(source)
     temporal_file = write_source_file_at(
         (folder.strpath,),
         source_code=full_content,
-        filename='configure.zcml',
+        filename="configure.zcml",
     )
 
     fti_file = FTIFile(folder.strpath, temporal_file)
     dotted_names = [x.name for x in fti_file.scan()]
     return dotted_names
 
 
@@ -62,18 +62,18 @@
     path, package_name = minimal_structure
     modules_found = list(FTIFile.create_from_files(path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_deep_nested(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     write_source_file_at(
-        [src_path, 'a', 'b', 'c', 'types'],
-        filename='test.xml',
+        [src_path, "a", "b", "c", "types"],
+        filename="test.xml",
     )
 
     modules_found = list(FTIFile.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_ignore_nodes_without_name(tmpdir):
@@ -94,47 +94,47 @@
 def test_one_behavior(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, ONE_BEHAVIOR)
     assert len(dotted_names) == 1
 
 
 def test_one_behavior_details(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, ONE_BEHAVIOR)
-    assert dotted_names == ['my.behavior']
+    assert dotted_names == ["my.behavior"]
 
 
 def test_more_behaviors(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, MORE_BEHAVIORS)
     assert len(dotted_names) == 3
 
 
 def test_more_behaviors_details(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, MORE_BEHAVIORS)
-    assert 'my.behavior1' in dotted_names
-    assert 'my.behavior2' in dotted_names
-    assert 'my.behavior3' in dotted_names
+    assert "my.behavior1" in dotted_names
+    assert "my.behavior2" in dotted_names
+    assert "my.behavior3" in dotted_names
 
 
 def test_klass(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, KLASS)
     assert len(dotted_names) == 1
 
 
 def test_klass_details(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, KLASS)
-    assert 'my.class.package' in dotted_names
+    assert "my.class.package" in dotted_names
 
 
 def test_schema(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, SCHEMA)
     assert len(dotted_names) == 1
 
 
 def test_schema_details(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, SCHEMA)
-    assert 'my.path.to.schema' in dotted_names
+    assert "my.path.to.schema" in dotted_names
 
 
 def test_something_to_ignore(tmpdir):
     dotted_names = _get_fti_imports_on_file(tmpdir, SOMETHING_ELSE_IGNORE)
     assert len(dotted_names) == 0
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_gs_metadata.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_gs_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 def _get_dependencies_on_file(folder, source):
     full_content = XML_TEMPLATE.format(source)
     temporal_file = write_source_file_at(
         (folder.strpath,),
         source_code=full_content,
-        filename='configure.zcml',
+        filename="configure.zcml",
     )
 
     gs_metadata = GSMetadata(folder.strpath, temporal_file)
     dotted_names = [x.name for x in gs_metadata.scan()]
     return dotted_names
 
 
@@ -44,18 +44,18 @@
     path, package_name = minimal_structure
     modules_found = list(GSMetadata.create_from_files(path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_deep_nested(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     write_source_file_at(
-        [src_path, 'a', 'b', 'c'],
-        filename='metadata.xml',
+        [src_path, "a", "b", "c"],
+        filename="metadata.xml",
     )
 
     modules_found = list(GSMetadata.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_ignore_other_nodes(tmpdir):
@@ -89,19 +89,19 @@
 def test_one_dependency(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, ONE_DEPENDENCY)
     assert len(dotted_names) == 1
 
 
 def test_one_dependency_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, ONE_DEPENDENCY)
-    assert dotted_names == ['plone.app.caching']
+    assert dotted_names == ["plone.app.caching"]
 
 
 def test_more_dependencies(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, MORE_DEPENDENCIES)
     assert len(dotted_names) == 2
 
 
 def test_more_dependencies_details(tmpdir):
     dotted_names = _get_dependencies_on_file(tmpdir, MORE_DEPENDENCIES)
-    assert 'plone.app.caching' in dotted_names
-    assert 'plone.app.dexterity' in dotted_names
+    assert "plone.app.caching" in dotted_names
+    assert "plone.app.dexterity" in dotted_names
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_python.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 import tempfile
 
 import pytest
 
 from z3c.dependencychecker.modules import PythonModule
 from z3c.dependencychecker.tests.utils import write_source_file_at
 
-IMPORT = 'import foo'
-IMPORT_MULTIPLE = 'import foo, bar'
-IMPORT_AS = 'import foo as bar'
-IMPORT_AS_MULTIPLE = 'import foo as bar, boo as bla'
-
-FROM_IMPORT = 'from foo import bar'
-FROM_IMPORT_MULTIPLE = 'from foo import bar, ber'
-FROM_IMPORT_AS = 'from foo import bar as ber'
-FROM_IMPORT_AS_MULTIPLE = 'from foo import bar as ber, boo as bla'
-FROM_IMPORT_ASTERISK = 'from os import *'
-FROM_IMPORT_DOT = 'from . import something'
-FROM_IMPORT_DOT_DOT = 'from .. import something'
-FROM_IMPORT_DOT_RELATIVE = 'from .local import something'
+IMPORT = "import foo"
+IMPORT_MULTIPLE = "import foo, bar"
+IMPORT_AS = "import foo as bar"
+IMPORT_AS_MULTIPLE = "import foo as bar, boo as bla"
+
+FROM_IMPORT = "from foo import bar"
+FROM_IMPORT_MULTIPLE = "from foo import bar, ber"
+FROM_IMPORT_AS = "from foo import bar as ber"
+FROM_IMPORT_AS_MULTIPLE = "from foo import bar as ber, boo as bla"
+FROM_IMPORT_ASTERISK = "from os import *"
+FROM_IMPORT_DOT = "from . import something"
+FROM_IMPORT_DOT_DOT = "from .. import something"
+FROM_IMPORT_DOT_RELATIVE = "from .local import something"
 
 
 def _get_imports_of_python_module(folder, source):
     temporal_file = write_source_file_at(
         (folder.strpath,),
         source_code=source,
     )
@@ -35,148 +35,148 @@
 def test_create_from_files_nothing(minimal_structure):
     path, package_name = minimal_structure
     modules_found = list(PythonModule.create_from_files(path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_single_file():
-    _, tmp_file = tempfile.mkstemp('.py')
+    _, tmp_file = tempfile.mkstemp(".py")
     modules_found = list(PythonModule.create_from_files(tmp_file))
     assert len(modules_found) == 1
     assert modules_found[0].path == tmp_file
 
 
 def test_create_from_files_no_init(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
+    src_path = os.path.join(path, "src")
     assert len(os.listdir(src_path)) == 0
 
     write_source_file_at([src_path])
     assert len(os.listdir(src_path)) == 1
 
     modules_found = list(PythonModule.create_from_files(src_path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_ignore_no_python(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
-    write_source_file_at([src_path], filename='__init__.py')
-    tempfile.mkstemp('.pt', 'bla', src_path)
+    src_path = os.path.join(path, "src")
+    write_source_file_at([src_path], filename="__init__.py")
+    tempfile.mkstemp(".pt", "bla", src_path)
 
     modules_found = list(PythonModule.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_create_from_files_found_python(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
-    write_source_file_at([src_path], filename='__init__.py')
-    write_source_file_at([src_path], filename='bla.py')
+    src_path = os.path.join(path, "src")
+    write_source_file_at([src_path], filename="__init__.py")
+    write_source_file_at([src_path], filename="bla.py")
 
     modules_found = list(PythonModule.create_from_files(src_path))
     assert len(modules_found) == 2
 
 
 def test_create_from_files_deep_nested(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
-    write_source_file_at([src_path], filename='__init__.py')
-    write_source_file_at([src_path], filename='bla.py')
-    write_source_file_at([src_path, 'a'], filename='__init__.py')
-    write_source_file_at([src_path, 'a'], filename='bla.py')
-    write_source_file_at([src_path, 'a', 'b'], filename='__init__.py')
-    write_source_file_at([src_path, 'a', 'b'], filename='bla.py')
+    src_path = os.path.join(path, "src")
+    write_source_file_at([src_path], filename="__init__.py")
+    write_source_file_at([src_path], filename="bla.py")
+    write_source_file_at([src_path, "a"], filename="__init__.py")
+    write_source_file_at([src_path, "a"], filename="bla.py")
+    write_source_file_at([src_path, "a", "b"], filename="__init__.py")
+    write_source_file_at([src_path, "a", "b"], filename="bla.py")
 
     modules_found = list(PythonModule.create_from_files(src_path))
     assert len(modules_found) == 6
 
 
 def test_import(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT)
     assert len(dotted_names) == 1
 
 
 def test_import_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT)
-    assert dotted_names == ['foo']
+    assert dotted_names == ["foo"]
 
 
 def test_import_multiple(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT_MULTIPLE)
     assert len(dotted_names) == 2
 
 
 def test_import_multiple_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT_MULTIPLE)
-    assert sorted(dotted_names) == ['bar', 'foo']
+    assert sorted(dotted_names) == ["bar", "foo"]
 
 
 def test_import_as(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT_AS)
     assert len(dotted_names) == 1
 
 
 def test_import_as_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT_AS)
-    assert dotted_names == ['foo']
+    assert dotted_names == ["foo"]
 
 
 def test_import_as_multiple(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT_AS_MULTIPLE)
     assert len(dotted_names) == 2
 
 
 def test_import_as_multiple_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, IMPORT_AS_MULTIPLE)
-    assert sorted(dotted_names) == ['boo', 'foo']
+    assert sorted(dotted_names) == ["boo", "foo"]
 
 
 def test_from_import(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT)
     assert len(dotted_names) == 1
 
 
 def test_from_import_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT)
-    assert dotted_names == ['foo.bar']
+    assert dotted_names == ["foo.bar"]
 
 
 def test_from_import_multiple(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT_MULTIPLE)
     assert len(dotted_names) == 2
 
 
 def test_from_import_multiple_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT_MULTIPLE)
-    assert sorted(dotted_names) == ['foo.bar', 'foo.ber']
+    assert sorted(dotted_names) == ["foo.bar", "foo.ber"]
 
 
 def test_from_import_as(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT_AS)
     assert len(dotted_names) == 1
 
 
 def test_from_import_as_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT_AS)
-    assert dotted_names == ['foo.bar']
+    assert dotted_names == ["foo.bar"]
 
 
 def test_import_asterisk(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT_ASTERISK)
     assert len(dotted_names) == 1
 
 
 def test_import_asterisk_details(tmpdir):
     dotted_names = _get_imports_of_python_module(tmpdir, FROM_IMPORT_ASTERISK)
-    assert dotted_names == ['os']
+    assert dotted_names == ["os"]
 
 
 @pytest.mark.parametrize(
-    'statement',
+    "statement",
     [
         FROM_IMPORT_DOT,
         FROM_IMPORT_DOT_DOT,
         FROM_IMPORT_DOT_RELATIVE,
     ],
 )
 def test_ignore_local_imports(statement, tmpdir):
@@ -193,16 +193,16 @@
 
 
 def test_from_import_as_multiple_details(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
         FROM_IMPORT_AS_MULTIPLE,
     )
-    assert sorted(dotted_names) == ['foo.bar', 'foo.boo']
+    assert sorted(dotted_names) == ["foo.bar", "foo.boo"]
 
 
 def test_imports_multiple_lines(tmpdir):
     dotted_names = _get_imports_of_python_module(
         tmpdir,
-        'import foo\nimport bar',
+        "import foo\nimport bar",
     )
-    assert sorted(dotted_names) == ['bar', 'foo']
+    assert sorted(dotted_names) == ["bar", "foo"]
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_modules_zcml.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_modules_zcml.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 def _get_zcml_imports_on_file(folder, source):
     full_content = ZCML_TEMPLATE.format(source)
     temporal_file = write_source_file_at(
         (folder.strpath,),
         source_code=full_content,
-        filename='configure.zcml',
+        filename="configure.zcml",
     )
 
     zcml_file = ZCMLFile(folder.strpath, temporal_file)
     dotted_names = [x.name for x in zcml_file.scan()]
     return dotted_names
 
 
@@ -56,164 +56,164 @@
     path, package_name = minimal_structure
     modules_found = list(ZCMLFile.create_from_files(path))
     assert len(modules_found) == 0
 
 
 def test_create_from_files_deep_nested(minimal_structure):
     path, package_name = minimal_structure
-    src_path = os.path.join(path, 'src')
-    write_source_file_at([src_path, 'a', 'b'], filename='configure.zcml')
+    src_path = os.path.join(path, "src")
+    write_source_file_at([src_path, "a", "b"], filename="configure.zcml")
 
     modules_found = list(ZCMLFile.create_from_files(src_path))
     assert len(modules_found) == 1
 
 
 def test_include(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, INCLUDE)
     assert len(dotted_names) == 1
 
 
 def test_include_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, INCLUDE)
-    assert dotted_names == ['my.package.include']
+    assert dotted_names == ["my.package.include"]
 
 
 def test_adapter_factory(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_FACTORY)
     assert len(dotted_names) == 1
 
 
 def test_adapter_factory_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_FACTORY)
-    assert dotted_names == ['my.package.factory']
+    assert dotted_names == ["my.package.factory"]
 
 
 def test_adapter_for(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_FOR)
     assert len(dotted_names) == 1
 
 
 def test_adapter_for_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_FOR)
-    assert dotted_names == ['my.package.for']
+    assert dotted_names == ["my.package.for"]
 
 
 def test_adapter_for_multiple(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_FOR_MULTIPLE)
     assert len(dotted_names) == 3
 
 
 def test_adapter_for_multiple_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_FOR_MULTIPLE)
-    assert 'my.package.for' in dotted_names
-    assert 'another.package.foo' in dotted_names
-    assert 'yet.another.one' in dotted_names
+    assert "my.package.for" in dotted_names
+    assert "another.package.foo" in dotted_names
+    assert "yet.another.one" in dotted_names
 
 
 def test_adapter_provides(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_PROVIDES)
     assert len(dotted_names) == 1
 
 
 def test_adapter_provides_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, ADAPTER_PROVIDES)
-    assert dotted_names == ['my.package.provides']
+    assert dotted_names == ["my.package.provides"]
 
 
 def test_utility_component(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, UTILITY_COMPONENT)
     assert len(dotted_names) == 1
 
 
 def test_utility_component_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, UTILITY_COMPONENT)
-    assert dotted_names == ['my.package.component']
+    assert dotted_names == ["my.package.component"]
 
 
 def test_utility_provides(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, UTILITY_PROVIDES)
     assert len(dotted_names) == 1
 
 
 def test_utility_provides_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, UTILITY_PROVIDES)
-    assert dotted_names == ['my.package.provides']
+    assert dotted_names == ["my.package.provides"]
 
 
 def test_browser_page_class(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, BROWSER_PAGE_CLASS)
     assert len(dotted_names) == 1
 
 
 def test_browser_page_class_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, BROWSER_PAGE_CLASS)
-    assert dotted_names == ['my.package.class']
+    assert dotted_names == ["my.package.class"]
 
 
 def test_browser_page_for(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, BROWSER_PAGE_FOR)
     assert len(dotted_names) == 1
 
 
 def test_browser_page_for_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, BROWSER_PAGE_FOR)
-    assert dotted_names == ['my.package.for']
+    assert dotted_names == ["my.package.for"]
 
 
 def test_browser_page_layer(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, BROWSER_PAGE_LAYER)
     assert len(dotted_names) == 1
 
 
 def test_browser_page_layer_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, BROWSER_PAGE_LAYER)
-    assert dotted_names == ['my.package.layer']
+    assert dotted_names == ["my.package.layer"]
 
 
 def test_subscriber_for(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SUBSCRIBER_FOR)
     assert len(dotted_names) == 1
 
 
 def test_subscriber_for_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SUBSCRIBER_FOR)
-    assert dotted_names == ['my.package.for']
+    assert dotted_names == ["my.package.for"]
 
 
 def test_subscriber_for_multiple(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SUBSCRIBER_FOR_MULTIPLE)
     assert len(dotted_names) == 2
 
 
 def test_subscriber_for_multiple_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SUBSCRIBER_FOR_MULTIPLE)
     assert dotted_names == [
-        'my.package.for',
-        'another.package',
+        "my.package.for",
+        "another.package",
     ]
 
 
 def test_subscriber_handler(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SUBSCRIBER_HANDLER)
     assert len(dotted_names) == 1
 
 
 def test_subscriber_handler_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SUBSCRIBER_HANDLER)
-    assert dotted_names == ['my.package.handler']
+    assert dotted_names == ["my.package.handler"]
 
 
 def test_securitypolicy_component(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SECURITYPOLICY_COMPONENT)
     assert len(dotted_names) == 1
 
 
 def test_securitypolicy_component_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, SECURITYPOLICY_COMPONENT)
-    assert dotted_names == ['my.package.component']
+    assert dotted_names == ["my.package.component"]
 
 
 def test_gs_registerprofile_provides(tmpdir):
     dotted_names = _get_zcml_imports_on_file(
         tmpdir,
         GS_REGISTERPROFILE_PROVIDES,
     )
@@ -221,15 +221,15 @@
 
 
 def test_gs_registerprofile_provides_details(tmpdir):
     dotted_names = _get_zcml_imports_on_file(
         tmpdir,
         GS_REGISTERPROFILE_PROVIDES,
     )
-    assert dotted_names == ['my.package.provides']
+    assert dotted_names == ["my.package.provides"]
 
 
 def test_ignore_local_import(tmpdir):
     dotted_names = _get_zcml_imports_on_file(tmpdir, IGNORE_LOCAL_IMPORT)
     assert len(dotted_names) == 0
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_package.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_package.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,164 +10,164 @@
 )
 
 
 def test_package_has_metadata(minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
 
-    assert bool(getattr(package, 'metadata', False))
+    assert bool(getattr(package, "metadata", False))
     assert isinstance(package.metadata, PackageMetadata)
 
 
 def test_declared_dependencies(minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
     package.set_declared_dependencies()
 
     requirements = get_requirements_names(package.imports)
     assert len(requirements) == 2
-    assert 'one' in requirements
-    assert 'two' in requirements
+    assert "one" in requirements
+    assert "two" in requirements
 
 
 def test_declared_dependencies_empty(minimal_structure):
     path, package_name = minimal_structure
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires:
-        requires.write('')
+    with open(requires_file_path, "w") as requires:
+        requires.write("")
 
     package = Package(path)
     package.set_declared_dependencies()
 
     assert len(get_requirements_names(package.imports)) == 0
 
 
 def test_declared_extras_dependencies_one_extra(minimal_structure):
     path, package_name = minimal_structure
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires:
-        requires.write('\n'.join(['[extra]', 'my.package', 'another.package']))
+    with open(requires_file_path, "w") as requires:
+        requires.write("\n".join(["[extra]", "my.package", "another.package"]))
 
     package = Package(path)
     package.set_declared_dependencies()
     package.set_declared_extras_dependencies()
 
     extras_names = get_extras_requirements_names(package.imports)
     assert len(extras_names) == 1
-    assert 'extra' in extras_names
-    names = get_requirements_names_for_extra(package.imports, extra='extra')
-    assert 'another.package' in names
-    assert 'my.package' in names
+    assert "extra" in extras_names
+    names = get_requirements_names_for_extra(package.imports, extra="extra")
+    assert "another.package" in names
+    assert "my.package" in names
 
 
 def test_declared_extras_dependencies_only_on_extras(minimal_structure):
     """Check that main dependencies are not bundled on the extras"""
     path, package_name = minimal_structure
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires:
+    with open(requires_file_path, "w") as requires:
         requires.write(
-            '\n'.join(['setuptools', '', '[extra]', 'my_package', 'my_other_package'])
+            "\n".join(["setuptools", "", "[extra]", "my_package", "my_other_package"])
         )
 
     package = Package(path)
     package.set_declared_dependencies()
     package.set_declared_extras_dependencies()
 
-    names = get_requirements_names_for_extra(package.imports, extra='extra')
-    assert 'setuptools' not in names
+    names = get_requirements_names_for_extra(package.imports, extra="extra")
+    assert "setuptools" not in names
 
 
 def test_multiple_extras(minimal_structure):
     path, package_name = minimal_structure
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires:
+    with open(requires_file_path, "w") as requires:
         requires.write(
-            '\n'.join(
+            "\n".join(
                 [
-                    'setuptools',
-                    '',
-                    '[extra]',
-                    'my_package',
-                    'my_other_package',
-                    '[second]',
-                    'just',
-                    'laughs',
+                    "setuptools",
+                    "",
+                    "[extra]",
+                    "my_package",
+                    "my_other_package",
+                    "[second]",
+                    "just",
+                    "laughs",
                 ]
             )
         )
 
     package = Package(path)
     package.set_declared_extras_dependencies()
 
     extras_names = get_extras_requirements_names(package.imports)
     assert len(extras_names) == 2
-    assert 'second' in extras_names
-    assert 'extra' in extras_names
+    assert "second" in extras_names
+    assert "extra" in extras_names
 
 
 def test_no_python_modules_found(minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
     package.analyze_package()
     assert len(package.imports.imports_used) == 0
 
 
 def test_python_modules_on_top_level_sources(minimal_structure):
     path, package_name = minimal_structure
-    write_source_file_at((path, package_name), '__init__.py')
+    write_source_file_at((path, package_name), "__init__.py")
     package = Package(path)
     package.analyze_package()
 
     assert len(package.imports.imports_used) == 1
     paths = get_sorted_imports_paths(package.imports)
-    assert paths[0].endswith('__init__.py')
+    assert paths[0].endswith("__init__.py")
 
 
 def test_python_modules_found_inner_folders(minimal_structure):
     path, package_name = minimal_structure
-    write_source_file_at((path, package_name), '__init__.py')
-    write_source_file_at((path, package_name, 'test'), '__init__.py')
-    write_source_file_at((path, package_name, 'test'), 'test.py')
+    write_source_file_at((path, package_name), "__init__.py")
+    write_source_file_at((path, package_name, "test"), "__init__.py")
+    write_source_file_at((path, package_name, "test"), "test.py")
 
     package = Package(path)
     package.analyze_package()
     paths = get_sorted_imports_paths(package.imports)
     assert len(paths) == 3
-    assert paths[0].endswith('__init__.py')
-    assert paths[1].endswith('__init__.py')
-    assert paths[2].endswith('test.py')
+    assert paths[0].endswith("__init__.py")
+    assert paths[1].endswith("__init__.py")
+    assert paths[2].endswith("test.py")
 
 
 def test_top_level_is_a_file(minimal_structure):
     path, package_name = minimal_structure
 
-    egg_info_folder = os.path.join(path, f'{package_name}.egg-info')
-    top_level_file_path = os.path.join(egg_info_folder, 'top_level.txt')
+    egg_info_folder = os.path.join(path, f"{package_name}.egg-info")
+    top_level_file_path = os.path.join(egg_info_folder, "top_level.txt")
     with open(top_level_file_path) as top_level_file:
         top_level_folder = top_level_file.read().strip()
 
     top_level_sources = os.path.join(path, top_level_folder)
     os.removedirs(top_level_sources)
-    with open(f'{top_level_sources}.py', 'w') as top_level_file:
-        top_level_file.write('import one')
+    with open(f"{top_level_sources}.py", "w") as top_level_file:
+        top_level_file.write("import one")
 
     package = Package(path)
     package.analyze_package()
     paths = get_sorted_imports_paths(package.imports)
     assert len(paths) == 1
-    assert paths[0].endswith(f'{top_level_folder}.py')
+    assert paths[0].endswith(f"{top_level_folder}.py")
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_package_metadata.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_package_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,102 +25,102 @@
     assert metadata.distribution_root == path
 
 
 def test_setup_py_path(minimal_structure):
     path, package_name = minimal_structure
     metadata = PackageMetadata(path)
 
-    assert metadata.setup_py_path == os.path.join(path, 'setup.py')
+    assert metadata.setup_py_path == os.path.join(path, "setup.py")
 
 
 def test_package_dir_on_distribution_root(minimal_structure):
     path, package_name = minimal_structure
     metadata = PackageMetadata(path)
 
     assert metadata.package_dir == path
 
 
 def test_package_dir_on_src_folder(minimal_structure):
     def move_top_level_to_src(package_path, egg_folder, src_path):
-        top_level_file_path = os.path.join(egg_folder, 'top_level.txt')
+        top_level_file_path = os.path.join(egg_folder, "top_level.txt")
         with open(top_level_file_path) as top_level_file:
             top_level_folder = top_level_file.read().strip()
 
         top_level_sources = os.path.join(package_path, top_level_folder)
 
         shutil.move(top_level_sources, src_path)
         shutil.move(egg_folder, src_path)
 
     path, package_name = minimal_structure
 
-    egg_info_folder = os.path.join(path, f'{package_name}.egg-info')
-    src_folder = os.path.join(path, 'src')
+    egg_info_folder = os.path.join(path, f"{package_name}.egg-info")
+    src_folder = os.path.join(path, "src")
 
     move_top_level_to_src(path, egg_info_folder, src_folder)
 
     metadata = PackageMetadata(path)
 
     assert metadata.package_dir == src_folder
 
 
 def test_package_dir_on_another_folder(minimal_structure):
     def move_top_level_to_folder(package_path, egg_folder, folder_path):
-        top_level_file_path = os.path.join(egg_folder, 'top_level.txt')
+        top_level_file_path = os.path.join(egg_folder, "top_level.txt")
         with open(top_level_file_path) as top_level_file:
             top_level_folder = top_level_file.read().strip()
 
         top_level_sources = os.path.join(package_path, top_level_folder)
 
         shutil.move(top_level_sources, folder_path)
         shutil.move(egg_folder, folder_path)
 
     path, package_name = minimal_structure
 
-    egg_info_folder = os.path.join(path, f'{package_name}.egg-info')
-    folder_path = os.path.join(path, 'somewhere')
+    egg_info_folder = os.path.join(path, f"{package_name}.egg-info")
+    folder_path = os.path.join(path, "somewhere")
 
     move_top_level_to_folder(path, egg_info_folder, folder_path)
 
     metadata = PackageMetadata(path)
 
     assert metadata.package_dir == folder_path
 
 
 def test_no_package_dir_found(minimal_structure):
     path, package_name = minimal_structure
-    shutil.rmtree(os.path.join(path, f'{package_name}.egg-info'))
+    shutil.rmtree(os.path.join(path, f"{package_name}.egg-info"))
 
     sys_exit = False
     try:
         PackageMetadata(path)
     except SystemExit:
         sys_exit = True
 
     assert sys_exit
 
 
 def test_no_package_dir_and_no_src_folder(minimal_structure):
     path, package_name = minimal_structure
-    shutil.rmtree(os.path.join(path, f'{package_name}.egg-info'))
-    shutil.rmtree(os.path.join(path, 'src'))
+    shutil.rmtree(os.path.join(path, f"{package_name}.egg-info"))
+    shutil.rmtree(os.path.join(path, "src"))
 
     sys_exit = False
     try:
         PackageMetadata(path)
     except SystemExit:
         sys_exit = True
 
     assert sys_exit
 
 
 def test_egg_info_dir_path(minimal_structure):
     path, package_name = minimal_structure
     metadata = PackageMetadata(path)
 
-    egg_info_path = os.path.join(path, f'{package_name}.egg-info')
+    egg_info_path = os.path.join(path, f"{package_name}.egg-info")
 
     assert metadata.egg_info_dir == egg_info_path
 
 
 def test_package_name(minimal_structure):
     path, package_name = minimal_structure
     metadata = PackageMetadata(path)
@@ -144,16 +144,16 @@
 
 
 def test_package_missing_pkg_info_file(minimal_structure):
     path, package_name = minimal_structure
 
     pkg_info = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'PKG-INFO',
+        f"{package_name}.egg-info",
+        "PKG-INFO",
     )
     os.remove(pkg_info)
 
     metadata = PackageMetadata(path)
 
     sys_exit = False
     try:
@@ -165,20 +165,20 @@
 
 
 def test_package_broken_pkg_info_file(minimal_structure):
     path, package_name = minimal_structure
 
     pkg_info_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'PKG-INFO',
+        f"{package_name}.egg-info",
+        "PKG-INFO",
     )
     os.remove(pkg_info_path)
-    with open(pkg_info_path, 'w') as pkg_info_file:
-        pkg_info_file.write('\n'.join(['Name: bla']))
+    with open(pkg_info_path, "w") as pkg_info_file:
+        pkg_info_file.write("\n".join(["Name: bla"]))
 
     metadata = PackageMetadata(path)
     sys_exit = False
     try:
         metadata._get_ourselves_from_working_set()
     except SystemExit:
         sys_exit = True
@@ -187,103 +187,138 @@
 
 
 def test_get_dependencies(minimal_structure):
     path, package_name = minimal_structure
     metadata = PackageMetadata(path)
 
     names = [x.name for x in metadata.get_required_dependencies()]
-    assert 'one' in names
-    assert 'two' in names
+    assert "one" in names
+    assert "two" in names
 
 
 def test_get_no_dependencies(minimal_structure):
     path, package_name = minimal_structure
 
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
     os.remove(requires_file_path)
 
     metadata = PackageMetadata(path)
 
     requirements = list(metadata.get_required_dependencies())
     assert len(requirements) == 0
 
 
 def test_dependencies_with_extras(minimal_structure):
     path, package_name = minimal_structure
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires:
+    with open(requires_file_path, "w") as requires:
         requires.write(
-            '\n'.join(
+            "\n".join(
                 [
-                    'one [with_extra]',
-                    'another[with_extra]',
-                    'yet[one,two,three,extras]',
-                    'something[only, two, with, spaces]',
+                    "one [with_extra]",
+                    "another[with_extra]",
+                    "yet[one,two,three,extras]",
+                    "something[only, two, with, spaces]",
                 ]
             )
         )
 
     metadata = PackageMetadata(path)
     names = [x.name for x in metadata.get_required_dependencies()]
 
     assert len(names) == 4
-    assert 'one' in names
-    assert 'another' in names
-    assert 'yet' in names
-    assert 'something' in names
+    assert "one" in names
+    assert "another" in names
+    assert "yet" in names
+    assert "something" in names
 
 
 def test_dependencies_with_version_specifiers(minimal_structure):
     path, package_name = minimal_structure
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires:
+    with open(requires_file_path, "w") as requires:
         requires.write(
-            '\n'.join(
-                ['one > 8.5', 'another<=3.4', 'yet==5.2', 'something >=2.2.1,<2.3dev']
+            "\n".join(
+                ["one > 8.5", "another<=3.4", "yet==5.2", "something >=2.2.1,<2.3dev"]
             )
         )
 
     metadata = PackageMetadata(path)
     names = [x.name for x in metadata.get_required_dependencies()]
 
     assert len(names) == 4
-    assert 'one' in names
-    assert 'another' in names
-    assert 'yet' in names
+    assert "one" in names
+    assert "another" in names
+    assert "yet" in names
+
+
+def test_dependencies_ignore_zope(minimal_structure):
+    path, package_name = minimal_structure
+    requires_file_path = os.path.join(
+        path,
+        f"{package_name}.egg-info",
+        "requires.txt",
+    )
+    with open(requires_file_path, "w") as requires:
+        requires.write("\n".join(["Zope", "one"]))
+
+    metadata = PackageMetadata(path)
+    names = [x.name for x in metadata.get_required_dependencies()]
+
+    assert len(names) == 1
+    assert "one" in names
 
 
 def test_get_extra_dependencies(minimal_structure):
     path, package_name = minimal_structure
 
     requires_file_path = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'requires.txt',
+        f"{package_name}.egg-info",
+        "requires.txt",
+    )
+    with open(requires_file_path, "w") as requires_file:
+        requires_file.write("\n".join(["one", "", "[test]", "pytest", "mock"]))
+
+    metadata = PackageMetadata(path)
+    extras = list(metadata.get_extras_dependencies())
+    extra_packages = [x.name for x in extras[0][1]]
+    assert len(extras) == 1
+    assert "pytest" in extra_packages
+    assert "mock" in extra_packages
+
+
+def test_get_extra_dependencies_ignore_zope(minimal_structure):
+    path, package_name = minimal_structure
+
+    requires_file_path = os.path.join(
+        path,
+        f"{package_name}.egg-info",
+        "requires.txt",
     )
-    with open(requires_file_path, 'w') as requires_file:
-        requires_file.write('\n'.join(['one', '', '[test]', 'pytest', 'mock']))
+    with open(requires_file_path, "w") as requires_file:
+        requires_file.write("\n".join(["one", "", "[test]", "Zope"]))
 
     metadata = PackageMetadata(path)
     extras = list(metadata.get_extras_dependencies())
     extra_packages = [x.name for x in extras[0][1]]
     assert len(extras) == 1
-    assert 'pytest' in extra_packages
-    assert 'mock' in extra_packages
+    assert "Zope" not in extra_packages
 
 
 def test_no_extras(minimal_structure):
     path, package_name = minimal_structure
 
     metadata = PackageMetadata(path)
 
@@ -296,15 +331,15 @@
     metadata = PackageMetadata(path)
 
     assert metadata.top_level == [os.path.join(path, package_name)]
 
 
 def test_no_top_level_txt_file_found(minimal_structure):
     path, package_name = minimal_structure
-    os.remove(os.path.join(path, f'{package_name}.egg-info', 'top_level.txt'))
+    os.remove(os.path.join(path, f"{package_name}.egg-info", "top_level.txt"))
 
     sys_exit = False
     metadata = PackageMetadata(path)
     try:
         metadata.top_level
     except SystemExit:
         sys_exit = True
@@ -326,39 +361,39 @@
     assert sys_exit
 
 
 def test_top_level_is_module(minimal_structure):
     path, package_name = minimal_structure
     top_level_path = os.path.join(path, package_name)
     os.removedirs(top_level_path)
-    top_level_module_path = f'{top_level_path}.py'
-    with open(top_level_module_path, 'w') as top_level_file:
-        top_level_file.write('Does not matter')
+    top_level_module_path = f"{top_level_path}.py"
+    with open(top_level_module_path, "w") as top_level_file:
+        top_level_file.write("Does not matter")
 
     metadata = PackageMetadata(path)
 
     assert metadata.top_level == [top_level_module_path]
 
 
 def test_top_level_multiple(minimal_structure):
     path, package_name = minimal_structure
     top_level_file = os.path.join(
         path,
-        f'{package_name}.egg-info',
-        'top_level.txt',
+        f"{package_name}.egg-info",
+        "top_level.txt",
     )
-    with open(top_level_file, 'w') as top_level:
-        top_level.write('one\n')
-        top_level.write('two\n')
-        top_level.write('three\n')
+    with open(top_level_file, "w") as top_level:
+        top_level.write("one\n")
+        top_level.write("two\n")
+        top_level.write("three\n")
 
     top_level_folders = [
-        f'{path}/one',
-        f'{path}/two',
-        f'{path}/three',
+        f"{path}/one",
+        f"{path}/two",
+        f"{path}/three",
     ]
     for new_top_level in top_level_folders:
         os.makedirs(new_top_level)
 
     metadata = PackageMetadata(path)
 
     assert metadata.top_level == top_level_folders
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_report.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,621 +6,621 @@
 
 
 def test_print_header_nothing(capsys):
     fake_package = mock.MagicMock()
     report = Report(fake_package)
     report._print_header(None)
     out, err = capsys.readouterr()
-    assert out == ''
+    assert out == ""
 
 
 def test_print_header_text(capsys):
     fake_project = mock.MagicMock()
     report = Report(fake_project)
-    report._print_header('hi')
+    report._print_header("hi")
     out, err = capsys.readouterr()
 
-    assert 'hi' in out
-    assert '==' in out
-    assert '===' not in out
+    assert "hi" in out
+    assert "==" in out
+    assert "===" not in out
 
 
 def test_print_report(capsys, minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
     report = Report(package)
     report.print_report()
     out, err = capsys.readouterr()
-    assert '======' not in out  # there are no errors on the dependencies
-    assert '' == err
+    assert "======" not in out  # there are no errors on the dependencies
+    assert "" == err
 
 
 def test_missing_requirements_nothing(capsys):
     fake_project = mock.MagicMock()
     report = Report(fake_project)
     report.missing_requirements()
     out, err = capsys.readouterr()
-    assert out == ''
+    assert out == ""
 
 
 def test_missing_requirements(capsys, minimal_structure):
     path, package_name = minimal_structure
-    write_source_file_at((path, package_name), '__init__.py', 'import another.package')
+    write_source_file_at((path, package_name), "__init__.py", "import another.package")
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Missing requirements\n====================' in out
-    assert 'another.package' in out
+    assert "Missing requirements\n====================" in out
+    assert "another.package" in out
 
 
 def test_missing_requirements_with_user_mapping(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import Products.Five.browser.views.BrowserView',
+        "__init__.py",
+        "import Products.Five.browser.views.BrowserView",
     )
     write_source_file_at(
-        (path, f'{package_name}.egg-info'),
-        'requires.txt',
-        'Zope2',
+        (path, f"{package_name}.egg-info"),
+        "requires.txt",
+        "Zope2",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(
+        "pyproject.toml",
+        "\n".join(
             [
-                '[tool.dependencychecker]',
+                "[tool.dependencychecker]",
                 'Zope2 = ["Four", "Products.Five", "Three" ]',
             ]
         ),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Missing requirements\n====================' not in out
-    assert 'Products.Five' not in out
-    assert 'Zope2' not in out
+    assert "Missing requirements\n====================" not in out
+    assert "Products.Five" not in out
+    assert "Zope2" not in out
 
 
 def test_missing_requirements_with_ignored_packages(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import Products.Five.browser.views.BrowserView',
+        "__init__.py",
+        "import Products.Five.browser.views.BrowserView",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(
+        "pyproject.toml",
+        "\n".join(
             [
-                '[tool.dependencychecker]',
+                "[tool.dependencychecker]",
                 'ignore-packages = ["Four", "Products.Five", "Three" ]',
             ]
         ),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Missing requirements\n====================' not in out
-    assert 'Products.Five' not in out
-    assert 'Four' not in out
-    assert 'Three' not in out
+    assert "Missing requirements\n====================" not in out
+    assert "Products.Five" not in out
+    assert "Four" not in out
+    assert "Three" not in out
 
 
 def test_missing_test_requirements(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        '',
+        "__init__.py",
+        "",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        'import another.package',
+        (path, package_name, "tests"),
+        "__init__.py",
+        "import another.package",
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_test_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Missing test requirements\n=========================' in out
-    assert 'another.package' in out
+    assert "Missing test requirements\n=========================" in out
+    assert "another.package" in out
 
 
 def test_missing_test_requirements_with_user_mapping(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        '',
+        "__init__.py",
+        "",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        'import Products.Five.browser.views.BrowserView',
+        (path, package_name, "tests"),
+        "__init__.py",
+        "import Products.Five.browser.views.BrowserView",
     )
     write_source_file_at(
-        (path, f'{package_name}.egg-info'),
-        'requires.txt',
-        'Zope2',
+        (path, f"{package_name}.egg-info"),
+        "requires.txt",
+        "Zope2",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', 'Zope2 = ["Products.Five" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", 'Zope2 = ["Products.Five" ]']),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_test_requirements()
     out, err = capsys.readouterr()
 
-    assert '' == out
-    assert 'Missing requirements\n====================' not in out
-    assert 'Products.Five' not in out
-    assert 'Zope2' not in out
+    assert "" == out
+    assert "Missing requirements\n====================" not in out
+    assert "Products.Five" not in out
+    assert "Zope2" not in out
 
 
 def test_missing_test_requirements_with_user_mapping_on_test_extra(
     capsys, minimal_structure
 ):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        '',
+        "__init__.py",
+        "",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        'import Products.Five.browser.views.BrowserView',
+        (path, package_name, "tests"),
+        "__init__.py",
+        "import Products.Five.browser.views.BrowserView",
     )
     write_source_file_at(
-        (path, f'{package_name}.egg-info'),
-        'requires.txt',
-        '\n'.join(['[test]', 'Zope2']),
+        (path, f"{package_name}.egg-info"),
+        "requires.txt",
+        "\n".join(["[test]", "Zope2"]),
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', 'Zope2 = ["Products.Five" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", 'Zope2 = ["Products.Five" ]']),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_test_requirements()
     out, err = capsys.readouterr()
 
-    assert '' == out
-    assert 'Missing requirements\n====================' not in out
-    assert 'Products.Five' not in out
-    assert 'Zope2' not in out
+    assert "" == out
+    assert "Missing requirements\n====================" not in out
+    assert "Products.Five" not in out
+    assert "Zope2" not in out
 
 
 def test_missing_test_requirements_with_ignored_packages(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        '',
+        "__init__.py",
+        "",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        'import Products.Five.browser.views.BrowserView',
+        (path, package_name, "tests"),
+        "__init__.py",
+        "import Products.Five.browser.views.BrowserView",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(
+        "pyproject.toml",
+        "\n".join(
             [
-                '[tool.dependencychecker]',
+                "[tool.dependencychecker]",
                 'ignore-packages = ["Products.Five" ]',
             ]
         ),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.missing_test_requirements()
     out, err = capsys.readouterr()
 
-    assert '' == out
-    assert 'Missing requirements\n====================' not in out
-    assert 'Products.Five' not in out
+    assert "" == out
+    assert "Missing requirements\n====================" not in out
+    assert "Products.Five" not in out
 
 
 def test_unneeded_requirements(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import this.package',
+        "__init__.py",
+        "import this.package",
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded requirements\n=====================' in out
-    assert 'one' in out
-    assert 'two' in out
+    assert "Unneeded requirements\n=====================" in out
+    assert "one" in out
+    assert "two" in out
 
 
 def test_unneeded_requirements_with_ignored_packages(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import this.package',
+        "__init__.py",
+        "import this.package",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(
+        "pyproject.toml",
+        "\n".join(
             [
-                '[tool.dependencychecker]',
+                "[tool.dependencychecker]",
                 'ignore-packages = ["one" ]',
             ]
         ),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded requirements\n=====================' in out
-    assert 'one' not in out
-    assert 'two' in out
+    assert "Unneeded requirements\n=====================" in out
+    assert "one" not in out
+    assert "two" in out
 
 
 def test_unneeded_requirements_with_user_mapping(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'from BTrees import Tree',
+        "__init__.py",
+        "from BTrees import Tree",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', '"ZODB3" = ["BTrees" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", '"ZODB3" = ["BTrees" ]']),
     )
     write_source_file_at(
-        (path, f'{package_name}.egg-info'),
-        'requires.txt',
-        '\n'.join(['ZODB3', 'setuptools', 'one']),
+        (path, f"{package_name}.egg-info"),
+        "requires.txt",
+        "\n".join(["ZODB3", "setuptools", "one"]),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded requirements\n=====================' in out
-    assert 'ZODB3' not in out
-    assert 'one' in out
+    assert "Unneeded requirements\n=====================" in out
+    assert "ZODB3" not in out
+    assert "one" in out
 
 
 def test_unneeded_requirements_with_user_mapping2(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'from Plone import Tree',
+        "__init__.py",
+        "from Plone import Tree",
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', '"ZODB3" = ["BTrees" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", '"ZODB3" = ["BTrees" ]']),
     )
     write_source_file_at(
-        (path, f'{package_name}.egg-info'),
-        'requires.txt',
-        '\n'.join(['ZODB3', 'setuptools', 'one']),
+        (path, f"{package_name}.egg-info"),
+        "requires.txt",
+        "\n".join(["ZODB3", "setuptools", "one"]),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded requirements\n=====================' in out
-    assert 'ZODB3' in out
-    assert 'one' in out
+    assert "Unneeded requirements\n=====================" in out
+    assert "ZODB3" in out
+    assert "one" in out
 
 
 def test_unneeded_test_requirements(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['[test]', 'pytest', 'mock']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["[test]", "pytest", "mock"]),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_test_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded test requirements\n==========================' in out
-    assert 'pytest' in out
-    assert 'mock' in out
+    assert "Unneeded test requirements\n==========================" in out
+    assert "pytest" in out
+    assert "mock" in out
 
 
 def test_unneeded_test_requirements_with_ignore_packages(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['[test]', 'pytest', 'mock']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["[test]", "pytest", "mock"]),
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', 'ignore-packages = ["mock" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", 'ignore-packages = ["mock" ]']),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_test_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded test requirements\n==========================' in out
-    assert 'pytest' in out
-    assert 'mock' not in out
+    assert "Unneeded test requirements\n==========================" in out
+    assert "pytest" in out
+    assert "mock" not in out
 
 
 def test_unneeded_test_requirements_with_user_mappings(capsys, minimal_structure):
     path, package_name = minimal_structure
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['[test]', 'pytest', 'ZODB3']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["[test]", "pytest", "ZODB3"]),
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', '"ZODB3" = ["BTrees" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", '"ZODB3" = ["BTrees" ]']),
     )
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        '',
+        "__init__.py",
+        "",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        'from BTrees import Tree',
+        (path, package_name, "tests"),
+        "__init__.py",
+        "from BTrees import Tree",
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_test_requirements()
     out, err = capsys.readouterr()
 
-    assert 'Unneeded test requirements\n==========================' in out
-    assert 'pytest' in out
-    assert 'ZODB3' not in out
-    assert 'BTrees' not in out
+    assert "Unneeded test requirements\n==========================" in out
+    assert "pytest" in out
+    assert "ZODB3" not in out
+    assert "BTrees" not in out
 
 
 def test_unneeded_test_requirements_no_tests_requirements(
     capsys,
     minimal_structure,
 ):
     path, package_name = minimal_structure
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.unneeded_test_requirements()
     out, err = capsys.readouterr()
 
-    assert '' == out
+    assert "" == out
 
 
 def test_requirements_that_should_be_test_requirements(
     capsys,
     minimal_structure,
 ):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import one',
+        "__init__.py",
+        "import one",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        'import two',
+        (path, package_name, "tests"),
+        "__init__.py",
+        "import two",
     )
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['one', 'two', '[test]', 'pytest', 'mock']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["one", "two", "[test]", "pytest", "mock"]),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.requirements_that_should_be_test_requirements()
     out, err = capsys.readouterr()
 
     assert (
-        'Requirements that should be test requirements\n'
-        '=============================================' in out
+        "Requirements that should be test requirements\n"
+        "=============================================" in out
     )
-    assert 'two' in out
+    assert "two" in out
 
 
 def test_requirements_that_should_be_test_requirements_with_ignored_packages(
     capsys,
     minimal_structure,
 ):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import one',
+        "__init__.py",
+        "import one",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        '\n'.join(['import two', 'import three']),
+        (path, package_name, "tests"),
+        "__init__.py",
+        "\n".join(["import two", "import three"]),
     )
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['one', 'two', 'three', '[test]', 'pytest', 'mock']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["one", "two", "three", "[test]", "pytest", "mock"]),
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', 'ignore-packages = ["two" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", 'ignore-packages = ["two" ]']),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.requirements_that_should_be_test_requirements()
     out, err = capsys.readouterr()
 
     assert (
-        'Requirements that should be test requirements\n'
-        '=============================================' in out
+        "Requirements that should be test requirements\n"
+        "=============================================" in out
     )
-    assert 'three' in out
-    assert 'two' not in out
+    assert "three" in out
+    assert "two" not in out
 
 
 def test_requirements_that_should_be_test_requirements_with_user_mappings(
     capsys,
     minimal_structure,
 ):
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        'import one',
+        "__init__.py",
+        "import one",
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        '\n'.join(['import two', 'import BTrees']),
+        (path, package_name, "tests"),
+        "__init__.py",
+        "\n".join(["import two", "import BTrees"]),
     )
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['one', 'two', 'ZODB3', '[test]', 'pytest', 'mock']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["one", "two", "ZODB3", "[test]", "pytest", "mock"]),
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', '"ZODB3" = ["BTrees" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", '"ZODB3" = ["BTrees" ]']),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.requirements_that_should_be_test_requirements()
     out, err = capsys.readouterr()
 
     assert (
-        'Requirements that should be test requirements\n'
-        '=============================================' in out
+        "Requirements that should be test requirements\n"
+        "=============================================" in out
     )
-    assert 'ZODB3' in out
-    assert 'two' in out
-    assert 'one' not in out
+    assert "ZODB3" in out
+    assert "two" in out
+    assert "one" not in out
 
 
 def test_requirements_that_should_be_test_requirements_with_user_mapping2(
     capsys,
     minimal_structure,
 ):
     """Test that user mappings used in both regular and test imports are
     not downgraded to test imports only.
     """
     path, package_name = minimal_structure
     write_source_file_at(
         (path, package_name),
-        '__init__.py',
-        '\n'.join(['import one', 'import two', 'import part.of.meta']),
+        "__init__.py",
+        "\n".join(["import one", "import two", "import part.of.meta"]),
     )
     write_source_file_at(
-        (path, package_name, 'tests'),
-        '__init__.py',
-        '\n'.join(['import three', 'import four', 'import part.of.meta']),
+        (path, package_name, "tests"),
+        "__init__.py",
+        "\n".join(["import three", "import four", "import part.of.meta"]),
     )
     write_source_file_at(
-        (path, package_name + '.egg-info'),
-        'requires.txt',
-        '\n'.join(['one', 'two', 'three', 'meta-package', '[test]', 'four']),
+        (path, package_name + ".egg-info"),
+        "requires.txt",
+        "\n".join(["one", "two", "three", "meta-package", "[test]", "four"]),
     )
     write_source_file_at(
         (path,),
-        'pyproject.toml',
-        '\n'.join(['[tool.dependencychecker]', 'meta-package = ["part.of.meta" ]']),
+        "pyproject.toml",
+        "\n".join(["[tool.dependencychecker]", 'meta-package = ["part.of.meta" ]']),
     )
 
     package = Package(path)
     package.inspect()
     report = Report(package)
     report.requirements_that_should_be_test_requirements()
     out, err = capsys.readouterr()
 
     assert (
-        'Requirements that should be test requirements\n'
-        '=============================================' in out
+        "Requirements that should be test requirements\n"
+        "=============================================" in out
     )
-    assert 'three' in out
-    assert 'one' not in out
-    assert 'two' not in out
-    assert 'part.of.meta' not in out
-    assert 'meta-package' not in out
+    assert "three" in out
+    assert "one" not in out
+    assert "two" not in out
+    assert "part.of.meta" not in out
+    assert "meta-package" not in out
 
 
 def test_print_notice(capsys, minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
     report = Report(package)
     report.print_notice()
     out, err = capsys.readouterr()
-    assert 'Note: ' in out
-    assert '' == err
+    assert "Note: " in out
+    assert "" == err
 
 
 def test_exit_status_set(minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
     package.inspect()
     report = Report(package)
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/test_user_mappings.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/test_user_mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from z3c.dependencychecker.dotted_name import DottedName
 from z3c.dependencychecker.package import Package
 
-EMPTY_FILE = ''
+EMPTY_FILE = ""
 IGNORE_OTHER_KEYS = """[servers]
 one = "1.2.3.4"
 """
 ONLY_TOOL_TABLE = """[tool]
 two = "5.6.7.8"
 """
 EMPTY_DEPENDENCY_TABLE_NESTED = """[tool]
@@ -33,26 +33,26 @@
 """
 
 
 def _write_user_config(path, content):
     file_path = os.sep.join(
         [
             path,
-            'pyproject.toml',
+            "pyproject.toml",
         ]
     )
-    with open(file_path, 'w') as config_file:
+    with open(file_path, "w") as config_file:
         config_file.write(content)
 
 
 def _update_requires_txt(path, package_name, packages):
-    file_path = os.sep.join([path, f'{package_name}.egg-info', 'requires.txt'])
-    with open(file_path, 'w') as config_file:
+    file_path = os.sep.join([path, f"{package_name}.egg-info", "requires.txt"])
+    with open(file_path, "w") as config_file:
         for package in packages:
-            config_file.write(f'{package}\n')
+            config_file.write(f"{package}\n")
 
 
 def test_no_file(minimal_structure):
     path, package_name = minimal_structure
     package = Package(path)
     package.set_user_mappings()
     assert package.imports.user_mappings == {}
@@ -110,21 +110,21 @@
 def test_one_user_mapping(minimal_structure):
     path, package_name = minimal_structure
     _write_user_config(path, ONE_MAPPING)
     _update_requires_txt(
         path,
         package_name,
         [
-            'Zope2',
+            "Zope2",
         ],
     )
     package = Package(path)
     package.inspect()
-    five_dotted_name = DottedName('Products.Five')
-    zope_dotted_name = DottedName('Zope2')
+    five_dotted_name = DottedName("Products.Five")
+    zope_dotted_name = DottedName("Zope2")
 
     assert len(package.imports.user_mappings) == 1
     assert zope_dotted_name in package.imports.user_mappings
 
     mappings = package.imports.user_mappings[zope_dotted_name]
     assert len(mappings) == 1
     assert {
@@ -134,21 +134,21 @@
 
 def test_filter_out_mappings_on_test(minimal_structure):
     path, package_name = minimal_structure
     _write_user_config(path, ONE_MAPPING)
     _update_requires_txt(
         path,
         package_name,
-        ['plone.reload', '[test]', 'Zope2'],
+        ["plone.reload", "[test]", "Zope2"],
     )
     package = Package(path)
     package.inspect()
-    five_dotted_name = DottedName('Products.Five')
-    plone_reload_dotted_name = DottedName('plone.reload')
-    zope_dotted_name = DottedName('Zope2')
+    five_dotted_name = DottedName("Products.Five")
+    plone_reload_dotted_name = DottedName("plone.reload")
+    zope_dotted_name = DottedName("Zope2")
 
     assert len(package.imports.user_mappings) == 1
     assert zope_dotted_name in package.imports.user_mappings
 
     # The next two aren'd in the mapping, so they shouldn't be filtered out:
     assert package.imports._filter_out_mappings_on_test(plone_reload_dotted_name)
     assert package.imports._filter_out_mappings_on_test(five_dotted_name)
@@ -159,22 +159,22 @@
 def test_more_user_mappings(minimal_structure):
     path, package_name = minimal_structure
     _write_user_config(path, MORE_MAPPINGS)
     _update_requires_txt(
         path,
         package_name,
         [
-            'Zope2',
-            'Zope4',
+            "Zope2",
+            "Zope4",
         ],
     )
     package = Package(path)
     package.inspect()
-    zope2_dotted_name = DottedName('Zope2')
-    zope4_dotted_name = DottedName('Zope4')
+    zope2_dotted_name = DottedName("Zope2")
+    zope4_dotted_name = DottedName("Zope4")
 
     assert len(package.imports.user_mappings) == 2
     assert zope2_dotted_name in package.imports.user_mappings
     assert zope4_dotted_name in package.imports.user_mappings
 
     assert len(package.imports.user_mappings[zope4_dotted_name]) == 2
 
@@ -182,20 +182,20 @@
 def test_subtables(minimal_structure):
     path, package_name = minimal_structure
     _write_user_config(path, SUBTABLES)
     _update_requires_txt(
         path,
         package_name,
         [
-            'Zope2',
+            "Zope2",
         ],
     )
     package = Package(path)
     package.inspect()
-    zope2_dotted_name = DottedName('Zope2')
+    zope2_dotted_name = DottedName("Zope2")
 
     assert len(package.imports.user_mappings) == 1
     assert zope2_dotted_name in package.imports.user_mappings
 
 
 def test_ignore_packages_no_list(minimal_structure):
     path, package_name = minimal_structure
@@ -207,19 +207,19 @@
 
 def test_ignore_packages(minimal_structure):
     path, package_name = minimal_structure
     _write_user_config(path, IGNORE_PACKAGES)
     _update_requires_txt(
         path,
         package_name,
-        ['Zope2', 'plone.reload', 'django-toolbar'],
+        ["Zope2", "plone.reload", "django-toolbar"],
     )
     package = Package(path)
     package.inspect()
-    django_toolbar = DottedName('django-toolbar')
-    plone_reload = DottedName('plone.reload')
+    django_toolbar = DottedName("django-toolbar")
+    plone_reload = DottedName("plone.reload")
     ignored_packages = package.imports.ignored_packages
 
     assert len(package.imports.user_mappings) == 0
     assert len(ignored_packages) == 2
     assert django_toolbar in ignored_packages
     assert plone_reload in ignored_packages
```

### Comparing `z3c.dependencychecker-2.8/z3c/dependencychecker/tests/utils.py` & `z3c.dependencychecker-2.9/z3c/dependencychecker/tests/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os
 
 
 def write_source_file_at(
     path_parts,
-    filename='test.py',
-    source_code='import unknown.dependency',
+    filename="test.py",
+    source_code="import unknown.dependency",
 ):
     folder_path = os.path.join(*path_parts)
 
     try:
         os.makedirs(folder_path)
     except OSError:
         pass
 
     file_path = os.path.join(folder_path, filename)
-    with open(file_path, 'w') as new_file:
+    with open(file_path, "w") as new_file:
         new_file.write(source_code)
 
     return file_path
 
 
 def get_requirements_names(database):
     return [requirement.name for requirement in database._requirements]
 
 
 def get_extras_requirements_names(database):
     return database._extras_requirements.keys()
 
 
-def get_requirements_names_for_extra(database, extra=''):
+def get_requirements_names_for_extra(database, extra=""):
     return [requirement.name for requirement in database._extras_requirements[extra]]
 
 
 def get_sorted_imports_paths(database):
     return sorted([x.file_path for x in database.imports_used])
```

### Comparing `z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/PKG-INFO` & `z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.dependencychecker
-Version: 2.8
+Version: 2.9
 Summary: Reports on missing or unneeded setup.py dependencies
 Home-page: https://github.com/reinout/z3c.dependencychecker
 Author: Reinout van Rees
 Author-email: reinout@vanrees.org
 License: BSD
 Keywords: dependencies requirements missing imports
 Classifier: Development Status :: 5 - Production/Stable
@@ -169,21 +169,18 @@
 
 To run the tests (there's some pytest configuration in ``setup.cfg``)::
 
   $ bin/pytest
 
 Some checks that are run by github actions::
 
-  $ bin/black --skip-string-normalization
+  $ bin/black
   $ bin/codespell setup.py z3c/
   $ bin/flake8 setup.py z3c/
 
-Note that the string quoting style is currently not black-standard, so you'll
-have to manage it yourself.
-
 
 Usage of z3c.dependencychecker
 ==============================
 
 .. :doctest:
 
 
@@ -266,14 +263,20 @@
     setup.py to have effect.
     <BLANKLINE>
 
 
 Changelog of z3c.dependencychecker
 ==================================
 
+2.9 (2023-01-23)
+----------------
+
+- Ignore `Zope` package, as otherwise it swallows all `zope.` namespace packages.
+  [gforcada]
+
 2.8 (2022-11-30)
 ----------------
 
 - Drop python 2.7 support.
   [gforcada]
 
 - Replace travis for GitHub actions.
```

### Comparing `z3c.dependencychecker-2.8/z3c.dependencychecker.egg-info/SOURCES.txt` & `z3c.dependencychecker-2.9/z3c.dependencychecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

