# Comparing `tmp/eatb-0.1.9.tar.gz` & `tmp/eatb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eatb-0.1.9.tar", last modified: Sun Nov 12 22:54:32 2023, max compression
+gzip compressed data, was "eatb-0.2.0.tar", last modified: Thu Apr 11 17:16:02 2024, max compression
```

## Comparing `eatb-0.1.9.tar` & `eatb-0.2.0.tar`

### file list

```diff
@@ -1,96 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.018441 eatb-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-12 22:54:19.000000 eatb-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-12 22:54:19.000000 eatb-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-12 22:54:32.018441 eatb-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-11-12 22:54:19.000000 eatb-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.006441 eatb-0.1.9/eatb/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/csip_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/directory_pairtree_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/ipstate.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/logging_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.010441 eatb-0.1.9/eatb/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/dip_parsed_premis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/ead.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/mets.py
--rw-r--r--   0 runner    (1001) docker     (127)    26379 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/mets_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/mets_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/parsed_dcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/parsed_ead.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/parsed_mets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/parsed_premis.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/premis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13263 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/metadata/premis_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46958 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/oais_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/package_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9602 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/pairtree_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.010441 eatb-0.1.9/eatb/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.010441 eatb-0.1.9/eatb/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/DILCISExtensionMETS.xsd
--rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   125569 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml
--rw-r--r--   0 runner    (1001) docker     (127)   145565 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/IP.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/csip.xsd
--rwxr-xr-x   0 runner    (1001) docker     (127)   133920 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/mets.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   133018 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/mets_1_11.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    65126 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/premis-v2-2.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/schemas/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/resources/validation_rules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/settings.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.014441 eatb-0.1.9/eatb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/XmlHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/dictutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/listhandling.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/randomutils.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/stringutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2023-11-12 22:54:19.000000 eatb-0.1.9/eatb/utils/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.006441 eatb-0.1.9/eatb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-12 22:54:31.000000 eatb-0.1.9/eatb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-11-12 22:54:31.000000 eatb-0.1.9/eatb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 22:54:31.000000 eatb-0.1.9/eatb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 22:54:31.000000 eatb-0.1.9/eatb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-12 22:54:31.000000 eatb-0.1.9/eatb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-11-12 22:54:32.018441 eatb-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-12 22:54:19.000000 eatb-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:32.018441 eatb-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/dip_premis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_csip_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_directorypairtreestorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_filehandling.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_formatidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_metadata_dcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_metadata_ead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_mets_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_mets_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_mets_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_pairtreestorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_parsed_mets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_premis_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-11-12 22:54:19.000000 eatb-0.1.9/tests/test_premis_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-11-12 22:54:20.000000 eatb-0.1.9/tests/test_stringutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-11-12 22:54:20.000000 eatb-0.1.9/tests/test_tarentryreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-11-12 22:54:20.000000 eatb-0.1.9/tests/test_unzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2023-11-12 22:54:20.000000 eatb-0.1.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-11-12 22:54:20.000000 eatb-0.1.9/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.883865 eatb-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-11 17:15:56.000000 eatb-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 17:15:56.000000 eatb-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-11 17:16:02.883865 eatb-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-11 17:15:56.000000 eatb-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.867864 eatb-0.2.0/eatb/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/csip_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/ipstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/logging_config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.871865 eatb-0.2.0/eatb/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/dip_parsed_premis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/ead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/mets_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/mets_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/parsed_dcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/parsed_ead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/parsed_mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/parsed_premis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/premis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/premis_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/metadata/premis_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46968 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/oais_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/package_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/pairtree_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.871865 eatb-0.2.0/eatb/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.875865 eatb-0.2.0/eatb/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/DILCISExtensionMETS.xsd
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   125569 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   145565 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/IP.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/csip.xsd
+-rwxr-xr-x   0 runner    (1001) docker     (127)   133920 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/mets.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   133018 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/mets_1_11.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    65126 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/premis-v2-2.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/schemas/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/resources/validation_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/settings.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.879865 eatb-0.2.0/eatb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/XmlHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/dictutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/listhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/randomutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/stringutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-11 17:15:56.000000 eatb-0.2.0/eatb/utils/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.883865 eatb-0.2.0/eatb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-11 17:16:02.000000 eatb-0.2.0/eatb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-11 17:16:02.000000 eatb-0.2.0/eatb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:16:02.000000 eatb-0.2.0/eatb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:16:02.000000 eatb-0.2.0/eatb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 17:16:02.000000 eatb-0.2.0/eatb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 17:16:02.883865 eatb-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-11 17:15:56.000000 eatb-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:02.883865 eatb-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/dip_premis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_csip_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_filehandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_formatidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_metadata_dcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_metadata_ead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_mets_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_mets_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_mets_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_pairtreestorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_parsed_mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_premis_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_premis_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_stringutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_tarentryreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_unzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-11 17:15:56.000000 eatb-0.2.0/tests/test_xml.py
```

### Comparing `eatb-0.1.9/LICENSE` & `eatb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/PKG-INFO` & `eatb-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eatb
-Version: 0.1.9
+Version: 0.2.0
 Summary: A suite of tools for the creation of information packages for archival purposes.
 Home-page: https://www.e-ark-foundation.eu/e-ark-software-eatb
 Author: E-ARK Foundation
 Author-email: admin@e-ark-foundation.eu
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Archiving
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# eatb - eArchiving Tool Box
+# eatb - eArchiving Tool Box ![Build](https://github.com/E-ARK-Software/eatb/actions/workflows/python-app.yml/badge.svg?sanitize=true) ![Coverage](https://raw.githubusercontent.com/E-ARK-Software/eatb/master/coverage_badge.svg?sanitize=true) 
 
 ## About
 
 The archiving tool box is a suite of tools for the creation of information packages for archival purposes. The archival
 information package must follow the structure and comply with metadata requirements defined by the E-ARK specification 
 for information packages (CSIP available at https://earkcsip.dilcis.eu).
 
@@ -111,15 +111,15 @@
     |             - file1.csv                               |
     |             - file2.csv                               |
     |         - metadata/                                   |
     |         - documentation/                              |
     |-------------------------------------------------------|
     | - schemas/                                            | <--- Schema files for validation
     |     - IP_CS_mets.xsd                                  |
-    |     - premis-v2-2.xsd                                 |
+    |     - premis-v3-0.xsd                                 |
     |     - xlink.xsd                                       |
     |-------------------------------------------------------|
     | - METS.xml                                            | <--- Root METS file (structural metadata)
     `-------------------------------------------------------'
  
 ## Set up a development environment for the project
```

### Comparing `eatb-0.1.9/README.md` & `eatb-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# eatb - eArchiving Tool Box
+# eatb - eArchiving Tool Box ![Build](https://github.com/E-ARK-Software/eatb/actions/workflows/python-app.yml/badge.svg?sanitize=true) ![Coverage](https://raw.githubusercontent.com/E-ARK-Software/eatb/master/coverage_badge.svg?sanitize=true) 
 
 ## About
 
 The archiving tool box is a suite of tools for the creation of information packages for archival purposes. The archival
 information package must follow the structure and comply with metadata requirements defined by the E-ARK specification 
 for information packages (CSIP available at https://earkcsip.dilcis.eu).
 
@@ -90,15 +90,15 @@
     |             - file1.csv                               |
     |             - file2.csv                               |
     |         - metadata/                                   |
     |         - documentation/                              |
     |-------------------------------------------------------|
     | - schemas/                                            | <--- Schema files for validation
     |     - IP_CS_mets.xsd                                  |
-    |     - premis-v2-2.xsd                                 |
+    |     - premis-v3-0.xsd                                 |
     |     - xlink.xsd                                       |
     |-------------------------------------------------------|
     | - METS.xml                                            | <--- Root METS file (structural metadata)
     `-------------------------------------------------------'
  
 ## Set up a development environment for the project
```

### Comparing `eatb-0.1.9/eatb/checksum.py` & `eatb-0.2.0/eatb/checksum.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/cli.py` & `eatb-0.2.0/eatb/cli.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/csip_validation.py` & `eatb-0.2.0/eatb/csip_validation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/directory_pairtree_storage.py` & `eatb-0.2.0/eatb/pairtree_storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,243 @@
-import fnmatch
 import os
+import pathlib
+import re
 import shutil
 import tarfile
+import fnmatch
 
+from itertools import groupby
+from eatb import VersionDirFormat
+from eatb.checksum import check_transfer
+from eatb.ipstate import IpState
+from eatb.utils.fileutils import rec_find_files, fsize, FileBinaryDataChunks
+from eatb.utils.fileutils import to_safe_filename, list_files_in_dir, copy_file_with_base_directory
 from pairtree import PairtreeStorageFactory, ObjectNotFoundException
-
 from eatb import logger
-from eatb.checksum import check_transfer, files_identical
-from eatb.ipstate import IpState
+from eatb.checksum import files_identical
 from eatb.packaging import ChunkedTarEntryReader
-from eatb.pairtree_storage import PairtreeStorage
-from eatb.utils.fileutils import to_safe_filename, list_files_in_dir, copy_file_with_base_directory, fsize, \
-    FileBinaryDataChunks
 from eatb.utils.reporters import default_reporter
 
 
-def update_state(state_xml_file, identifier, version):
-    ip_state = IpState.from_path(state_xml_file) if os.path.exists(state_xml_file) \
-        else IpState.from_parameters(0, False, last_task_value="stored")
-    ip_state.set_version(version)
-    ip_state.set_identifier(identifier)
-    ip_state.write_doc(state_xml_file)
-
-
-def get_package_from_directory_storage(task_context_path, package_uuid, package_extension,
-                                       tl, config_path_storage):
-    pts = DirectoryPairtreeStorage(config_path_storage)
-    parent_object_path = pts.get_object_path(package_uuid)
-
-    package_in_dip_work_dir = os.path.join(task_context_path, ("%s.%s" % (package_uuid, package_extension)))
-    package_source_size = fsize(parent_object_path)
-    tl.addinfo("Source: %s (%d)" % (parent_object_path, package_source_size))
-    tl.addinfo("Target: %s" % package_in_dip_work_dir)
-    total_bytes_read = 0
-    with open(package_in_dip_work_dir, 'wb') as target_file:
-        for chunk in FileBinaryDataChunks(parent_object_path, 65536).chunks(total_bytes_read):
-            target_file.write(chunk)
-        total_bytes_read += package_source_size
-        target_file.close()
-        check_transfer(parent_object_path, package_in_dip_work_dir)
-
-
-def make_storage_directory_path(identifier, version, config_path_storage):
-    """Used for remote (no access to storage backend)"""
-    pts = DirectoryPairtreeStorage(config_path_storage)
-    return os.path.join(pts.get_dir_path_from_id(identifier), "data", version, to_safe_filename(identifier))
-
-
-def make_storage_data_directory_path(identifier, config_path_storage):
-    """Used for remote (no access to storage backend)"""
-    pts = DirectoryPairtreeStorage(config_path_storage)
-    return os.path.join(pts.get_dir_path_from_id(identifier), "data")
-
-
-class DirectoryPairtreeStorage(PairtreeStorage):
+class PairtreeStorage:
     """
-    Pairtree storage class allowing to build a filesystem hierarchy to store objects that are located by mapping
-    identifier strings to object directory (or folder) paths.
+    Pairtree storage class allowing to build a filesystem hierarchy for holding objects that are located by mapping
+    identifier strings to object directory (or folder) paths with two characters at a time.
     """
     storage_factory = None
     repository_storage_dir = None
 
     def __init__(self, repository_storage_dir, representations_directory="representations"):
         """
         Constructor initialises pairtree repository
         :param repository_storage_dir: repository storage directory
         :param representations_directory: representations directory
         """
-        super().__init__(repository_storage_dir)
+        #super().__init__(repository_storage_dir)
         self.storage_factory = PairtreeStorageFactory()
         self.repository_storage_dir = repository_storage_dir
         self.representations_directory = representations_directory
         self.repo_storage_client = self.storage_factory.get_store(store_dir=repository_storage_dir, uri_base="http://")
         self.representations_directory = representations_directory
 
     # noinspection PyProtectedMember
+    def store(self, identifier, source_file_path, progress_reporter=default_reporter):
+        """
+        Storing a directory in the pairtree path according to the given identifier. If a version of the object exists,
+        a new version is created.
+        :param identifier: identifier
+        :param source_file_path: source file path
+        :param progress_reporter: progress reporter
+        :return:
+        """
+        # pairtree object path
+        pairtree_object_path = self.repo_storage_client._id_to_dirpath(identifier)
+        # next version string
+        next_version = self._next_version(identifier)
+        # data directory
+        target_data_directory = os.path.join(pairtree_object_path, "data")
+        # create data directory path
+        pathlib.Path(target_data_directory).mkdir(parents=True, exist_ok=True)
+        # data version directory
+        target_data_version_directory = os.path.join(target_data_directory, next_version)
+        # create data version directory
+        os.makedirs(target_data_version_directory, exist_ok=True)
+
+        # archive file name
+        safe_identifier_name = to_safe_filename(identifier)
+        archive_file = "%s.tar" % safe_identifier_name
+        # check source file exists
+        if not os.path.exists(source_file_path):
+            raise ValueError("Source file does not exist: %s" % source_file_path)
+        # target file path
+        target_file_path = os.path.join(target_data_version_directory, archive_file)
+        # copy file
+        shutil.copy2(source_file_path, target_file_path)
+        progress_reporter(100)
+        return next_version
+
+
+    def get_bag_name(self, identifier: str, version: str, bagnr: int):
+        safe_identifier_name = to_safe_filename(identifier)
+        bag_dir_name = "b%05d" % int(bagnr)
+        bag_name = "%s_%s_%s" % (safe_identifier_name, version, bag_dir_name)
+        return bag_name
+
+    def identifier_object_exists(self, identifier):
+        """
+        Verify if an object of the given identifier exists in the repository
+
+        @type       identifier: string
+        @param      identifier: Identifier
+        @rtype:     boolean
+        @return:    True if the object exists, false otherwise
+        """
+        logger.debug("Looking for object at path: %s/data" % (self.repo_storage_client._id_to_dirpath(identifier)))
+        return self.repo_storage_client.exists(identifier, os.path.join("data"))
+
+    def identifier_version_object_exists(self, identifier, version_num):
+        """
+        Verify if the given version of the object exists in the repository
+        :param identifier: identifier
+        :param version_num: version number
+        :return:
+        """
+        version = VersionDirFormat % version_num
+        return self.repo_storage_client.exists(identifier, "data/%s" % version)
+
+    def _get_version_parts(self, identifier):
+        """
+        Get version directories
+        :param identifier: identifier
+        :return: version parts
+        """
+        return self.repo_storage_client.list_parts(identifier, "data")
+
+    def _next_version(self, identifier):
+        """
+        Get next formatted version directory name
+        :param identifier: identifier
+        :return: next formatted version directory name
+        """
+        if not self.identifier_object_exists(identifier):
+            return VersionDirFormat % 0
+        version_num = 1
+        while self.identifier_version_object_exists(identifier, version_num):
+            version_num += 1
+        return VersionDirFormat % version_num
+
+    def curr_version(self, identifier):
+        """
+        Get current formatted version directory name
+        :param identifier: identifier
+        :return: current formatted version directory name
+        """
+        curr_version_num = self.curr_version_num(identifier)
+        return VersionDirFormat % curr_version_num
+
+    def curr_version_num(self, identifier):
+        """
+        Get current version number
+        :param identifier: identifier
+        :return: current version number
+        """
+        if not self.identifier_object_exists(identifier):
+            return -1
+        version_num = 0
+        while self.identifier_version_object_exists(identifier, version_num):
+            version_num += 1
+        version_num -= 1
+        return version_num
+
+    def get_object_path(self, identifier):
+        """
+        Get absolute file path of the stored object. If the version number is omitted, the path of the highest version
+        number is returned.
+        :param identifier: identifier
+        :param version_num: version number
+        :return: absolute file path of the stored object
+        """
+        curr_version = self.curr_version(identifier)
+        dirpath = self.repo_storage_client._id_to_dirpath(identifier)
+        target_data_directory = os.path.join(dirpath, "data")
+        target_data_version_directory = os.path.join(target_data_directory, curr_version)
+        path_to_object = os.path.join(target_data_version_directory, "%s.tar" % to_safe_filename(identifier))
+        if os.path.exists(path_to_object):
+            logger.debug("Package file found at: %s" % path_to_object)
+            return path_to_object
+        raise ObjectNotFoundException("Package file not found")
+
+    def get_chunked_tar_entry_reader(self, identifier: str) -> ChunkedTarEntryReader:
+        tar_file_path = os.path.join(self.get_object_path(identifier), "%s.tar" % to_safe_filename(identifier))
+        tar_file = tarfile.open(tar_file_path, 'r')
+        return ChunkedTarEntryReader(tar_file)
+
+    # noinspection PyProtectedMember
+    def latest_version_ip_list(self) -> list:
+        """
+        Get a list of latest version packages from repository storage.
+        :return: list of latest version packages
+        """
+        files = rec_find_files(self.repository_storage_dir)
+        sortkeyfn = lambda s: s[1]
+        tuples = []
+        for repofile in files:
+            if repofile.endswith(".tar"):
+                f, _ = os.path.split(repofile)
+                version = re.search(r'v[0-9]{5,5}', f).group(0)
+                repoitem = (repofile, int(re.search(r'\d+', version).group(0)))
+                tuples.append(repoitem)
+        tuples.sort(key=sortkeyfn, reverse=True)
+        items_grouped_by_version = []
+        for key, valuesiter in groupby(tuples, key=sortkeyfn):
+            items_grouped_by_version.append(dict(version=key, items=list(v[0] for v in valuesiter)))
+        lastversionfiles = []
+        for version_items in items_grouped_by_version:
+            for item in version_items['items']:
+                p, f = os.path.split(item)
+                p2 = os.path.join(self.repository_storage_dir, p[:p.find("/data/v")])
+                obj_id = self.repo_storage_client._get_id_from_dirpath(p2)
+                if obj_id not in [x['id'] for x in lastversionfiles]:
+                    lastversionfiles.append({"id": obj_id, "version": version_items['version'], "path": item})
+        return lastversionfiles
+
+
+    # noinspection PyProtectedMember
     def get_dir_path_from_id(self, identifier):
         """
         Get directory path from id
         :param identifier: identifier
         :return: directory path
         """
         return self.repo_storage_client._id_to_dirpath(identifier)
 
-    def get_tar_file_path(self, identifier, representation_label=None):
+    def get_tar_file_path(self, identifier):
         curr_version = self.curr_version(identifier)
         dirpath = self.repo_storage_client._id_to_dirpath(identifier)
         target_data_directory = os.path.join(dirpath, "data")
         target_data_version_directory = os.path.join(target_data_directory, curr_version)
         bag_name = self.get_bag_name(identifier, curr_version, 1)
-        target_data_version_asset_directory = os.path.join(target_data_version_directory, "content", bag_name)
-        if representation_label:
-            tar_file_path = os.path.join(target_data_version_asset_directory, self.representations_directory, "%s.tar" % representation_label)
-        else:
-            tar_file_path = os.path.join(target_data_version_asset_directory, "%s.tar" % to_safe_filename(identifier))
+        target_data_version_asset_directory = os.path.join(target_data_version_directory, "content")
+        tar_file_path = os.path.join(target_data_version_asset_directory, "%s.tar" % bag_name)
         if os.path.exists(tar_file_path):
             logger.debug("Package file found at: %s" % tar_file_path)
             return tar_file_path
         raise ObjectNotFoundException("Package file not found")
 
-    def get_object_item_stream(self, identifier, representation_label, entry, tar_file=None):
+    def get_object_item_stream(self, identifier, entry, tar_file=None):
         """
         Get stream of a representation tar file entry
         :param identifier: package identifier
-        :param representation_label: label of the representation (used in directory and file names), can be empty,
-        tar assumed to be single package in that case
         :param entry: entry of the tar file
+        :tar_file: path to tar file (optional)
         :return: chunks iterator of the tar file
         """
-        object_path = self.get_object_path(identifier)
-        tar_file_name = "%s.tar" % representation_label if representation_label else to_safe_filename(identifier)
-        tar_file_path = os.path.join(object_path, self.representations_directory, tar_file_name)
+        tar_file_path = self.get_object_path(identifier)
         if os.path.exists(tar_file_path):
-            logger.debug("Packaged representation file found at: %s" % entry)
+            logger.debug("tar file found at: %s" % entry)
         t = tar_file if tar_file else tarfile.open(tar_file_path, 'r')
         logger.debug("Accessing access entry %s" % entry)
         try:
             inst = ChunkedTarEntryReader(t)
             return inst.chunks(entry)
         except KeyError:
             logger.error('ERROR: Did not find %s in tar archive' % entry)
@@ -149,64 +270,62 @@
                 files_ident = files_identical(dataset_package_file, dataset_package_stored_file)
                 if not files_ident:
                     logger.debug("New version triggered because hash of dataset packages is not identical")
                     return True
         logger.debug("New version not triggered.")
         return False
 
-    def store(self, identifier, source_directory, progress_reporter=default_reporter, single_package=True):
-        sdir = source_directory[:-1] if source_directory.endswith('/') else source_directory
-        uuid = sdir[sdir.rfind('/')+1:]
-        working_dir = sdir[:sdir.rfind('/')]
-        return self.store_working_directory(uuid, identifier, working_dir, single_package=single_package)
 
-    def store_working_directory(self, uuid, identifier, working_directory, single_package=True):
-        """
-        Store working directory either as single package or as representation packages
-        :param uuid: UUID of working directory
-        :param identifier: Object identifier
-        :param working_directory: working directory
-        :param single_package: store as single package or as representation packages
-        :return: version of the stored object
-        """
-        if single_package:
-            version = super().store(identifier, working_directory, copy_dir=True)
-        else:
-            version = self.store_working_directory_as_representation_packages(uuid, identifier, working_directory)
-        return version
+def update_state(state_xml_file, identifier, version):
+    ip_state = IpState.from_path(state_xml_file) if os.path.exists(state_xml_file) \
+        else IpState.from_parameters(0, False, last_task_value="stored")
+    ip_state.set_version(version)
+    ip_state.set_identifier(identifier)
+    ip_state.write_doc(state_xml_file)
 
-    def store_working_directory_as_representation_packages(self, uuid, identifier, working_directory):
-        """
-        Store working directory
-        :param storage_directory:
-        :param working_directory: working directory
-        :param uuid: UUID of working directory
-        :param identifier: Object identifier
-        :return: version
-        """
-        working_dir = os.path.join(working_directory, uuid)
-        trigger_nv = self.trigger_new_version(uuid, identifier, working_directory, self.repository_storage_dir)
-        nv = self._next_version(identifier)
-        cv = self.curr_version(identifier)
-        version = nv if  trigger_nv else cv
-        target_dir = os.path.join(make_storage_data_directory_path(identifier, self.repository_storage_dir), version,
-                                  to_safe_filename(identifier))
-        changed = False
-        for path, _, files in os.walk(os.path.abspath(working_dir)):
-            sub_path = path.replace(working_dir, "").lstrip("/")
-            for file in files:
-                # copy only packaged datasets, not the directories
-                if not path.startswith(os.path.join(working_dir, self.representations_directory)) \
-                        or fnmatch.fnmatch(file, "*.tar"):
-                    source = os.path.join(working_dir, sub_path, file)
-                    target = os.path.join(target_dir, sub_path, file)
-                    # copy files only if they are not identical
-                    if not files_identical(source, target):
-                        copy_file_with_base_directory(working_dir, target_dir, sub_path, file)
-                        changed = True
-        # update state in storage and working directory if any files have been changed
-        if changed:
-            storage_state_file = os.path.join(target_dir, "state.xml")
-            working_state_file = os.path.join(working_dir, "state.xml")
-            update_state(working_state_file, identifier, version)
-            shutil.copy2(working_state_file, storage_state_file)
-        return version
+
+def get_package_from_directory_storage(task_context_path, package_uuid, package_extension,
+                                       tl, config_path_storage):
+    pts = PairtreeStorage(config_path_storage)
+    parent_object_path = pts.get_object_path(package_uuid)
+
+    package_in_dip_work_dir = os.path.join(task_context_path, ("%s.%s" % (package_uuid, package_extension)))
+    package_source_size = fsize(parent_object_path)
+    tl.addinfo("Source: %s (%d)" % (parent_object_path, package_source_size))
+    tl.addinfo("Target: %s" % package_in_dip_work_dir)
+    total_bytes_read = 0
+    with open(package_in_dip_work_dir, 'wb') as target_file:
+        for chunk in FileBinaryDataChunks(parent_object_path, 65536).chunks(total_bytes_read):
+            target_file.write(chunk)
+        total_bytes_read += package_source_size
+        target_file.close()
+        check_transfer(parent_object_path, package_in_dip_work_dir)
+
+
+def make_storage_directory_path(identifier, version, config_path_storage):
+    """Used for remote (no access to storage backend)"""
+    pts = PairtreeStorage(config_path_storage)
+    return os.path.join(pts.get_dir_path_from_id(identifier), "data", version, to_safe_filename(identifier))
+
+
+def make_storage_data_directory_path(identifier, config_path_storage):
+    """Used for remote (no access to storage backend)"""
+    pts = PairtreeStorage(config_path_storage)
+    return os.path.join(pts.get_dir_path_from_id(identifier), "data")
+
+
+def get_package_from_storage(storage, task_context_path, package_uuid, package_extension, tl):
+
+    pts = PairtreeStorage(storage)
+    parent_object_path = pts.get_object_path(package_uuid)
+
+    package_in_dip_work_dir = os.path.join(task_context_path, ("%s.%s" % (package_uuid, package_extension)))
+    package_source_size = fsize(parent_object_path)
+    tl.addinfo("Source: %s (%d)" % (parent_object_path, package_source_size))
+    tl.addinfo("Target: %s" % package_in_dip_work_dir)
+    total_bytes_read = 0
+    with open(package_in_dip_work_dir, 'wb') as target_file:
+        for chunk in FileBinaryDataChunks(parent_object_path, 65536).chunks(total_bytes_read):
+            target_file.write(chunk)
+        total_bytes_read += package_source_size
+        target_file.close()
+        check_transfer(parent_object_path, package_in_dip_work_dir)
```

### Comparing `eatb-0.1.9/eatb/file_format.py` & `eatb-0.2.0/eatb/file_format.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/ipstate.py` & `eatb-0.2.0/eatb/ipstate.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/__init__.py` & `eatb-0.2.0/eatb/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/dip_parsed_premis.py` & `eatb-0.2.0/eatb/metadata/dip_parsed_premis.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/ead.py` & `eatb-0.2.0/eatb/metadata/ead.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/mets.py` & `eatb-0.2.0/eatb/metadata/mets.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/mets_generator.py` & `eatb-0.2.0/eatb/metadata/mets_generator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/mets_validation.py` & `eatb-0.2.0/eatb/metadata/mets_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class MetsValidation(object):
     '''
     Validation of the Mets file. This includes also the validation of Premis files that are linked in the amdSec!
     '''
 
     def __init__(self, root, mets_schema_file=os.path.join(ROOT, "eatb/resources/schemas/mets.xsd"),
-                 premis_schema_file=os.path.join(ROOT, "eatb/resources/schemas/premis-v2-2.xsd")):
+                 premis_schema_file=os.path.join(ROOT, "eatb/resources/schemas/premis-v3-0.xsd")):
         self.validation_errors = []
         self.total_files = 0
         self.schema_mets = etree.XMLSchema(file=mets_schema_file)
         self.schema_premis = etree.XMLSchema(file=premis_schema_file)
         self.rootpath = root
         self.subsequent_mets = []
```

### Comparing `eatb-0.1.9/eatb/metadata/parsed_dcat.py` & `eatb-0.2.0/eatb/metadata/parsed_dcat.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/parsed_ead.py` & `eatb-0.2.0/eatb/metadata/parsed_ead.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/parsed_mets.py` & `eatb-0.2.0/eatb/metadata/parsed_mets.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/parsed_premis.py` & `eatb-0.2.0/eatb/metadata/parsed_premis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from lxml import objectify
 from eatb.utils.XmlHelper import sequence_insert
 
-PREMIS_NS = 'info:lc/xmlns/premis-v2'
-PREMIS_NSMAP = {None: PREMIS_NS}
-P = objectify.ElementMaker(
-    annotate=False,
-    namespace=PREMIS_NS,
-    nsmap=PREMIS_NSMAP)
-
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from datetime import datetime
 
 from lxml import etree, objectify
 
 from eatb.utils.XmlHelper import q, XSI_NS
 
-PREMIS_NS = 'info:lc/xmlns/premis-v2'
+PREMIS_NS = 'http://www.loc.gov/premis/v3'
 PREMIS_NSMAP = {None: PREMIS_NS}
 P = objectify.ElementMaker(
     annotate=False,
     namespace=PREMIS_NS,
     nsmap=PREMIS_NSMAP)
 
 
 class ParsedPremis:
 
     premis_successor_sections = ['object', 'event', 'agent', 'right']
 
     def __init__(self, f=None):
         if f is None:
             self.root = P.premis(
-                {q(XSI_NS, 'schemaLocation'): PREMIS_NS + ' ../schemas/premis-v2-2.xsd'},
+                {q(XSI_NS, 'schemaLocation'): PREMIS_NS + ' ../schemas/premis-3-0.xsd'},
             )
             self.root.set('version', '2.0')
         else:
             self.root = objectify.parse(f).getroot()
 
     def add_object(self, identifier_value):
         sequence_insert(
```

### Comparing `eatb-0.1.9/eatb/metadata/premis.py` & `eatb-0.2.0/eatb/metadata/premis.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/metadata/premis_generator.py` & `eatb-0.2.0/eatb/metadata/premis_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,17 +256,17 @@
             path_premis = os.path.join(self.root_path, 'metadata/preservation/premis.xml')
             with open(path_premis, 'w') as output_file:
                 output_file.write(str.decode('utf-8'))
 
             return
 
     def createPremis(self, path_premis=None):
-        PREMIS_ATTRIBUTES = {"version" : "2.0"}
+        PREMIS_ATTRIBUTES = {"version" : "3.0"}
         premis = P.premis(PREMIS_ATTRIBUTES)
-        premis.attrib['{%s}schemaLocation' % XSI_NS] = "info:lc/xmlns/premis-v2 ../../schemas/premis-v2-2.xsd"
+        premis.attrib['{%s}schemaLocation' % XSI_NS] = "http://www.loc.gov/premis/v3 https://www.loc.gov/standards/premis/v3/premis-v3-0.xsd"
 
         # if there are no /data files, this will ensure that there is at least one object (the IP itself)
         premis_id = 'ID' + uuid.uuid4().__str__()
         object = P.object(
             {q(XSI_NS, 'type'): 'representation', "xmlID": premis_id},
             P.objectIdentifier(
                 P.objectIdentifierType('repository'),
```

### Comparing `eatb-0.1.9/eatb/oais_ip.py` & `eatb-0.2.0/eatb/oais_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         log.append("Checksum validity: \"%s\"" % str(valid_checksum))
         valid = (valid_checksum)
         return ValidationResult(valid, log, err)
 
 
 METS_NS = 'http://www.loc.gov/METS/'
 METSEXT_NS = 'ExtensionMETS'
-PREMIS_NS = 'info:lc/xmlns/premis-v2'
+PREMIS_NS = 'http://www.loc.gov/premis/v3'
 PREMIS_NSMAP = {None: PREMIS_NS}
 XLINK_NS = "http://www.w3.org/1999/xlink"
 METS_NSMAP = {None: METS_NS, "xlink": "http://www.w3.org/1999/xlink", "ext": METSEXT_NS,
                   "xsi": "http://www.w3.org/2001/XMLSchema-instance"}
 DELIVERY_METS_NSMAP = {None: METS_NS, "xlink": "http://www.w3.org/1999/xlink",
                            "xsi": "http://www.w3.org/2001/XMLSchema-instance"}
 P = objectify.ElementMaker(
@@ -393,15 +393,15 @@
     # def createPremis(self, enable_jhove = False):
     #     jhove_parser = None
     #     if enable_jhove == True:
     #         jhove_parser = etree.XMLParser(remove_blank_text=True)
     #
     #     PREMIS_ATTRIBUTES = {"version" : "2.0"}
     #     premis = P.premis(PREMIS_ATTRIBUTES)
-    #     premis.attrib['{%s}schemaLocation' % XSI_NS] = "info:lc/xmlns/premis-v2 ../../schemas/premis-v2-2.xsd"
+    #     premis.attrib['{%s}schemaLocation' % XSI_NS] = "http://www.loc.gov/premis/v3 ../../schemas/premis-v3-0.xsd"
     #
     #     premis_ids = []
     #     for top, dirs, files in os.walk(os.path.join(self.root_path, 'data')):
     #         for nm in files:
     #             file_name = os.path.join(top,nm)
     #             hash = self.sha256(file_name)
     #             file_url = "./%s" % os.path.relpath(file_name, self.root_path)
```

### Comparing `eatb-0.1.9/eatb/package_creator.py` & `eatb-0.2.0/eatb/package_creator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/packaging.py` & `eatb-0.2.0/eatb/packaging.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/DILCISExtensionMETS.xsd` & `eatb-0.2.0/eatb/resources/schemas/DILCISExtensionMETS.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml` & `eatb-0.2.0/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml` & `eatb-0.2.0/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/IP.xsd` & `eatb-0.2.0/eatb/resources/schemas/IP.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/csip.xsd` & `eatb-0.2.0/eatb/resources/schemas/csip.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/mets.xsd` & `eatb-0.2.0/eatb/resources/schemas/mets.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/mets_1_11.xsd` & `eatb-0.2.0/eatb/resources/schemas/mets_1_11.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/premis-v2-2.xsd` & `eatb-0.2.0/eatb/resources/schemas/premis-v2-2.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/schemas/xlink.xsd` & `eatb-0.2.0/eatb/resources/schemas/xlink.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/resources/validation_rules.xml` & `eatb-0.2.0/eatb/resources/validation_rules.xml`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/settings.cfg` & `eatb-0.2.0/eatb/settings.cfg`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/settings.py` & `eatb-0.2.0/eatb/settings.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/storage.py` & `eatb-0.2.0/eatb/storage.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/utils/datetime.py` & `eatb-0.2.0/eatb/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/utils/dictutils.py` & `eatb-0.2.0/eatb/utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/utils/encrypt.py` & `eatb-0.2.0/eatb/utils/encrypt.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/utils/fileutils.py` & `eatb-0.2.0/eatb/utils/fileutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,15 +501,15 @@
 
 def to_safe_filename(uri):
     """
     Convert URI to safe filename
     :param uri: URI
     :return: safe file name
     """
-    return uri.replace(":", "+")
+    return uri.replace(" ", "").replace(":", "+")
 
 
 class FileBinaryDataChunks(object):
     """
     Generator to iteratively read binary chunks of a large file
     """
```

### Comparing `eatb-0.1.9/eatb/utils/stringutils.py` & `eatb-0.2.0/eatb/utils/stringutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/utils/terminal.py` & `eatb-0.2.0/eatb/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb/utils/xmlutils.py` & `eatb-0.2.0/eatb/utils/xmlutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/eatb.egg-info/PKG-INFO` & `eatb-0.2.0/eatb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eatb
-Version: 0.1.9
+Version: 0.2.0
 Summary: A suite of tools for the creation of information packages for archival purposes.
 Home-page: https://www.e-ark-foundation.eu/e-ark-software-eatb
 Author: E-ARK Foundation
 Author-email: admin@e-ark-foundation.eu
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Archiving
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# eatb - eArchiving Tool Box
+# eatb - eArchiving Tool Box ![Build](https://github.com/E-ARK-Software/eatb/actions/workflows/python-app.yml/badge.svg?sanitize=true) ![Coverage](https://raw.githubusercontent.com/E-ARK-Software/eatb/master/coverage_badge.svg?sanitize=true) 
 
 ## About
 
 The archiving tool box is a suite of tools for the creation of information packages for archival purposes. The archival
 information package must follow the structure and comply with metadata requirements defined by the E-ARK specification 
 for information packages (CSIP available at https://earkcsip.dilcis.eu).
 
@@ -111,15 +111,15 @@
     |             - file1.csv                               |
     |             - file2.csv                               |
     |         - metadata/                                   |
     |         - documentation/                              |
     |-------------------------------------------------------|
     | - schemas/                                            | <--- Schema files for validation
     |     - IP_CS_mets.xsd                                  |
-    |     - premis-v2-2.xsd                                 |
+    |     - premis-v3-0.xsd                                 |
     |     - xlink.xsd                                       |
     |-------------------------------------------------------|
     | - METS.xml                                            | <--- Root METS file (structural metadata)
     `-------------------------------------------------------'
  
 ## Set up a development environment for the project
```

### Comparing `eatb-0.1.9/eatb.egg-info/SOURCES.txt` & `eatb-0.2.0/eatb.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 setup.cfg
 setup.py
 eatb/__init__.py
 eatb/checksum.py
 eatb/cli.py
 eatb/csip_validation.py
-eatb/directory_pairtree_storage.py
 eatb/file_format.py
 eatb/ipstate.py
 eatb/logging_config.ini
 eatb/oais_ip.py
 eatb/package_creator.py
 eatb/packaging.py
 eatb/pairtree_storage.py
@@ -30,14 +29,15 @@
 eatb/metadata/mets_generator.py
 eatb/metadata/mets_validation.py
 eatb/metadata/parsed_dcat.py
 eatb/metadata/parsed_ead.py
 eatb/metadata/parsed_mets.py
 eatb/metadata/parsed_premis.py
 eatb/metadata/premis.py
+eatb/metadata/premis_creator.py
 eatb/metadata/premis_generator.py
 eatb/resources/__init__.py
 eatb/resources/validation_rules.xml
 eatb/resources/schemas/DILCISExtensionMETS.xsd
 eatb/resources/schemas/DILCISExtensionMETS.xsd.xml
 eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml
 eatb/resources/schemas/IP.xsd
@@ -62,15 +62,14 @@
 tests/__init__.py
 tests/base.py
 tests/dip_premis_test.py
 tests/test_checksum.py
 tests/test_cli.py
 tests/test_csip_validation.py
 tests/test_datetime.py
-tests/test_directorypairtreestorage.py
 tests/test_encryption.py
 tests/test_extract.py
 tests/test_filehandling.py
 tests/test_formatidentification.py
 tests/test_metadata_dcat.py
 tests/test_metadata_ead.py
 tests/test_mets_generator.py
```

### Comparing `eatb-0.1.9/setup.py` & `eatb-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eatb",
-    version="0.1.9",
+    version="0.2.0",
     author="E-ARK Foundation",
     author_email="admin@e-ark-foundation.eu",
     license='MIT',
     description="A suite of tools for the creation of information packages for archival purposes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.e-ark-foundation.eu/e-ark-software-eatb",
```

### Comparing `eatb-0.1.9/tests/dip_premis_test.py` & `eatb-0.2.0/tests/dip_premis_test.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_checksum.py` & `eatb-0.2.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_cli.py` & `eatb-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_csip_validation.py` & `eatb-0.2.0/tests/test_csip_validation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_datetime.py` & `eatb-0.2.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_encryption.py` & `eatb-0.2.0/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_extract.py` & `eatb-0.2.0/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_filehandling.py` & `eatb-0.2.0/tests/test_filehandling.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_formatidentification.py` & `eatb-0.2.0/tests/test_formatidentification.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_metadata_dcat.py` & `eatb-0.2.0/tests/test_metadata_dcat.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_metadata_ead.py` & `eatb-0.2.0/tests/test_metadata_ead.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_mets_generator.py` & `eatb-0.2.0/tests/test_mets_generator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_mets_util.py` & `eatb-0.2.0/tests/test_mets_util.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_mets_validation.py` & `eatb-0.2.0/tests/test_mets_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,14 +353,14 @@
     def test_csip112(self):
         validation_result, _ = validate(self.rules_lines, self.IP_path + '/METS.xml', rule_id=112)
         self.assertTrue(validation_result)
 
     def test_IP_mets(self):
         mets_file = 'METS.xml'
         mets_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/mets_1_11.xsd')
-        premis_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/premis-v2-2.xsd')
+        premis_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/premis-v3-0.xsd')
         mets_validator = MetsValidation(self.IP_path, mets_schema_file, premis_schema_file)
         mets_validator.validate_mets(os.path.join(self.IP_path, mets_file))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eatb-0.1.9/tests/test_pairtreestorage.py` & `eatb-0.2.0/tests/test_pairtreestorage.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from eatb import ROOT
 from eatb.pairtree_storage import PairtreeStorage
 from eatb.utils import randomutils
 
 source_dir = os.path.join(ROOT, 'tests/test_resources/storage-test/')
 package_file = "xyz.tar"
+package_file_path = os.path.join(source_dir, package_file)
 repository_storage_dir = '/tmp/temp-' + randomutils.randomword(10)
 test_repo = os.path.join(ROOT, 'tests/test_resources/test-repo/')
 
 
 class TestPairtreeStorage(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
@@ -50,35 +51,21 @@
     def test_curr_version(self):
         pts = PairtreeStorage(test_repo)
         identifier = "bar"
         self.assertEqual("v00002", pts.curr_version(identifier))
 
     def test_store(self):
         pts = PairtreeStorage(repository_storage_dir)
-        pts.store("xyz", os.path.join(source_dir))
+        pts.store("xyz", package_file_path)
         self.assertEqual(0, pts.curr_version_num("xyz"))
-        pts.store("xyz", os.path.join(source_dir))
+        pts.store("xyz", package_file_path)
         self.assertEqual(1, pts.curr_version_num("xyz"))
 
     def test_get_object_path(self):
         pts = PairtreeStorage(test_repo)
-        expected = os.path.join(test_repo, "pairtree_root/ba/r/data/v00002/content/bar_v00002_b00001")
+        expected = os.path.join(test_repo, "pairtree_root/ba/r/data/v00002/bar.tar")
         actual = pts.get_object_path("bar")
         self.assertEqual(expected, actual)
 
-    def test_read_tar_file_entry_as_chunks(self):
-        pts = PairtreeStorage(test_repo)
-        identifier = "bar"
-        entry = "739f9c5f-c402-42af-a18b-3d0bdc4e8751/METS.xml"
-        chunked_tar_entry_reader = pts.get_chunked_tar_entry_reader(identifier)
-        try:
-            chunks = chunked_tar_entry_reader.chunks(entry)
-            content = ''.join([chunk.decode('utf-8') for chunk in chunks])
-            self.assertTrue(content.startswith("<?xml"))
-        except KeyError:
-            raise ObjectNotFoundException("Entry '%s' not found in package '%s'" % (entry, identifier))
-        finally:
-            chunked_tar_entry_reader.close()
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eatb-0.1.9/tests/test_parsed_mets.py` & `eatb-0.2.0/tests/test_parsed_mets.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_premis_generation.py` & `eatb-0.2.0/tests/test_premis_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     tmp_ip_dir_mig = os.path.join(temp_working_dir, test_ip_mig)
 
     test_ip_dir = os.path.join(test_source_directory, test_ip)
     test_ip_dir_mig = os.path.join(test_source_directory, test_ip_mig)
 
     premis_file_path = os.path.join(temp_working_dir, test_ip, './metadata/preservation/premis.xml')
 
-    premis_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/premis-v2-2.xsd')
+    premis_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/premis-v3-0.xsd')
 
     @classmethod
     def setUpClass(cls):
         shutil.copytree(TestPremisCreation.test_ip_dir, TestPremisCreation.tmp_ip_dir)
         shutil.copytree(TestPremisCreation.test_ip_dir_mig, TestPremisCreation.tmp_ip_dir_mig)
 
     @classmethod
@@ -49,21 +49,14 @@
 
     def test_create_premis(self):
 
         premisgen = PremisGenerator(TestPremisCreation.tmp_ip_dir)
         premisgen.createPremis()
         self.validate_xml(TestPremisCreation.premis_file_path, TestPremisCreation.premis_schema_file)
 
-    def test_reate_migration_premis(self):
-        premisgen = PremisGenerator(TestPremisCreation.tmp_ip_dir_mig)
-        premis_info = {'info': '%s/representations/repr1_mig-1/metadata/preservation/premis.xml' % TestPremisCreation.tmp_ip_dir_mig}
-        premisgen.createMigrationPremis(premis_info)
-        premis = '%s/representations/repr1_mig-1/metadata/preservation/premis.xml' % TestPremisCreation.tmp_ip_dir_mig
-        self.validate_xml(premis, TestPremisCreation.premis_schema_file)
-
     def test_add_premis_event(self):
         premisgen = PremisGenerator(TestPremisCreation.tmp_ip_dir_mig)
 
         premisinfo = {'outcome': 'success',
                       'task_name': 'SIPValidation',
                       'event_type': 'SIP validation',
                       'linked_object': 'this-is-a-package-id'}
```

### Comparing `eatb-0.1.9/tests/test_premis_manipulate.py` & `eatb-0.2.0/tests/test_premis_manipulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import eatb.metadata.premis
 from eatb import ROOT
 from eatb.metadata.parsed_premis import ParsedPremis
 from eatb.utils.xmlutils import pretty_xml_string
 from eatb.csip_validation import XmlValidation
 
 premis_skeleton = os.path.join(ROOT, 'tests/test_resources/metadata/premis/PREMIS_skeleton.xml')
-premis_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/premis-v2-2.xsd')
+premis_schema_file = os.path.join(ROOT, 'tests/test_resources/schemas/premis-v3-0.xsd')
 
 
 class TestPremisManipulate(unittest.TestCase):
 
 
     def test_premis_manipulate(self):
         with open(os.path.join(ROOT, premis_skeleton), 'r') as premis_file:
```

### Comparing `eatb-0.1.9/tests/test_stringutils.py` & `eatb-0.2.0/tests/test_stringutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_tarentryreader.py` & `eatb-0.2.0/tests/test_tarentryreader.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_unzip.py` & `eatb-0.2.0/tests/test_unzip.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_utils.py` & `eatb-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.1.9/tests/test_xml.py` & `eatb-0.2.0/tests/test_xml.py`

 * *Files identical despite different names*

