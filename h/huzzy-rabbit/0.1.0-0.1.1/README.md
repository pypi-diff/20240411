# Comparing `tmp/huzzy_rabbit-0.1.0.tar.gz` & `tmp/huzzy_rabbit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huzzy_rabbit-0.1.0.tar", max compression
+gzip compressed data, was "huzzy_rabbit-0.1.1.tar", max compression
```

## Comparing `huzzy_rabbit-0.1.0.tar` & `huzzy_rabbit-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.0/huzzy_rabbit/__init__.py
--rw-r--r--   0        0        0     2051 2024-03-26 10:41:34.149582 huzzy_rabbit-0.1.0/huzzy_rabbit/rabbit_mq.py
--rw-r--r--   0        0        0      291 2024-03-26 10:42:34.913578 huzzy_rabbit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 huzzy_rabbit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.1/huzzy_rabbit/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-11 14:42:53.905731 huzzy_rabbit-0.1.1/huzzy_rabbit/rabbit_mq.py
+-rw-r--r--   0        0        0      291 2024-04-11 14:44:22.765849 huzzy_rabbit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 huzzy_rabbit-0.1.1/PKG-INFO
```

