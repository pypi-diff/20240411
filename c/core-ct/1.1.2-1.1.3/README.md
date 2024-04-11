# Comparing `tmp/core_ct-1.1.2.tar.gz` & `tmp/core_ct-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_ct-1.1.2.tar", max compression
+gzip compressed data, was "core_ct-1.1.3.tar", max compression
```

## Comparing `core_ct-1.1.2.tar` & `core_ct-1.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2024-03-29 14:18:57.936328 core_ct-1.1.2/LICENSE
--rw-r--r--   0        0        0     2593 2024-03-29 14:18:57.936328 core_ct-1.1.2/README.md
--rw-r--r--   0        0        0      981 2024-03-29 14:18:57.940328 core_ct-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       72 2024-03-29 14:18:57.940328 core_ct-1.1.2/src/core_ct/__init__.py
--rw-r--r--   0        0        0      747 2024-03-29 14:18:57.940328 core_ct-1.1.2/src/core_ct/analysis.py
--rw-r--r--   0        0        0    21970 2024-03-29 14:18:57.940328 core_ct-1.1.2/src/core_ct/core.py
--rw-r--r--   0        0        0     3477 2024-03-29 14:18:57.940328 core_ct-1.1.2/src/core_ct/importers.py
--rw-r--r--   0        0        0     4454 2024-03-29 14:18:57.940328 core_ct-1.1.2/src/core_ct/slice.py
--rw-r--r--   0        0        0     7286 2024-03-29 14:18:57.940328 core_ct-1.1.2/src/core_ct/visualize.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-11 01:05:32.636641 core_ct-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2593 2024-04-11 01:05:32.636641 core_ct-1.1.3/README.md
+-rw-r--r--   0        0        0      981 2024-04-11 01:05:32.640641 core_ct-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/analysis.py
+-rw-r--r--   0        0        0    21970 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/core.py
+-rw-r--r--   0        0        0     4313 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/importers.py
+-rw-r--r--   0        0        0     4454 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/slice.py
+-rw-r--r--   0        0        0     7286 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/visualize.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.1.3/PKG-INFO
```

### Comparing `core_ct-1.1.2/LICENSE` & `core_ct-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.2/README.md` & `core_ct-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.2/pyproject.toml` & `core_ct-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-ct"
-version = "1.1.2"
+version = "1.1.3"
 description = "A Python library to assist geologists with the analysis of rock core CT scans"
 authors = [
     "Kira Hanson <khanson@mines.edu>",
     "Carla Ellefsen <cellefsen@mines.edu>",
     "Connor Sparks <csparks@mines.edu>",
     "Asa Sprow <arsprow@mines.edu>",
 ]
```

### Comparing `core_ct-1.1.2/src/core_ct/analysis.py` & `core_ct-1.1.3/src/core_ct/analysis.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.2/src/core_ct/core.py` & `core_ct-1.1.3/src/core_ct/core.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.2/src/core_ct/importers.py` & `core_ct-1.1.3/src/core_ct/importers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,112 @@
 """Methods that assist in importing CT scans of rock cores."""
 
 from .core import Core
 from pydicom import dcmread
+from pydicom.errors import InvalidDicomError
 from os import listdir
 import os.path
 import numpy as np
 
 
 def dicom(
     dir: str | None = None,
     files: list[str] | None = None,
     force: bool = False,
     ignore_hidden_files: bool = True,
+    ignore_file_extensions: bool = False
 ) -> Core:
     """
     Load a DICOM dataset into a `Core` object.
 
     Files containing the DICOM dataset can be specified by providing a directory or a
     list of files. If both `dir` and `files` are provided, `dir` will be ignored.
 
     When specifying a directory all files in that directory will be treated as
     part of the DICOM dataset. If this is undesirable, use `files` instead.
 
+    Subfolders/directories are ignored. All dicom data files must be explicitly
+    specified via `files` or located in the `dir` provided.
+
+    By default, only files with the `.dcm` file extension are read. If this is
+    undesirable, set `ignore_file_extensions` to `False`.
+
     Arguments
     ---------
     dir : str
         Path to directory containing DICOM dataset; ignored if `files` is specified
 
     files : list[str]
         List of filepaths belonging to DICOM dataset
 
     force : bool
         If set to `True`, files that produce errors will be ignored
 
     ignore_hidden_files : bool
         If set to `True`, hidden files will be ignored
+
+    ignore_file_extensions : bool
+        If set to `False`, only files with the extension `.dcm` will be read.
     """
     # if files was not provided, load files from the provided directory
-    if files is None:
+    if files is None or len(files) == 0:
         # throw error if directory not provided
         if dir is None:
-            raise Exception("Must provide a directory or file list")
+            raise ValueError("Must provide a non-empty directory or file list")
         # get the list of files for the core
         files = [os.path.join(dir, file_name) for file_name in listdir(dir)]
 
     # skip files with no SliceLocation information (should be a float)
     slices = []
     skipped: list[str] = []
     for f in files:
         # get the basename of the file and then check if it is a hidden file
         f_name = os.path.basename(f)
         if ignore_hidden_files and f_name.startswith("."):
             continue
+        # check file extension
+        if not ignore_file_extensions and not f_name.endswith(".dcm"):
+            continue
+        # ignore subdirectories
+        if os.path.isdir(f):
+            continue
 
         # try to read slice
         try:
             ds = dcmread(f, force=force)
-        except Exception as e:
+        except InvalidDicomError:
             if not force:
                 # forward pydicom exception so the stack trace is more useful
-                raise e
+                raise
             else:
                 continue
 
         # make sure SliceLocation exists in the slice
         try:
             if isinstance(ds.SliceLocation, float):
                 slices.append(ds)
             else:
                 skipped.append(f)
         # in case SliceLocation isn't an attribute of ds
-        except Exception as pydicom_exception:
-            if not force:
-                raise Exception(
-                    f"File does not contain SliceLocation in header: {f}"
-                ) from pydicom_exception
-            else:
-                skipped.append(f)
+        except UnboundLocalError:
+            skipped.append(f)
 
     if not force and len(skipped) > 0:
-        raise Exception(
+        raise ValueError(
             f"Failed to load {len(skipped)} files, missing SliceLocation: {skipped}"
         )
 
+    # make sure we actually loaded data
+    if len(slices) == 0:
+        raise RuntimeError(
+            "No data loaded. This could mean an empty directory was provided, "
+            "no files could be parsed, or no files had the `.dcm` file "
+            "extension (if `ignore_file_extensions` is set to `False`)."
+        )
+
     # re-sort to put the slices in the right order
     slices = sorted(slices, key=lambda s: s.SliceLocation)
 
     # pixel dimensions, assuming all slices are the same
     x_dim: float = float(slices[0].PixelSpacing[0])
     y_dim: float = float(slices[0].PixelSpacing[1])
     z_dim: float = float(slices[0].SliceThickness)
```

### Comparing `core_ct-1.1.2/src/core_ct/slice.py` & `core_ct-1.1.3/src/core_ct/slice.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.2/src/core_ct/visualize.py` & `core_ct-1.1.3/src/core_ct/visualize.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.2/PKG-INFO` & `core_ct-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-ct
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library to assist geologists with the analysis of rock core CT scans
 License: MIT
 Author: Kira Hanson
 Author-email: khanson@mines.edu
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

