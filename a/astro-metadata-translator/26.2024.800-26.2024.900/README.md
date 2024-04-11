# Comparing `tmp/astro-metadata-translator-26.2024.800.tar.gz` & `tmp/astro-metadata-translator-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-metadata-translator-26.2024.800.tar", last modified: Thu Feb 22 10:43:01 2024, max compression
+gzip compressed data, was "astro-metadata-translator-26.2024.900.tar", last modified: Thu Feb 29 10:20:49 2024, max compression
```

## Comparing `astro-metadata-translator-26.2024.800.tar` & `astro-metadata-translator-26.2024.900.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.936301 astro-metadata-translator-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-22 10:43:01.936301 astro-metadata-translator-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.924301 astro-metadata-translator-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.928301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.928301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/translateheader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/writeindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/writesidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.928301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/cli/astrometadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.924301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.932301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00042600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00186800.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187600.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188000.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188200.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/observationGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/observationInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.932301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/serialize/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    50088 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.936301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/decam.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/hsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/megaprime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/sdss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/subaru.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/suprimecam.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.936301 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:01.000000 astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-22 10:43:01.940301 astro-metadata-translator-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:01.936301 astro-metadata-translator-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_cfht.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_decam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_sdss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_shadowing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_subaru.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_translate_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-02-22 10:42:49.000000 astro-metadata-translator-26.2024.800/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.184474 astro-metadata-translator-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.188474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.188474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/translateheader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writeindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writesidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.192474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/astrometadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.184474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.196474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00042600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00120800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00121800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00122800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00123800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00124800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00186800.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00187600.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188000.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/corrections/HSC/HSC-HSCA00188200.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.196474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50088 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.196474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/decam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/hsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/megaprime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/sdss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/subaru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/suprimecam.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:49.000000 astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:49.200474 astro-metadata-translator-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_cfht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_decam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_sdss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_shadowing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_subaru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_translate_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-02-29 10:20:37.000000 astro-metadata-translator-26.2024.900/tests/test_translation.py
```

### Comparing `astro-metadata-translator-26.2024.800/LICENSE` & `astro-metadata-translator-26.2024.900/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/PKG-INFO` & `astro-metadata-translator-26.2024.900/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-metadata-translator
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A translator for astronomical metadata.
 Home-page: https://github.com/lsst/astro_metadata_translator
 Author: Rubin Observatory Data Management
 Author-email: dm-admin@lists.lsst.org
 License: BSD 3-Clause License
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `astro-metadata-translator-26.2024.800/README.md` & `astro-metadata-translator-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/pyproject.toml` & `astro-metadata-translator-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/__init__.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/translateheader.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/translateheader.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/writeindex.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writeindex.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/bin/writesidecar.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/bin/writesidecar.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/cli/astrometadata.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/cli/astrometadata.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/file_helpers.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/file_helpers.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/headers.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/headers.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/indexing.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/indexing.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/observationGroup.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationGroup.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/observationInfo.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/observationInfo.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/properties.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/properties.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/serialize/fits.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/serialize/fits.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/tests.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/tests.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translator.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translator.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/__init__.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/decam.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/decam.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/fits.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/fits.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/helpers.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/helpers.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/hsc.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/hsc.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/megaprime.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/megaprime.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/sdss.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/sdss.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/subaru.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/subaru.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator/translators/suprimecam.py` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator/translators/suprimecam.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/PKG-INFO` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-metadata-translator
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A translator for astronomical metadata.
 Home-page: https://github.com/lsst/astro_metadata_translator
 Author: Rubin Observatory Data Management
 Author-email: dm-admin@lists.lsst.org
 License: BSD 3-Clause License
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `astro-metadata-translator-26.2024.800/python/astro_metadata_translator.egg-info/SOURCES.txt` & `astro-metadata-translator-26.2024.900/python/astro_metadata_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/setup.cfg` & `astro-metadata-translator-26.2024.900/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_basics.py` & `astro-metadata-translator-26.2024.900/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_cfht.py` & `astro-metadata-translator-26.2024.900/tests/test_cfht.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_decam.py` & `astro-metadata-translator-26.2024.900/tests/test_decam.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_extensions.py` & `astro-metadata-translator-26.2024.900/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_groups.py` & `astro-metadata-translator-26.2024.900/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_headers.py` & `astro-metadata-translator-26.2024.900/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_indexing.py` & `astro-metadata-translator-26.2024.900/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_sdss.py` & `astro-metadata-translator-26.2024.900/tests/test_sdss.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_shadowing.py` & `astro-metadata-translator-26.2024.900/tests/test_shadowing.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_subaru.py` & `astro-metadata-translator-26.2024.900/tests/test_subaru.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_translate_header.py` & `astro-metadata-translator-26.2024.900/tests/test_translate_header.py`

 * *Files identical despite different names*

### Comparing `astro-metadata-translator-26.2024.800/tests/test_translation.py` & `astro-metadata-translator-26.2024.900/tests/test_translation.py`

 * *Files identical despite different names*

