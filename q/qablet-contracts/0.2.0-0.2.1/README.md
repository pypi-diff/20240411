# Comparing `tmp/qablet_contracts-0.2.0.tar.gz` & `tmp/qablet_contracts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qablet_contracts-0.2.0.tar", last modified: Tue Apr  9 16:46:10 2024, max compression
+gzip compressed data, was "qablet_contracts-0.2.1.tar", last modified: Thu Apr 11 16:00:29 2024, max compression
```

## Comparing `qablet_contracts-0.2.0.tar` & `qablet_contracts-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/docs/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/docs/specifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/docs/specifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/qablet_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/qablet_contracts/bnd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bnd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bnd/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bnd/zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/bond/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bond/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bond/zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/eq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/autocall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/cliquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/equity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/autocall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/cliquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/forward_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/dcf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/swaption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/rate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/rate/swaption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/timetable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/qablet_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/test_equity.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.937814 qablet_contracts-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 16:00:29.937814 qablet_contracts-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/docs/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/docs/specifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/docs/specifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/bnd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bnd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bnd/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bnd/zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/bond/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bond/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bond/zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/eq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/autocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/cliquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts/equity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/autocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/cliquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/forward_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/swaption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/rate/swaption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/timetable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 16:00:29.937814 qablet_contracts-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/test_equity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/test_schema.py
```

### Comparing `qablet_contracts-0.2.0/LICENSE` & `qablet_contracts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.0/PKG-INFO` & `qablet_contracts-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qablet_contracts
-Version: 0.2.0
+Version: 0.2.1
 Summary: qablet_contracts created by qablet
 Home-page: https://github.com/qablet/qablet-contracts/
 Author: qablet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
 Requires-Dist: pandas
```

### Comparing `qablet_contracts-0.2.0/README.md` & `qablet_contracts-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.0/qablet_contracts/bnd/fixed.py` & `qablet_contracts-0.2.1/qablet_contracts/bnd/fixed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains examples of creating timetables for Fixed Rate Bonds.
+This module contains examples of fixed rate bonds.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
 import numpy as np
@@ -20,15 +20,15 @@
         indices=np.full(n, 0, dtype=np.int64),
         dictionary=[val],
     )
 
 
 @dataclass
 class FixedCashFlows:
-    """Create timetable from cashflows in a single currency. This example also shows how to create a timetable from arrays
+    """A set of **Fixed Cashflows** in a single currency. This example also shows how to create a timetable from arrays
     instead of a list of dictionaries, which is more efficient.
 
     Args:
         ccy: the currency of cashflows.
         times: a list or ndarray of cashflows times.
         amounts: a list ndarray of cashflows amounts.
         track: an optional identifier for the contract.
@@ -70,15 +70,15 @@
             ),
             "expressions": {},
         }
 
 
 @dataclass
 class FixedBond:
-    """Create timetable for a fixed rate bond.
+    """A **Fixed Rate Bond** pays a fixed rate at regular intervals, and the principal at maturity.
 
     Args:
         ccy: the currency of cashflows.
         coupon: the coupon rate per year.
         maturity: the maturity of the bond.
         freq: the number of coupon payments per year.
         track: an optional identifier for the contract.
@@ -86,41 +86,43 @@
     Examples:
         >>> tt = FixedBond(
             "USD", 0.05, datetime(2023, 12, 31), datetime(2025, 12, 31), "2QE"
         ).timetable()
         >>> print(tt["events"].to_pandas())
           track                      time op  quantity unit
         0       2024-06-30 00:00:00+00:00  +     0.025  USD
-        1       2024-12-31 00:00:00+00:00  +     0.050  USD
-        2       2025-06-30 00:00:00+00:00  +     0.075  USD
-        3       2025-12-31 00:00:00+00:00  +     1.100  USD
+        1       2024-12-31 00:00:00+00:00  +     0.025  USD
+        2       2025-06-30 00:00:00+00:00  +     0.025  USD
+        3       2025-12-31 00:00:00+00:00  +     1.025  USD
     """
 
     ccy: str
     coupon: float
     accrual_start: datetime
     maturity: datetime
     freq: str = "2BQE"
     track: str = ""
 
     def timetable(self):
+        # Coupon period dates including the start of first period, and end of last period.
         cpn_dates = pd.bdate_range(
             self.accrual_start,
             self.maturity,
             freq=self.freq,
-            inclusive="right",
+            inclusive="both",
         )
 
         amounts = [
-            dcf(dt, self.accrual_start) * self.coupon for dt in cpn_dates
+            dcf(end, start) * self.coupon
+            for start, end in zip(cpn_dates[:-1], cpn_dates[1:])
         ]
 
         amounts[-1] += 1  # The last payment includes the principal
         return FixedCashFlows(
-            self.ccy, cpn_dates, amounts, self.track
+            self.ccy, cpn_dates[1:], amounts, self.track
         ).timetable()
 
 
 if __name__ == "__main__":
     # Create a timetable from cashflows
     timetable = FixedCashFlows(
         "USD",
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/bnd/zero.py` & `qablet_contracts-0.2.1/qablet_contracts/bnd/zero.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-This module contains examples of creating timetables for Zero Coupon Bond and related contracts.
+This module contains examples of zero coupon bond and related contracts.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class Bond(EventsMixin):
-    """A zero coupon bond.
+    """A **zero coupon bond** pays a single fixed payment at a future time.
 
     Args:
         ccy: the currency of the bond.
-        maturity: the maturity of the bond in years.
+        maturity: the maturity of the bond.
         track: an optional identifier for the contract.
 
     Examples:
         >>> tt = Bond("USD", datetime(2025, 3, 31)).timetable()
         >>> print(tt["events"].to_pandas())
           track                      time op  quantity unit
         0       2025-03-31 00:00:00+00:00  +       1.0  USD
@@ -38,20 +38,21 @@
                 "unit": self.ccy,
             }
         ]
 
 
 @dataclass
 class BondPut(EventsMixin):
-    """Create timetable for a **zero coupon bond put**.
+    """A **zero coupon bond put** offers the holder the option to sell a zero coupon bond for
+    a fixed strike price, on the option maturity date.
 
     Args:
         ccy: the currency of the bond.
-        opt_maturity: the maturity of the option in years.
-        bond_maturity: the maturity of the option in years.
+        opt_maturity: the maturity of the option.
+        bond_maturity: the maturity of the bond.
         strike: the option strike.
         track: an optional identifier for the contract.
 
     Examples:
         >>> tt = BondPut(
             "USD", datetime(2024, 9, 30), datetime(2025, 3, 31), 0.95
         ).timetable()
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/bond/fixed.py` & `qablet_contracts-0.2.1/qablet_contracts/bond/fixed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-This module contains examples of creating timetables for Fixed Rate Bonds.
+This module contains examples of fixed rate bonds.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/bnd/fixed to create timetables with timestamps.
 """
 
 from math import ceil
 
 import numpy as np
 import pyarrow as pa
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/bond/zero.py` & `qablet_contracts-0.2.1/qablet_contracts/bond/zero.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
-This module contains examples of creating timetables for Zero Coupon Bond and related contracts.
+This module contains examples of zero coupon bond and related contracts.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/bnd/zero to create timetables with timestamps.
 """
 
 from qablet_contracts.timetable import timetable_from_dicts
 
 
 def zcb_timetable(ccy: str, maturity: float, track: str = "") -> dict:
-    """Create timetable for a **zero coupon bond**.
+    """A **zero coupon bond** pays a single fixed payment at a future time.
 
     Args:
         ccy: the currency of the bond.
         maturity: the maturity of the bond in years.
         track: an optional identifier for the contract.
 
     Examples:
@@ -34,20 +36,21 @@
 def zbp_timetable(
     ccy: str,
     opt_maturity: float,
     bond_maturity: float,
     strike: float,
     track: str = "",
 ) -> dict:
-    """Create timetable for a **zero coupon bond put**.
+    """A **zero coupon bond put** offers the holder the option to sell a zero coupon bond for
+    a fixed strike price, on the option maturity date.
 
     Args:
         ccy: the currency of the bond.
         opt_maturity: the maturity of the option in years.
-        bond_maturity: the maturity of the option in years.
+        bond_maturity: the maturity of the bond in years.
         strike: the option strike.
         track: an optional identifier for the contract.
 
     Examples:
         >>> tt = zbp_timetable("USD", 0.5, 1.0, 0.95)
         >>> tt["events"].to_pandas()
           track  time op  quantity unit
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/eq/autocall.py` & `qablet_contracts-0.2.1/qablet_contracts/eq/autocall.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Create an autocallable note timetable
+This module contains examples of autocallable notes.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
 import numpy as np
@@ -11,15 +11,20 @@
 
 from qablet_contracts.ir.dcf import dcf_30_360 as dcf
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class AutoCallable(EventsMixin):
-    """An **Autocallable Note**.
+    """In an **Autocallable Note** the note is called if the asset price is above the barrier level
+    on any of the barrier observation dates. On being called the note pays the principal and the coupon accreted
+    till the call date. At maturity, if the note is not called by then,
+
+    - if the asset is above strike, it pays the principal and the coupon at maturity.
+    - if the asset is below strike, it pays the notional scaled down.
 
     Args:
         ccy: the currency of the option.
         asset_name: the name of the underlying asset.
         initial_spot: the initial spot price of the asset.
         strike: downside participation below this strike.
         maturity: the maturity of the option in years.
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/eq/barrier.py` & `qablet_contracts-0.2.1/qablet_contracts/eq/barrier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """
-Utils for creating barrier options timetable
+This module contains examples of barrier options.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
 import pandas as pd
 
 from qablet_contracts.eq.vanilla import Option
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class OptionKO(EventsMixin):
-    """Create timetable for a **Knock Out Option**.
+    """In a **Dn/Out Option** the contract is cancelled if the underlying asset price
+    falls below the barrier level on any of the barrier observation dates.
+    In an **Up/Out Option** the contract is cancelled if the underlying asset price
+    rises above the barrier level on any of the observation dates.
 
     Args:
         ccy: the currency of the option.
         asset_name: the name of the underlying asset.
         strike: the option strike.
         maturity: the maturity of the option in years.
         is_call: true if the option is a call.
         barrier: the barrier level.
         barrier_type: the type of barrier option, e.g "Dn/Out" or "Up/Out".
         barrier_dates: the barrier observation points.
-        rebate: the rebate amount.
+        rebate: the rebate amount paid at cancellation.
         track: an optional identifier for the contract.
 
     Examples:
         >>> start = datetime(2024, 3, 31)
         >>> maturity = datetime(2024, 9, 30)
         >>> barrier_dates = pd.date_range(start, maturity, freq="2ME")
         >>> tt = OptionKO(
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/eq/cliquet.py` & `qablet_contracts-0.2.1/qablet_contracts/eq/cliquet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
-This module contains examples of creating timetables for equity cliquet contracts.
+This module contains examples of equity cliquet contracts.
 """
 
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import List
 
 import numpy as np
 import pandas as pd
 
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class Accumulator(EventsMixin):
-    """An **Accumulator Cliquet**.
+    """In an **Accumulator** the returns over consecutive periods are
+
+    - subject to a local floor and cap
+    - accumulated by adding
+    - the accumulated payoff is subject to a global floor
 
     Args:
         ccy: the currency of the bond.
         asset_name: the name of the underlying asset.
         fix_dates: the fixing times of the cliquet.
         global_floor: the global floor of the cliquet.
         local_floor: the local floor of the cliquet.
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/eq/forward.py` & `qablet_contracts-0.2.1/qablet_contracts/eq/forward.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
-Utils for creating forward starting options timetable
+This module contains examples of forward starting options.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class ForwardOption(EventsMixin):
-    """A **Forward Starting Option**.
+    """In a **Forward Starting Option** the strike price is set on a future date as
+    a predetermine percent of the stock price on the strike fixing date.
 
     Args:
         ccy: the currency of the option.
         asset_name: the name of the underlying asset.
         strike_rate: the option strike in percent of fixing.
         strike_date: the datetime at which the strike is fixed.
         maturity: the maturity of the option in years.
@@ -75,15 +76,15 @@
 
     def expressions(self):
         # Define the strike expression, return the spot itself.
         def strike_fn(inputs):
             return inputs
 
         return {
-            "FIX": {
+            f"{self.track}.FIX_K": {
                 "type": "snapper",
                 "inp": [self.asset_name],
                 "fn": strike_fn,
                 "out": [f"{self.track}.K"],
             }
         }
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/eq/rainbow.py` & `qablet_contracts-0.2.1/qablet_contracts/eq/rainbow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
-This module contains examples of creating timetables for equity rainbow options.
+This module contains examples of equity rainbow options.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class Rainbow(EventsMixin):
-    """Create timetable for an **Equity Rainbow Option**.
+    """A **Rainbow Call Option** offers the holder the option to buy the best of
+    a list of stocks (or none) for corresponding fixed strike prices, on the option maturity date.
+    Similarly, a **Rainbow Put Option** offers the holder the option to sell the worst of
+    a list of stocks (or none) for corresponding fixed strike prices.
 
     Args:
         ccy: the currency of the option.
         asset_names: the name of the underlying assets.
         strikes: the option strikes.
         notional: the notional of the option.
         maturity: the maturity of the option.
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/eq/vanilla.py` & `qablet_contracts-0.2.1/qablet_contracts/eq/vanilla.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
-This module contains examples of creating timetables for equity vanilla options.
+This module contains examples of equity vanilla options.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class Option(EventsMixin):
-    """An **Equity Vanilla Option**.
+    """An **European Call Option** offers the holder the option to buy a stock for
+    a fixed strike price, on the option maturity date.
+    Similarly, a **Put Option** offers the holder the option to sell a stock for
+    a fixed strike price.
 
     Args:
         ccy: the currency of the option.
         asset_name: the name of the underlying asset.
         strike: the option strike.
-        maturity: the maturity of the option in years.
+        maturity: the maturity of the option.
         is_call: true if the option is a call.
         track: an optional identifier for the contract.
 
     Examples:
         >>> call = Option("USD", "SPX", 2900, datetime(2024, 3, 31), True, "<SPX2900>")
         >>> call.timetable()["events"].to_pandas()
           track  time op  quantity  unit
@@ -71,11 +74,15 @@
             },
         ]
 
 
 if __name__ == "__main__":
     # Create the option timetable
     timetable = Option(
-        "USD", "SPX", 2900, datetime(2024, 3, 31), True, "<SPX2900>"
+        "USD",
+        "SPX",
+        2900,
+        datetime(2024, 3, 31),
+        True,
     ).timetable()
 
     print(timetable["events"].to_pandas())
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/equity/autocall.py` & `qablet_contracts-0.2.1/qablet_contracts/equity/autocall.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-Create an autocallable note timetable
+Create an autocallable note timetable.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/eq/autocall to create timetables with timestamps.
 """
 
 import numpy as np
 import pyarrow as pa
 
 from qablet_contracts.timetable import EVENT_SCHEMA
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/equity/barrier.py` & `qablet_contracts-0.2.1/qablet_contracts/equity/barrier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-Utils for creating barrier options timetable
+Utils for creating barrier options timetable.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/eq/barrier to create timetables with timestamps.
 """
 
 import numpy as np
 import pyarrow as pa
 
 from qablet_contracts.equity.vanilla import _option_events
 from qablet_contracts.timetable import EVENT_SCHEMA
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/equity/cliquet.py` & `qablet_contracts-0.2.1/qablet_contracts/equity/cliquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 This module contains examples of creating timetables for equity cliquet contracts.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/eq/cliquet to create timetables with timestamps.
 """
 
 from typing import List, Optional
 
 import numpy as np
 import pyarrow as pa
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/equity/forward_start.py` & `qablet_contracts-0.2.1/qablet_contracts/equity/forward_start.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-Utils for creating forward starting options timetable
+Utils for creating forward starting options timetable.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/eq/forward to create timetables with timestamps.
 """
 
 import pyarrow as pa
 
 from qablet_contracts.timetable import EVENT_SCHEMA
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/equity/rainbow.py` & `qablet_contracts-0.2.1/qablet_contracts/equity/rainbow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 This module contains examples of creating timetables for equity rainbow options.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/eq/rainbow to create timetables with timestamps.
 """
 
 from typing import List
 
 from qablet_contracts.timetable import timetable_from_dicts
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/equity/vanilla.py` & `qablet_contracts-0.2.1/qablet_contracts/equity/vanilla.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 This module contains examples of creating timetables for equity vanilla options.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/eq/vanilla to create timetables with timestamps.
 """
 
 from qablet_contracts.timetable import timetable_from_dicts
 
 
 def _option_events(ccy, asset_name, strike, maturity, is_call, track):
     events = [
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/ir/dcf.py` & `qablet_contracts-0.2.1/qablet_contracts/ir/dcf.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.0/qablet_contracts/ir/swap.py` & `qablet_contracts-0.2.1/qablet_contracts/ir/swap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains examples of creating timetables for rate contracts such as swaps and swaptions.
+This module contains examples of interest rate swaps.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
 import pandas as pd
@@ -44,15 +44,17 @@
             "unit": ccy,
         },
     ]
 
 
 @dataclass
 class Swap(EventsMixin):
-    """A **Vanilla Swap**.
+    """In a **Vanilla Swap**, at the end of each period the holder pays a fixed rate and receives a floating rate.
+    In this simple version the floating rate payment is replaced by receiving notional at the beginning of the period
+    and paying the notional at the end of the period.
 
     Args:
         ccy: the currency of the swap.
         dates: the period datetimes of the swap, including the inception and maturity.
         strike_rate: the strike rate of the swaption (in units, i.e. 0.02 means 200 bps).
         track: an optional identifier for the contract.
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/ir/swaption.py` & `qablet_contracts-0.2.1/qablet_contracts/ir/swaption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains examples of creating timetables for rate contracts such as swaps and swaptions.
+This module contains examples of interest rate swaptions.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List
 
 import pandas as pd
@@ -60,16 +60,15 @@
             )
 
         return events
 
 
 @dataclass
 class BermudaSwaption(EventsMixin):
-    """A **Co-terminal Bermuda Swaption**.
-    In a Co-terminal Bermuda swaption, the holder can exercise his option at the beginning of each swap period.
+    """In a **Co-terminal Bermuda Swaption**, the holder can exercise his option at the beginning of each swap period.
     If exercised, the holder pays and receives all remaining payments of the swap. If not exercised, there are
     no payments in the next swap period. Irrespective of the time of exercise, the swap terminates at the same date.
 
     Args:
         ccy: the currency of the swap.
         dates: the period datetimes of the underlying swap, including the inception and maturity.
         strike_rate: the strike rate of the swaption (in units, i.e. 0.02 means 200 bps).
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/rate/swaption.py` & `qablet_contracts-0.2.1/qablet_contracts/rate/swaption.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-This module contains examples of creating timetables for rate contracts such as swaps and swaptions.
+This module contains examples of interest rate swaps.
+These methods creates a timetable with floating point for time, which is now being deprecated.
+See qablet_contracts/ir/swap to create timetables with timestamps.
 """
 
 from typing import Dict, List
 
 import numpy as np
 
 from qablet_contracts.timetable import timetable_from_dicts
@@ -12,16 +14,16 @@
 def simple_swap_period(
     ccy: str, start: float, end: float, fixed_rate: float, track: str = ""
 ) -> list:
     """Simple representation of a swap period, paying fixed, receiving floating rate.
 
     Args:
         ccy: the currency of the swap.
-        start: the start of the period in years.
-        end: the end of the period in years.
+        start: the start of the period.
+        end: the end of the period.
         fixed_rate: the fixed annual rate of the swap.
         track: an optional identifier for the contract.
     """
     return [
         {
             "track": track,
             "time": start,
@@ -38,15 +40,17 @@
         },
     ]
 
 
 def swap_timetable(
     ccy: str, times: List[float], strike_rate: float, track: str = ""
 ) -> Dict:
-    """Create timetable for a **Vanilla Swap**.
+    """In a **Vanilla Swap**, at the end of each period the holder pays a fixed rate and receives a floating rate.
+    In this simple version the floating rate payment is replaced by receiving notional at the beginning of the period
+    and paying the notional at the end of the period.
 
     Args:
         ccy: the currency of the swap.
         times: the period times of the swap, including the inception and maturity.
         strike_rate: the strike rate of the swaption (in units, i.e. 0.02 means 200 bps).
         track: an optional identifier for the contract.
 
@@ -68,16 +72,16 @@
 
     return timetable_from_dicts(events)
 
 
 def swaption_timetable(
     ccy: str, times: List[float], strike_rate: float, track: str = ""
 ) -> Dict:
-    """Create timetable for a **Vanilla Swaption**.
-    In a Vanilla swaption the holder gets the opportunity to enter into the swap at the beginning of the first period.
+    """In a **Vanilla swaption** the holder gets the opportunity to enter into the swap
+    at the beginning of the first period.
 
     Args:
         ccy: the currency of the swap.
         times: the period times of the underlying swap, including the inception and maturity.
         strike_rate: the strike rate of the swaption (in units, i.e. 0.02 means 200 bps).
         track: an optional identifier for the contract.
 
@@ -110,16 +114,15 @@
 
     return timetable_from_dicts(events)
 
 
 def bermuda_swaption_timetable(
     ccy: str, times: List[float], strike_rate: float, track: str = ""
 ) -> Dict:
-    """Create timetable for a **Co-terminal Bermuda Swaption**.
-    In a Co-terminal Bermuda swaption, the holder can exercise his option at the beginning of each swap period.
+    """In a **Co-terminal Bermuda Swaption**, the holder can exercise his option at the beginning of each swap period.
     If exercised, the holder pays and receives all remaining payments of the swap. If not exercised, there are
     no payments in the next swap period. Irrespective of the time of exercise, the swap terminates at the same date.
 
 
     Args:
         ccy: the currency of the swap.
         times: the period times of the underlying swap, including the inception and maturity.
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts/timetable.py` & `qablet_contracts-0.2.1/qablet_contracts/timetable.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         pa.field("quantity", pa.float64()),
         pa.field("unit", DICT_TYPE),
     ]
 )
 
 
 def timetable_from_dicts(events: List[Dict]) -> Dict:
-    """Create timetable from a list of dicts.
+    """Create timetable from a list of dicts. This method creates a timetable
+    with floating point for time, which is now being deprecated.
 
     Args:
         events: a list of dicts with the following fields:
 
             - track: string
             - time: float
             - op: string
@@ -59,15 +60,17 @@
 
 def py_to_ts(py_dt):
     """Convert a python datetime to a pyarrow timestamp (milliseconds)."""
     return pa.scalar(py_dt, type=TS_TYPE)
 
 
 class EventsMixin(ABC):
-    """A mixin class for contracts that generates a timetable from events list."""
+    """A mixin class for contracts that generates a timetable from events list.
+    A derived class needs to implement the events method that returns a list of dicts,
+    and the expressions method (optional) that returns a dictionary of expressions, batches, and snappers."""
 
     @abstractmethod
     def events(self) -> List[Dict]: ...
 
     def expressions(self) -> Dict:
         return {}
 
@@ -95,9 +98,9 @@
             [
                 events["track"],
                 ts_list,
                 events["op"],
                 events["quantity"],
                 events["unit"],
             ],
-            schema=EVENT_SCHEMA,
+            schema=TS_EVENT_SCHEMA,
         )
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts.egg-info/PKG-INFO` & `qablet_contracts-0.2.1/qablet_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qablet_contracts
-Version: 0.2.0
+Version: 0.2.1
 Summary: qablet_contracts created by qablet
 Home-page: https://github.com/qablet/qablet-contracts/
 Author: qablet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
 Requires-Dist: pandas
```

### Comparing `qablet_contracts-0.2.0/qablet_contracts.egg-info/SOURCES.txt` & `qablet_contracts-0.2.1/qablet_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.0/setup.py` & `qablet_contracts-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.0/tests/test_eq.py` & `qablet_contracts-0.2.1/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.0/tests/test_equity.py` & `qablet_contracts-0.2.1/tests/test_equity.py`

 * *Files identical despite different names*

