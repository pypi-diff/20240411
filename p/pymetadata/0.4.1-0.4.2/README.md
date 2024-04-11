# Comparing `tmp/pymetadata-0.4.1.tar.gz` & `tmp/pymetadata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetadata-0.4.1.tar", last modified: Thu Feb  1 22:21:20 2024, max compression
+gzip compressed data, was "pymetadata-0.4.2.tar", last modified: Thu Apr 11 10:28:34 2024, max compression
```

## Comparing `pymetadata-0.4.1.tar` & `pymetadata-0.4.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.514973 pymetadata-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-01 22:21:13.000000 pymetadata-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-01 22:21:13.000000 pymetadata-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-02-01 22:21:20.514973 pymetadata-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-01 22:21:13.000000 pymetadata-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-01 22:21:20.514973 pymetadata-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-01 22:21:13.000000 pymetadata-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.498973 pymetadata-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.502973 pymetadata-0.4.1/src/pymetadata/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/chebi.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.506973 pymetadata-0.4.1/src/pymetadata/core/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/core/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/core/synonym.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/core/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.506973 pymetadata-0.4.1/src/pymetadata/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/examples/omex_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.506973 pymetadata-0.4.1/src/pymetadata/identifiers/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/identifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/identifiers/miriam.py
--rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/identifiers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.506973 pymetadata-0.4.1/src/pymetadata/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   662767 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/metadata/eco.py
--rw-r--r--   0 runner    (1001) docker     (127)    88999 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/metadata/kisao.py
--rw-r--r--   0 runner    (1001) docker     (127)   141756 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/metadata/sbo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29867 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/omex.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/omex_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.506973 pymetadata-0.4.1/src/pymetadata/ontologies/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/ontologies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/ontologies/ols.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/ontologies/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.506973 pymetadata-0.4.1/src/pymetadata/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/resources/chebi_webservice_wsdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)  2086194 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/resources/identifiers_registry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.510973 pymetadata-0.4.1/src/pymetadata/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/resources/templates/ontology_enum.pytemplate
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-02-01 22:21:13.000000 pymetadata-0.4.1/src/pymetadata/unichem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.510973 pymetadata-0.4.1/src/pymetadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-02-01 22:21:20.000000 pymetadata-0.4.1/src/pymetadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-01 22:21:20.000000 pymetadata-0.4.1/src/pymetadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:21:20.000000 pymetadata-0.4.1/src/pymetadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-01 22:21:20.000000 pymetadata-0.4.1/src/pymetadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-01 22:21:20.000000 pymetadata-0.4.1/src/pymetadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:21:20.000000 pymetadata-0.4.1/src/pymetadata.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:21:20.510973 pymetadata-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_chebi.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_ols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_omex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_sbo_kisao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-01 22:21:13.000000 pymetadata-0.4.1/tests/test_unichem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.189374 pymetadata-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-11 10:28:26.000000 pymetadata-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-11 10:28:26.000000 pymetadata-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-11 10:28:34.189374 pymetadata-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-11 10:28:26.000000 pymetadata-0.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-11 10:28:34.189374 pymetadata-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-11 10:28:26.000000 pymetadata-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.173374 pymetadata-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.177374 pymetadata-0.4.2/src/pymetadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/chebi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.177374 pymetadata-0.4.2/src/pymetadata/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/core/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/core/synonym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/core/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.181374 pymetadata-0.4.2/src/pymetadata/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/examples/omex_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.181374 pymetadata-0.4.2/src/pymetadata/identifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/identifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/identifiers/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/identifiers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.181374 pymetadata-0.4.2/src/pymetadata/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   662767 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/metadata/eco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89273 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/metadata/kisao.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141756 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/metadata/sbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29867 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/omex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/omex_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.181374 pymetadata-0.4.2/src/pymetadata/ontologies/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/ontologies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/ontologies/ols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/ontologies/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.181374 pymetadata-0.4.2/src/pymetadata/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/resources/chebi_webservice_wsdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  2097405 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/resources/identifiers_registry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.185374 pymetadata-0.4.2/src/pymetadata/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/resources/templates/ontology_enum.pytemplate
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-11 10:28:26.000000 pymetadata-0.4.2/src/pymetadata/unichem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.185374 pymetadata-0.4.2/src/pymetadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-11 10:28:34.000000 pymetadata-0.4.2/src/pymetadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-11 10:28:34.000000 pymetadata-0.4.2/src/pymetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:28:34.000000 pymetadata-0.4.2/src/pymetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-11 10:28:34.000000 pymetadata-0.4.2/src/pymetadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 10:28:34.000000 pymetadata-0.4.2/src/pymetadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:28:34.000000 pymetadata-0.4.2/src/pymetadata.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:28:34.185374 pymetadata-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_chebi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_ols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_omex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_sbo_kisao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-11 10:28:26.000000 pymetadata-0.4.2/tests/test_unichem.py
```

### Comparing `pymetadata-0.4.1/LICENSE` & `pymetadata-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/PKG-INFO` & `pymetadata-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetadata
-Version: 0.4.1
+Version: 0.4.2
 Summary: pymetadata are python utilities for working with metadata.
 Home-page: https://github.com/matthiaskoenig/pymetadata
 Download-URL: https://pypi.org/project/pymetadata
 Author: Matthias Koenig
 Author-email: konigmatt@googlemail.com
 Maintainer: Matthias Koenig
 Maintainer-email: konigmatt@googlemail.com
@@ -24,72 +24,63 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: depinfo>=1.7
-Requires-Dist: uuid>=1.30
-Requires-Dist: lxml>=4.9
-Requires-Dist: rich>=13.6
+Requires-Dist: lxml>=5.2
+Requires-Dist: rich>=13.7
 Requires-Dist: requests>=2.31
 Requires-Dist: zeep>=4.2.1
-Requires-Dist: pronto>=2.5.5
-Requires-Dist: fastobo>=0.12.2
-Requires-Dist: jinja2>=3.1.2
+Requires-Dist: pronto>=2.5.6
+Requires-Dist: fastobo>=0.12.3
+Requires-Dist: jinja2>=3.1
 Requires-Dist: xmltodict>=0.13.0
-Requires-Dist: pydantic>=2.4
+Requires-Dist: pydantic>=2.6
 Provides-Extra: development
-Requires-Dist: pip-tools>6.10; extra == "development"
-Requires-Dist: black>=24.1.1; extra == "development"
+Requires-Dist: pip-tools>=7.4.1; extra == "development"
+Requires-Dist: black>=24.3.0; extra == "development"
 Requires-Dist: bump2version>=1.0.1; extra == "development"
 Requires-Dist: isort>=5.13.2; extra == "development"
-Requires-Dist: tox>=4.12.1; extra == "development"
-Requires-Dist: flake8>=6.1.0; extra == "development"
+Requires-Dist: tox>=4.12.2; extra == "development"
+Requires-Dist: flake8>=7.0.0; extra == "development"
 Requires-Dist: flake8-mypy>=17.8.0; extra == "development"
-Requires-Dist: mypy>=1.8.0; extra == "development"
-Requires-Dist: pytest>=8.0.0; extra == "development"
-Requires-Dist: pytest-cov>=4.1.0; extra == "development"
+Requires-Dist: mypy>=1.9.0; extra == "development"
+Requires-Dist: pytest>=8.1.1; extra == "development"
+Requires-Dist: pytest-cov>=5.0.0; extra == "development"
 
 .. image:: https://github.com/matthiaskoenig/pymetadata/raw/develop/docs/images/favicon/pymetadata-100x100-300dpi.png
    :align: left
    :alt: pymetadata logo
 
 pymetadata: python utilities for metadata and COMBINE archives
 ==============================================================
+|icon1| |icon2| |icon3| |icon4| |icon5| |icon6| |icon7|
 
-.. image:: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD/badge.svg
+
+.. |icon1| image:: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD/badge.svg
    :target: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD
    :alt: GitHub Actions CI/CD Status
-
-.. image:: https://img.shields.io/pypi/v/pymetadata.svg
+.. |icon2| image:: https://img.shields.io/pypi/v/pymetadata.svg
    :target: https://pypi.org/project/pymetadata/
    :alt: Current PyPI Version
-
-.. image:: https://img.shields.io/pypi/pyversions/pymetadata.svg
+.. |icon3| image:: https://img.shields.io/pypi/pyversions/pymetadata.svg
    :target: https://pypi.org/project/pymetadata/
    :alt: Supported Python Versions
-
-.. image:: https://img.shields.io/pypi/l/pymetadata.svg
+.. |icon4| image:: https://img.shields.io/pypi/l/pymetadata.svg
    :target: http://opensource.org/licenses/LGPL-3.0
    :alt: GNU Lesser General Public License 3
-
-.. image:: https://codecov.io/gh/matthiaskoenig/pymetadata/branch/develop/graph/badge.svg
-   :target: https://codecov.io/gh/matthiaskoenig/pymetadata
-   :alt: Codecov
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5308801.svg
+.. |icon5| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5308801.svg
    :target: https://doi.org/10.5281/zenodo.5308801
    :alt: Zenodo DOI
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |icon6| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
    :alt: Black
-
-.. image:: http://www.mypy-lang.org/static/mypy_badge.svg
+.. |icon7| image:: http://www.mypy-lang.org/static/mypy_badge.svg
    :target: http://mypy-lang.org/
    :alt: mypy
 
 pymetadata is a collection of python utilities for working with
 metadata in the context of COMBINE standards with source code available from 
 `https://github.com/matthiaskoenig/pymetadata <https://github.com/matthiaskoenig/pymetadata>`__.
 
@@ -136,19 +127,19 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 Funding
 =======
-Matthias König is supported by the Federal Ministry of Education and Research (BMBF, Germany)
+Matthias König was supported by the Federal Ministry of Education and Research (BMBF, Germany)
 within the research network Systems Medicine of the Liver (**LiSyM**, grant number 031L0054) 
-and by the German Research Foundation (DFG) within the Research Unit Programme FOR 5151 
+and is supported by the German Research Foundation (DFG) within the Research Unit Programme FOR 5151 
 "`QuaLiPerF <https://qualiperf.de>`__ (Quantifying Liver Perfusion-Function Relationship in Complex Resection - 
-A Systems Medicine Approach)" by grant number 436883643 and by grant number 465194077 (Priority Programme SPP 2311, Subproject SimLivA).
+A Systems Medicine Approach)" by grant number 436883643 and by grant number 465194077 (Priority Programme SPP 2311, Subproject SimLivA), and 
 
 Installation
 ============
 `pymetadata` is available from `pypi <https://pypi.python.org/pypi/pymetadata>`__ and 
 can be installed via:: 
 
     pip install pymetadata
@@ -165,8 +156,8 @@
     cd pymetadata
     pip install -e .
 
 To install for development use::
 
     pip install -e .[development]
 
-© 2021-2022 Matthias König
+© 2021-2024 Matthias König
```

### Comparing `pymetadata-0.4.1/README.rst` & `pymetadata-0.4.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 .. image:: https://github.com/matthiaskoenig/pymetadata/raw/develop/docs/images/favicon/pymetadata-100x100-300dpi.png
    :align: left
    :alt: pymetadata logo
 
 pymetadata: python utilities for metadata and COMBINE archives
 ==============================================================
+|icon1| |icon2| |icon3| |icon4| |icon5| |icon6| |icon7|
 
-.. image:: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD/badge.svg
+
+.. |icon1| image:: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD/badge.svg
    :target: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD
    :alt: GitHub Actions CI/CD Status
-
-.. image:: https://img.shields.io/pypi/v/pymetadata.svg
+.. |icon2| image:: https://img.shields.io/pypi/v/pymetadata.svg
    :target: https://pypi.org/project/pymetadata/
    :alt: Current PyPI Version
-
-.. image:: https://img.shields.io/pypi/pyversions/pymetadata.svg
+.. |icon3| image:: https://img.shields.io/pypi/pyversions/pymetadata.svg
    :target: https://pypi.org/project/pymetadata/
    :alt: Supported Python Versions
-
-.. image:: https://img.shields.io/pypi/l/pymetadata.svg
+.. |icon4| image:: https://img.shields.io/pypi/l/pymetadata.svg
    :target: http://opensource.org/licenses/LGPL-3.0
    :alt: GNU Lesser General Public License 3
-
-.. image:: https://codecov.io/gh/matthiaskoenig/pymetadata/branch/develop/graph/badge.svg
-   :target: https://codecov.io/gh/matthiaskoenig/pymetadata
-   :alt: Codecov
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5308801.svg
+.. |icon5| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5308801.svg
    :target: https://doi.org/10.5281/zenodo.5308801
    :alt: Zenodo DOI
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |icon6| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
    :alt: Black
-
-.. image:: http://www.mypy-lang.org/static/mypy_badge.svg
+.. |icon7| image:: http://www.mypy-lang.org/static/mypy_badge.svg
    :target: http://mypy-lang.org/
    :alt: mypy
 
 pymetadata is a collection of python utilities for working with
 metadata in the context of COMBINE standards with source code available from 
 `https://github.com/matthiaskoenig/pymetadata <https://github.com/matthiaskoenig/pymetadata>`__.
 
@@ -84,19 +76,19 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 Funding
 =======
-Matthias König is supported by the Federal Ministry of Education and Research (BMBF, Germany)
+Matthias König was supported by the Federal Ministry of Education and Research (BMBF, Germany)
 within the research network Systems Medicine of the Liver (**LiSyM**, grant number 031L0054) 
-and by the German Research Foundation (DFG) within the Research Unit Programme FOR 5151 
+and is supported by the German Research Foundation (DFG) within the Research Unit Programme FOR 5151 
 "`QuaLiPerF <https://qualiperf.de>`__ (Quantifying Liver Perfusion-Function Relationship in Complex Resection - 
-A Systems Medicine Approach)" by grant number 436883643 and by grant number 465194077 (Priority Programme SPP 2311, Subproject SimLivA).
+A Systems Medicine Approach)" by grant number 436883643 and by grant number 465194077 (Priority Programme SPP 2311, Subproject SimLivA), and 
 
 Installation
 ============
 `pymetadata` is available from `pypi <https://pypi.python.org/pypi/pymetadata>`__ and 
 can be installed via:: 
 
     pip install pymetadata
@@ -113,8 +105,8 @@
     cd pymetadata
     pip install -e .
 
 To install for development use::
 
     pip install -e .[development]
 
-© 2021-2022 Matthias König
+© 2021-2024 Matthias König
```

### Comparing `pymetadata-0.4.1/setup.cfg` & `pymetadata-0.4.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.1
+current_version = 0.4.2
 commit = True
 tag = True
 parse = (?P<major>\d+)
 	\.(?P<minor>\d+)
 	\.(?P<patch>\d+)
 	(?P<release>[a]*)(?P<num>\d*)
 serialize = 
@@ -48,27 +48,26 @@
 	annotation
 
 [options]
 zip_safe = True
 python_requires = >=3.9
 install_requires = 
 	depinfo>=1.7
-	uuid>=1.30
-	lxml>=4.9
-	rich>=13.6
+	lxml>=5.2
+	rich>=13.7
 	requests>=2.31
 	zeep>=4.2.1
-	pronto>=2.5.5
-	fastobo>=0.12.2
-	jinja2>=3.1.2
+	pronto>=2.5.6
+	fastobo>=0.12.3
+	jinja2>=3.1
 	xmltodict>=0.13.0
-	pydantic>=2.4
+	pydantic>=2.6
 tests_require = 
-	tox>=3.27
-	pytest
+	tox>=4.14.2
+	pytest>=8.1.1
 packages = find:
 package_dir = 
 	= src
 include_package_data = True
 
 [options.package_data]
 pymetadata = py.typed
@@ -77,24 +76,24 @@
 test = pytest
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 development = 
-	pip-tools>6.10
-	black>=24.1.1
+	pip-tools>=7.4.1
+	black>=24.3.0
 	bump2version>=1.0.1
 	isort>=5.13.2
-	tox>=4.12.1
-	flake8>=6.1.0
+	tox>=4.12.2
+	flake8>=7.0.0
 	flake8-mypy>=17.8.0
-	mypy>=1.8.0
-	pytest>=8.0.0
-	pytest-cov>=4.1.0
+	mypy>=1.9.0
+	pytest>=8.1.1
+	pytest-cov>=5.0.0
 
 [bdist_wheel]
 universal = 1
 
 [bumpversion:part:release]
 optional_value = placeholder
 first_value = placeholder
```

### Comparing `pymetadata-0.4.1/src/pymetadata/cache.py` & `pymetadata-0.4.2/src/pymetadata/cache.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/chebi.py` & `pymetadata-0.4.2/src/pymetadata/chebi.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/core/annotation.py` & `pymetadata-0.4.2/src/pymetadata/core/annotation.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/core/creator.py` & `pymetadata-0.4.2/src/pymetadata/core/creator.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/core/xref.py` & `pymetadata-0.4.2/src/pymetadata/core/xref.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/examples/omex_example.py` & `pymetadata-0.4.2/src/pymetadata/examples/omex_example.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/identifiers/miriam.py` & `pymetadata-0.4.2/src/pymetadata/identifiers/miriam.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/identifiers/registry.py` & `pymetadata-0.4.2/src/pymetadata/identifiers/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -185,26 +185,14 @@
             pattern=r"^MONDO:\d+$",
             name="MONDO",
             description="MONDO",
             namespaceEmbeddedInLui=True,
         ),
         Namespace(
             id=None,
-            prefix="stato",
-            pattern=r"^STATO:\d+$",
-            name="STATO",
-            description="STATO is the statistical methods ontology. It contains "
-            "concepts and properties related to statistical methods, "
-            "probability distributions and other concepts related to "
-            "statistical analysis, including relationships to study "
-            "designs and plots.",
-            namespaceEmbeddedInLui=True,
-        ),
-        Namespace(
-            id=None,
             prefix="atol",
             pattern=r"^ATOL:\d+$",
             name="ATOL",
             description="Animal Trait Ontology for Livestock",
             namespaceEmbeddedInLui=True,
         ),
         Namespace(
@@ -345,15 +333,15 @@
 
     @staticmethod
     def update_registry(
         custom_namespaces: Dict[str, Namespace] = CUSTOM_NAMESPACES,
         registry_path: Optional[Path] = None,
     ) -> Dict[str, Namespace]:
         """Update registry from identifiers.org webservice."""
-        logger.warning(f"Update registry: '{Registry.URL}' -> '{registry_path}'")
+        logger.info(f"Update registry from '{Registry.URL}'")
         response = requests.get(Registry.URL)
         namespaces = response.json()["payload"]["namespaces"]
 
         ns_dict = {}
         for _, data in enumerate(namespaces):
             ns = Namespace.from_dict(data)
 
@@ -370,17 +358,14 @@
                         resource.resourceHomeUrl = resource.resourceHomeUrl.replace(
                             "/ols/", "/ols4/"
                         )
 
             ns_dict[ns.prefix] = ns
 
         if custom_namespaces is not None:
-            logger.warning(
-                f"Adding custom namespaces: {sorted(custom_namespaces.keys())}"
-            )
             for key, ns in custom_namespaces.items():
                 if key in ns_dict:
                     logger.error(
                         f"Namespace with key '{key}' exists in MIRIAM. Overwrite namespace!"
                     )
                 ns_dict[key] = ns
```

### Comparing `pymetadata-0.4.1/src/pymetadata/log.py` & `pymetadata-0.4.2/src/pymetadata/log.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/metadata/eco.py` & `pymetadata-0.4.2/src/pymetadata/metadata/eco.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/metadata/kisao.py` & `pymetadata-0.4.2/src/pymetadata/metadata/kisao.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,14 +477,16 @@
     "KISAO_0000691": "metabolic system",
     "KISAO_0000692": "cellular system",
     "KISAO_0000693": "biochemical system",
     "KISAO_0000694": "ODE solver",
     "KISAO_0000695": "parameters for",
     "KISAO_0000696": "steady state root-finding problem",
     "KISAO_0000697": "SDE solver",
+    "KISAO_0000698": "particle coordinates",
+    "KISAO_0000699": "DAE Solver",
     "KISAO_0000800": "systems property",
     "KISAO_0000801": "concentration control coefficient matrix (unscaled)",
     "KISAO_0000802": "control coefficient (scaled)",
     "KISAO_0000803": "control coefficient (unscaled)",
     "KISAO_0000804": "elasticity matrix (unscaled)",
     "KISAO_0000805": "elasticity coefficient (unscaled)",
     "KISAO_0000806": "elasticity matrix (scaled)",
@@ -2451,14 +2453,22 @@
     KISAO_0000696 = "KISAO_0000696"
     STEADY_STATE_ROOT_FINDING_PROBLEM = "KISAO_0000696"
 
     # SDE solver
     KISAO_0000697 = "KISAO_0000697"
     SDE_SOLVER = "KISAO_0000697"
 
+    # particle coordinates
+    KISAO_0000698 = "KISAO_0000698"
+    PARTICLE_COORDINATES = "KISAO_0000698"
+
+    # DAE Solver
+    KISAO_0000699 = "KISAO_0000699"
+    DAE_SOLVER = "KISAO_0000699"
+
     # systems property
     KISAO_0000800 = "KISAO_0000800"
     SYSTEMS_PROPERTY = "KISAO_0000800"
 
     # concentration control coefficient matrix (unscaled)
     KISAO_0000801 = "KISAO_0000801"
     CONCENTRATION_CONTROL_COEFFICIENT_MATRIX__UNSCALED_ = "KISAO_0000801"
```

### Comparing `pymetadata-0.4.1/src/pymetadata/metadata/sbo.py` & `pymetadata-0.4.2/src/pymetadata/metadata/sbo.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/omex.py` & `pymetadata-0.4.2/src/pymetadata/omex.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 logger = log.get_logger(__name__)
 
 
 __all__ = ["EntryFormat", "ManifestEntry", "Manifest", "Omex"]
 
 
-IDENTIFIERS_PREFIX = "http://identifiers.org/combine.specifications:"
+IDENTIFIERS_PREFIX = "http://identifiers.org/combine.specifications/"
 PURL_PREFIX = "https://purl.org/NET/mediatypes/"
 
 
 class EntryFormat(str, Enum):
     """Enum for common formats."""
 
     OMEX = IDENTIFIERS_PREFIX + "omex"
```

### Comparing `pymetadata-0.4.1/src/pymetadata/omex_v2.py` & `pymetadata-0.4.2/src/pymetadata/omex_v2.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/ontologies/ols.py` & `pymetadata-0.4.2/src/pymetadata/ontologies/ols.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,21 +76,21 @@
     def __init__(
         self,
         ontologies: List[OLSOntology],
         cache_path: Path = CACHE_PATH,
         cache: bool = CACHE_USE,
     ):
         """Initialize OLSQuery."""
-        self.ontologies = {
+        self.ontologies: Dict[str, OLSOntology] = {
             ontology.name: ontology for ontology in ontologies
-        }  # type: Dict[str, OLSOntology]
+        }
         self.cache_path = cache_path / "ols"
         self.cache = cache
 
-        if not self.cache_path.exists():
+        if cache and not self.cache_path.exists():
             self.cache_path.mkdir(parents=True)
 
     def get_iri(self, ontology: str, term: str) -> str:
         """Get IRI information."""
         ols_ontology: Optional[OLSOntology] = self.ontologies.get(ontology, None)
         # remove prefix if existing
         if term.startswith(ontology.upper()):
@@ -133,19 +133,14 @@
             ontology = "ncbitaxon"
 
         iri = self.get_iri(ontology=ontology, term=term)
 
         # double urlencode iri for OLS
         urliri = urllib.parse.quote(iri, safe="")
         urliri = urllib.parse.quote(urliri, safe="")
-        # urliri = iri.replace(":", "%253A")
-        # urliri = urliri.replace("/", "%252F")
-
-        # term_id = term.split(":")[-1]
-        # url = ols_pattern.replace('{$id}', term_id)
         cache_path = self.cache_path / f"{urliri}.json"
         data: Dict[str, Any] = {}
         if self.cache:
             try:
                 data = read_json_cache(cache_path=cache_path)
             except IOError:
                 # cache does not exist
@@ -173,15 +168,16 @@
                         "errors": [error_msg],
                         "warnings": [],
                     }
                     return data
                 else:
                     data["errors"] = []
                     data["warnings"] = []
-                    write_json_cache(data=data, cache_path=cache_path)  # type: ignore
+                    if self.cache:
+                        write_json_cache(data=data, cache_path=cache_path)  # type: ignore
 
         return data
 
     def process_response(self, term: Dict) -> Dict[str, Any]:
         """Process the response dictionary."""
         data = {
             "errors": term["errors"],
```

### Comparing `pymetadata-0.4.1/src/pymetadata/ontologies/ontology.py` & `pymetadata-0.4.2/src/pymetadata/ontologies/ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     """Try import of created module."""
     # try to import
     importlib.import_module(f"pymetadata.metadata.{ontology_id.lower()}")
 
 
 if __name__ == "__main__":
     # download latest versions
-    # update_ontology_files()
+    update_ontology_files()
 
     # test loading of OWL files
     # ofile: OntologyFile
     # for oid, ofile in ontology_files.items():
     #     console.rule(style="white")
     #     ontology = Ontology(ontology_id=oid)
     #     console.print(ontology)
```

### Comparing `pymetadata-0.4.1/src/pymetadata/resources/chebi_webservice_wsdl.xml` & `pymetadata-0.4.2/src/pymetadata/resources/chebi_webservice_wsdl.xml`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/resources/identifiers_registry.json` & `pymetadata-0.4.2/src/pymetadata/resources/identifiers_registry.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937483716256094%*

 * *Differences: {"'3dmet'": "{'modified': '2024-02-12T09:37:02.753+0000', 'deprecated': True, 'deprecationDate': "*

 * *            "'2024-02-12T09:35:45.473+0000'}",*

 * * "'cheminf'": "OrderedDict([('id', 3819), ('prefix', 'cheminf'), ('name', 'Chemical Information "*

 * *              "Ontology'), ('pattern', '^CHEMINF:\\\\d+$'), ('namespaceEmbeddedInLui', True), "*

 * *              "('description', 'The chemical information ontology (cheminf) describes information "*

 * *              'entities about chemical entities. It provides qualitative […]*

```diff
@@ -1,16 +1,16 @@
 {
     "3dmet": {
         "created": "2019-06-11T14:15:50.652+0000",
-        "deprecated": false,
-        "deprecationDate": null,
+        "deprecated": true,
+        "deprecationDate": "2024-02-12T09:35:45.473+0000",
         "description": "3DMET is a database collecting three-dimensional structures of natural metabolites.",
         "id": 230,
         "mirId": "MIR:00000066",
-        "modified": "2019-06-11T14:15:50.652+0000",
+        "modified": "2024-02-12T09:37:02.753+0000",
         "name": "3DMET",
         "namespaceEmbeddedInLui": false,
         "pattern": "^B\\d{5}$",
         "prefix": "3dmet",
         "resources": [
             {
                 "authHelpDescription": null,
@@ -6410,14 +6410,62 @@
                 "resourceHomeUrl": "https://chem.nlm.nih.gov/chemidplus/chemidheavy.jsp",
                 "sampleId": "57-27-2",
                 "urlPattern": "https://chem.nlm.nih.gov/chemidplus/rn/{$id}"
             }
         ],
         "sampleId": "57-27-2"
     },
+    "cheminf": {
+        "created": "2024-03-20T10:24:50.346+0000",
+        "deprecated": false,
+        "deprecationDate": null,
+        "description": "The chemical information ontology (cheminf) describes information entities about chemical entities. It provides qualitative and quantitative attributes to richly describe chemicals.",
+        "id": 3819,
+        "mirId": "MIR:00001045",
+        "modified": "2024-03-20T10:29:26.220+0000",
+        "name": "Chemical Information Ontology",
+        "namespaceEmbeddedInLui": true,
+        "pattern": "^CHEMINF:\\d+$",
+        "prefix": "cheminf",
+        "resources": [
+            {
+                "authHelpDescription": null,
+                "authHelpUrl": null,
+                "deprecated": false,
+                "deprecationDate": null,
+                "description": "The chemical information ontology (cheminf) describes information entities about chemical entities. It provides qualitative and quantitative attributes to richly describe chemicals.",
+                "id": 3820,
+                "institution": {
+                    "description": "At EMBL-EBI, we make the world\u2019s public biological data freely available to the scientific community via a range of services and tools, perform basic research and provide professional training in bioinformatics. \nWe are part of the European Molecular Biology Laboratory (EMBL), an international, innovative and interdisciplinary research organisation funded by 26 member states and two associate member states.",
+                    "homeUrl": "https://www.ebi.ac.uk",
+                    "id": 2,
+                    "location": {
+                        "countryCode": "GB",
+                        "countryName": "United Kingdom"
+                    },
+                    "name": "European Bioinformatics Institute",
+                    "rorId": "https://ror.org/02catss52"
+                },
+                "location": {
+                    "countryCode": "GB",
+                    "countryName": "United Kingdom"
+                },
+                "mirId": "MIR:00001044",
+                "name": "CHEMINF via OLS",
+                "official": true,
+                "protectedUrls": false,
+                "providerCode": "ols",
+                "renderProtectedLanding": false,
+                "resourceHomeUrl": "https://www.ebi.ac.uk/ols4/ontologies/cheminf",
+                "sampleId": "000306",
+                "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/cheminf/classes?obo_id=CHEMINF:{$id}"
+            }
+        ],
+        "sampleId": "000306"
+    },
     "chemspider": {
         "created": "2019-06-11T14:16:10.254+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "ChemSpider is a collection of compound data from across the web, which aggregates chemical structures and their associated information into a single searchable repository entry. These entries are supplemented with additional properties, related information and links back to original data sources.",
         "id": 438,
         "mirId": "MIR:00000138",
@@ -9539,15 +9587,15 @@
                 },
                 "mirId": "MIR:00100803",
                 "name": "dbGaP through NCBI",
                 "official": true,
                 "protectedUrls": false,
                 "providerCode": "ncbi",
                 "renderProtectedLanding": false,
-                "resourceHomeUrl": "https://www.ncbi.nlm.nih.gov/projects/gap",
+                "resourceHomeUrl": "https://www.ncbi.nlm.nih.gov/gap/",
                 "sampleId": "phs000768.v2.p1",
                 "urlPattern": "https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id={$id}"
             }
         ],
         "sampleId": "phs000768.v2.p1"
     },
     "dbprobe": {
@@ -12817,15 +12865,15 @@
     "edam": {
         "created": "2019-06-11T14:16:22.318+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "EDAM is an ontology of general bioinformatics concepts, including topics, data types, formats, identifiers and operations. EDAM provides a controlled vocabulary for the description, in semantic terms, of things such as: web services (e.g. WSDL files), applications, tool collections and packages, work-benches and workflow software, databases and ontologies, XSD data schema and data objects, data syntax and file formats, web portals and pages, resource catalogues and documents (such as scientific publications).",
         "id": 575,
         "mirId": "MIR:00000189",
-        "modified": "2019-06-11T14:16:22.318+0000",
+        "modified": "2024-03-20T11:53:50.927+0000",
         "name": "EDAM Ontology",
         "namespaceEmbeddedInLui": false,
         "pattern": "^(data|topic|operation|format)\\_\\d{4}$",
         "prefix": "edam",
         "resources": [
             {
                 "authHelpDescription": null,
@@ -19061,15 +19109,15 @@
                 "name": "HGNC Symbol at HUGO Genome Nomenclature Committee",
                 "official": false,
                 "protectedUrls": false,
                 "providerCode": "ebi",
                 "renderProtectedLanding": false,
                 "resourceHomeUrl": "https://www.genenames.org/",
                 "sampleId": "DAPK1",
-                "urlPattern": "https://www.genenames.org/cgi-bin/gene_symbol_report?match={$id}"
+                "urlPattern": "https://www.genenames.org/data/gene-symbol-report/#!/symbol/{$id}"
             }
         ],
         "sampleId": "DAPK1"
     },
     "hinv.locus": {
         "created": "2019-06-11T14:16:17.382+0000",
         "deprecated": false,
@@ -20101,15 +20149,15 @@
                 "name": "International Statistical Classification of Diseases and Related Health Problems",
                 "official": false,
                 "protectedUrls": false,
                 "providerCode": "CURATOR_REVIEW",
                 "renderProtectedLanding": false,
                 "resourceHomeUrl": "http://www.who.int/classifications/icd/en/",
                 "sampleId": "C34",
-                "urlPattern": "http://apps.who.int/classifications/icd10/browse/2010/en#/{$id}"
+                "urlPattern": "https://icd.who.int/browse10/2019/en#/{$id}"
             }
         ],
         "sampleId": "C34"
     },
     "icdc": {
         "created": "2021-05-10T19:40:34.200+0000",
         "deprecated": false,
@@ -25018,14 +25066,62 @@
                 "resourceHomeUrl": "https://www.ebi.ac.uk/ols4/ontologies/maxo",
                 "sampleId": "0001073",
                 "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/maxo/terms?obo_id=MAXO:{$id}"
             }
         ],
         "sampleId": "0001073"
     },
+    "mcro": {
+        "created": "2024-03-20T10:56:06.644+0000",
+        "deprecated": false,
+        "deprecationDate": null,
+        "description": "An ontology representing the model card structure, he aim of this work is to describe machine learning models to communicate information about specific details about the model (trade offs, intended users, licensing, etc.). ",
+        "id": 3832,
+        "mirId": "MIR:00001049",
+        "modified": "2024-03-20T10:56:06.644+0000",
+        "name": "Model Card Ontology",
+        "namespaceEmbeddedInLui": true,
+        "pattern": "^MCRO:\\d+$",
+        "prefix": "mcro",
+        "resources": [
+            {
+                "authHelpDescription": null,
+                "authHelpUrl": null,
+                "deprecated": false,
+                "deprecationDate": null,
+                "description": "ontology modeling the model card report for machine learning model assests",
+                "id": 3833,
+                "institution": {
+                    "description": "At EMBL-EBI, we make the world\u2019s public biological data freely available to the scientific community via a range of services and tools, perform basic research and provide professional training in bioinformatics. \nWe are part of the European Molecular Biology Laboratory (EMBL), an international, innovative and interdisciplinary research organisation funded by 26 member states and two associate member states.",
+                    "homeUrl": "https://www.ebi.ac.uk",
+                    "id": 2,
+                    "location": {
+                        "countryCode": "GB",
+                        "countryName": "United Kingdom"
+                    },
+                    "name": "European Bioinformatics Institute",
+                    "rorId": "https://ror.org/02catss52"
+                },
+                "location": {
+                    "countryCode": "GB",
+                    "countryName": "United Kingdom"
+                },
+                "mirId": "MIR:00001048",
+                "name": "MCRO via OLS",
+                "official": true,
+                "protectedUrls": false,
+                "providerCode": "ols",
+                "renderProtectedLanding": false,
+                "resourceHomeUrl": "https://www.ebi.ac.uk/ols4/ontologies/mcro",
+                "sampleId": "0000027",
+                "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/mcro/classes?obo_id=MCRO:{$id}"
+            }
+        ],
+        "sampleId": "0000027"
+    },
     "mdm": {
         "created": "2019-06-11T14:17:52.138+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "The MDM (Medical Data Models) Portal is a meta-data registry for creating, analysing, sharing and reusing medical forms. Electronic forms are central in numerous processes involving data, including the collection of data through electronic health records (EHRs), Electronic Data Capture (EDC), and as case report forms (CRFs) for clinical trials. The MDM Portal provides medical forms in numerous export formats, facilitating the sharing and reuse of medical data models and exchange between information systems.",
         "id": 1598,
         "mirId": "MIR:00000574",
@@ -26960,15 +27056,15 @@
     "miriam.collection": {
         "created": "2019-06-11T14:15:31.442+0000",
         "deprecated": true,
         "deprecationDate": "2020-06-04T11:17:21.453+0000",
         "description": "MIRIAM Registry is an online resource created to catalogue collections (Gene Ontology, Taxonomy or PubMed are some examples) and the corresponding resources (physical locations) providing access to those data collections. The Registry provides unique and perennial URIs for each entity of those data collections.",
         "id": 41,
         "mirId": "MIR:00000008",
-        "modified": "2023-09-13T08:57:20.977+0000",
+        "modified": "2024-02-06T14:56:58.330+0000",
         "name": "MIRIAM Registry collection",
         "namespaceEmbeddedInLui": false,
         "pattern": "^MIR:000\\d{5}$",
         "prefix": "miriam.collection",
         "resources": [
             {
                 "authHelpDescription": null,
@@ -28864,27 +28960,27 @@
     "mzspec": {
         "created": "2019-06-11T14:18:05.468+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "The Universal Spectrum Identifier (USI) is a compound identifier that provides an abstract path to refer to a single spectrum generated by a mass spectrometer, and potentially the ion that is thought to have produced it.",
         "id": 1735,
         "mirId": "MIR:00000625",
-        "modified": "2019-06-11T14:18:05.468+0000",
+        "modified": "2024-03-22T09:42:52.380+0000",
         "name": "Universal Spectrum Identifier",
         "namespaceEmbeddedInLui": true,
         "pattern": "^mzspec:.+$",
         "prefix": "mzspec",
         "resources": [
             {
                 "authHelpDescription": null,
                 "authHelpUrl": null,
                 "deprecated": false,
                 "deprecationDate": null,
-                "description": "Universal Spectrum Identifier through Peptide Atlas",
-                "id": 1737,
+                "description": "Institute for Systems Biology (ISB), Seattle, USA is an independent research institute focusing on systems biology.",
+                "id": 2394,
                 "institution": {
                     "description": "ISB was created in 2000 as the first-ever institute dedicated to systems biology.",
                     "homeUrl": "https://isbscience.org/",
                     "id": 193,
                     "location": {
                         "countryCode": "US",
                         "countryName": "United States"
@@ -28892,31 +28988,31 @@
                     "name": "Institute for Systems Biology",
                     "rorId": "https://ror.org/02tpgw303"
                 },
                 "location": {
                     "countryCode": "US",
                     "countryName": "United States"
                 },
-                "mirId": "MIR:00100829",
-                "name": "Universal Spectrum Identifier through Peptide Atlas",
-                "official": false,
+                "mirId": "MIR:00000771",
+                "name": "Institute for Systems Biology, Seattle, USA",
+                "official": true,
                 "protectedUrls": false,
-                "providerCode": "CURATOR_REVIEW",
+                "providerCode": "pc",
                 "renderProtectedLanding": false,
-                "resourceHomeUrl": "https://db.systemsbiology.net/sbeams/cgi/PeptideAtlas/ShowObservedSpectrum",
-                "sampleId": "PXD002255::ES_XP_Ubi_97H_HCD_349:scan:9617:LAEIYVNSSFYK/2",
-                "urlPattern": "https://db.systemsbiology.net/sbeams/cgi/PeptideAtlas/ShowObservedSpectrum?usi=mzspec:{$id}"
+                "resourceHomeUrl": "http://proteomecentral.proteomexchange.org/",
+                "sampleId": "PXD000865:00603_F01_P004608_B00F_A00_R1:scan:14453:SSLLDVLAAR/2",
+                "urlPattern": "http://proteomecentral.proteomexchange.org/usi/?usi=mzspec:{$id}"
             },
             {
                 "authHelpDescription": null,
                 "authHelpUrl": null,
                 "deprecated": false,
                 "deprecationDate": null,
-                "description": "Institute for Systems Biology (ISB), Seattle, USA is an independent research institute focusing on systems biology.",
-                "id": 2394,
+                "description": "Universal Spectrum Identifier through Peptide Atlas",
+                "id": 1737,
                 "institution": {
                     "description": "ISB was created in 2000 as the first-ever institute dedicated to systems biology.",
                     "homeUrl": "https://isbscience.org/",
                     "id": 193,
                     "location": {
                         "countryCode": "US",
                         "countryName": "United States"
@@ -28924,26 +29020,26 @@
                     "name": "Institute for Systems Biology",
                     "rorId": "https://ror.org/02tpgw303"
                 },
                 "location": {
                     "countryCode": "US",
                     "countryName": "United States"
                 },
-                "mirId": "MIR:00000771",
-                "name": "Institute for Systems Biology, Seattle, USA",
-                "official": true,
+                "mirId": "MIR:00100829",
+                "name": "Universal Spectrum Identifier through Peptide Atlas",
+                "official": false,
                 "protectedUrls": false,
-                "providerCode": "pc",
+                "providerCode": "CURATOR_REVIEW",
                 "renderProtectedLanding": false,
-                "resourceHomeUrl": "http://proteomecentral.proteomexchange.org/",
-                "sampleId": "PXD000865:00603_F01_P004608_B00F_A00_R1:scan:14453:SSLLDVLAAR/2",
-                "urlPattern": "http://proteomecentral.proteomexchange.org/usi/?usi=mzspec:{$id}"
+                "resourceHomeUrl": "https://db.systemsbiology.net/sbeams/cgi/PeptideAtlas/ShowObservedSpectrum",
+                "sampleId": "PXD002255:ES_XP_Ubi_97H_HCD_349:scan:9617:LAEIYVNSSFYK/2",
+                "urlPattern": "https://db.systemsbiology.net/sbeams/cgi/PeptideAtlas/ShowObservedSpectrum?usi=mzspec:{$id}"
             }
         ],
-        "sampleId": "PXD002255::ES_XP_Ubi_97H_HCD_349:scan:9617:LAEIYVNSSFYK/2"
+        "sampleId": "PXD002255:ES_XP_Ubi_97H_HCD_349:scan:9617:LAEIYVNSSFYK/2"
     },
     "nando": {
         "created": "2023-05-09T12:26:02.992+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "Nanbyo Disease Ontology (NANDO) is the ontology creating a comprehensive hierarchical controlled vocabulary for intractable and rare disease (i.e., nanbyo) representation in Japan.",
         "id": 3536,
@@ -30745,14 +30841,62 @@
                 "resourceHomeUrl": null,
                 "sampleId": null,
                 "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/oba/terms?obo_id=OBA:{$id}"
             }
         ],
         "sampleId": null
     },
+    "obcs": {
+        "created": "2024-03-21T14:43:39.901+0000",
+        "deprecated": false,
+        "deprecationDate": null,
+        "description": "OBCS stands for the Ontology of Biological and Clinical Statistics. OBCS is an ontology in the domain of biological and clinical statistics. It is aligned with the Basic Formal Ontology (BFO) and the Ontology for Biomedical Investigations (OBI)",
+        "id": 3852,
+        "mirId": "MIR:00001053",
+        "modified": "2024-03-21T14:43:39.901+0000",
+        "name": " Ontology of Biological and Clinical Statistics",
+        "namespaceEmbeddedInLui": true,
+        "pattern": "^OBCS:\\d+$",
+        "prefix": "obcs",
+        "resources": [
+            {
+                "authHelpDescription": null,
+                "authHelpUrl": null,
+                "deprecated": false,
+                "deprecationDate": null,
+                "description": "OBCS stands for the Ontology of Biological and Clinical Statistics",
+                "id": 3853,
+                "institution": {
+                    "description": "At EMBL-EBI, we make the world\u2019s public biological data freely available to the scientific community via a range of services and tools, perform basic research and provide professional training in bioinformatics. \nWe are part of the European Molecular Biology Laboratory (EMBL), an international, innovative and interdisciplinary research organisation funded by 26 member states and two associate member states.",
+                    "homeUrl": "https://www.ebi.ac.uk",
+                    "id": 2,
+                    "location": {
+                        "countryCode": "GB",
+                        "countryName": "United Kingdom"
+                    },
+                    "name": "European Bioinformatics Institute",
+                    "rorId": "https://ror.org/02catss52"
+                },
+                "location": {
+                    "countryCode": "GB",
+                    "countryName": "United Kingdom"
+                },
+                "mirId": "MIR:00001052",
+                "name": "OBCS via OLS",
+                "official": true,
+                "protectedUrls": false,
+                "providerCode": "ols",
+                "renderProtectedLanding": false,
+                "resourceHomeUrl": "https://www.ebi.ac.uk/ols4/ontologies/obcs",
+                "sampleId": "0000086",
+                "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/obcs/classes?obo_id=OBCS:{$id}"
+            }
+        ],
+        "sampleId": "0000086"
+    },
     "obi": {
         "created": "2019-06-11T14:16:06.780+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "The Ontology for Biomedical Investigations (OBI) project is developing an integrated ontology for the description of biological and clinical investigations. The ontology will represent the design of an investigation, the protocols and instrumentation used, the material used, the data generated and the type analysis performed on it. Currently OBI is being built under the Basic Formal Ontology (BFO).",
         "id": 402,
         "mirId": "MIR:00000127",
@@ -31753,14 +31897,62 @@
                 "resourceHomeUrl": "http://bioportal.bioontology.org/ontologies/OPB",
                 "sampleId": "OPB_00573",
                 "urlPattern": "http://purl.bioontology.org/ontology/OPB?conceptid=http%3A%2F%2Fbhi.washington.edu%2FOPB%23{$id}"
             }
         ],
         "sampleId": "OPB_00573"
     },
+    "opl": {
+        "created": "2024-03-20T10:39:56.678+0000",
+        "deprecated": false,
+        "deprecationDate": null,
+        "description": "The Ontology for Parasite Lifecycle (OPL) models the life cycle stage details of various parasites, including Trypanosoma sp., Leishmania major, and Plasmodium sp., etc.",
+        "id": 3827,
+        "mirId": "MIR:00001047",
+        "modified": "2024-03-20T10:39:56.678+0000",
+        "name": "Ontology for Parasite Lifecycle",
+        "namespaceEmbeddedInLui": true,
+        "pattern": "^OPL:\\d+$",
+        "prefix": "opl",
+        "resources": [
+            {
+                "authHelpDescription": null,
+                "authHelpUrl": null,
+                "deprecated": false,
+                "deprecationDate": null,
+                "description": "The Ontology for Parasite Lifecycle (OPL) models the life cycle stage details of various parasites, including Trypanosoma sp., Leishmania major, and Plasmodium sp., etc",
+                "id": 3828,
+                "institution": {
+                    "description": "At EMBL-EBI, we make the world\u2019s public biological data freely available to the scientific community via a range of services and tools, perform basic research and provide professional training in bioinformatics. \nWe are part of the European Molecular Biology Laboratory (EMBL), an international, innovative and interdisciplinary research organisation funded by 26 member states and two associate member states.",
+                    "homeUrl": "https://www.ebi.ac.uk",
+                    "id": 2,
+                    "location": {
+                        "countryCode": "GB",
+                        "countryName": "United Kingdom"
+                    },
+                    "name": "European Bioinformatics Institute",
+                    "rorId": "https://ror.org/02catss52"
+                },
+                "location": {
+                    "countryCode": "GB",
+                    "countryName": "United Kingdom"
+                },
+                "mirId": "MIR:00001046",
+                "name": "OPL via OLS",
+                "official": true,
+                "protectedUrls": false,
+                "providerCode": "ols",
+                "renderProtectedLanding": false,
+                "resourceHomeUrl": "https://www.ebi.ac.uk/ols4/ontologies/opl",
+                "sampleId": "0000134",
+                "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/opl/classes?obo_id=OPL:{$id}"
+            }
+        ],
+        "sampleId": "0000134"
+    },
     "opm": {
         "created": "2019-06-11T14:16:54.970+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "The Orientations of Proteins in Membranes (OPM) database provides spatial positions of membrane-bound peptides and proteins of known three-dimensional structure in the lipid bilayer, together with their structural classification, topology and intracellular localization.",
         "id": 955,
         "mirId": "MIR:00000333",
@@ -35531,20 +35723,20 @@
                 "urlPattern": "https://proconsortium.org/app/entry/PR:{$id}"
             }
         ],
         "sampleId": "000000024"
     },
     "pride": {
         "created": "2019-06-11T14:15:50.454+0000",
-        "deprecated": false,
-        "deprecationDate": null,
+        "deprecated": true,
+        "deprecationDate": "2024-03-22T09:58:34.344+0000",
         "description": "The PRIDE PRoteomics IDEntifications database is a centralized, standards compliant, public data repository that provides protein and peptide identifications together with supporting evidence. This collection references experiments and assays.",
         "id": 228,
         "mirId": "MIR:00000065",
-        "modified": "2019-06-11T14:15:50.454+0000",
+        "modified": "2024-03-22T10:18:22.059+0000",
         "name": "PRIDE",
         "namespaceEmbeddedInLui": false,
         "pattern": "^\\d+$",
         "prefix": "pride",
         "resources": [
             {
                 "authHelpDescription": null,
@@ -37506,17 +37698,17 @@
                 },
                 "mirId": "MIR:00100686",
                 "name": "Rfam at EMBL-EBI",
                 "official": true,
                 "protectedUrls": false,
                 "providerCode": "ebi",
                 "renderProtectedLanding": false,
-                "resourceHomeUrl": "https://rfam.xfam.org/",
+                "resourceHomeUrl": "https://rfam.org/",
                 "sampleId": "RF00230",
-                "urlPattern": "https://rfam.xfam.org/family/{$id}"
+                "urlPattern": "https://rfam.org/family/{$id}"
             }
         ],
         "sampleId": "RF00230"
     },
     "rgd": {
         "created": "2019-06-11T14:15:45.062+0000",
         "deprecated": false,
@@ -40698,33 +40890,33 @@
                 "sampleId": "1a24",
                 "urlPattern": "http://psb.kobic.re.kr/STAP/refinement1/result.php?search={$id}"
             }
         ],
         "sampleId": "1a24"
     },
     "stato": {
-        "created": null,
+        "created": "2024-03-20T11:10:30.918+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "STATO is the statistical methods ontology. It contains concepts and properties related to statistical methods, probability distributions and other concepts related to statistical analysis, including relationships to study designs and plots.",
-        "id": null,
-        "mirId": null,
-        "modified": null,
-        "name": "STATO",
+        "id": 3842,
+        "mirId": "MIR:00001051",
+        "modified": "2024-03-20T11:10:30.918+0000",
+        "name": "Statistical Ontology",
         "namespaceEmbeddedInLui": true,
         "pattern": "^STATO:\\d+$",
         "prefix": "stato",
         "resources": [
             {
                 "authHelpDescription": null,
                 "authHelpUrl": null,
                 "deprecated": false,
                 "deprecationDate": null,
-                "description": "stato through OLS",
-                "id": null,
+                "description": "At EMBL-EBI, we make the world\u2019s public biological data freely available to the scientific community via a range of services and tools, perform basic research and provide professional training in bioinformatics. \nWe are part of the European Molecular Biology Laboratory (EMBL), an international, innovative and interdisciplinary research organisation funded by 26 member states and two associate member states.",
+                "id": 3843,
                 "institution": {
                     "description": "At EMBL-EBI, we make the world\u2019s public biological data freely available to the scientific community via a range of services and tools, perform basic research and provide professional training in bioinformatics. \nWe are part of the European Molecular Biology Laboratory (EMBL), an international, innovative and interdisciplinary research organisation funded by 26 member states and two associate member states.",
                     "homeUrl": "https://www.ebi.ac.uk",
                     "id": 2,
                     "location": {
                         "countryCode": "GB",
                         "countryName": "United Kingdom"
@@ -40732,26 +40924,26 @@
                     "name": "European Bioinformatics Institute",
                     "rorId": "https://ror.org/02catss52"
                 },
                 "location": {
                     "countryCode": "GB",
                     "countryName": "United Kingdom"
                 },
-                "mirId": null,
-                "name": "stato through OLS",
-                "official": false,
+                "mirId": "MIR:00001050",
+                "name": "European Bioinformatics Institute",
+                "official": true,
                 "protectedUrls": false,
                 "providerCode": "ols",
                 "renderProtectedLanding": false,
-                "resourceHomeUrl": null,
-                "sampleId": null,
-                "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/stato/terms?obo_id=STATO:{$id}"
+                "resourceHomeUrl": "https://www.ebi.ac.uk",
+                "sampleId": "0000138",
+                "urlPattern": "https://www.ebi.ac.uk/ols4/ontologies/stato/classes?obo_id=STATO:{$id}"
             }
         ],
-        "sampleId": null
+        "sampleId": "0000138"
     },
     "stitch": {
         "created": "2019-06-11T14:16:40.524+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "STITCH is a resource to explore known and predicted interactions of chemicals and proteins. Chemicals are linked to other chemicals and proteins by evidence derived from experiments, databases and the literature.",
         "id": 781,
@@ -41257,14 +41449,62 @@
                 "resourceHomeUrl": "http://swissregulon.unibas.ch",
                 "sampleId": "AHR",
                 "urlPattern": "http://swissregulon.unibas.ch/query/{$id}"
             }
         ],
         "sampleId": "AHR"
     },
+    "synapse": {
+        "created": "2024-03-20T10:13:27.272+0000",
+        "deprecated": false,
+        "deprecationDate": null,
+        "description": "Synapse is a collaborative, open-source research platform that allows teams to share data, track analyses, and collaborate.",
+        "id": 3808,
+        "mirId": "MIR:00001043",
+        "modified": "2024-03-20T10:13:27.272+0000",
+        "name": "Synapse Data Repository",
+        "namespaceEmbeddedInLui": false,
+        "pattern": "[0-9]*\\.*[0-9]*",
+        "prefix": "synapse",
+        "resources": [
+            {
+                "authHelpDescription": null,
+                "authHelpUrl": null,
+                "deprecated": false,
+                "deprecationDate": null,
+                "description": "Sage Bionetworks is a trusted leader in data sharing and reuse, enabling a rapid acceleration in biomedical discoveries and the transformation of medicine.",
+                "id": 3809,
+                "institution": {
+                    "description": "Sage Bionetworks is a trusted leader in data sharing and reuse, enabling a rapid acceleration in biomedical discoveries and the transformation of medicine.",
+                    "homeUrl": "https://www.sagebionetworks.org",
+                    "id": 3807,
+                    "location": {
+                        "countryCode": "US",
+                        "countryName": "United States"
+                    },
+                    "name": "Sage Bionetworks",
+                    "rorId": null
+                },
+                "location": {
+                    "countryCode": "US",
+                    "countryName": "United States"
+                },
+                "mirId": "MIR:00001042",
+                "name": "Sage Bionetworks",
+                "official": true,
+                "protectedUrls": false,
+                "providerCode": "synapse",
+                "renderProtectedLanding": false,
+                "resourceHomeUrl": "https://sagebionetworks.org",
+                "sampleId": "41455251.1",
+                "urlPattern": "https://repo-prod.prod.sagebase.org/ga4gh/drs/v1/objects/syn{$id}"
+            }
+        ],
+        "sampleId": "41455251.1"
+    },
     "t3db": {
         "created": "2019-06-11T14:16:00.251+0000",
         "deprecated": false,
         "deprecationDate": null,
         "description": "Toxin and Toxin Target Database (T3DB) is a bioinformatics resource that combines detailed toxin data with comprehensive toxin target information.",
         "id": 333,
         "mirId": "MIR:00000103",
```

### Comparing `pymetadata-0.4.1/src/pymetadata/resources/templates/ontology_enum.pytemplate` & `pymetadata-0.4.2/src/pymetadata/resources/templates/ontology_enum.pytemplate`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/src/pymetadata/unichem.py` & `pymetadata-0.4.2/src/pymetadata/unichem.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,19 +92,20 @@
 
             sources_list: List[UnichemSource] = [
                 UnichemSource(**v) for v in data["sources"]
             ]
             sources = {source.sourceID: source for source in sources_list}
 
             # write cache
-            write_json_cache(
-                data=sources,
-                cache_path=unichem_sources_path,
-                json_encoder=DataclassJSONEncoder,
-            )
+            if cache:
+                write_json_cache(
+                    data=sources,
+                    cache_path=unichem_sources_path,
+                    json_encoder=DataclassJSONEncoder,
+                )
 
         return sources
 
     def query_xrefs_for_inchikey(self, inchikey: str) -> List[CrossReference]:
         """Get the cross references for a given inchikey."""
 
         # cache files
```

### Comparing `pymetadata-0.4.1/src/pymetadata.egg-info/PKG-INFO` & `pymetadata-0.4.2/src/pymetadata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetadata
-Version: 0.4.1
+Version: 0.4.2
 Summary: pymetadata are python utilities for working with metadata.
 Home-page: https://github.com/matthiaskoenig/pymetadata
 Download-URL: https://pypi.org/project/pymetadata
 Author: Matthias Koenig
 Author-email: konigmatt@googlemail.com
 Maintainer: Matthias Koenig
 Maintainer-email: konigmatt@googlemail.com
@@ -24,72 +24,63 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: depinfo>=1.7
-Requires-Dist: uuid>=1.30
-Requires-Dist: lxml>=4.9
-Requires-Dist: rich>=13.6
+Requires-Dist: lxml>=5.2
+Requires-Dist: rich>=13.7
 Requires-Dist: requests>=2.31
 Requires-Dist: zeep>=4.2.1
-Requires-Dist: pronto>=2.5.5
-Requires-Dist: fastobo>=0.12.2
-Requires-Dist: jinja2>=3.1.2
+Requires-Dist: pronto>=2.5.6
+Requires-Dist: fastobo>=0.12.3
+Requires-Dist: jinja2>=3.1
 Requires-Dist: xmltodict>=0.13.0
-Requires-Dist: pydantic>=2.4
+Requires-Dist: pydantic>=2.6
 Provides-Extra: development
-Requires-Dist: pip-tools>6.10; extra == "development"
-Requires-Dist: black>=24.1.1; extra == "development"
+Requires-Dist: pip-tools>=7.4.1; extra == "development"
+Requires-Dist: black>=24.3.0; extra == "development"
 Requires-Dist: bump2version>=1.0.1; extra == "development"
 Requires-Dist: isort>=5.13.2; extra == "development"
-Requires-Dist: tox>=4.12.1; extra == "development"
-Requires-Dist: flake8>=6.1.0; extra == "development"
+Requires-Dist: tox>=4.12.2; extra == "development"
+Requires-Dist: flake8>=7.0.0; extra == "development"
 Requires-Dist: flake8-mypy>=17.8.0; extra == "development"
-Requires-Dist: mypy>=1.8.0; extra == "development"
-Requires-Dist: pytest>=8.0.0; extra == "development"
-Requires-Dist: pytest-cov>=4.1.0; extra == "development"
+Requires-Dist: mypy>=1.9.0; extra == "development"
+Requires-Dist: pytest>=8.1.1; extra == "development"
+Requires-Dist: pytest-cov>=5.0.0; extra == "development"
 
 .. image:: https://github.com/matthiaskoenig/pymetadata/raw/develop/docs/images/favicon/pymetadata-100x100-300dpi.png
    :align: left
    :alt: pymetadata logo
 
 pymetadata: python utilities for metadata and COMBINE archives
 ==============================================================
+|icon1| |icon2| |icon3| |icon4| |icon5| |icon6| |icon7|
 
-.. image:: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD/badge.svg
+
+.. |icon1| image:: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD/badge.svg
    :target: https://github.com/matthiaskoenig/pymetadata/workflows/CI-CD
    :alt: GitHub Actions CI/CD Status
-
-.. image:: https://img.shields.io/pypi/v/pymetadata.svg
+.. |icon2| image:: https://img.shields.io/pypi/v/pymetadata.svg
    :target: https://pypi.org/project/pymetadata/
    :alt: Current PyPI Version
-
-.. image:: https://img.shields.io/pypi/pyversions/pymetadata.svg
+.. |icon3| image:: https://img.shields.io/pypi/pyversions/pymetadata.svg
    :target: https://pypi.org/project/pymetadata/
    :alt: Supported Python Versions
-
-.. image:: https://img.shields.io/pypi/l/pymetadata.svg
+.. |icon4| image:: https://img.shields.io/pypi/l/pymetadata.svg
    :target: http://opensource.org/licenses/LGPL-3.0
    :alt: GNU Lesser General Public License 3
-
-.. image:: https://codecov.io/gh/matthiaskoenig/pymetadata/branch/develop/graph/badge.svg
-   :target: https://codecov.io/gh/matthiaskoenig/pymetadata
-   :alt: Codecov
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5308801.svg
+.. |icon5| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5308801.svg
    :target: https://doi.org/10.5281/zenodo.5308801
    :alt: Zenodo DOI
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |icon6| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
    :alt: Black
-
-.. image:: http://www.mypy-lang.org/static/mypy_badge.svg
+.. |icon7| image:: http://www.mypy-lang.org/static/mypy_badge.svg
    :target: http://mypy-lang.org/
    :alt: mypy
 
 pymetadata is a collection of python utilities for working with
 metadata in the context of COMBINE standards with source code available from 
 `https://github.com/matthiaskoenig/pymetadata <https://github.com/matthiaskoenig/pymetadata>`__.
 
@@ -136,19 +127,19 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 Funding
 =======
-Matthias König is supported by the Federal Ministry of Education and Research (BMBF, Germany)
+Matthias König was supported by the Federal Ministry of Education and Research (BMBF, Germany)
 within the research network Systems Medicine of the Liver (**LiSyM**, grant number 031L0054) 
-and by the German Research Foundation (DFG) within the Research Unit Programme FOR 5151 
+and is supported by the German Research Foundation (DFG) within the Research Unit Programme FOR 5151 
 "`QuaLiPerF <https://qualiperf.de>`__ (Quantifying Liver Perfusion-Function Relationship in Complex Resection - 
-A Systems Medicine Approach)" by grant number 436883643 and by grant number 465194077 (Priority Programme SPP 2311, Subproject SimLivA).
+A Systems Medicine Approach)" by grant number 436883643 and by grant number 465194077 (Priority Programme SPP 2311, Subproject SimLivA), and 
 
 Installation
 ============
 `pymetadata` is available from `pypi <https://pypi.python.org/pypi/pymetadata>`__ and 
 can be installed via:: 
 
     pip install pymetadata
@@ -165,8 +156,8 @@
     cd pymetadata
     pip install -e .
 
 To install for development use::
 
     pip install -e .[development]
 
-© 2021-2022 Matthias König
+© 2021-2024 Matthias König
```

### Comparing `pymetadata-0.4.1/src/pymetadata.egg-info/SOURCES.txt` & `pymetadata-0.4.2/src/pymetadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/tests/test_chebi.py` & `pymetadata-0.4.2/tests/test_chebi.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/tests/test_ols.py` & `pymetadata-0.4.2/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/tests/test_omex.py` & `pymetadata-0.4.2/tests/test_omex.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/tests/test_ontology.py` & `pymetadata-0.4.2/tests/test_ontology.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/tests/test_sbo_kisao.py` & `pymetadata-0.4.2/tests/test_sbo_kisao.py`

 * *Files identical despite different names*

### Comparing `pymetadata-0.4.1/tests/test_unichem.py` & `pymetadata-0.4.2/tests/test_unichem.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pymetadata.unichem import UnichemQuery, UnichemSource
 
 
 def test_get_sources(tmp_path: Path) -> None:
     """Test retrieving sources."""
     cache_path: Path = tmp_path
-    sources = UnichemQuery.get_sources(cache=False, cache_path=cache_path)
+    sources = UnichemQuery.get_sources(cache=True, cache_path=cache_path)
     assert sources
     assert (cache_path / "unichem_sources.json").exists()
 
     sources = UnichemQuery.get_sources(cache=True, cache_path=cache_path)
     assert sources
```

