# Comparing `tmp/dyff-schema-0.3.5.tar.gz` & `tmp/dyff-schema-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-schema-0.3.5.tar", last modified: Wed Apr 10 20:49:05 2024, max compression
+gzip compressed data, was "dyff-schema-0.3.7.tar", last modified: Thu Apr 11 01:15:08 2024, max compression
```

## Comparing `dyff-schema-0.3.5.tar` & `dyff-schema-0.3.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.407671 dyff-schema-0.3.5/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-10 20:49:05.406671 dyff-schema-0.3.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.388671 dyff-schema-0.3.5/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.397671 dyff-schema-0.3.5/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.399671 dyff-schema-0.3.5/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.399671 dyff-schema-0.3.5/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.400671 dyff-schema-0.3.5/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.402671 dyff-schema-0.3.5/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.403671 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.404671 dyff-schema-0.3.5/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    54641 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.406671 dyff-schema-0.3.5/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-10 20:49:05.000000 dyff-schema-0.3.5/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-10 20:49:05.000000 dyff-schema-0.3.5/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 20:49:05.000000 dyff-schema-0.3.5/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-10 20:49:05.000000 dyff-schema-0.3.5/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 20:49:05.000000 dyff-schema-0.3.5/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 20:49:05.407671 dyff-schema-0.3.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:49:05.406671 dyff-schema-0.3.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-10 20:48:59.000000 dyff-schema-0.3.5/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.876616 dyff-schema-0.3.7/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-11 01:15:08.875615 dyff-schema-0.3.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.861616 dyff-schema-0.3.7/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.868615 dyff-schema-0.3.7/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.869616 dyff-schema-0.3.7/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.869616 dyff-schema-0.3.7/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.870616 dyff-schema-0.3.7/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.871616 dyff-schema-0.3.7/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.873616 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.873616 dyff-schema-0.3.7/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    55462 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.875615 dyff-schema-0.3.7/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-11 01:15:08.000000 dyff-schema-0.3.7/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-11 01:15:08.000000 dyff-schema-0.3.7/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 01:15:08.000000 dyff-schema-0.3.7/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-11 01:15:08.000000 dyff-schema-0.3.7/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-11 01:15:08.000000 dyff-schema-0.3.7/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 01:15:08.876616 dyff-schema-0.3.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:15:08.874616 dyff-schema-0.3.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-11 01:15:03.000000 dyff-schema-0.3.7/tests/test_import.py
```

### Comparing `dyff-schema-0.3.5/.gitlab-ci.yml` & `dyff-schema-0.3.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/.pre-commit-config.yaml` & `dyff-schema-0.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/.secrets.baseline` & `dyff-schema-0.3.7/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/CODE_OF_CONDUCT.md` & `dyff-schema-0.3.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/LICENSE` & `dyff-schema-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/PKG-INFO` & `dyff-schema-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.5
+Version: 0.3.7
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.5/README.md` & `dyff-schema-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/__init__.py` & `dyff-schema-0.3.7/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/copydoc.py` & `dyff-schema-0.3.7/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/ids.py` & `dyff-schema-0.3.7/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/quantity.py` & `dyff-schema-0.3.7/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/adapters.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/base.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/__init__.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/arrow.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/binary.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/dataset/text.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/io/vllm.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/platform.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1137,41 +1137,21 @@
     level: MeasurementLevel = pydantic.Field(description="Measurement level")
     schema_: DataSchema = pydantic.Field(
         alias="schema",
         description="Schema of the measurement data. Instance-level measurements must include an _index_ field.",
     )
 
 
-class Measurement(DyffEntity, MeasurementSpec, AnalysisOutputQueryFields):
-    kind: Literal["Measurement"] = Entities.Measurement.value
-
-    def dependencies(self) -> list[str]:
-        return [self.analysis]
-
-    def resource_allocation(self) -> Optional[ResourceAllocation]:
-        return None
-
-
 class SafetyCaseSpec(DyffSchemaBaseModel):
     name: str = pydantic.Field(description="Descriptive name of the SafetyCase.")
     description: Optional[str] = pydantic.Field(
         default=None, description="Long-form description, interpreted as Markdown."
     )
 
 
-class SafetyCase(DyffEntity, SafetyCaseSpec, AnalysisOutputQueryFields):
-    kind: Literal["SafetyCase"] = Entities.SafetyCase.value
-
-    def dependencies(self) -> list[str]:
-        return [self.analysis]
-
-    def resource_allocation(self) -> Optional[ResourceAllocation]:
-        return None
-
-
 class MethodImplementationKind(str, enum.Enum):
     JupyterNotebook = "JupyterNotebook"
     PythonFunction = "PythonFunction"
 
     PythonRubric = "PythonRubric"
     """A Rubric generates an instance-level measurement, consuming a Dataset and an
     Evaluation.
@@ -1273,17 +1253,27 @@
         default=None, description="Specification of a Measurement output."
     )
     safetyCase: Optional[SafetyCaseSpec] = pydantic.Field(
         default=None, description="Specification of a SafetyCase output."
     )
 
 
+class MethodScope(str, enum.Enum):
+    InferenceService = Entities.InferenceService.value
+    Evaluation = Entities.Evaluation.value
+
+
 class MethodBase(DyffSchemaBaseModel):
     name: str = pydantic.Field(description="Descriptive name of the Method.")
 
+    scope: MethodScope = pydantic.Field(
+        description="The scope of the Method. The Method produces outputs that"
+        " are specific to one entity of the type specified in the .scope field."
+    )
+
     description: Optional[str] = pydantic.Field(
         default=None, description="Long-form description, interpreted as Markdown."
     )
 
     implementation: MethodImplementation = pydantic.Field(
         description="How the Method is implemented."
     )
@@ -1314,20 +1304,14 @@
     def dependencies(self) -> list[str]:
         return self.modules
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
         return None
 
 
-AnalysisOutputType = Union[
-    Measurement,
-    SafetyCase,
-]
-
-
 class AnalysisInput(DyffSchemaBaseModel):
     keyword: str = pydantic.Field(
         description="The 'keyword' specified for this input in the MethodSpec."
     )
     entity: str = pydantic.Field(
         description="The ID of the entity whose data should be made available as 'keyword'."
     )
@@ -1343,44 +1327,82 @@
     )
 
 
 class ForeignMethod(DyffModelWithID, MethodBase):
     pass
 
 
+class AnalysisScope(DyffSchemaBaseModel):
+    dataset: Optional[str]
+    inferenceService: Optional[str]
+    evaluation: Optional[str]
+    model: Optional[str]
+
+
 class AnalysisBase(DyffSchemaBaseModel):
+    scope: AnalysisScope = pydantic.Field(
+        description="The specific entities to which the analysis results apply."
+        " At a minimum, the field corresponding to method.scope must be set."
+    )
+
     arguments: list[AnalysisArgument] = pydantic.Field(
         default_factory=list,
         description="Arguments to pass to the Method implementation.",
     )
 
     inputs: list[AnalysisInput] = pydantic.Field(
         default_factory=list, description="Mapping of keywords to data entities."
     )
 
 
-class Analysis(DyffEntity, AnalysisBase):
-    kind: Literal["Analysis"] = Entities.Analysis.value
-
+class Analysis(AnalysisBase):
     method: ForeignMethod = pydantic.Field(
         description="The analysis Method to run.",
     )
 
+
+class Measurement(DyffEntity, MeasurementSpec, Analysis):
+    kind: Literal["Measurement"] = Entities.Measurement.value
+
     def dependencies(self) -> list[str]:
         return [self.method.id] + [x.entity for x in self.inputs]
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
         return None
 
 
-class AnalysisAndOutputs(DyffSchemaBaseModel):
-    analysis: Analysis = pydantic.Field(description="The Analysis entity")
-    outputs: list[AnalysisOutputType] = pydantic.Field(
-        description="Concrete outputs of the Analysis"
-    )
+class SafetyCase(DyffEntity, SafetyCaseSpec, Analysis):
+    kind: Literal["SafetyCase"] = Entities.SafetyCase.value
+
+    def dependencies(self) -> list[str]:
+        return [self.method.id] + [x.entity for x in self.inputs]
+
+    def resource_allocation(self) -> Optional[ResourceAllocation]:
+        return None
+
+
+# class Analysis(DyffEntity, AnalysisBase):
+#     kind: Literal["Analysis"] = Entities.Analysis.value
+
+#     method: ForeignMethod = pydantic.Field(
+#         description="The analysis Method to run.",
+#     )
+
+#     def dependencies(self) -> list[str]:
+#         return [self.method.id] + [x.entity for x in self.inputs]
+
+#     def resource_allocation(self) -> Optional[ResourceAllocation]:
+#         return None
+
+
+# class AnalysisAndOutputs(DyffSchemaBaseModel):
+#     analysis: Analysis = pydantic.Field(description="The Analysis entity")
+#     outputs: list[AnalysisOutputType] = pydantic.Field(
+#         description="Concrete outputs of the Analysis"
+#     )
 
 
 # ---------------------------------------------------------------------------
 # Status enumerations
 
 
 class _JobStatus(NamedTuple):
@@ -1638,15 +1660,14 @@
 
 
 def entity_class(kind: Entities):
     return _ENTITY_CLASS[kind]
 
 
 DyffEntityType = Union[
-    Analysis,
     Audit,
     AuditProcedure,
     DataSource,
     Dataset,
     Evaluation,
     InferenceService,
     InferenceSession,
@@ -1660,20 +1681,18 @@
 
 
 __all__ = [
     "Accelerator",
     "AcceleratorGPU",
     "AccessGrant",
     "Analysis",
-    "AnalysisAndOutputs",
     "AnalysisArgument",
     "AnalysisBase",
     "AnalysisInput",
     "AnalysisOutputQueryFields",
-    "AnalysisOutputType",
     "Annotation",
     "APIFunctions",
     "APIKey",
     "ArchiveFormat",
     "Artifact",
     "Audit",
     "AuditProcedure",
@@ -1691,14 +1710,15 @@
     "DyffModelWithID",
     "DyffSchemaBaseModel",
     "Entities",
     "Evaluation",
     "EvaluationBase",
     "ExtractorStep",
     "ForeignInferenceService",
+    "ForeignMethod",
     "ForeignModel",
     "Frameworks",
     "InferenceInterface",
     "InferenceService",
     "InferenceServiceBase",
     "InferenceServiceBuilder",
     "InferenceServiceRunner",
@@ -1724,14 +1744,15 @@
     "MethodImplementationPythonFunction",
     "MethodImplementationPythonRubric",
     "MethodInput",
     "MethodInputKind",
     "MethodOutput",
     "MethodOutputKind",
     "MethodParameter",
+    "MethodScope",
     "Model",
     "ModelArtifact",
     "ModelArtifactHuggingFaceCache",
     "ModelArtifactKind",
     "ModelBase",
     "ModelStorageMedium",
     "ModelResources",
```

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/requests.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/requests.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff/schema/v0/r1/test.py` & `dyff-schema-0.3.7/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/dyff_schema.egg-info/PKG-INFO` & `dyff-schema-0.3.7/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.5
+Version: 0.3.7
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.5/dyff_schema.egg-info/SOURCES.txt` & `dyff-schema-0.3.7/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/pyproject.toml` & `dyff-schema-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.5/tests/test_import.py` & `dyff-schema-0.3.7/tests/test_import.py`

 * *Files identical despite different names*

