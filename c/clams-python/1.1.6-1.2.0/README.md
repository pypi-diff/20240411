# Comparing `tmp/clams-python-1.1.6.tar.gz` & `tmp/clams-python-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.1.6.tar", last modified: Tue Apr  2 20:03:39 2024, max compression
+gzip compressed data, was "clams-python-1.2.0.tar", last modified: Thu Apr 11 14:18:10 2024, max compression
```

## Comparing `clams-python-1.1.6.tar` & `clams-python-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.480415 clams-python-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-02 20:03:06.000000 clams-python-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 20:03:06.000000 clams-python-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-02 20:03:39.476415 clams-python-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 20:03:06.000000 clams-python-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 20:03:06.000000 clams-python-1.1.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/app/
--rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.468416 clams-python-1.1.6/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/mmif_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/mmif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/mmif_utils/rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/mmif_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 20:03:06.000000 clams-python-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:03:39.480415 clams-python-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-02 20:03:06.000000 clams-python-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-02 20:03:06.000000 clams-python-1.1.6/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-02 20:03:06.000000 clams-python-1.1.6/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.853357 clams-python-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-11 14:17:48.000000 clams-python-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 14:17:48.000000 clams-python-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-11 14:18:10.853357 clams-python-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-11 14:17:48.000000 clams-python-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 14:17:49.000000 clams-python-1.2.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/mmif_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/mmif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/mmif_utils/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/mmif_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.853357 clams-python-1.2.0/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 14:17:49.000000 clams-python-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:18:10.853357 clams-python-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 14:17:49.000000 clams-python-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.853357 clams-python-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23502 2024-04-11 14:17:49.000000 clams-python-1.2.0/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-11 14:17:49.000000 clams-python-1.2.0/tests/test_clamscli.py
```

### Comparing `clams-python-1.1.6/LICENSE` & `clams-python-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/PKG-INFO` & `clams-python-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.1.6
+Version: 1.2.0
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.1.6/README.md` & `clams-python-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/__init__.py` & `clams-python-1.2.0/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/app/__init__.py` & `clams-python-1.2.0/clams/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,42 +186,36 @@
     def get_configuration(self, **runtime_params):
         warnings.warn("ClamsApp.get_configuration() is deprecated. "
                       "If you are using this method in `_annotate()` method,"
                       "it is no longer needed since `clams-python>1.0.9`.", 
                       DeprecationWarning, stacklevel=2)
         return self._refine_params(**runtime_params)
 
-    def sign_view(self, view: View, runtime_conf: Optional[dict] = None) -> None:
+    def sign_view(self, view: View, runtime_conf: dict) -> None:
         """
         A method to "sign" a new view that this app creates at the beginning of annotation.
         Signing will populate the view metadata with information and configuration of this app.
         The parameters passed to the :meth:`~clams.app.ClamsApp._annotate` must be
         passed to this method. This means all parameters for "common" configuration that
         are consumed in :meth:`~clams.app.ClamsApp.annotate` should not be recorded in the
         view metadata.
         :param view: a view to sign
         :param runtime_conf: runtime configuration of the app as k-v pairs
         """
-        # TODO (krim @ 8/2/23): once all devs understood this change, make runtime_conf a required argument
-        if runtime_conf is None:
-            warnings.warn("`runtime_conf` argument for ClamsApp.sign_view() will "
-                          "no longer be optional in the future. Please pass `runtime_params` "
-                          "from _annotate() method.",
-                          FutureWarning, stacklevel=2)
-            return
         view.metadata.app = self.metadata.identifier
         if self._RAW_PARAMS_KEY in runtime_conf:
             for k, v in runtime_conf.items():
                 if k == self._RAW_PARAMS_KEY:
                     for orik, oriv in v.items():
                         if orik in self.metadata.parameters and self.metadata.parameters[orik].multivalued:
                             view.metadata.add_parameter(orik, str(oriv))
                         else:
                             view.metadata.add_parameter(orik, oriv[0])
-                view.metadata.add_app_configuration(k, v)
+                else:
+                    view.metadata.add_app_configuration(k, v)
         else:
             # meaning the parameters directly from flask or argparser and values are in lists
             for k, v in runtime_conf.items():
                 if k in self.metadata.parameters and self.metadata.parameters[k].multivalued:
                     view.metadata.add_parameter(k, str(v))
                 else:
                     view.metadata.add_parameter(k, v[0])
```

### Comparing `clams-python-1.1.6/clams/appmetadata/__init__.py` & `clams-python-1.2.0/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/__init__.py` & `clams-python-1.2.0/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/app/.gitignore.template` & `clams-python-1.2.0/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/app/Containerfile.template` & `clams-python-1.2.0/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/app/README.md.template` & `clams-python-1.2.0/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/app/app.py.template` & `clams-python-1.2.0/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/app/metadata.py.template` & `clams-python-1.2.0/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/gha/for-clams-team.md.template` & `clams-python-1.2.0/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.2.0/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/mmif_utils/rewind.py` & `clams-python-1.2.0/clams/mmif_utils/rewind.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams/mmif_utils/source.py` & `clams-python-1.2.0/clams/mmif_utils/source.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import itertools
 import json
+import pathlib
 import sys
 import textwrap
-from os import path
 from typing import Union, Generator, List, Optional, Iterable
 from urllib.parse import urlparse
 
 from mmif import Mmif, Document, DocumentTypes, __specver__
 from mmif.serialize.mmif import MmifMetadata
 
 __all__ = ['WorkflowSource']
@@ -167,94 +167,51 @@
         gets re-primed.
         """
         self.prime()
         while True:
             yield self.produce()
 
 
-def generate_source_mmif_from_file(documents, prefix=None, **ignored):
-    from string import Template
+def generate_source_mmif_from_file(documents, prefix=None, scheme='file', **ignored):
     at_types = {
         'video': DocumentTypes.VideoDocument,
         'audio': DocumentTypes.AudioDocument,
         'text': DocumentTypes.TextDocument,
         'image': DocumentTypes.ImageDocument
     }
-    template = Template('''{
-          "@type": "${at_type}",
-          "properties": {
-            "id": "${aid}",
-            "mime": "${mime}",
-            "location": "${location}" }
-        }''')
     pl = WorkflowSource()
-    if prefix and not path.isabs(prefix):
-        raise ValueError(f"prefix must be an absolute path; given \"{prefix}\".")
+    if prefix:
+        prefix = pathlib.PurePosixPath(prefix)
+        if not prefix.is_absolute():
+            raise ValueError(f"prefix must be an absolute path; given \"{prefix}\".")
     for doc_id, arg in enumerate(documents, start=1):
         arg = arg.strip()
         if len(arg) < 1:
             continue
         result = arg.split(':', maxsplit=1)
         if len(result) == 2 and result[0].split('/', maxsplit=1)[0] in at_types:
             mime, location = result
         else:
             raise ValueError(
                 f'Invalid MIME types, or no MIME type and/or path provided, in argument {doc_id-1} to source'
             )
-        if prefix and path.isabs(location):
-            raise ValueError(f"when prefix is used, file location must not be an absolute path; given \"{location}\".")
-        elif not prefix and not path.isabs(location):
-            raise ValueError(f'file location must be an absolute path, or --prefix must be used; given \"{location}\".')
-        elif prefix and not path.isabs(location):
-            location = path.join(prefix, location)
-        doc = template.substitute(
-            at_type=str(at_types[mime.split('/', maxsplit=1)[0]]),
-            aid=f'd{doc_id}',
-            mime=mime,
-            location=location
-        )
-        pl.add_document(doc)
-    return pl.produce().serialize(pretty=True)
-
-
-def generate_source_mmif_from_customscheme(documents, scheme, **ignored):
-    from string import Template
-    at_types = {
-        'video': DocumentTypes.VideoDocument,
-        'audio': DocumentTypes.AudioDocument,
-        'text': DocumentTypes.TextDocument,
-        'image': DocumentTypes.ImageDocument
-    }
-    template = Template('''{
-          "@type": "${at_type}",
-          "properties": {
-            "id": "${aid}",
-            "mime": "${mime}",
-            "location": "${location}" }
-        }''')
-    pl = WorkflowSource()
-    for doc_id, arg in enumerate(documents, start=1):
-        arg = arg.strip()
-        if len(arg) < 1:
-            continue
-        result = arg.split(':', maxsplit=1)
-        if len(result) == 2 and result[0].split('/', maxsplit=1)[0] in at_types:
-            mime, location = result
-        else:
-            raise ValueError(
-                f'Invalid MIME types, or no MIME type and/or path provided, in argument {doc_id-1} to source'
-            )
-        if urlparse(location).scheme == '':
-            location = scheme + '://' + location
-        doc = template.substitute(
-            at_type=str(at_types[mime.split('/', maxsplit=1)[0]]),
-            aid=f'd{doc_id}',
-            mime=mime,
-            location=location
-        )
+        location_uri = urlparse(location, scheme=scheme)
+        if location_uri.scheme == 'file':
+            location = pathlib.PurePosixPath(location_uri.path)
+            if prefix and location.is_absolute():
+                raise ValueError(f"when prefix is used, file location must not be an absolute path; given \"{location}\".")
+            elif not prefix and not location.is_absolute():
+                raise ValueError(f'file location must be an absolute path, or --prefix must be used; given \"{location}\".')
+            elif prefix and not location.is_absolute():
+                location = prefix / location
+        doc = Document()
+        doc.at_type = at_types[mime.split('/', maxsplit=1)[0]]
+        doc.properties.location = f"{location_uri.scheme}://{location}"
+        doc.properties.id = f'd{doc_id}'
+        doc.properties.mime = mime
         pl.add_document(doc)
     return pl.produce().serialize(pretty=True)
 
 
 def describe_argparser():
     """
     returns two strings: one-line description of the argparser, and addition material, 
@@ -270,54 +227,54 @@
 def prep_argparser(**kwargs):
     parser = argparse.ArgumentParser(description=describe_argparser()[1], formatter_class=argparse.RawDescriptionHelpFormatter, **kwargs)
     parser.add_argument(
         'documents',
         default=None,
         action='store',
         nargs='+',
-        help="This list of documents should be colon-joined pairs of document types and file paths. A document type "
-             "can be one of ``audio``, ``video``, ``text``, ``image``, or a MIME type string (such as video/mp4). The "
-             "output will be a MMIF file containing a document for each of those file paths, with the appropriate "
-             "``@type`` and MIME type (if given), printed to the standard output. "
+        help='This list of documents MUST be colon-delimited pairs of document types and file locations. A document '
+             'type can be one of `audio`, `video`, `text`, `image`, or a MIME type string (such as video/mp4). The '
+             'file locations MUST be valid URI strings (e.g. `file:///path/to/file.mp4`, or URI scheme part can be '
+             'omitted, when `--scheme` flag is used). Note that when `file://` scheme is used (default), locations '
+             'MUST BE POSIX forms (Windows forms are not supported). The output will be a MMIF file containing a '
+             'document for each of those file paths, with the appropriate ``@type`` and MIME type (if given).'
     )
     parser.add_argument(
         '-p', '--prefix',
         default=None,
         metavar='PATH',
         nargs='?',
-        help='An absolute path to use as prefix for file paths (ONLY WORKS with `file` scheme, ignored otherwise). If '
-             'prefix is set, document file paths MUST be relative. Useful when creating source MMIF files from a '
-             'system that\'s different from the system that actually runs the workflow (e.g. in a container).'
+        help='An absolute path to use as prefix for file paths (ONLY WORKS with the default `file://` scheme, ignored '
+             'otherwise. MUST BE a POSIX form, Windows form is not supported). If prefix is set, document file paths '
+             'MUST be relative. Useful when creating source MMIF files from a system that\'s different from the '
+             'environment that actually runs the workflow (e.g. in a container).'
     )
     parser.add_argument(
         '-o', '--output',
         default=None,
         action='store',
         nargs='?',
         help='A name of a file to capture a generated MMIF json. When not given, MMIF is printed to stdout.'
     )
     parser.add_argument(
         '-s', '--scheme',
         default='file',
         action='store',
         nargs='?',
-        help='A scheme to associate with the document location URI. When not given, the default scheme is `file`.'
+        help='A scheme to associate with the document location URI. When not given, the default scheme is `file://`.'
     )
     return parser
 
 
 def main(args):
     if args.output:
         out_f = open(args.output, 'w')
     else:
         out_f = sys.stdout
-    if args.scheme == 'file':
-        mmif = generate_source_mmif_from_file(**vars(args))
-    else:
-        mmif = generate_source_mmif_from_customscheme(**vars(args))
+    mmif = generate_source_mmif_from_file(windows_path=False, **vars(args))
     out_f.write(mmif)
     return mmif
 
 if __name__ == '__main__':
     parser = prep_argparser()
     args = parser.parse_args()
     main(args)
```

### Comparing `clams-python-1.1.6/clams/restify/__init__.py` & `clams-python-1.2.0/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/clams_python.egg-info/PKG-INFO` & `clams-python-1.2.0/clams_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.1.6
+Version: 1.2.0
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.1.6/clams_python.egg-info/SOURCES.txt` & `clams-python-1.2.0/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/setup.py` & `clams-python-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.6/tests/test_clamsapp.py` & `clams-python-1.2.0/tests/test_clamsapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,15 +224,34 @@
         try:
             self.app.annotate(in_mmif)
         except ValueError:
             pytest.fail(f"current app ({__specver__}) should be able to process compatible input {compat_ver}.")
         in_mmif.metadata.mmif = f"http://mmif.clams.ai/{incompat_ver}"
         with pytest.raises(ValueError):
             self.app.annotate(in_mmif)
-        
+
+    def test_sign_view(self):
+        m = Mmif(self.in_mmif)
+        v1 = m.new_view()
+        self.app.sign_view(v1, {})
+        self.assertEqual(v1.metadata.app, self.app.metadata.identifier)
+        self.assertEqual(len(v1.metadata.parameters), 0)
+        v2 = m.new_view()
+        raw_query_string_arguments = {'undefined_param1': ['value1']}  # values are lists as our restifier uses `to_dict(flat=False)`
+        self.app.sign_view(v2, self.app._refine_params(**raw_query_string_arguments))
+        self.assertEqual(v2.metadata.app, self.app.metadata.identifier)
+        self.assertEqual(len(v2.metadata.parameters), 1)
+        self.assertFalse(clams.ClamsApp._RAW_PARAMS_KEY in v2.metadata.appConfiguration)
+        for param in self.app.metadata.parameters:
+            # any parameter with defaults should be recorded
+            if param.default is not None:
+                self.assertTrue(param.name in v2.metadata.appConfiguration)
+            elif param.name not in raw_query_string_arguments:
+                self.assertFalse(param.name in v2.metadata.appConfiguration)
+
     def test_annotate(self):
         # The example app is hard-coded to **always** emit version mismatch warning
         out_mmif = self.app.annotate(self.in_mmif)
         # TODO (krim @ 9/3/19): more robust test cases
         self.assertIsNotNone(out_mmif)
         out_mmif = Mmif(out_mmif)
         self.assertEqual(len(out_mmif.views), 2)
```

### Comparing `clams-python-1.1.6/tests/test_clamscli.py` & `clams-python-1.2.0/tests/test_clamscli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import copy
 import io
 import os
 import unittest
+import unittest.mock
 
 from mmif.serialize import Mmif
 from mmif.vocabulary import DocumentTypes, AnnotationTypes
 
 import clams
 from clams.mmif_utils import rewind
 from clams.mmif_utils import source
@@ -59,14 +60,18 @@
         self.assertTrue(all(map(lambda x: x.location_scheme() == 'file', source_mmif.documents)))
 
         # relative path
         self.docs.append('audio:a/b/c.mp3')
         with self.assertRaises(ValueError):
             self.generate_source_mmif()
 
+    @unittest.mock.patch('os.name', 'nt')
+    def test_on_windows(self):
+        self.test_accept_file_paths()
+
     def test_accept_prefixed_file_paths(self):
         self.prefix = '/a/b'
         self.docs.append("video:c.mp4")
         self.docs.append("text:c.txt")
         source_mmif = Mmif(self.generate_source_mmif())
         self.assertEqual(len(source_mmif.documents), 2)
```

