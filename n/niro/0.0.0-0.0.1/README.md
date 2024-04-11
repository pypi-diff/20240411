# Comparing `tmp/niro-0.0.0.tar.gz` & `tmp/niro-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niro-0.0.0.tar", max compression
+gzip compressed data, was "niro-0.0.1.tar", max compression
```

## Comparing `niro-0.0.0.tar` & `niro-0.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-11 12:32:42.191798 niro-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-11 12:33:26.835379 niro-0.0.0/niro/__init__.py
--rw-r--r--   0        0        0      267 2024-04-11 12:33:20.381437 niro-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 niro-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-07 19:07:59.681186 niro-0.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 19:08:28.359815 niro-0.0.1/niro/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-07 19:15:24.996664 niro-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 niro-0.0.1/PKG-INFO
```

