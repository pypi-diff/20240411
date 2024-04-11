# Comparing `tmp/large-image-source-vips-1.28.1.dev4.tar.gz` & `tmp/large-image-source-vips-1.28.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.28.1.dev4.tar", last modified: Mon Apr  8 20:37:55 2024, max compression
+gzip compressed data, was "large-image-source-vips-1.28.1.dev8.tar", last modified: Wed Apr 10 16:17:08 2024, max compression
```

## Comparing `large-image-source-vips-1.28.1.dev4.tar` & `large-image-source-vips-1.28.1.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 20:37:55.567505 large-image-source-vips-1.28.1.dev4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-04-08 20:37:55.567505 large-image-source-vips-1.28.1.dev4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 20:37:55.563505 large-image-source-vips-1.28.1.dev4/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25419 2024-04-08 20:32:15.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2024-04-08 20:32:15.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 20:37:55.567505 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-08 20:37:55.000000 large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-08 20:32:15.000000 large-image-source-vips-1.28.1.dev4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 20:37:55.567505 large-image-source-vips-1.28.1.dev4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2024-04-08 20:32:15.000000 large-image-source-vips-1.28.1.dev4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:08.397626 large-image-source-vips-1.28.1.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-04-10 16:17:08.397626 large-image-source-vips-1.28.1.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:08.393626 large-image-source-vips-1.28.1.dev8/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25562 2024-04-10 16:11:56.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2024-04-10 16:11:56.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:08.397626 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-10 16:17:08.000000 large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-10 16:11:56.000000 large-image-source-vips-1.28.1.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-10 16:17:08.397626 large-image-source-vips-1.28.1.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2024-04-10 16:11:56.000000 large-image-source-vips-1.28.1.dev8/setup.py
```

### Comparing `large-image-source-vips-1.28.1.dev4/LICENSE` & `large-image-source-vips-1.28.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.28.1.dev4/PKG-INFO` & `large-image-source-vips-1.28.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.28.1.dev4
+Version: 1.28.1.dev8
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.28.1.dev4/README.rst` & `large-image-source-vips-1.28.1.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.28.1.dev4/large_image_source_vips/__init__.py` & `large-image-source-vips-1.28.1.dev8/large_image_source_vips/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from large_image import config
 from large_image.cache_util import LruCacheMetaclass, _cacheClearFuncs, methodcache
 from large_image.constants import (NEW_IMAGE_PATH_FLAG, TILE_FORMAT_NUMPY,
                                    GValueToDtype, SourcePriority,
                                    dtypeToGValue)
 from large_image.exceptions import TileSourceError, TileSourceFileNotFoundError
 from large_image.tilesource import FileTileSource
-from large_image.tilesource.utilities import _imageToNumpy
+from large_image.tilesource.utilities import _imageToNumpy, _newFromFileLock
 
 logging.getLogger('pyvips').setLevel(logging.ERROR)
 
 # Default to ignoring files with no extension and some specific extensions.
 config.ConfigValues['source_vips_ignored_names'] = \
     r'(^[^.]*|\.(yml|yaml|json|png|svs|mrxs))$'
 
@@ -68,30 +68,32 @@
             self._initNew(**kwargs)
             return
         self._largeImagePath = str(self._getLargeImagePath())
         self._editable = False
 
         config._ignoreSourceNames('vips', self._largeImagePath)
         try:
-            self._image = pyvips.Image.new_from_file(self._largeImagePath)
+            with _newFromFileLock:
+                self._image = pyvips.Image.new_from_file(self._largeImagePath)
         except pyvips.error.Error:
             if not os.path.isfile(self._largeImagePath):
                 raise TileSourceFileNotFoundError(self._largeImagePath) from None
             msg = 'File cannot be opened via pyvips'
             raise TileSourceError(msg)
         self.sizeX = self._image.width
         self.sizeY = self._image.height
         self.tileWidth = self.tileHeight = self._tileSize
         pages = 1
         if 'n-pages' in self._image.get_fields():
             pages = self._image.get('n-pages')
         self._frames = [0]
         for page in range(1, pages):
             subInputPath = self._largeImagePath + '[page=%d]' % page
-            subImage = pyvips.Image.new_from_file(subInputPath)
+            with _newFromFileLock:
+                subImage = pyvips.Image.new_from_file(subInputPath)
             if subImage.width == self.sizeX and subImage.height == self.sizeY:
                 self._frames.append(page)
                 continue
             if subImage.width * subImage.height < self.sizeX * self.sizeY:
                 continue
             self._frames = [page]
             self.sizeX = subImage.width
@@ -183,15 +185,16 @@
         if self._image is None and self._output:
             self._outputToImage()
         img = self._image
         if frame > 0:
             with self._frameLock:
                 if frame not in self._recentFrames:
                     subpath = self._largeImagePath + '[page=%d]' % self._frames[frame]
-                    img = pyvips.Image.new_from_file(subpath)
+                    with _newFromFileLock:
+                        img = pyvips.Image.new_from_file(subpath)
                     self._recentFrames[frame] = img
                 else:
                     img = self._recentFrames[frame]
         return img
 
     def getNativeMagnification(self):
         """
```

### Comparing `large-image-source-vips-1.28.1.dev4/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.28.1.dev8/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.28.1.dev4
+Version: 1.28.1.dev8
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.28.1.dev4/setup.py` & `large-image-source-vips-1.28.1.dev8/setup.py`

 * *Files identical despite different names*

