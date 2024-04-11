# Comparing `tmp/tg_model-1.0.1.tar.gz` & `tmp/tg_model-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_model-1.0.1.tar", last modified: Wed Mar 27 15:26:44 2024, max compression
+gzip compressed data, was "tg_model-1.0.2.tar", last modified: Thu Apr 11 13:57:07 2024, max compression
```

## Comparing `tg_model-1.0.1.tar` & `tg_model-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-03-27 15:26:44.767497 tg_model-1.0.1/
--rw-rw-r--   0 ralf      (1000) ralf      (1000)    11358 2022-05-16 19:23:11.000000 tg_model-1.0.1/LICENSE.txt
--rw-rw-r--   0 ralf      (1000) ralf      (1000)       46 2024-02-19 10:24:04.000000 tg_model-1.0.1/MANIFEST.in
--rw-r--r--   0 ralf      (1000) ralf      (1000)     8540 2024-03-27 15:26:44.767497 tg_model-1.0.1/PKG-INFO
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     8224 2024-01-30 09:41:48.000000 tg_model-1.0.1/README.MD
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      130 2023-06-09 11:50:03.000000 tg_model-1.0.1/pyproject.toml
--rw-rw-r--   0 ralf      (1000) ralf      (1000)       38 2024-03-27 15:26:44.767497 tg_model-1.0.1/setup.cfg
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      853 2024-03-27 15:26:08.000000 tg_model-1.0.1/setup.py
-drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-03-27 15:26:44.763496 tg_model-1.0.1/tg_model/
--rw-rw-r--   0 ralf      (1000) ralf      (1000)        0 2023-06-08 14:17:49.000000 tg_model-1.0.1/tg_model/__init__.py
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     8235 2024-03-27 12:50:16.000000 tg_model-1.0.1/tg_model/cli.py
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     5305 2024-03-27 08:30:48.000000 tg_model-1.0.1/tg_model/collection.py
--rw-rw-r--   0 ralf      (1000) ralf      (1000)    25894 2024-03-27 12:09:59.000000 tg_model-1.0.1/tg_model/tei.py
-drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-03-27 15:26:44.767497 tg_model-1.0.1/tg_model/templates/
-drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-03-27 15:26:44.767497 tg_model-1.0.1/tg_model/templates/collection/
-drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-03-27 15:26:44.767497 tg_model-1.0.1/tg_model/templates/collection/id/
--rw-rw-r--   0 ralf      (1000) ralf      (1000)       40 2021-09-15 07:58:02.000000 tg_model-1.0.1/tg_model/templates/collection/id/{{ id }}.work
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     1953 2024-03-27 08:32:59.000000 tg_model-1.0.1/tg_model/templates/collection/id/{{ id }}.work.meta
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      525 2024-01-23 12:07:47.000000 tg_model-1.0.1/tg_model/templates/collection/id/{{ id }}.xml.meta
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      536 2024-03-14 12:27:07.000000 tg_model-1.0.1/tg_model/templates/collection/{{ id }}.edition
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     1762 2024-03-27 10:08:56.000000 tg_model-1.0.1/tg_model/templates/collection/{{ id }}.edition.meta
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     6195 2024-03-27 12:05:58.000000 tg_model-1.0.1/tg_model/templates/collection.yaml
--rw-rw-r--   0 ralf      (1000) ralf      (1000)       38 2023-09-20 13:59:28.000000 tg_model-1.0.1/tg_model/templates/main.yaml
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      701 2023-07-03 13:36:30.000000 tg_model-1.0.1/tg_model/templates/synergy.yaml
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      623 2024-03-14 12:27:52.000000 tg_model-1.0.1/tg_model/templates/{{ collection }}.collection
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      536 2024-01-23 12:08:23.000000 tg_model-1.0.1/tg_model/templates/{{ collection }}.collection.meta
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     5701 2024-03-27 09:41:07.000000 tg_model-1.0.1/tg_model/util.py
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     2169 2024-01-26 14:19:25.000000 tg_model-1.0.1/tg_model/util_eltec.py
--rw-rw-r--   0 ralf      (1000) ralf      (1000)     2704 2024-02-08 12:01:25.000000 tg_model-1.0.1/tg_model/xml.py
--rw-rw-r--   0 ralf      (1000) ralf      (1000)    17441 2024-03-27 15:18:52.000000 tg_model-1.0.1/tg_model/yaml.py
-drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-03-27 15:26:44.767497 tg_model-1.0.1/tg_model.egg-info/
--rw-r--r--   0 ralf      (1000) ralf      (1000)     8540 2024-03-27 15:26:44.000000 tg_model-1.0.1/tg_model.egg-info/PKG-INFO
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      844 2024-03-27 15:26:44.000000 tg_model-1.0.1/tg_model.egg-info/SOURCES.txt
--rw-rw-r--   0 ralf      (1000) ralf      (1000)        1 2024-03-27 15:26:44.000000 tg_model-1.0.1/tg_model.egg-info/dependency_links.txt
--rw-rw-r--   0 ralf      (1000) ralf      (1000)      125 2024-03-27 15:26:44.000000 tg_model-1.0.1/tg_model.egg-info/entry_points.txt
--rw-rw-r--   0 ralf      (1000) ralf      (1000)       45 2024-03-27 15:26:44.000000 tg_model-1.0.1/tg_model.egg-info/requires.txt
--rw-rw-r--   0 ralf      (1000) ralf      (1000)        9 2024-03-27 15:26:44.000000 tg_model-1.0.1/tg_model.egg-info/top_level.txt
+drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-04-11 13:57:07.783389 tg_model-1.0.2/
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)    11358 2022-05-16 19:23:11.000000 tg_model-1.0.2/LICENSE.txt
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)       46 2024-02-19 10:24:04.000000 tg_model-1.0.2/MANIFEST.in
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     8540 2024-04-11 13:57:07.783389 tg_model-1.0.2/PKG-INFO
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     8224 2024-01-30 09:41:48.000000 tg_model-1.0.2/README.MD
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      130 2023-06-09 11:50:03.000000 tg_model-1.0.2/pyproject.toml
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)       38 2024-04-11 13:57:07.783389 tg_model-1.0.2/setup.cfg
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      853 2024-04-11 13:55:56.000000 tg_model-1.0.2/setup.py
+drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-04-11 13:57:07.783389 tg_model-1.0.2/tg_model/
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)        0 2023-06-08 14:17:49.000000 tg_model-1.0.2/tg_model/__init__.py
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     8235 2024-03-27 12:50:16.000000 tg_model-1.0.2/tg_model/cli.py
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     5305 2024-03-27 08:30:48.000000 tg_model-1.0.2/tg_model/collection.py
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)    27448 2024-04-11 13:51:27.000000 tg_model-1.0.2/tg_model/tei.py
+drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-04-11 13:57:07.783389 tg_model-1.0.2/tg_model/templates/
+drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-04-11 13:57:07.783389 tg_model-1.0.2/tg_model/templates/collection/
+drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-04-11 13:57:07.783389 tg_model-1.0.2/tg_model/templates/collection/id/
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)       40 2021-09-15 07:58:02.000000 tg_model-1.0.2/tg_model/templates/collection/id/{{ id }}.work
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     1953 2024-03-27 08:32:59.000000 tg_model-1.0.2/tg_model/templates/collection/id/{{ id }}.work.meta
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      525 2024-01-23 12:07:47.000000 tg_model-1.0.2/tg_model/templates/collection/id/{{ id }}.xml.meta
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      536 2024-03-14 12:27:07.000000 tg_model-1.0.2/tg_model/templates/collection/{{ id }}.edition
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     1762 2024-03-27 10:08:56.000000 tg_model-1.0.2/tg_model/templates/collection/{{ id }}.edition.meta
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     6195 2024-03-27 12:05:58.000000 tg_model-1.0.2/tg_model/templates/collection.yaml
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)       38 2023-09-20 13:59:28.000000 tg_model-1.0.2/tg_model/templates/main.yaml
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      701 2023-07-03 13:36:30.000000 tg_model-1.0.2/tg_model/templates/synergy.yaml
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      623 2024-03-14 12:27:52.000000 tg_model-1.0.2/tg_model/templates/{{ collection }}.collection
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      536 2024-01-23 12:08:23.000000 tg_model-1.0.2/tg_model/templates/{{ collection }}.collection.meta
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     5701 2024-03-27 09:41:07.000000 tg_model-1.0.2/tg_model/util.py
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     2169 2024-01-26 14:19:25.000000 tg_model-1.0.2/tg_model/util_eltec.py
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)     2704 2024-02-08 12:01:25.000000 tg_model-1.0.2/tg_model/xml.py
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)    17441 2024-04-11 13:51:14.000000 tg_model-1.0.2/tg_model/yaml.py
+drwxrwxr-x   0 ralf      (1000) ralf      (1000)        0 2024-04-11 13:57:07.783389 tg_model-1.0.2/tg_model.egg-info/
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     8540 2024-04-11 13:57:07.000000 tg_model-1.0.2/tg_model.egg-info/PKG-INFO
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      844 2024-04-11 13:57:07.000000 tg_model-1.0.2/tg_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)        1 2024-04-11 13:57:07.000000 tg_model-1.0.2/tg_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)      125 2024-04-11 13:57:07.000000 tg_model-1.0.2/tg_model.egg-info/entry_points.txt
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)       45 2024-04-11 13:57:07.000000 tg_model-1.0.2/tg_model.egg-info/requires.txt
+-rw-rw-r--   0 ralf      (1000) ralf      (1000)        9 2024-04-11 13:57:07.000000 tg_model-1.0.2/tg_model.egg-info/top_level.txt
```

### Comparing `tg_model-1.0.1/LICENSE.txt` & `tg_model-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/PKG-INFO` & `tg_model-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg_model
-Version: 1.0.1
+Version: 1.0.2
 Author: Ralf Klammer
 Author-email: ralf.klammer@tu-dresden.de
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
 Requires-Dist: iso639-lang
 Requires-Dist: jinja2
```

### Comparing `tg_model-1.0.1/README.MD` & `tg_model-1.0.2/README.MD`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/setup.py` & `tg_model-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 with open("README.MD", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="tg_model",
-    version="1.0.1",
+    version="1.0.2",
     description="",
     author="Ralf Klammer",
     author_email="ralf.klammer@tu-dresden.de",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `tg_model-1.0.1/tg_model/cli.py` & `tg_model-1.0.2/tg_model/cli.py`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/collection.py` & `tg_model-1.0.2/tg_model/collection.py`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/tei.py` & `tg_model-1.0.2/tg_model/tei.py`

 * *Files 16% similar despite different names*

```diff
@@ -78,14 +78,18 @@
         self._author_gender = None
         self._genre = None
         self._wordcount = None
         self._eltec_time_slot = None
         self._eltec_author_gender = None
         self._eltec_size = None
         self._eltec_reprint_count = None
+        self._rights_holder_url = None
+        self._rights_holder_fullname = None
+        self._rights_holder_firstname = None
+        self._rights_holder_lastname = None
         self._as_dict = None
 
     def __repr__(self):
         return "<TEIParser: %s>" % self.uri
 
     def get_via_config_value(self, value, section):
         config_val = section.get(value, None)
@@ -331,14 +335,46 @@
             self._eltec_reprint_count = self.get_via_config_value(
                 "reprint_count", self.config.optional["eltec_specs"]
             )
             # ToDo:
             #   find an alternative xpaths and build formatter
         return self._eltec_reprint_count
 
+    @property
+    def rights_holder_url(self):
+        if self._rights_holder_url is None:
+            self._rights_holder_url = self.config.content["collection"][
+                "rights_holder"
+            ]["url"]
+        return self._rights_holder_url
+
+    @property
+    def rights_holder_fullname(self):
+        if self._rights_holder_fullname is None:
+            self._rights_holder_fullname = self.config.content["collection"][
+                "rights_holder"
+            ]["fullname"]
+        return self._rights_holder_fullname
+
+    @property
+    def rights_holder_firstname(self):
+        if self._rights_holder_firstname is None:
+            self._rights_holder_firstname = self.config.content["collection"][
+                "rights_holder"
+            ]["firstname"]
+        return self._rights_holder_firstname
+
+    @property
+    def rights_holder_lastname(self):
+        if self._rights_holder_lastname is None:
+            self._rights_holder_lastname = self.config.content["collection"][
+                "rights_holder"
+            ]["lastname"]
+        return self._rights_holder_lastname
+
     # **********
 
     @property
     def as_dict(self):
         if self._as_dict is None:
             self._as_dict = {
                 "id": self.pure_filename,
@@ -362,14 +398,18 @@
                 },
                 "eltec": {
                     "time_slot": self.eltec_time_slot,
                     "gender": self.eltec_author_gender,
                     "size": self.eltec_size,
                     "reprint_count": self.eltec_reprint_count,
                 },
+                "right_holder_url": self.rights_holder_url,
+                "right_holder_forename": self.rights_holder_firstname,
+                "right_holder_surname": self.rights_holder_lastname,
+                "right_holder_name": self.rights_holder_fullname,
             }
         return self._as_dict
 
 
 class SynergyParser(TEIParser):
     def __init__(self, projectpath, *args, **kw):
         super().__init__(*args, **kw)
@@ -445,18 +485,18 @@
             )
         return self._rights_holder_lastname
 
     @property
     def as_dict(self):
         if self._as_dict is None:
             self._as_dict = {
-                "right_holder_url": self.rights_holder_url,
-                "right_holder_forename": self.rights_holder_firstname,
-                "right_holder_surname": self.rights_holder_lastname,
-                "right_holder_name": self.rights_holder_fullname,
+                # "right_holder_url": self.rights_holder_url,
+                # "right_holder_forename": self.rights_holder_firstname,
+                # "right_holder_surname": self.rights_holder_lastname,
+                # "right_holder_name": self.rights_holder_fullname,
             }
         return self._as_dict
 
 
 class SynergyAnalyzer(object):
     """
     This class helps to find completely synergetic nodes in a set of given
```

### Comparing `tg_model-1.0.1/tg_model/templates/collection/id/{{ id }}.work.meta` & `tg_model-1.0.2/tg_model/templates/collection/id/{{ id }}.work.meta`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/collection/id/{{ id }}.xml.meta` & `tg_model-1.0.2/tg_model/templates/collection/id/{{ id }}.xml.meta`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/collection/{{ id }}.edition` & `tg_model-1.0.2/tg_model/templates/collection/{{ id }}.edition`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/collection/{{ id }}.edition.meta` & `tg_model-1.0.2/tg_model/templates/collection/{{ id }}.edition.meta`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/collection.yaml` & `tg_model-1.0.2/tg_model/templates/collection.yaml`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/synergy.yaml` & `tg_model-1.0.2/tg_model/templates/synergy.yaml`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/{{ collection }}.collection` & `tg_model-1.0.2/tg_model/templates/{{ collection }}.collection`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/templates/{{ collection }}.collection.meta` & `tg_model-1.0.2/tg_model/templates/{{ collection }}.collection.meta`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/util.py` & `tg_model-1.0.2/tg_model/util.py`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/util_eltec.py` & `tg_model-1.0.2/tg_model/util_eltec.py`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/xml.py` & `tg_model-1.0.2/tg_model/xml.py`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model/yaml.py` & `tg_model-1.0.2/tg_model/yaml.py`

 * *Files identical despite different names*

### Comparing `tg_model-1.0.1/tg_model.egg-info/PKG-INFO` & `tg_model-1.0.2/tg_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg_model
-Version: 1.0.1
+Version: 1.0.2
 Author: Ralf Klammer
 Author-email: ralf.klammer@tu-dresden.de
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
 Requires-Dist: iso639-lang
 Requires-Dist: jinja2
```

### Comparing `tg_model-1.0.1/tg_model.egg-info/SOURCES.txt` & `tg_model-1.0.2/tg_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

