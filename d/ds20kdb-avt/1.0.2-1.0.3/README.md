# Comparing `tmp/ds20kdb-avt-1.0.2.tar.gz` & `tmp/ds20kdb-avt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds20kdb-avt-1.0.2.tar", last modified: Wed Apr  3 17:30:49 2024, max compression
+gzip compressed data, was "ds20kdb-avt-1.0.3.tar", last modified: Thu Apr 11 07:49:10 2024, max compression
```

## Comparing `ds20kdb-avt-1.0.2.tar` & `ds20kdb-avt-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.346766 ds20kdb-avt-1.0.2/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-03 17:30:49.345959 ds20kdb-avt-1.0.2/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.2/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-03 17:30:49.346975 ds20kdb-avt-1.0.2/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-03 17:30:23.000000 ds20kdb-avt-1.0.2/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.309522 ds20kdb-avt-1.0.2/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.338715 ds20kdb-avt-1.0.2/src/ds20kdb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/src/ds20kdb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.2/src/ds20kdb/auth.py
--rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/common.py
--rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.2/src/ds20kdb/constants.py
--rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/src/ds20kdb/create_credentials_file.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33510 2024-04-03 17:21:01.000000 ds20kdb-avt-1.0.2/src/ds20kdb/gen_tray_files_gui.py
--rw-r--r--   0 avt        (501) staff       (20)    93422 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.2/src/ds20kdb/qr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.2/src/ds20kdb/qrgen.py
--rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/scanner_auto.py
--rwxr-xr-x   0 avt        (501) staff       (20)   117866 2024-03-28 13:27:09.000000 ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile.py
--rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile_json.py
--rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.2/src/ds20kdb/veto_location.py
--rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/veto_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.2/src/ds20kdb/visual.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8909 2023-09-17 11:55:13.000000 ds20kdb-avt-1.0.2/src/ds20kdb/vtile_test_submit_cr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb-avt-1.0.2/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
--rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.2/src/ds20kdb/wafer_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.2/src/ds20kdb/wafer_map_from_db.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.345085 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.418032 ds20kdb-avt-1.0.3/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-11 07:49:10.417028 ds20kdb-avt-1.0.3/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.3/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-11 07:49:10.418317 ds20kdb-avt-1.0.3/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-11 07:48:39.000000 ds20kdb-avt-1.0.3/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.380797 ds20kdb-avt-1.0.3/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.408246 ds20kdb-avt-1.0.3/src/ds20kdb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/src/ds20kdb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.3/src/ds20kdb/auth.py
+-rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.3/src/ds20kdb/constants.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/src/ds20kdb/create_credentials_file.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb-avt-1.0.3/src/ds20kdb/gen_tray_files_gui.py
+-rw-r--r--   0 avt        (501) staff       (20)    93422 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.3/src/ds20kdb/qr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.3/src/ds20kdb/qrgen.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/scanner_auto.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   117866 2024-03-28 13:27:09.000000 ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile_json.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.3/src/ds20kdb/veto_location.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/veto_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.3/src/ds20kdb/visual.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8909 2023-09-17 11:55:13.000000 ds20kdb-avt-1.0.3/src/ds20kdb/vtile_test_submit_cr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb-avt-1.0.3/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
+-rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.3/src/ds20kdb/wafer_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.3/src/ds20kdb/wafer_map_from_db.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.415727 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/top_level.txt
```

### Comparing `ds20kdb-avt-1.0.2/PKG-INFO` & `ds20kdb-avt-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.2
+Version: 1.0.3
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.2/README.md` & `ds20kdb-avt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/setup.py` & `ds20kdb-avt-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ds20kdb-avt",
-    version="1.0.2",
+    version="1.0.3",
     author="Alan Taylor, Paolo Franchini, Seraphim Koulosousas",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="A cross-platform Python interface to the DarkSide-20k production database",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/auth.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/auth.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/common.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/common.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/create_credentials_file.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/create_credentials_file.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/gen_tray_files_gui.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/gen_tray_files_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 import collections
 from enum import IntEnum
 import functools
 import itertools
 import os
 from pathlib import Path
+import platform
 import sys
 import webbrowser
 
 import tkinter
 from tkinter import ttk
 from tkinter import filedialog
+from tkinter import font
 
 from ds20kdb import interface
 from ds20kdb import common
 
 
 ##############################################################################
 # data structures
@@ -55,27 +57,49 @@
     inner_split = 16
     outer_split = 8
     left_frame_width = right_frame_width = (root_w - outer_split * 3) // 2
 
     max_filenames_per_tab = 12
     directory_label_width_chars = 64
     console_width_chars = 58
-    console_height_chars = 21
+    console_height_chars = 20
 
     try:
         dbi = interface.Database()
     except AssertionError:
         sys.exit()
 
     def __init__(self):
         self.root = tkinter.Tk()
         self.root.geometry(f'{self.root_w}x{self.root_h}+0+0')
         self.root.title('DarkSide-20k generate tray files')
         self.root.resizable(False, False)
 
+        ######################################################################
+        # platform specific items related to detecting paste, font handling
+        ######################################################################
+
+        self.system = platform.system()
+
+        default_fonts = [
+            # labelframe, label
+            font.nametofont('TkDefaultFont'),
+            # combobox
+            font.nametofont('TkTextFont'),
+            # entry (console)
+            font.nametofont('TkFixedFont'),
+            # menu bar
+            font.nametofont('TkMenuFont'),
+        ]
+
+        for dfont in default_fonts:
+            self.amend_font(dfont)
+
+        ######################################################################
+
         self.frame = {}
         self.button = {}
         self.combobox = {}
         self.filenames = collections.defaultdict(set)
         self.directory = os.path.expanduser('~')
 
         self.frame_tab = {}
@@ -598,14 +622,57 @@
         ----------------------------------------------------------------------
         returns : none
         ----------------------------------------------------------------------
         """
         self.root.mainloop()
 
     ##########################################################################
+    # Platform-specific font handling
+    ##########################################################################
+
+    def amend_font(self, tkf):
+        """
+        Amend font size if it will limit visibility.
+
+        Windows 10:
+            {'family': 'Segoe UI', 'size': 9, ...}
+            {'family': 'Courier New', 'size': 10, ...}
+
+        Ubuntu 22.04, Pop!_OS 22.04, CentOS 7 (size=0):
+            {'family': 'DejaVu Sans', 'size': 10, ...}
+            {'family': 'DejaVu Sans Mono', 'size': 10, ...}
+
+        Raspberry Pi OS (RPi4, bullseye):
+            {'family': 'Bitstream Vera Sans', 'size': 10, ...}
+            {'family': 'Liberation Mono', 'size': 10, ...}
+
+        Raspberry Pi OS (RPi5, bookworm):
+            {'family': 'Noto Sans', 'size': 10, ...}
+            {'family': 'Liberation Mono', 'size': 10, ...}
+
+        macOS Ventura:
+            {'family': 'Verdana', 'size': 9, ...}
+            {'family': 'Andale Mono', 'size': 9, ...}
+
+        ----------------------------------------------------------------------
+        args
+            tkf : <class 'tkinter.font.Font'>
+        ----------------------------------------------------------------------
+        returns : none
+            GUI state changed
+        ----------------------------------------------------------------------
+        """
+        font_list = [
+            'Noto Sans', 'Liberation Mono', 'Courier New', 'DejaVu Sans Mono'
+        ]
+        details = tkf.actual()
+        if details['family'] in font_list and details['size'] > 9:
+            tkf.configure(size=9)
+
+    ##########################################################################
     # GUI button actions
     ##########################################################################
 
     def clear_console(self):
         """
         ----------------------------------------------------------------------
         args : none
```

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/interface.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/interface.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/qr.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/qr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/qrgen.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/qrgen.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/scanner_auto.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/scanner_auto.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile_json.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile_json.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/veto_location.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/veto_location.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/veto_location_gui.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/veto_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/visual.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/visual.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/vtile_test_submit_cr.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/vtile_test_submit_cr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/wafer_location_gui.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/wafer_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb/wafer_map_from_db.py` & `ds20kdb-avt-1.0.3/src/ds20kdb/wafer_map_from_db.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/PKG-INFO` & `ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.2
+Version: 1.0.3
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/SOURCES.txt` & `ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/entry_points.txt` & `ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/entry_points.txt`

 * *Files identical despite different names*

