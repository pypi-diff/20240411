# Comparing `tmp/arxiv-downloader-0.0.1.tar.gz` & `tmp/arxiv-downloader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-downloader-0.0.1.tar", last modified: Mon Jun 28 09:27:07 2021, max compression
+gzip compressed data, was "arxiv-downloader-1.0.0.tar", last modified: Thu Apr 11 11:23:46 2024, max compression
```

## Comparing `arxiv-downloader-0.0.1.tar` & `arxiv-downloader-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2021-06-28 09:27:07.713842 arxiv-downloader-0.0.1/
--rw-r--r--   0 tak       (1000) tak       (1000)     1055 2021-06-28 08:14:47.000000 arxiv-downloader-0.0.1/LICENSE
--rw-r--r--   0 tak       (1000) tak       (1000)      678 2021-06-28 09:27:07.713842 arxiv-downloader-0.0.1/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)       68 2021-06-28 08:10:27.000000 arxiv-downloader-0.0.1/README.md
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2021-06-28 09:27:07.712841 arxiv-downloader-0.0.1/bin/
--rw-r--r--   0 tak       (1000) tak       (1000)     1174 2021-06-28 09:13:58.000000 arxiv-downloader-0.0.1/bin/arxiv-downloader
--rw-r--r--   0 tak       (1000) tak       (1000)      104 2021-06-28 08:01:31.000000 arxiv-downloader-0.0.1/pyproject.toml
--rw-r--r--   0 tak       (1000) tak       (1000)       38 2021-06-28 09:27:07.713842 arxiv-downloader-0.0.1/setup.cfg
--rw-r--r--   0 tak       (1000) tak       (1000)      988 2021-06-28 09:26:57.000000 arxiv-downloader-0.0.1/setup.py
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2021-06-28 09:27:07.712841 arxiv-downloader-0.0.1/src/
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2021-06-28 09:27:07.713842 arxiv-downloader-0.0.1/src/arxiv_downloader/
--rw-r--r--   0 tak       (1000) tak       (1000)        0 2021-06-28 09:04:48.000000 arxiv-downloader-0.0.1/src/arxiv_downloader/__init__.py
--rwxrwxr-x   0 tak       (1000) tak       (1000)     1490 2021-06-28 09:11:54.000000 arxiv-downloader-0.0.1/src/arxiv_downloader/utils.py
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2021-06-28 09:27:07.713842 arxiv-downloader-0.0.1/src/arxiv_downloader.egg-info/
--rw-r--r--   0 tak       (1000) tak       (1000)      678 2021-06-28 09:27:07.000000 arxiv-downloader-0.0.1/src/arxiv_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)      344 2021-06-28 09:27:07.000000 arxiv-downloader-0.0.1/src/arxiv_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tak       (1000) tak       (1000)        1 2021-06-28 09:27:07.000000 arxiv-downloader-0.0.1/src/arxiv_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tak       (1000) tak       (1000)       13 2021-06-28 09:27:07.000000 arxiv-downloader-0.0.1/src/arxiv_downloader.egg-info/requires.txt
--rw-r--r--   0 tak       (1000) tak       (1000)       17 2021-06-28 09:27:07.000000 arxiv-downloader-0.0.1/src/arxiv_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2024-04-11 11:23:46.406464 arxiv-downloader-1.0.0/
+-rw-r--r--   0 steven    (1000) steven    (1000)     1056 2024-04-11 11:23:20.000000 arxiv-downloader-1.0.0/LICENSE
+-rw-r--r--   0 steven    (1000) steven    (1000)     1970 2024-04-11 11:23:46.406464 arxiv-downloader-1.0.0/PKG-INFO
+-rw-r--r--   0 steven    (1000) steven    (1000)     1365 2024-04-11 11:19:19.000000 arxiv-downloader-1.0.0/README.md
+drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2024-04-11 11:23:46.405464 arxiv-downloader-1.0.0/bin/
+-rw-r--r--   0 steven    (1000) steven    (1000)     3099 2024-04-11 11:07:05.000000 arxiv-downloader-1.0.0/bin/arxiv-downloader
+-rw-r--r--   0 steven    (1000) steven    (1000)      221 2024-04-11 10:17:49.000000 arxiv-downloader-1.0.0/pyproject.toml
+-rw-r--r--   0 steven    (1000) steven    (1000)       38 2024-04-11 11:23:46.406464 arxiv-downloader-1.0.0/setup.cfg
+-rw-r--r--   0 steven    (1000) steven    (1000)      938 2024-04-11 11:01:54.000000 arxiv-downloader-1.0.0/setup.py
+drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2024-04-11 11:23:46.405464 arxiv-downloader-1.0.0/src/
+drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2024-04-11 11:23:46.405464 arxiv-downloader-1.0.0/src/arxiv_downloader/
+-rw-r--r--   0 steven    (1000) steven    (1000)        0 2024-04-11 10:09:01.000000 arxiv-downloader-1.0.0/src/arxiv_downloader/__init__.py
+drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2024-04-11 11:23:46.406464 arxiv-downloader-1.0.0/src/arxiv_downloader.egg-info/
+-rw-r--r--   0 steven    (1000) steven    (1000)     1970 2024-04-11 11:23:46.000000 arxiv-downloader-1.0.0/src/arxiv_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 steven    (1000) steven    (1000)      314 2024-04-11 11:23:46.000000 arxiv-downloader-1.0.0/src/arxiv_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 steven    (1000) steven    (1000)        1 2024-04-11 11:23:46.000000 arxiv-downloader-1.0.0/src/arxiv_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 steven    (1000) steven    (1000)       13 2024-04-11 11:23:46.000000 arxiv-downloader-1.0.0/src/arxiv_downloader.egg-info/requires.txt
+-rw-r--r--   0 steven    (1000) steven    (1000)       17 2024-04-11 11:23:46.000000 arxiv-downloader-1.0.0/src/arxiv_downloader.egg-info/top_level.txt
```

### Comparing `arxiv-downloader-0.0.1/LICENSE` & `arxiv-downloader-1.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 Steven Lang
+Copyright (c) 2024 Steven Braun
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `arxiv-downloader-0.0.1/setup.py` & `arxiv-downloader-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arxiv-downloader",
-    version="0.0.1",
-    author="Steven Lang",
-    author_email="steven.lang.mz@gmail.com  ",
+    version="1.0.0",
+    author="Steven Braun",
+    author_email="steven.braun.mz@gmail.com  ",
     description="A command line interface to download PDF files from https://arxiv.org.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/steven-lang/arxiv-downloader",
+    url="https://github.com/braun-steven/arxiv-downloader",
     project_urls={
-        "Bug Tracker": "https://github.com/steven-lang/arxiv-downloader/issues",
+        "Bug Tracker": "https://github.com/braun-steven/arxiv-downloader/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
-    # packages=setuptools.find_packages(where="src"),
     packages=["arxiv_downloader"],
     python_requires=">=3.6",
     scripts=["bin/arxiv-downloader"],
-        install_requires="arxiv==1.2.0"
+        install_requires="arxiv==2.1.0"
 )
```

