# Comparing `tmp/ignutils-0.0.2.tar.gz` & `tmp/ignutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignutils-0.0.2.tar", last modified: Thu Apr 11 08:56:55 2024, max compression
+gzip compressed data, was "ignutils-0.0.3.tar", last modified: Thu Apr 11 09:16:53 2024, max compression
```

## Comparing `ignutils-0.0.2.tar` & `ignutils-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-04-11 08:56:55.282026 ignutils-0.0.2/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)    11356 2024-04-11 07:54:45.000000 ignutils-0.0.2/LICENSE
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      752 2024-04-11 08:56:55.282026 ignutils-0.0.2/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      133 2024-04-11 07:54:45.000000 ignutils-0.0.2/README.md
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-04-11 08:56:55.282026 ignutils-0.0.2/ignutils/
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       33 2024-04-11 07:54:45.000000 ignutils-0.0.2/ignutils/__init__.py
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)     3070 2024-04-11 07:54:45.000000 ignutils-0.0.2/ignutils/json_utils.py
-drwxrwxr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-04-11 08:56:55.282026 ignutils-0.0.2/ignutils.egg-info/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      752 2024-04-11 08:56:55.000000 ignutils-0.0.2/ignutils.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      252 2024-04-11 08:56:55.000000 ignutils-0.0.2/ignutils.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2024-04-11 08:56:55.000000 ignutils-0.0.2/ignutils.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       10 2024-04-11 08:56:55.000000 ignutils-0.0.2/ignutils.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        9 2024-04-11 08:56:55.000000 ignutils-0.0.2/ignutils.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)      806 2024-04-11 07:54:45.000000 ignutils-0.0.2/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)        9 2024-04-11 07:54:45.000000 ignutils-0.0.2/requirements.txt
--rw-rw-r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2024-04-11 08:56:55.282026 ignutils-0.0.2/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 09:16:53.361853 ignutils-0.0.3/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-11 07:58:25.000000 ignutils-0.0.3/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-11 09:16:53.361853 ignutils-0.0.3/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      602 2024-04-11 09:16:46.000000 ignutils-0.0.3/README.md
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 09:16:53.361853 ignutils-0.0.3/ignutils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       33 2024-04-11 07:58:25.000000 ignutils-0.0.3/ignutils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3070 2024-04-11 07:58:25.000000 ignutils-0.0.3/ignutils/json_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 09:16:53.361853 ignutils-0.0.3/ignutils.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      252 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       10 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      806 2024-04-11 09:16:46.000000 ignutils-0.0.3/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-11 07:58:25.000000 ignutils-0.0.3/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-11 09:16:53.361853 ignutils-0.0.3/setup.cfg
```

### Comparing `ignutils-0.0.2/LICENSE` & `ignutils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.2/ignutils/json_utils.py` & `ignutils-0.0.3/ignutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.2/pyproject.toml` & `ignutils-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ignutils"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

