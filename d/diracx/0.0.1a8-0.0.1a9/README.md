# Comparing `tmp/diracx-0.0.1a8.tar.gz` & `tmp/diracx-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-0.0.1a8.tar", last modified: Thu Nov 30 08:41:04 2023, max compression
+gzip compressed data, was "diracx-0.0.1a9.tar", last modified: Sun Jan 28 09:12:50 2024, max compression
```

## Comparing `diracx-0.0.1a8.tar` & `diracx-0.0.1a9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:41:04.085972 diracx-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)    32452 2023-11-30 08:39:21.000000 diracx-0.0.1a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-30 08:41:04.085972 diracx-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-30 08:39:21.000000 diracx-0.0.1a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:41:04.085972 diracx-0.0.1a8/diracx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-30 08:41:04.000000 diracx-0.0.1a8/diracx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2023-11-30 08:39:21.000000 diracx-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:41:04.085972 diracx-0.0.1a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:50.480892 diracx-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    32452 2024-01-28 09:11:11.000000 diracx-0.0.1a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-28 09:12:50.480892 diracx-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-28 09:11:11.000000 diracx-0.0.1a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:50.480892 diracx-0.0.1a9/diracx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-28 09:12:50.000000 diracx-0.0.1a9/diracx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-28 09:11:11.000000 diracx-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:12:50.480892 diracx-0.0.1a9/setup.cfg
```

### Comparing `diracx-0.0.1a8/LICENSE` & `diracx-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `diracx-0.0.1a8/PKG-INFO` & `diracx-0.0.1a9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Client installation for users of DiracX installations
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-0.0.1a8/pyproject.toml` & `diracx-0.0.1a9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "E",    # pycodestyle errrors
     "F",    # pyflakes
     "B",    # flake8-bugbear
     "I",    # isort
     "PLE",  # pylint errors
     # "UP",   # pyUpgrade
     "FLY",  # flynt
+    "DTZ",  # flake8-datetimez
 ]
 ignore = ["B905", "B008", "B006"]
 line-length = 120
 src = ["diracx-*/src", "diracx-*/tests"]
 exclude = ["diracx-client/src/diracx/client/"]
 
 [tool.isort]
@@ -100,7 +101,10 @@
 addopts = [
     "-v",
     "--cov=diracx", "--cov-report=term-missing",
     "-pdiracx.testing", "-pdiracx.testing.osdb",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

