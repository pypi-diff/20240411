# Comparing `tmp/dyn_libs-0.2.8.tar.gz` & `tmp/dyn_libs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyn_libs-0.2.8.tar", last modified: Tue Dec  5 16:15:57 2023, max compression
+gzip compressed data, was "dyn_libs-0.2.9.tar", last modified: Wed Dec  6 03:24:21 2023, max compression
```

## Comparing `dyn_libs-0.2.8.tar` & `dyn_libs-0.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.252384 dyn_libs-0.2.8/
--rw-r--r--   0 root         (0) root         (0)     6976 2023-12-05 16:15:57.251384 dyn_libs-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6030 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.249384 dyn_libs-0.2.8/dyn_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6976 2023-12-05 16:15:57.000000 dyn_libs-0.2.8/dyn_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1373 2023-12-05 16:15:57.000000 dyn_libs-0.2.8/dyn_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-05 16:15:57.000000 dyn_libs-0.2.8/dyn_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-05 16:15:57.000000 dyn_libs-0.2.8/dyn_libs.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-05 16:15:57.000000 dyn_libs-0.2.8/dyn_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-05 16:15:57.000000 dyn_libs-0.2.8/dyn_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.223383 dyn_libs-0.2.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.234384 dyn_libs-0.2.8/mobio/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.235384 dyn_libs-0.2.8/mobio/libs/dynamic_field/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.237384 dyn_libs-0.2.8/mobio/libs/dynamic_field/common/
--rw-r--r--   0 root         (0) root         (0)     1777 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/common/es_paginate.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.240384 dyn_libs-0.2.8/mobio/libs/dynamic_field/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9184 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py
--rw-r--r--   0 root         (0) root         (0)    13828 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.240384 dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/
--rw-r--r--   0 root         (0) root         (0)     1951 2023-12-05 16:10:53.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.242384 dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/field_helper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/field_helper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22327 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/field_helper/base_field.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.243384 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.244384 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/elastic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/elastic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/elastic/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-05 16:15:57.249384 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/base_model.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/db_manager.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/field_history_model.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/merchant_config.py
--rw-r--r--   0 root         (0) root         (0)      782 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-12-05 10:23:51.000000 dyn_libs-0.2.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-05 16:15:57.252384 dyn_libs-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9277 2023-12-05 16:15:56.000000 dyn_libs-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.777642 dyn_libs-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)     7103 2023-12-06 03:24:21.775642 dyn_libs-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6157 2023-12-06 03:18:08.000000 dyn_libs-0.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.774642 dyn_libs-0.2.9/dyn_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7103 2023-12-06 03:24:21.000000 dyn_libs-0.2.9/dyn_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-12-06 03:24:21.000000 dyn_libs-0.2.9/dyn_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-06 03:24:21.000000 dyn_libs-0.2.9/dyn_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-06 03:24:21.000000 dyn_libs-0.2.9/dyn_libs.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-12-06 03:24:21.000000 dyn_libs-0.2.9/dyn_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-06 03:24:21.000000 dyn_libs-0.2.9/dyn_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.743641 dyn_libs-0.2.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.756641 dyn_libs-0.2.9/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.757641 dyn_libs-0.2.9/mobio/libs/dynamic_field/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.759642 dyn_libs-0.2.9/mobio/libs/dynamic_field/common/
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/common/es_paginate.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.762642 dyn_libs-0.2.9/mobio/libs/dynamic_field/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py
+-rw-r--r--   0 root         (0) root         (0)    13828 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.762642 dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-12-05 16:10:53.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.765642 dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/field_helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/field_helper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22482 2023-12-06 03:18:08.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/field_helper/base_field.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.766641 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.767642 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/elastic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/elastic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/elastic/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 03:24:21.773642 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/db_manager.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/field_history_model.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/merchant_config.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-12-05 10:23:51.000000 dyn_libs-0.2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-06 03:24:21.777642 dyn_libs-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9277 2023-12-06 03:24:20.000000 dyn_libs-0.2.9/setup.py
```

### Comparing `dyn_libs-0.2.8/PKG-INFO` & `dyn_libs-0.2.9/dyn_libs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dyn_libs
-Version: 0.2.8
+Name: dyn-libs
+Version: 0.2.9
 Summary: Mobio Dynamic Fields
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,dyn_libs
@@ -205,14 +205,18 @@
 [Elastic]
 index = dyn_test
 doc_type = df
 ```
 
 
 # Change logs
+* 0.2.9
+    - Thêm index cho thuộc tính field mới
+* 0.2.8
+    - Thay đổi thuộc tính field là tiền tệ sang 88 
 * 0.2.7
     - Thêm thuộc tính field là tiền tệ 
 
 * 0.2.6
     - upgrade requests library
 * 0.2.5.1
     1) fix issue remove doc_type
```

### Comparing `dyn_libs-0.2.8/README.md` & `dyn_libs-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,18 @@
 [Elastic]
 index = dyn_test
 doc_type = df
 ```
 
 
 # Change logs
+* 0.2.9
+    - Thêm index cho thuộc tính field mới
+* 0.2.8
+    - Thay đổi thuộc tính field là tiền tệ sang 88 
 * 0.2.7
     - Thêm thuộc tính field là tiền tệ 
 
 * 0.2.6
     - upgrade requests library
 * 0.2.5.1
     1) fix issue remove doc_type
```

### Comparing `dyn_libs-0.2.8/dyn_libs.egg-info/PKG-INFO` & `dyn_libs-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dyn-libs
-Version: 0.2.8
+Name: dyn_libs
+Version: 0.2.9
 Summary: Mobio Dynamic Fields
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,dyn_libs
@@ -205,14 +205,18 @@
 [Elastic]
 index = dyn_test
 doc_type = df
 ```
 
 
 # Change logs
+* 0.2.9
+    - Thêm index cho thuộc tính field mới
+* 0.2.8
+    - Thay đổi thuộc tính field là tiền tệ sang 88 
 * 0.2.7
     - Thêm thuộc tính field là tiền tệ 
 
 * 0.2.6
     - upgrade requests library
 * 0.2.5.1
     1) fix issue remove doc_type
```

### Comparing `dyn_libs-0.2.8/dyn_libs.egg-info/SOURCES.txt` & `dyn_libs-0.2.9/dyn_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/common/__init__.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/common/es_paginate.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/common/es_paginate.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/common/utils.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/common/utils.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/controllers/i_base_dyn_controller.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/controllers/i_base_filter_controller.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/__init__.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/field_helper/base_field.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/field_helper/base_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,16 @@
             )
             return None
 
         if self.result.get(self.FIELD_PROPERTY) == DynamicFieldProperty.INTEGER:
             return {self.result.get(self.FIELD_KEY): {"type": "long"}}
         elif self.result.get(self.FIELD_PROPERTY) == DynamicFieldProperty.FLOAT:
             return {self.result.get(self.FIELD_KEY): {"type": "double"}}
+        elif self.result.get(self.FIELD_PROPERTY) == DynamicFieldProperty.CURRENCY:
+            return {self.result.get(self.FIELD_KEY): {"type": "long"}}
         if self.result.get(self.FIELD_PROPERTY) == DynamicFieldProperty.STRING:
             return {
                 self.result.get(self.FIELD_KEY): {
                     "type": "keyword",
                     "normalizer": "lowerasciinormalizer",
                 }
             }
```

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/helpers/field_helper/i_base_config.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/elastic/base_model.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/elastic/base_model.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/base_model.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/base_model.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/db_manager.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/db_manager.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/field_history_model.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/field_history_model.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/merchant_base_fields.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/merchant_config.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/merchant_config.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py` & `dyn_libs-0.2.9/mobio/libs/dynamic_field/models/mongo/staff_display_fields.py`

 * *Files identical despite different names*

### Comparing `dyn_libs-0.2.8/setup.py` & `dyn_libs-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         :param filename:
         :return:
         """
         requirements = ["m-singleton>=0.3", "requests>=2.31.0", "unidecode==1.1.1", "elasticsearch==7.17.4"]
         return requirements
 
 
-version_dev='0.2.8'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
-version_prod='0.2.7'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_dev='0.2.9'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_prod='0.2.8'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode = ''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="dyn_libs" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.2.8',  # Required, Phần này cũng không được format file.
+    version='0.2.9',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Dynamic Fields",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

