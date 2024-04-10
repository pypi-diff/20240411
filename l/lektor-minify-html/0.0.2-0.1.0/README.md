# Comparing `tmp/lektor-minify-html-0.0.2.tar.gz` & `tmp/lektor-minify-html-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-minify-html-0.0.2.tar", last modified: Sun Mar 31 15:03:50 2024, max compression
+gzip compressed data, was "lektor-minify-html-0.1.0.tar", last modified: Wed Apr 10 23:05:07 2024, max compression
```

## Comparing `lektor-minify-html-0.0.2.tar` & `lektor-minify-html-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:03:50.099944 lektor-minify-html-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-31 15:03:45.000000 lektor-minify-html-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-31 15:03:50.099944 lektor-minify-html-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-31 15:03:45.000000 lektor-minify-html-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:03:50.099944 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-31 15:03:50.000000 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 15:03:50.000000 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 15:03:50.000000 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-31 15:03:50.000000 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 15:03:50.000000 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-31 15:03:50.000000 lektor-minify-html-0.0.2/lektor_minify_html.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-31 15:03:45.000000 lektor-minify-html-0.0.2/lektor_minify_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-31 15:03:45.000000 lektor-minify-html-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 15:03:50.099944 lektor-minify-html-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:03:50.099944 lektor-minify-html-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-31 15:03:45.000000 lektor-minify-html-0.0.2/tests/test_lektor_minify_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/lektor_minify_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/tests/test_lektor_minify_html.py
```

### Comparing `lektor-minify-html-0.0.2/LICENSE` & `lektor-minify-html-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-minify-html-0.0.2/PKG-INFO` & `lektor-minify-html-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-minify-html
-Version: 0.0.2
+Version: 0.1.0
 Summary: Minify content using minify-html
 Author: seralot
 License: MIT License
         
         Copyright (c) 2024 Sergio Alonso
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,9 +27,28 @@
         
 Project-URL: Repository, https://github.com/seralot/lektor-minify-html/
 Project-URL: Issues, https://github.com/seralot/lektor-minify-html/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: minify-html
 
-# lektor-minify-html
-Lektor plugin that minifies content using minify-html.
+# Lektor minify html
+
+Use [minify-html](https://github.com/wilsonzlin/minify-html), a Rust HTML minifier meticulously optimised for speed and effectiveness, with Lektor.
+
+### Installation
+
+Use the plugins add command
+
+```bash
+  lektor plugins add lektor-minify-html
+```
+
+> For more information, see the [Lektor plugins documentation](https://www.getlektor.com/docs/plugins/)
+
+### Reference
+
+For information about what minify-html does, refer to its [documentation](https://github.com/wilsonzlin/minify-html).
+
+### License
+
+This project is distributed under the MIT License. See the [LICENSE](https://github.com/seralot/lektor-minify-html/blob/main/LICENSE) file in the repository for more details.
```

### Comparing `lektor-minify-html-0.0.2/lektor_minify_html.egg-info/PKG-INFO` & `lektor-minify-html-0.1.0/lektor_minify_html.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-minify-html
-Version: 0.0.2
+Version: 0.1.0
 Summary: Minify content using minify-html
 Author: seralot
 License: MIT License
         
         Copyright (c) 2024 Sergio Alonso
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,9 +27,28 @@
         
 Project-URL: Repository, https://github.com/seralot/lektor-minify-html/
 Project-URL: Issues, https://github.com/seralot/lektor-minify-html/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: minify-html
 
-# lektor-minify-html
-Lektor plugin that minifies content using minify-html.
+# Lektor minify html
+
+Use [minify-html](https://github.com/wilsonzlin/minify-html), a Rust HTML minifier meticulously optimised for speed and effectiveness, with Lektor.
+
+### Installation
+
+Use the plugins add command
+
+```bash
+  lektor plugins add lektor-minify-html
+```
+
+> For more information, see the [Lektor plugins documentation](https://www.getlektor.com/docs/plugins/)
+
+### Reference
+
+For information about what minify-html does, refer to its [documentation](https://github.com/wilsonzlin/minify-html).
+
+### License
+
+This project is distributed under the MIT License. See the [LICENSE](https://github.com/seralot/lektor-minify-html/blob/main/LICENSE) file in the repository for more details.
```

### Comparing `lektor-minify-html-0.0.2/lektor_minify_html.py` & `lektor-minify-html-0.1.0/lektor_minify_html.py`

 * *Files identical despite different names*

### Comparing `lektor-minify-html-0.0.2/pyproject.toml` & `lektor-minify-html-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lektor-minify-html"
-version = "0.0.2"
+version = "0.1.0"
 license = {file = "LICENSE"}
 authors = [{ name = "seralot"}]
 description = "Minify content using minify-html"
 readme = "README.md"
 dependencies = ["minify-html"]
 
 [project.urls]
```

