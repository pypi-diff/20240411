# Comparing `tmp/new_rep-0.1.0.tar.gz` & `tmp/new_rep-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_rep-0.1.0.tar", max compression
+gzip compressed data, was "new_rep-0.1.1.tar", max compression
```

## Comparing `new_rep-0.1.0.tar` & `new_rep-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-11 09:03:02.877365 new_rep-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-11 09:03:02.877365 new_rep-0.1.0/new_rep/__init__.py
--rw-r--r--   0        0        0      619 2024-04-11 09:27:07.257285 new_rep-0.1.0/new_rep/tty.py
--rw-r--r--   0        0        0      262 2024-04-11 09:03:02.877365 new_rep-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 new_rep-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-11 09:03:02.877365 new_rep-0.1.1/README.md
+-rw-r--r--   0        0        0       41 2024-04-11 09:38:29.737993 new_rep-0.1.1/new_rep/__init__.py
+-rw-r--r--   0        0        0      307 2024-04-11 09:35:18.655315 new_rep-0.1.1/new_rep/tty/tty.py
+-rw-r--r--   0        0        0      355 2024-04-11 09:34:29.874582 new_rep-0.1.1/new_rep/tty/tty_object.py
+-rw-r--r--   0        0        0      262 2024-04-11 09:38:50.702271 new_rep-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 new_rep-0.1.1/PKG-INFO
```

