# Comparing `tmp/pelican_avatar-1.0.6.tar.gz` & `tmp/pelican_avatar-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_avatar-1.0.6.tar", last modified: Sun Apr  7 09:30:08 2024, max compression
+gzip compressed data, was "pelican_avatar-1.0.7.tar", last modified: Thu Apr 11 09:22:41 2024, max compression
```

## Comparing `pelican_avatar-1.0.6.tar` & `pelican_avatar-1.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    34523 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/LICENSE
--rw-r--r--   0        0        0     5141 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/README.md
--rw-r--r--   0        0        0     2311 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3164 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/tasks.py
--rw-r--r--   0        0        0     6609 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 09:22:34.000000 pelican_avatar-1.0.7/LICENSE
+-rw-r--r--   0        0        0     5141 2024-04-11 09:22:34.000000 pelican_avatar-1.0.7/README.md
+-rw-r--r--   0        0        0     2311 2024-04-11 09:22:34.000000 pelican_avatar-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3164 2024-04-11 09:22:34.000000 pelican_avatar-1.0.7/tasks.py
+-rw-r--r--   0        0        0     6609 2024-04-11 09:22:34.000000 pelican_avatar-1.0.7/PKG-INFO
```

### Comparing `pelican_avatar-1.0.6/LICENSE` & `pelican_avatar-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.6/README.md` & `pelican_avatar-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.6/pyproject.toml` & `pelican_avatar-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pelican-avatar"
-version = "1.0.6"
+version = "1.0.7"
 description = "Libravatar/Gravatar plugin for Pelican"
 authors = [
     { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
 ]
 readme = "README.md"
 keywords = [
     "pelican",
```

### Comparing `pelican_avatar-1.0.6/tasks.py` & `pelican_avatar-1.0.7/tasks.py`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.6/PKG-INFO` & `pelican_avatar-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-avatar
-Version: 1.0.6
+Version: 1.0.7
 Summary: Libravatar/Gravatar plugin for Pelican
 Keywords: pelican plugin libravatar gravatar
 Author-Email: Rafael Laboissière <rafael@laboissiere.net>
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
```

