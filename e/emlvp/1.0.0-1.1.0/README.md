# Comparing `tmp/emlvp-1.0.0.tar.gz` & `tmp/emlvp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlvp-1.0.0.tar", last modified: Sat Feb 17 17:47:09 2024, max compression
+gzip compressed data, was "emlvp-1.1.0.tar", last modified: Thu Apr 11 21:40:24 2024, max compression
```

## Comparing `emlvp-1.0.0.tar` & `emlvp-1.1.0.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.439225 emlvp-1.0.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    11357 2023-01-21 18:45:39.000000 emlvp-1.0.0/LICENSE
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      130 2023-02-01 23:07:16.000000 emlvp-1.0.0/MANIFEST.in
--rw-r--r--   0 servilla  (1000) servilla  (1000)    21514 2024-02-17 17:47:09.439225 emlvp-1.0.0/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8146 2024-02-17 17:40:25.000000 emlvp-1.0.0/README.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      766 2024-02-17 17:47:09.439225 emlvp-1.0.0/setup.cfg
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1252 2024-01-19 03:13:11.000000 emlvp-1.0.0/setup.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.431225 emlvp-1.0.0/src/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.431225 emlvp-1.0.0/src/emlvp/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-02-17 17:40:25.000000 emlvp-1.0.0/src/emlvp/VERSION.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      128 2023-01-21 19:41:00.000000 emlvp-1.0.0/src/emlvp/__init__.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      906 2024-02-17 17:40:25.000000 emlvp-1.0.0/src/emlvp/changelog.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1658 2023-02-06 20:43:54.000000 emlvp-1.0.0/src/emlvp/dereferencer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     6710 2024-02-17 17:40:25.000000 emlvp-1.0.0/src/emlvp/emlvp_cli.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1121 2023-01-27 21:12:55.000000 emlvp-1.0.0/src/emlvp/exceptions.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2206 2024-02-17 17:40:25.000000 emlvp-1.0.0/src/emlvp/normalizer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8193 2024-02-17 17:40:25.000000 emlvp-1.0.0/src/emlvp/parser.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.431225 emlvp-1.0.0/src/emlvp/schemas/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.435225 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    18447 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29487 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    58886 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    18745 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-text.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    19139 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:00.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/stmml.xsd
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.439225 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    20356 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29531 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    60720 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21204 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-text.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    19379 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:17.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/stmml.xsd
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.439225 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493311 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   102174 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.439225 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    11830 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    86976 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27152 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    72264 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7693 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    28001 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2899 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14949 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    58814 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21970 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    28924 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    76821 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29309 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     4952 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    68327 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    15511 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21403 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46367 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167250 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13021 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10334 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    32155 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    23090 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7008 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22368 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   133761 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      579 2023-01-31 04:06:28.000000 emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1978 2023-02-06 20:13:41.000000 emlvp-1.0.0/src/emlvp/validator.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.439225 emlvp-1.0.0/src/emlvp.egg-info/
--rw-r--r--   0 servilla  (1000) servilla  (1000)    21514 2024-02-17 17:47:09.000000 emlvp-1.0.0/src/emlvp.egg-info/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     4415 2024-02-17 17:47:09.000000 emlvp-1.0.0/src/emlvp.egg-info/SOURCES.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2024-02-17 17:47:09.000000 emlvp-1.0.0/src/emlvp.egg-info/dependency_links.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       47 2024-02-17 17:47:09.000000 emlvp-1.0.0/src/emlvp.egg-info/entry_points.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       41 2024-02-17 17:47:09.000000 emlvp-1.0.0/src/emlvp.egg-info/requires.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-02-17 17:47:09.000000 emlvp-1.0.0/src/emlvp.egg-info/top_level.txt
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-02-17 17:47:09.439225 emlvp-1.0.0/tests/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      647 2024-02-17 17:40:25.000000 emlvp-1.0.0/tests/test_dereferencer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      584 2024-02-17 17:40:25.000000 emlvp-1.0.0/tests/test_normalizer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2896 2023-07-22 01:19:36.000000 emlvp-1.0.0/tests/test_parser.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2065 2023-07-22 01:19:36.000000 emlvp-1.0.0/tests/test_validator.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.466695 emlvp-1.1.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    11357 2023-01-21 18:45:39.000000 emlvp-1.1.0/LICENSE
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      130 2023-02-01 23:07:16.000000 emlvp-1.1.0/MANIFEST.in
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    22001 2024-04-11 21:40:24.466695 emlvp-1.1.0/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8633 2024-04-11 21:27:52.000000 emlvp-1.1.0/README.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      766 2024-04-11 21:40:24.466695 emlvp-1.1.0/setup.cfg
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1252 2024-01-19 03:13:11.000000 emlvp-1.1.0/setup.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.458695 emlvp-1.1.0/src/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.458695 emlvp-1.1.0/src/emlvp/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-04-11 21:32:54.000000 emlvp-1.1.0/src/emlvp/VERSION.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      128 2023-01-21 19:41:00.000000 emlvp-1.1.0/src/emlvp/__init__.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1035 2024-04-11 21:30:12.000000 emlvp-1.1.0/src/emlvp/changelog.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1814 2024-04-11 21:30:42.000000 emlvp-1.1.0/src/emlvp/dereferencer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8829 2024-04-11 21:30:42.000000 emlvp-1.1.0/src/emlvp/emlvp_cli.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1161 2024-04-11 21:30:42.000000 emlvp-1.1.0/src/emlvp/exceptions.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2343 2024-04-11 21:30:42.000000 emlvp-1.1.0/src/emlvp/normalizer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8289 2024-04-11 21:30:42.000000 emlvp-1.1.0/src/emlvp/parser.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.458695 emlvp-1.1.0/src/emlvp/schemas/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.462695 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    18447 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29487 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    58886 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    18745 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-text.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    19139 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:00.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/stmml.xsd
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.462695 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    20356 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29531 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    60720 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21204 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-text.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    19379 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:17.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/stmml.xsd
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.466695 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493311 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   102174 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.466695 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    11830 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    86976 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27152 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    72264 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7693 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    28001 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2899 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14949 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    58814 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21970 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    28924 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    76821 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29309 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     4952 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    68327 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    15511 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21403 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46367 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167250 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13021 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10334 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    32155 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    23090 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7008 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22368 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   133761 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      579 2023-01-31 04:06:28.000000 emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      800 2024-04-11 21:27:52.000000 emlvp-1.1.0/src/emlvp/unicode_inspector.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2103 2024-04-11 21:30:42.000000 emlvp-1.1.0/src/emlvp/validator.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.466695 emlvp-1.1.0/src/emlvp.egg-info/
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    22001 2024-04-11 21:40:24.000000 emlvp-1.1.0/src/emlvp.egg-info/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     4468 2024-04-11 21:40:24.000000 emlvp-1.1.0/src/emlvp.egg-info/SOURCES.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2024-04-11 21:40:24.000000 emlvp-1.1.0/src/emlvp.egg-info/dependency_links.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       47 2024-04-11 21:40:24.000000 emlvp-1.1.0/src/emlvp.egg-info/entry_points.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       41 2024-04-11 21:40:24.000000 emlvp-1.1.0/src/emlvp.egg-info/requires.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-04-11 21:40:24.000000 emlvp-1.1.0/src/emlvp.egg-info/top_level.txt
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-11 21:40:24.466695 emlvp-1.1.0/tests/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      647 2024-02-17 17:40:25.000000 emlvp-1.1.0/tests/test_dereferencer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      584 2024-02-17 17:40:25.000000 emlvp-1.1.0/tests/test_normalizer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2896 2023-07-22 01:19:36.000000 emlvp-1.1.0/tests/test_parser.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      610 2024-04-11 19:56:52.000000 emlvp-1.1.0/tests/test_unicode.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2065 2023-07-22 01:19:36.000000 emlvp-1.1.0/tests/test_validator.py
```

### Comparing `emlvp-1.0.0/LICENSE` & `emlvp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/PKG-INFO` & `emlvp-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlvp
-Version: 1.0.0
+Version: 1.1.0
 Summary: EMLvp (validator and parser)
 Home-page: https://github.com/servilla/EMLvp
 Author: Mark Servilla
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -287,19 +287,23 @@
       3. Dereference references/id into expanded EML XML and re-validate/parse
 
       TARGET: EML XML file or directory containing EML XML file(s) (may be repeated)
 
 Options:
   -d, --dereference   Dereference EML XML file(s) (default is False).
   -f, --fail-fast     Exit on first exception encountered (default is False).
+  -l, --list_unicode  List non-ASCII unicode characters, along with unicode
+                      data
   -n, --normalize     Normalize EML XML file(s) before parsing and validating
                       (default is False).
   -p, --pretty-print  Pretty print output for dereferenced EML XML (default is
                       False).
   -s, --statistics    Show post processing inspection statistics.
+  -u, --unicode       Highlight non-ASCII unicode characters in EML output
+                      (-uu for line numbers)
   -v, --verbose       Send output to standard out (-v or -vv or -vvv for
                       increasing output).
   --version           Output emlvp version and exit.
   -h, --help          Show this message and exit.
 ```
 
 As noted above, the "TARGET" argument may be one or more space separate EML XML files or a directory containing many
@@ -339,15 +343,15 @@
 ```
 
 Applications that use the API should rely on exceptions to indicate an error has occurred in either validation or
 parsing of the EML XML document.
 
 ## EMLvp Class API
 
-### Validator:
+### validator:
 
 ```Python
 class Validator(object):
   """
   Validates an EML XML document for being well formed and schema syntax correct.
   """
 
@@ -362,15 +366,15 @@
   Validates an EML XML document instance
   :param xml: EML XML document instance as a unicode string
   :return: None
   :raises emlvp.exceptions.ValidationError: Raises ValidationError on any invalid content found
   """
 ```
 
-### Parser:
+### parser:
 
 ```Python
 class Parser(object):
    """
    Parses an EML XML document instance inspecting for non-schema related issues. See here for possible
    issues: https://eml.ecoinformatics.org/validation-and-content-references.html
    """
@@ -386,15 +390,15 @@
    Parses an EML XML document instance inspecting for non-schema related issues.
    :param xml: EML XML document instance as a unicode string
    :return: None
    :raises emlvp.exceptions.ParseError: Raises ParseError on any invalid content found
    """
 ```
 
-### Derferencer:
+### derferencer:
 
 ```Python
 class Dereferencer(object):
    """
    Expands EML XML content by dereferencing "references" element to content defined
    by the "id" attribute of a source element.
    """
@@ -411,17 +415,29 @@
    :param xml: EML XML document instance as a unicode string.
    :return str: Expanded EML XML.
    """
 ```
 
 ## EMLvp Helper Function API
 
-### Normalizer
+### normalizer
 
 ```Python
 def normalize(xml: str) -> str:
    """
    Normalize an EML XML document instance
    :param xml: EML XML document instance as a unicode string
    :return: Normalized EML XML document instance as a unicode string
    """
 ```
+
+### unicode_inspector
+
+```Python
+def unicode_list(xml: str) -> list:
+    """
+    List all unicode characters in the given XML with codepoints greater than ASCII 127
+    as a list of tuples: (row, col, char, cp, name)
+    :param xml:
+    :return list:
+    """
+```
```

### Comparing `emlvp-1.0.0/README.md` & `emlvp-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,19 +71,23 @@
       3. Dereference references/id into expanded EML XML and re-validate/parse
 
       TARGET: EML XML file or directory containing EML XML file(s) (may be repeated)
 
 Options:
   -d, --dereference   Dereference EML XML file(s) (default is False).
   -f, --fail-fast     Exit on first exception encountered (default is False).
+  -l, --list_unicode  List non-ASCII unicode characters, along with unicode
+                      data
   -n, --normalize     Normalize EML XML file(s) before parsing and validating
                       (default is False).
   -p, --pretty-print  Pretty print output for dereferenced EML XML (default is
                       False).
   -s, --statistics    Show post processing inspection statistics.
+  -u, --unicode       Highlight non-ASCII unicode characters in EML output
+                      (-uu for line numbers)
   -v, --verbose       Send output to standard out (-v or -vv or -vvv for
                       increasing output).
   --version           Output emlvp version and exit.
   -h, --help          Show this message and exit.
 ```
 
 As noted above, the "TARGET" argument may be one or more space separate EML XML files or a directory containing many
@@ -123,15 +127,15 @@
 ```
 
 Applications that use the API should rely on exceptions to indicate an error has occurred in either validation or
 parsing of the EML XML document.
 
 ## EMLvp Class API
 
-### Validator:
+### validator:
 
 ```Python
 class Validator(object):
   """
   Validates an EML XML document for being well formed and schema syntax correct.
   """
 
@@ -146,15 +150,15 @@
   Validates an EML XML document instance
   :param xml: EML XML document instance as a unicode string
   :return: None
   :raises emlvp.exceptions.ValidationError: Raises ValidationError on any invalid content found
   """
 ```
 
-### Parser:
+### parser:
 
 ```Python
 class Parser(object):
    """
    Parses an EML XML document instance inspecting for non-schema related issues. See here for possible
    issues: https://eml.ecoinformatics.org/validation-and-content-references.html
    """
@@ -170,15 +174,15 @@
    Parses an EML XML document instance inspecting for non-schema related issues.
    :param xml: EML XML document instance as a unicode string
    :return: None
    :raises emlvp.exceptions.ParseError: Raises ParseError on any invalid content found
    """
 ```
 
-### Derferencer:
+### derferencer:
 
 ```Python
 class Dereferencer(object):
    """
    Expands EML XML content by dereferencing "references" element to content defined
    by the "id" attribute of a source element.
    """
@@ -195,17 +199,29 @@
    :param xml: EML XML document instance as a unicode string.
    :return str: Expanded EML XML.
    """
 ```
 
 ## EMLvp Helper Function API
 
-### Normalizer
+### normalizer
 
 ```Python
 def normalize(xml: str) -> str:
    """
    Normalize an EML XML document instance
    :param xml: EML XML document instance as a unicode string
    :return: Normalized EML XML document instance as a unicode string
    """
+```
+
+### unicode_inspector
+
+```Python
+def unicode_list(xml: str) -> list:
+    """
+    List all unicode characters in the given XML with codepoints greater than ASCII 127
+    as a list of tuples: (row, col, char, cp, name)
+    :param xml:
+    :return list:
+    """
 ```
```

### Comparing `emlvp-1.0.0/setup.cfg` & `emlvp-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/setup.py` & `emlvp-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/dereferencer.py` & `emlvp-1.1.0/src/emlvp/dereferencer.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
     1/26/23
 """
 import copy
 
 import daiquiri
 from lxml import etree
 
+from emlvp import exceptions
+
 
 logger = daiquiri.getLogger(__name__)
 
 
-class Dereferencer():
+class Dereferencer:
     """
     Expands EML XML content by dereferencing "references" element to content defined
     by the "id" attribute of a source element.
     """
 
     def __init__(self, pretty_print=False):
         """
@@ -37,15 +39,20 @@
     def dereference(self, xml: str) -> str:
         """
         Dereferences an EML XML document instance.
         :param xml: EML XML document instance as a unicode string.
         :return str: Expanded EML XML.
         """
 
-        xml = xml.encode("utf-8")
+        try:
+            xml = xml.encode("utf-8")
+        except UnicodeEncodeError as e:
+            logger.debug(e)
+            raise exceptions.UTF8Error(e)
+
         root = etree.fromstring(xml)
 
         references_nodes = root.xpath(".//references")
         for references in references_nodes:
             source_node = root.xpath(f".//*[@id='{references.text.strip()}']")[0]
             source_children = source_node.getchildren()
             parent_node = references.getparent()
```

### Comparing `emlvp-1.0.0/src/emlvp/exceptions.py` & `emlvp-1.1.0/src/emlvp/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,14 +66,18 @@
     pass
 
 
 class SchemaIncludeError(EMLVPError):
     pass
 
 
+class UTF8Error(EMLVPError):
+    pass
+
+
 class ValidationError(EMLVPError):
     pass
 
 
 class XPathError(EMLVPError):
     pass
```

### Comparing `emlvp-1.0.0/src/emlvp/normalizer.py` & `emlvp-1.1.0/src/emlvp/normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 :Created:
     2/16/24
 """
 
 import daiquiri
 from lxml import etree
 
+from emlvp import exceptions
+
 
 logger = daiquiri.getLogger(__name__)
 
-normalize_whitespace = \
-    """<xsl:stylesheet version="1.0"
+normalize_whitespace = """<xsl:stylesheet version="1.0"
                        xmlns:xsl="http://www.w3.org/1999/XSL/Transform"
                        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                        >
            <xsl:output omit-xml-declaration="no" indent="yes"/>
        
            <!-- Template to copy nodes and apply templates to attributes and child nodes -->
            <xsl:template match="@*|node()">
@@ -56,9 +57,15 @@
 def normalize(xml: str) -> str:
     """
     Normalize an EML XML document instance
     :param xml: EML XML document instance as a unicode string
     :return: Normalized EML XML document instance as a unicode string
     """
     xslt = etree.XSLT(etree.XML(normalize_whitespace))
-    normalized = str(xslt(etree.XML(xml.replace('\xa0', ' ').encode("utf-8"))))
+
+    try:
+        normalized = str(xslt(etree.XML(xml.replace("\xa0", " ").encode("utf-8"))))
+    except UnicodeEncodeError as e:
+        logger.debug(e)
+        raise exceptions.UTF8Error(e)
+
     return normalized
```

### Comparing `emlvp-1.0.0/src/emlvp/parser.py` & `emlvp-1.1.0/src/emlvp/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,20 @@
         """
         Parses an EML XML document instance inspecting for non-schema related issues.
         :param xml: EML XML document instance as a unicode string
         :return: None
         :raises emlvp.exceptions.ParseError: Raises ParseError on any invalid content found
         """
 
-        xml = xml.encode("utf-8")
+        try:
+            xml = xml.encode("utf-8")
+        except UnicodeEncodeError as e:
+            logger.debug(e)
+            raise exceptions.UTF8Error(e)
+
         root = etree.fromstring(xml)
 
         msg_queue = ""
 
         # Inspect id attributes in all elements to ensure uniqueness
         id_nodes = root.findall(".//*[@id]")
         ids = [i.attrib["id"] for i in id_nodes]
@@ -166,17 +171,15 @@
             [reference.attrib["references"] for reference in annotation_nodes]
         )
         for annotation_reference in annotation_references:
             if annotation_reference not in ids:
                 has_missing_annotation_references_id = True
                 missing_annotation_references_ids.append(annotation_reference)
         if has_missing_annotation_references_id:
-            msg_missing_annotation_references = (
-                f"Missing subject id for annotation references: {missing_annotation_references_ids}\n"
-            )
+            msg_missing_annotation_references = f"Missing subject id for annotation references: {missing_annotation_references_ids}\n"
             msg_queue += msg_missing_annotation_references
             logger.debug(msg_missing_annotation_references)
             if self.fail_fast:
                 raise exceptions.ParseError(msg_missing_annotation_references)
 
         # Inspect additionalMetadata describes for subject id
         has_missing_describes_id = False
```

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-access.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-entity.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-literature.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-methods.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-party.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-physical.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-project.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-resource.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-software.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-text.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml-view.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/eml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.0/stmml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.0/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-access.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-entity.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-literature.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-methods.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-party.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-physical.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-project.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-resource.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-software.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-text.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml-view.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/eml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.1.1/stmml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.1.1/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd` & `emlvp-1.1.0/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/src/emlvp/validator.py` & `emlvp-1.1.0/src/emlvp/validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Return path to installed schemas.
     :return: Path to emlvp installed schemas
     :rtype: str
     """
     return os.path.abspath(os.path.dirname(__file__)) + "/schemas"
 
 
-class Validator():
+class Validator:
     """
     Validates an EML XML document for being well formed and schema syntax correct.
     """
 
     def __init__(self, schema: str):
         """
         Class init method.
@@ -52,15 +52,19 @@
         """
         Validates an EML XML document instance
         :param xml: EML XML document instance as a unicode string
         :return: None
         :raises emlvp.exceptions.ValidationError: Raises ValidationError on any invalid content found
         """
 
-        xml = xml.encode("utf-8")
+        try:
+            xml = xml.encode("utf-8")
+        except UnicodeEncodeError as e:
+            logger.debug(e)
+            raise exceptions.UTF8Error(e)
 
         try:
             doc = etree.fromstring(xml)
             schema = etree.XMLSchema(file=self.schema)
             schema.assertValid(doc)
         except etree.DocumentInvalid as e:
             logger.debug(e)
```

### Comparing `emlvp-1.0.0/src/emlvp.egg-info/PKG-INFO` & `emlvp-1.1.0/src/emlvp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlvp
-Version: 1.0.0
+Version: 1.1.0
 Summary: EMLvp (validator and parser)
 Home-page: https://github.com/servilla/EMLvp
 Author: Mark Servilla
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -287,19 +287,23 @@
       3. Dereference references/id into expanded EML XML and re-validate/parse
 
       TARGET: EML XML file or directory containing EML XML file(s) (may be repeated)
 
 Options:
   -d, --dereference   Dereference EML XML file(s) (default is False).
   -f, --fail-fast     Exit on first exception encountered (default is False).
+  -l, --list_unicode  List non-ASCII unicode characters, along with unicode
+                      data
   -n, --normalize     Normalize EML XML file(s) before parsing and validating
                       (default is False).
   -p, --pretty-print  Pretty print output for dereferenced EML XML (default is
                       False).
   -s, --statistics    Show post processing inspection statistics.
+  -u, --unicode       Highlight non-ASCII unicode characters in EML output
+                      (-uu for line numbers)
   -v, --verbose       Send output to standard out (-v or -vv or -vvv for
                       increasing output).
   --version           Output emlvp version and exit.
   -h, --help          Show this message and exit.
 ```
 
 As noted above, the "TARGET" argument may be one or more space separate EML XML files or a directory containing many
@@ -339,15 +343,15 @@
 ```
 
 Applications that use the API should rely on exceptions to indicate an error has occurred in either validation or
 parsing of the EML XML document.
 
 ## EMLvp Class API
 
-### Validator:
+### validator:
 
 ```Python
 class Validator(object):
   """
   Validates an EML XML document for being well formed and schema syntax correct.
   """
 
@@ -362,15 +366,15 @@
   Validates an EML XML document instance
   :param xml: EML XML document instance as a unicode string
   :return: None
   :raises emlvp.exceptions.ValidationError: Raises ValidationError on any invalid content found
   """
 ```
 
-### Parser:
+### parser:
 
 ```Python
 class Parser(object):
    """
    Parses an EML XML document instance inspecting for non-schema related issues. See here for possible
    issues: https://eml.ecoinformatics.org/validation-and-content-references.html
    """
@@ -386,15 +390,15 @@
    Parses an EML XML document instance inspecting for non-schema related issues.
    :param xml: EML XML document instance as a unicode string
    :return: None
    :raises emlvp.exceptions.ParseError: Raises ParseError on any invalid content found
    """
 ```
 
-### Derferencer:
+### derferencer:
 
 ```Python
 class Dereferencer(object):
    """
    Expands EML XML content by dereferencing "references" element to content defined
    by the "id" attribute of a source element.
    """
@@ -411,17 +415,29 @@
    :param xml: EML XML document instance as a unicode string.
    :return str: Expanded EML XML.
    """
 ```
 
 ## EMLvp Helper Function API
 
-### Normalizer
+### normalizer
 
 ```Python
 def normalize(xml: str) -> str:
    """
    Normalize an EML XML document instance
    :param xml: EML XML document instance as a unicode string
    :return: Normalized EML XML document instance as a unicode string
    """
 ```
+
+### unicode_inspector
+
+```Python
+def unicode_list(xml: str) -> list:
+    """
+    List all unicode characters in the given XML with codepoints greater than ASCII 127
+    as a list of tuples: (row, col, char, cp, name)
+    :param xml:
+    :return list:
+    """
+```
```

### Comparing `emlvp-1.0.0/src/emlvp.egg-info/SOURCES.txt` & `emlvp-1.1.0/src/emlvp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/emlvp/__init__.py
 src/emlvp/changelog.md
 src/emlvp/dereferencer.py
 src/emlvp/emlvp_cli.py
 src/emlvp/exceptions.py
 src/emlvp/normalizer.py
 src/emlvp/parser.py
+src/emlvp/unicode_inspector.py
 src/emlvp/validator.py
 src/emlvp.egg-info/PKG-INFO
 src/emlvp.egg-info/SOURCES.txt
 src/emlvp.egg-info/dependency_links.txt
 src/emlvp.egg-info/entry_points.txt
 src/emlvp.egg-info/requires.txt
 src/emlvp.egg-info/top_level.txt
@@ -100,8 +101,9 @@
 src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
 src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
 src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
 src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
 tests/test_dereferencer.py
 tests/test_normalizer.py
 tests/test_parser.py
+tests/test_unicode.py
 tests/test_validator.py
```

### Comparing `emlvp-1.0.0/tests/test_dereferencer.py` & `emlvp-1.1.0/tests/test_dereferencer.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/tests/test_normalizer.py` & `emlvp-1.1.0/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/tests/test_parser.py` & `emlvp-1.1.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.0.0/tests/test_validator.py` & `emlvp-1.1.0/tests/test_validator.py`

 * *Files identical despite different names*

