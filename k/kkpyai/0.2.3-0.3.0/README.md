# Comparing `tmp/kkpyai-0.2.3.tar.gz` & `tmp/kkpyai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.2.3.tar", max compression
+gzip compressed data, was "kkpyai-0.3.0.tar", max compression
```

## Comparing `kkpyai-0.2.3.tar` & `kkpyai-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.2.3/LICENSE
--rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.2.3/README.md
--rw-r--r--   0        0        0     1912 2024-04-07 20:52:34.507082 kkpyai-0.2.3/kkpyai/kktorch.py
--rw-r--r--   0        0        0      409 2024-04-07 20:52:48.423403 kkpyai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.3.0/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.3.0/README.md
+-rw-r--r--   0        0        0     4177 2024-04-10 15:04:17.074473 kkpyai-0.3.0/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      420 2024-04-10 15:05:02.672229 kkpyai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 kkpyai-0.3.0/PKG-INFO
```

### Comparing `kkpyai-0.2.3/LICENSE` & `kkpyai-0.3.0/LICENSE`

 * *Files identical despite different names*

