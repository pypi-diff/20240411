# Comparing `tmp/sciexp2-expdef-2.1.3.tar.gz` & `tmp/sciexp2-expdef-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sciexp2-expdef-2.1.3.tar", last modified: Thu Apr 11 15:33:26 2024, max compression
+gzip compressed data, was "dist/sciexp2-expdef-2.1.4.tar", last modified: Thu Apr 11 16:09:47 2024, max compression
```

## Comparing `sciexp2-expdef-2.1.3.tar` & `sciexp2-expdef-2.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/.requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     9636 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/gridengine.py
--rw-rw-rw-   0 root         (0) root         (0)    53040 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/experiments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/
--rwxrwxrwx   0 root         (0) root         (0)     5070 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.tpl
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.dsc
--rwxrwxrwx   0 root         (0) root         (0)     2687 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/shell.tpl
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/shell.dsc
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/dacupc-gridengine.dsc
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11349 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/launcher.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/env.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/common/
--rw-rw-rw-   0 root         (0) root         (0)    14817 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/text.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16498 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14779 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4835 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/pp.py
--rw-rw-rw-   0 root         (0) root         (0)    24868 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/instance.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)    12314 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/launcher
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/.requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/system/
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/system/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     9636 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/system/gridengine.py
+-rw-rw-rw-   0 root         (0) root         (0)    53070 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/experiments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates/
+-rwxrwxrwx   0 root         (0) root         (0)     5070 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates/gridengine.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates/gridengine.dsc
+-rwxrwxrwx   0 root         (0) root         (0)     2687 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates/shell.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates/shell.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates/dacupc-gridengine.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11349 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/launcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/expdef/env.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2/common/
+-rw-rw-rw-   0 root         (0) root         (0)    14817 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/text.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16498 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14779 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/pp.py
+-rw-rw-rw-   0 root         (0) root         (0)    24868 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/sciexp2/common/instance.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-11 16:09:47.000000 sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12314 2024-04-11 16:09:28.000000 sciexp2-expdef-2.1.4/launcher
```

### Comparing `sciexp2-expdef-2.1.3/PKG-INFO` & `sciexp2-expdef-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciexp2-expdef
-Version: 2.1.3
+Version: 2.1.4
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sciexp2-expdef-2.1.3/LICENSE` & `sciexp2-expdef-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/setup.py` & `sciexp2-expdef-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/README.md` & `sciexp2-expdef-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/system/shell.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/system/shell.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/system/__init__.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/system/__init__.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/system/gridengine.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/system/gridengine.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/experiments.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/experiments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1232,20 +1232,20 @@
         self._base._experiments = new_experiments[0]
         self._base._translate |= new_experiments[1]
 
     def pack(self, template_from, template_to, dereference=None):
         """Same as `Experiments.pack`"""
         _do_pack(self, template_from, template_to, dereference=None)
 
-    def generate(self, template_from, template_to):
+    def generate(self, template_from, template_to, parallel=True):
         """Same as `Experiments.generate`"""
         _do_generate_user(self, template_from, template_to)
 
     def generate_jobs(self, system, template_to, export=[], depends=[],
-                      submit_args=[], job_desc="jobs.jd"):
+                      submit_args=[], job_desc="jobs.jd", parallel=True):
         """Same as `Experiments.generate_jobs`"""
         _do_generate_jobs(self, system, template_to, export, depends,
                       submit_args, job_desc)
 
     def translate(self, template, with_exps=False, with_unique=True):
         """Same as `Experiments.translate`"""
         return _do_translate(self._base._experiments, self._filters, self._translate,
```

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.tpl` & `sciexp2-expdef-2.1.4/sciexp2/expdef/templates/gridengine.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.dsc` & `sciexp2-expdef-2.1.4/sciexp2/expdef/templates/gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/shell.tpl` & `sciexp2-expdef-2.1.4/sciexp2/expdef/templates/shell.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/dacupc-gridengine.dsc` & `sciexp2-expdef-2.1.4/sciexp2/expdef/templates/dacupc-gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/launcher.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/launcher.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/templates.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/templates.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/expdef/env.py` & `sciexp2-expdef-2.1.4/sciexp2/expdef/env.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/common/text.py` & `sciexp2-expdef-2.1.4/sciexp2/common/text.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/common/utils.py` & `sciexp2-expdef-2.1.4/sciexp2/common/utils.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/common/progress.py` & `sciexp2-expdef-2.1.4/sciexp2/common/progress.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/common/filter.py` & `sciexp2-expdef-2.1.4/sciexp2/common/filter.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/common/pp.py` & `sciexp2-expdef-2.1.4/sciexp2/common/pp.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2/common/instance.py` & `sciexp2-expdef-2.1.4/sciexp2/common/instance.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/PKG-INFO` & `sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciexp2-expdef
-Version: 2.1.3
+Version: 2.1.4
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/SOURCES.txt` & `sciexp2-expdef-2.1.4/sciexp2_expdef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.3/launcher` & `sciexp2-expdef-2.1.4/launcher`

 * *Files identical despite different names*

