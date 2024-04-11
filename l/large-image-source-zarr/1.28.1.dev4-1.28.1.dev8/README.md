# Comparing `tmp/large-image-source-zarr-1.28.1.dev4.tar.gz` & `tmp/large-image-source-zarr-1.28.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-zarr-1.28.1.dev4.tar", last modified: Mon Apr  8 20:38:09 2024, max compression
+gzip compressed data, was "large-image-source-zarr-1.28.1.dev8.tar", last modified: Wed Apr 10 16:17:19 2024, max compression
```

## Comparing `large-image-source-zarr-1.28.1.dev4.tar` & `large-image-source-zarr-1.28.1.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 20:38:09.639869 large-image-source-zarr-1.28.1.dev4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-08 20:38:09.639869 large-image-source-zarr-1.28.1.dev4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 20:38:09.639869 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34276 2024-04-08 20:32:15.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-08 20:32:15.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 20:38:09.639869 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 20:38:09.000000 large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 20:32:15.000000 large-image-source-zarr-1.28.1.dev4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 20:38:09.639869 large-image-source-zarr-1.28.1.dev4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-08 20:32:15.000000 large-image-source-zarr-1.28.1.dev4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-10 16:17:18.000000 large-image-source-zarr-1.28.1.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-10 16:17:18.000000 large-image-source-zarr-1.28.1.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:19.125867 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34406 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/setup.py
```

### Comparing `large-image-source-zarr-1.28.1.dev4/LICENSE` & `large-image-source-zarr-1.28.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.1.dev4/PKG-INFO` & `large-image-source-zarr-1.28.1.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.28.1.dev4
+Version: 1.28.1.dev8
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.28.1.dev4/README.rst` & `large-image-source-zarr-1.28.1.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.1.dev4/large_image_source_zarr/__init__.py` & `large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -815,15 +815,18 @@
                 zarr.copy_store(source._zarr_store, zip_store, if_exists='replace')
                 zip_store.close()
 
         else:
             from large_image_converter import convert
 
             attrs_path = Path(source._tempdir.name) / '.zattrs'
-            convert(str(attrs_path), path, overwrite=overwriteAllowed)
+            params = {}
+            if lossy and self.dtype == np.uint8:
+                params['compression'] = 'jpeg'
+            convert(str(attrs_path), path, overwrite=overwriteAllowed, **params)
 
 
 def open(*args, **kwargs):
     """
     Create an instance of the module class.
     """
     return ZarrFileTileSource(*args, **kwargs)
```

### Comparing `large-image-source-zarr-1.28.1.dev4/large_image_source_zarr.egg-info/PKG-INFO` & `large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-zarr
-Version: 1.28.1.dev4
+Version: 1.28.1.dev8
 Summary: A OME Zarr tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-zarr-1.28.1.dev4/setup.py` & `large-image-source-zarr-1.28.1.dev8/setup.py`

 * *Files identical despite different names*

