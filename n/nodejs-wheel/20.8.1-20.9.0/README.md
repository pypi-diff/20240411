# Comparing `tmp/nodejs_wheel-20.8.1.tar.gz` & `tmp/nodejs_wheel-20.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodejs_wheel-20.8.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "nodejs_wheel-20.9.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `nodejs_wheel-20.8.1.tar` & `nodejs_wheel-20.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1951 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/.github/workflows/build_wheel.yml
--rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/.nvmrc
--rw-r--r--   0        0        0     1928 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/CMakeLists.txt
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/LICENSE
--rw-r--r--   0        0        0     1935 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/README.md
--rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/nodejs_wheel/executable.py
--rw-r--r--   0        0        0     1135 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/pyproject.toml
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/renovate.json
--rw-r--r--   0        0        0     3478 2022-11-09 12:37:21.000000 nodejs_wheel-20.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1951 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/.github/workflows/build_wheel.yml
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/.nvmrc
+-rw-r--r--   0        0        0     1928 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/LICENSE
+-rw-r--r--   0        0        0     1935 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/README.md
+-rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/nodejs_wheel/executable.py
+-rw-r--r--   0        0        0     1135 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/pyproject.toml
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/renovate.json
+-rw-r--r--   0        0        0     3478 2022-11-09 12:37:21.000000 nodejs_wheel-20.9.0/PKG-INFO
```

### Comparing `nodejs_wheel-20.8.1/.github/workflows/build_wheel.yml` & `nodejs_wheel-20.9.0/.github/workflows/build_wheel.yml`

 * *Files identical despite different names*

### Comparing `nodejs_wheel-20.8.1/CMakeLists.txt` & `nodejs_wheel-20.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nodejs_wheel-20.8.1/LICENSE` & `nodejs_wheel-20.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodejs_wheel-20.8.1/README.md` & `nodejs_wheel-20.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nodejs_wheel-20.8.1/nodejs_wheel/executable.py` & `nodejs_wheel-20.9.0/nodejs_wheel/executable.py`

 * *Files identical despite different names*

### Comparing `nodejs_wheel-20.8.1/pyproject.toml` & `nodejs_wheel-20.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nodejs_wheel-20.8.1/PKG-INFO` & `nodejs_wheel-20.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodejs-wheel
-Version: 20.8.1
+Version: 20.9.0
 Summary: unoffical Node.js package
 Keywords: nodejs
 Author-Email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License: Copyright 2023 Jinzhe Zeng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

