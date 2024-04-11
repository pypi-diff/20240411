# Comparing `tmp/mediaflowimage-0.0.1.tar.gz` & `tmp/mediaflowimage-1.0.0.tar.gz`

## Comparing `mediaflowimage-0.0.1.tar` & `mediaflowimage-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/admin.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/apps.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/blocks.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/forms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/models.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/tests.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/views.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/wagtail_hooks.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/migrations/__init__.py
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/LICENSE
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/README.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 mediaflowimage-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/admin.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/apps.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/blocks.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/forms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/models.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/tests.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/views.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/wagtail_hooks.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/migrations/__init__.py
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/README.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 mediaflowimage-1.0.0/PKG-INFO
```

### Comparing `mediaflowimage-0.0.1/src/mediaflowimage/wagtail_hooks.py` & `mediaflowimage-1.0.0/src/mediaflowimage/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-0.0.1/src/mediaflowimage/widgets.py` & `mediaflowimage-1.0.0/src/mediaflowimage/widgets.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-0.0.1/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js` & `mediaflowimage-1.0.0/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js`

 * *Files identical despite different names*

### Comparing `mediaflowimage-0.0.1/LICENSE` & `mediaflowimage-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaflowimage-0.0.1/pyproject.toml` & `mediaflowimage-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "mediaflowimage"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Mediaflow Europe AB", email="support@mediaflow.com" },
 ]
 description = "Wagtail image plugin for Mediaflow"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

