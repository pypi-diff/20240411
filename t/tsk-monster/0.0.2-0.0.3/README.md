# Comparing `tmp/tsk_monster-0.0.2.tar.gz` & `tmp/tsk_monster-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.2.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.3.tar", max compression
```

## Comparing `tsk_monster-0.0.2.tar` & `tsk_monster-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-09 14:44:15.334597 tsk_monster-0.0.2/README.md
--rw-r--r--   0        0        0      442 2024-04-10 20:13:29.689253 tsk_monster-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2946 2024-04-10 20:12:55.221970 tsk_monster-0.0.2/tsk_monster/__init__.py
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 tsk_monster-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1865 2024-04-11 13:40:52.853815 tsk_monster-0.0.3/README.md
+-rw-r--r--   0        0        0      583 2024-04-11 13:42:21.816148 tsk_monster-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3170 2024-04-11 13:35:42.908464 tsk_monster-0.0.3/tsk_monster/__init__.py
+-rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 tsk_monster-0.0.3/PKG-INFO
```

