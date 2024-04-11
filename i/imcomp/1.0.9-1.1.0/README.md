# Comparing `tmp/imcomp-1.0.9.tar.gz` & `tmp/imcomp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imcomp-1.0.9.tar", last modified: Wed Dec  6 08:57:04 2023, max compression
+gzip compressed data, was "imcomp-1.1.0.tar", last modified: Thu Apr 11 21:09:51 2024, max compression
```

## Comparing `imcomp-1.0.9.tar` & `imcomp-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:57:04.043053 imcomp-1.0.9/
--rw-rw-r--   0 karl      (1000) karl      (1000)    11357 2023-10-21 21:07:40.000000 imcomp-1.0.9/LICENSE
--rw-rw-r--   0 karl      (1000) karl      (1000)       35 2023-10-22 21:44:45.000000 imcomp-1.0.9/MANIFEST.in
--rw-r--r--   0 karl      (1000) karl      (1000)      924 2023-12-06 08:57:04.043053 imcomp-1.0.9/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      136 2023-11-11 20:23:57.000000 imcomp-1.0.9/README.md
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:57:04.039054 imcomp-1.0.9/imcomp/
--rw-rw-r--   0 karl      (1000) karl      (1000)      156 2023-11-20 08:24:52.000000 imcomp-1.0.9/imcomp/__init__.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:57:04.043053 imcomp-1.0.9/imcomp/config/
--rw-rw-r--   0 karl      (1000) karl      (1000)      605 2023-10-21 21:07:40.000000 imcomp-1.0.9/imcomp/config/default.json
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:40.000000 imcomp-1.0.9/imcomp/default.cfg
--rw-rw-r--   0 karl      (1000) karl      (1000)     8823 2023-11-20 08:24:52.000000 imcomp-1.0.9/imcomp/fill_table_data.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:57:04.043053 imcomp-1.0.9/imcomp/help/
--rw-rw-r--   0 karl      (1000) karl      (1000)     5733 2023-10-21 21:07:40.000000 imcomp-1.0.9/imcomp/help/imcomp_help.html
--rw-rw-r--   0 karl      (1000) karl      (1000)     8675 2023-11-20 08:24:52.000000 imcomp-1.0.9/imcomp/imcomp.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      344 2023-11-20 08:24:52.000000 imcomp-1.0.9/imcomp/imcomp_config.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    21610 2023-11-20 08:24:52.000000 imcomp-1.0.9/imcomp/imcomp_table.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    30502 2023-12-02 17:49:14.000000 imcomp-1.0.9/imcomp/imcomp_window.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:57:04.043053 imcomp-1.0.9/imcomp/qimtools/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:40.000000 imcomp-1.0.9/imcomp/qimtools/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3625 2023-11-04 18:54:03.000000 imcomp-1.0.9/imcomp/qimtools/process_image_differences.py
--rw-rw-r--   0 karl      (1000) karl      (1000)       79 2023-12-06 08:55:13.000000 imcomp-1.0.9/imcomp/version.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:57:04.043053 imcomp-1.0.9/imcomp.egg-info/
--rw-r--r--   0 karl      (1000) karl      (1000)      924 2023-12-06 08:57:03.000000 imcomp-1.0.9/imcomp.egg-info/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      525 2023-12-06 08:57:04.000000 imcomp-1.0.9/imcomp.egg-info/SOURCES.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2023-12-06 08:57:03.000000 imcomp-1.0.9/imcomp.egg-info/dependency_links.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       46 2023-12-06 08:57:04.000000 imcomp-1.0.9/imcomp.egg-info/entry_points.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       83 2023-12-06 08:57:04.000000 imcomp-1.0.9/imcomp.egg-info/requires.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        7 2023-12-06 08:57:04.000000 imcomp-1.0.9/imcomp.egg-info/top_level.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)     1001 2023-12-06 08:55:24.000000 imcomp-1.0.9/pyproject.toml
--rw-rw-r--   0 karl      (1000) karl      (1000)       38 2023-12-06 08:57:04.043053 imcomp-1.0.9/setup.cfg
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:51.658981 imcomp-1.1.0/
+-rw-rw-r--   0 karl      (1000) karl      (1000)    11357 2023-10-21 21:07:40.000000 imcomp-1.1.0/LICENSE
+-rw-rw-r--   0 karl      (1000) karl      (1000)       35 2023-10-22 21:44:45.000000 imcomp-1.1.0/MANIFEST.in
+-rw-r--r--   0 karl      (1000) karl      (1000)      925 2024-04-11 21:09:51.658981 imcomp-1.1.0/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      136 2023-11-11 20:23:57.000000 imcomp-1.1.0/README.md
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:51.642981 imcomp-1.1.0/imcomp/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      156 2023-11-20 08:24:52.000000 imcomp-1.1.0/imcomp/__init__.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:51.642981 imcomp-1.1.0/imcomp/config/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      605 2023-10-21 21:07:40.000000 imcomp-1.1.0/imcomp/config/default.json
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:40.000000 imcomp-1.1.0/imcomp/default.cfg
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8823 2023-11-20 08:24:52.000000 imcomp-1.1.0/imcomp/fill_table_data.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:51.654981 imcomp-1.1.0/imcomp/help/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     5733 2023-10-21 21:07:40.000000 imcomp-1.1.0/imcomp/help/imcomp_help.html
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8696 2024-04-11 21:08:13.000000 imcomp-1.1.0/imcomp/imcomp.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      344 2023-11-20 08:24:52.000000 imcomp-1.1.0/imcomp/imcomp_config.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    21610 2023-11-20 08:24:52.000000 imcomp-1.1.0/imcomp/imcomp_table.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    31180 2024-04-11 21:08:13.000000 imcomp-1.1.0/imcomp/imcomp_window.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:51.658981 imcomp-1.1.0/imcomp/qimtools/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:40.000000 imcomp-1.1.0/imcomp/qimtools/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3625 2023-11-04 18:54:03.000000 imcomp-1.1.0/imcomp/qimtools/process_image_differences.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)       79 2024-04-11 21:08:13.000000 imcomp-1.1.0/imcomp/version.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:51.658981 imcomp-1.1.0/imcomp.egg-info/
+-rw-r--r--   0 karl      (1000) karl      (1000)      925 2024-04-11 21:09:51.000000 imcomp-1.1.0/imcomp.egg-info/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      525 2024-04-11 21:09:51.000000 imcomp-1.1.0/imcomp.egg-info/SOURCES.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-11 21:09:51.000000 imcomp-1.1.0/imcomp.egg-info/dependency_links.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       46 2024-04-11 21:09:51.000000 imcomp-1.1.0/imcomp.egg-info/entry_points.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       83 2024-04-11 21:09:51.000000 imcomp-1.1.0/imcomp.egg-info/requires.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        7 2024-04-11 21:09:51.000000 imcomp-1.1.0/imcomp.egg-info/top_level.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1002 2024-04-11 21:08:13.000000 imcomp-1.1.0/pyproject.toml
+-rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-11 21:09:51.658981 imcomp-1.1.0/setup.cfg
```

### Comparing `imcomp-1.0.9/LICENSE` & `imcomp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/PKG-INFO` & `imcomp-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: imcomp
-Version: 1.0.9
+Version: 1.1.0
 Summary: Image visualization and comparison for multiple series of images
 Author-email: Karl Krissian <karl.krissian@gmail.com>
 Project-URL: Homepage, https://github.com/qimview/imcomp
 Project-URL: Wiki, https://github.com/qimview/imcomp/wiki
 Project-URL: Bug Tracker, https://github.com/qimview/imcomp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: opencv_python>=4.2
 Requires-Dist: psutil>=5.8.0
 Requires-Dist: qimview>=1.0.9
 Provides-Extra: extra
```

### Comparing `imcomp-1.0.9/imcomp/config/default.json` & `imcomp-1.1.0/imcomp/config/default.json`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/imcomp/fill_table_data.py` & `imcomp-1.1.0/imcomp/fill_table_data.py`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/imcomp/help/imcomp_help.html` & `imcomp-1.1.0/imcomp/help/imcomp_help.html`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/imcomp/imcomp.py` & `imcomp-1.1.0/imcomp/imcomp.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 		else:
 			bundle = NSBundle.mainBundle()
 			if bundle:
 				info = (bundle.localizedInfoDictionary() or bundle.infoDictionary())
 				if info:
 					info["CFBundleName"] = "IMCOMP"
 
-	QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_ShareOpenGLContexts)
+	QtCore.QCoreApplication.setAttribute(QtCore.Qt.ApplicationAttribute.AA_ShareOpenGLContexts)
 	app = QtWidgets.QApplication(sys.argv)
 	try:
 		app.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps)
 	except Exception as e:
 		print("Attribute QtCore.Qt.AA_UseHighDpiPixmaps not available: {}".format(e))
 
 	_params['config_name'] = config['config_name']
```

### Comparing `imcomp-1.0.9/imcomp/imcomp_table.py` & `imcomp-1.1.0/imcomp/imcomp_table.py`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/imcomp/imcomp_window.py` & `imcomp-1.1.0/imcomp/imcomp_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,47 @@
 from qimview.utils.qt_imports       import QtWidgets, QtCore, QtGui
 from qimview.utils.viewer_image     import *
 from qimview.utils.menu_selection   import MenuSelection
 from qimview.image_viewers          import MultiView, ViewerType
 from .imcomp_table                  import ImCompTable
 from qimview.cache                  import FileCache
 from qimview.image_readers          import gb_image_reader
-import sys
 from typing                         import Optional, Any, Dict
 from .imcomp_config                 import ImCompConfig
 # Only enable vlc player for windows by default
 
 userconf = ImCompConfig.user_config()
 try:
     use_vlc_player = userconf.get_boolean('VIDEOPLAYER','UseVLC')
     print(f"use_vlc_player {use_vlc_player}")
 except Exception as e:
     print(f"Failed to get UseVLC config {e}")
     use_vlc_player = False # sys.platform == "win32"
 
-if use_vlc_player:
-    try:
-        from qimview.video_player.vlc_player import VLCPlayer as VideoPlayer
-        has_video_player = True
-    except Exception as e:
-        print(f"Failed to import VLCPlayer {e}")
-        has_video_player = False
-else:
-    try:
-        from qimview.video_player.video_player import VideoPlayer
-        has_video_player = True
-    except Exception as e:
-        print(f"Failed to import video_player {e}")
-        has_video_player = False
+try:
+    from qimview.video_player.video_player_av import VideoPlayerAV as VideoPlayer
+    has_video_player = True
+except Exception as e:
+    print(f"Failed to import VideoPlayerAV: {e}")
+    has_video_player = False
+
+# if use_vlc_player:
+#     try:
+#         from qimview.video_player.vlc_player import VLCPlayer as VideoPlayer
+#         has_video_player = True
+#     except Exception as e:
+#         print(f"Failed to import VLCPlayer {e}")
+#         has_video_player = False
+# else:
+#     try:
+#         from qimview.video_player.video_player import VideoPlayer
+#         has_video_player = True
+#     except Exception as e:
+#         print(f"Failed to import video_player {e}")
+#         has_video_player = False
 
 from imcomp import fill_table_data
 import sys
 import os
 from shutil import copyfile
 import copyreg
 import multiprocessing
@@ -492,15 +498,15 @@
         #print(f"set model root path to {user_path}")
         self.model.setRootPath(user_path)
         # self.model.setFilters(QDir::Files | QDir::AllDirs | QDir::NoDotAndDotDot)
         # *.dxr DXO image format
         # *.ARW sony raw image format
 
         extension_list = gb_image_reader.extensions()
-        extension_list.extend(['*.MP4'])
+        extension_list.extend(['*.MP4','*.360'])
         full_list = []
         for e in extension_list:
             if e.lower() not in full_list:
                 full_list.append(f'*{e}')
             if e.upper() not in full_list:
                 full_list.append(f'*{e}')
 
@@ -575,17 +581,17 @@
 
         # --- create video tab
         if has_video_player:
             video_tab = QtWidgets.QWidget()
             self.right_tabs_widget.setMovable(True)
             self.right_tabs_widget.addTab(video_tab, "Video")
             video_layout = QtWidgets.QHBoxLayout()
-            self.videoplayer1 = VideoPlayer(self)
+            self.videoplayer1 : VideoPlayer = VideoPlayer(self)
             video_layout.addWidget(self.videoplayer1, 1)
-            self.videoplayer2 = VideoPlayer(self)
+            self.videoplayer2 : VideoPlayer = VideoPlayer(self)
             video_layout.addWidget(self.videoplayer2, 1)
             video_tab.setLayout(video_layout)
 
         # --- main layout
         main_layout = QtWidgets.QHBoxLayout()
         splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal)
         splitter.addWidget(self.left_tabs_widget)
@@ -610,25 +616,36 @@
             if filePath not in file_list:
                 file_list.append(filePath)
         print(f"file_list {file_list}")
         self.on_selection(file_list)
 
     def on_selection(self, file_list):
         nb_selections = len(file_list)
-        if has_video_player and nb_selections == 1 and file_list[0].lower().endswith("mp4"):
+        # TODO: improve this part
+        def is_video(f):
+            return f.lower().endswith("mp4") or f.lower().endswith(".360")
+
+        if has_video_player and nb_selections == 1 and is_video(file_list[0]):
             self.videoplayer1.set_video(file_list[0])
             self.videoplayer1.set_synchronize(None)
             self.videoplayer2.hide()
+            self.videoplayer1.set_name('player1')
+            self.videoplayer1.init_and_display()
         else:
-            if has_video_player and nb_selections ==2 and file_list[0].lower().endswith("mp4") and file_list[1].lower().endswith("mp4"):
+            if has_video_player and nb_selections ==2 and is_video(file_list[0]) and is_video(file_list[1]):
                 self.videoplayer1.set_synchronize(self.videoplayer2)
                 self.videoplayer2.set_synchronize(self.videoplayer1)
                 self.videoplayer1.set_video(file_list[0])
                 self.videoplayer2.set_video(file_list[1])
                 self.videoplayer2.show()
+                self.videoplayer1.set_name('player1')
+                self.videoplayer1.init_and_display()
+
+                self.videoplayer2.set_name('player2')
+                self.videoplayer2.init_and_display()
             else:
                 def get_name(path, maxlength=15):
                     return os.path.splitext(os.path.basename(path))[0][-maxlength:]
 
                 images_dict = {}
                 for idx, im in enumerate(file_list):
                     image_key = f'{idx}...{get_name(im)}'
```

### Comparing `imcomp-1.0.9/imcomp/qimtools/process_image_differences.py` & `imcomp-1.1.0/imcomp/qimtools/process_image_differences.py`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/imcomp.egg-info/PKG-INFO` & `imcomp-1.1.0/imcomp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: imcomp
-Version: 1.0.9
+Version: 1.1.0
 Summary: Image visualization and comparison for multiple series of images
 Author-email: Karl Krissian <karl.krissian@gmail.com>
 Project-URL: Homepage, https://github.com/qimview/imcomp
 Project-URL: Wiki, https://github.com/qimview/imcomp/wiki
 Project-URL: Bug Tracker, https://github.com/qimview/imcomp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: opencv_python>=4.2
 Requires-Dist: psutil>=5.8.0
 Requires-Dist: qimview>=1.0.9
 Provides-Extra: extra
```

### Comparing `imcomp-1.0.9/imcomp.egg-info/SOURCES.txt` & `imcomp-1.1.0/imcomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imcomp-1.0.9/pyproject.toml` & `imcomp-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dynamic = ["version"]
 name = "imcomp"
 authors = [
   { name="Karl Krissian", email="karl.krissian@gmail.com" },
 ]
 description = "Image visualization and comparison for multiple series of images"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
```

