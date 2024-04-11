# Comparing `tmp/py_edgar_api-0.1.0.tar.gz` & `tmp/py_edgar_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_edgar_api-0.1.0.tar", max compression
+gzip compressed data, was "py_edgar_api-0.1.1.tar", max compression
```

## Comparing `py_edgar_api-0.1.0.tar` & `py_edgar_api-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-11 05:38:39.216667 py_edgar_api-0.1.0/README.md
--rw-r--r--   0        0        0       47 2024-04-11 05:46:53.982325 py_edgar_api-0.1.0/py_edgar_api/__init__.py
--rw-r--r--   0        0        0      149 2024-04-11 05:42:08.861786 py_edgar_api-0.1.0/py_edgar_api/client.py
--rw-r--r--   0        0        0      300 2024-04-11 05:39:27.350021 py_edgar_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 py_edgar_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-11 05:38:39.216667 py_edgar_api-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2024-04-11 17:44:22.068498 py_edgar_api-0.1.1/py_edgar_api/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-11 05:42:08.861786 py_edgar_api-0.1.1/py_edgar_api/client.py
+-rw-r--r--   0        0        0      300 2024-04-11 17:44:31.004299 py_edgar_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 py_edgar_api-0.1.1/PKG-INFO
```

