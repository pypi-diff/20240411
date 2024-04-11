# Comparing `tmp/term_ascii_diagram-0.0.1.tar.gz` & `tmp/term_ascii_diagram-0.0.2.tar.gz`

## Comparing `term_ascii_diagram-0.0.1.tar` & `term_ascii_diagram-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/test
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/src/term_ascii_diagram/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/src/term_ascii_diagram/core.py
--rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/src/term_ascii_diagram/diagram.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/src/term_ascii_diagram/main.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/src/term_ascii_diagram/status_bar.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/LICENSE
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/test
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/core.py
+-rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/diagram.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/main.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/src/term_ascii_diagram/status_bar.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/LICENSE
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/README.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.2/PKG-INFO
```

### Comparing `term_ascii_diagram-0.0.1/test` & `term_ascii_diagram-0.0.2/test`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.1/src/term_ascii_diagram/core.py` & `term_ascii_diagram-0.0.2/src/term_ascii_diagram/core.py`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.1/src/term_ascii_diagram/diagram.py` & `term_ascii_diagram-0.0.2/src/term_ascii_diagram/diagram.py`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.1/src/term_ascii_diagram/main.py` & `term_ascii_diagram-0.0.2/src/term_ascii_diagram/main.py`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.1/src/term_ascii_diagram/status_bar.py` & `term_ascii_diagram-0.0.2/src/term_ascii_diagram/status_bar.py`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.1/LICENSE` & `term_ascii_diagram-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.1/pyproject.toml` & `term_ascii_diagram-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "term-ascii-diagram"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Amir Karimi", email="me@amirkarimi.dev" },
 ]
 description = "Build ASCII diagrams in terminal using keyboard."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

