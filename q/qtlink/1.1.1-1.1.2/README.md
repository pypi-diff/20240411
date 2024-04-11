# Comparing `tmp/qtlink-1.1.1.tar.gz` & `tmp/qtlink-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.1.1.tar", last modified: Wed Apr 10 12:23:43 2024, max compression
+gzip compressed data, was "qtlink-1.1.2.tar", last modified: Wed Apr 10 12:42:36 2024, max compression
```

## Comparing `qtlink-1.1.1.tar` & `qtlink-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.517028 qtlink-1.1.1/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-10 12:23:43.517028 qtlink-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.485762 qtlink-1.1.1/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.1.1/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.501388 qtlink-1.1.1/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.1.1/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.1.1/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.1.1/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1406 2024-04-10 12:21:37.000000 qtlink-1.1.1/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     1086 2024-04-10 11:53:14.000000 qtlink-1.1.1/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.501388 qtlink-1.1.1/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.1/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     1971 2024-04-10 06:55:58.000000 qtlink-1.1.1/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.501388 qtlink-1.1.1/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.1/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     6668 2024-04-10 12:00:18.000000 qtlink-1.1.1/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     5455 2024-04-10 11:53:14.000000 qtlink-1.1.1/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     1919 2024-04-10 11:59:10.000000 qtlink-1.1.1/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     3647 2024-04-10 12:00:18.000000 qtlink-1.1.1/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.501388 qtlink-1.1.1/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.1.1/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.1.1/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.1.1/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:23:43.517028 qtlink-1.1.1/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-10 12:23:43.000000 qtlink-1.1.1/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-10 12:23:43.000000 qtlink-1.1.1/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:23:43.000000 qtlink-1.1.1/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-10 12:23:43.000000 qtlink-1.1.1/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 12:23:43.000000 qtlink-1.1.1/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 12:23:43.517028 qtlink-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-10 12:22:40.000000 qtlink-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.961713 qtlink-1.1.2/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-10 12:42:36.959713 qtlink-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.916189 qtlink-1.1.2/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.1.2/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.949196 qtlink-1.1.2/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.1.2/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.1.2/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.1.2/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1406 2024-04-10 12:21:37.000000 qtlink-1.1.2/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     1086 2024-04-10 11:53:14.000000 qtlink-1.1.2/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.950194 qtlink-1.1.2/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.2/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2042 2024-04-10 12:40:42.000000 qtlink-1.1.2/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.954194 qtlink-1.1.2/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.2/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     6668 2024-04-10 12:00:18.000000 qtlink-1.1.2/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     5455 2024-04-10 11:53:14.000000 qtlink-1.1.2/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     1919 2024-04-10 11:59:10.000000 qtlink-1.1.2/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     3647 2024-04-10 12:00:18.000000 qtlink-1.1.2/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.957713 qtlink-1.1.2/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.1.2/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.1.2/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.1.2/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.959713 qtlink-1.1.2/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:42:36.961713 qtlink-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-10 12:40:42.000000 qtlink-1.1.2/setup.py
```

### Comparing `qtlink-1.1.1/LICENSE` & `qtlink-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/PKG-INFO` & `qtlink-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.1.1
+Version: 1.1.2
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.1.1/qtlink/dialog/dialog_choice.py` & `qtlink-1.1.2/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/dialog/dialog_info.py` & `qtlink-1.1.2/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/dialog/dialog_table_check.py` & `qtlink-1.1.2/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/dialog/dialog_table_display.py` & `qtlink-1.1.2/qtlink/dialog/dialog_table_display.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.1.2/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from PySide6.QtWidgets import QWidget
 
 
 class MplCanvas(QWidget):
-    def __init__(self, enable_toolbar: bool = True, parent=None):
+    def __init__(self, width: float = 5, height: float = 4, dpi: int = 100, enable_toolbar: bool = True, parent=None):
         from matplotlib import pyplot as plt
         from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas, \
             NavigationToolbar2QT as NavigationToolbar
         from matplotlib.figure import Figure
         from PySide6.QtWidgets import QVBoxLayout
         plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
         plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
 
         super(MplCanvas, self).__init__(parent)
-        self.canvas = FigureCanvas(Figure(figsize=(5, 4), constrained_layout=True))
+        self.canvas = FigureCanvas(Figure(figsize=(width, height), dpi=dpi, constrained_layout=True))
         self.ax = self.canvas.figure.subplots()
 
         self.vertical_layout = QVBoxLayout()
         if enable_toolbar:
             self.toolbar = NavigationToolbar(self.canvas, self)
             self.vertical_layout.addWidget(self.toolbar)
         self.vertical_layout.addWidget(self.canvas)
```

### Comparing `qtlink-1.1.1/qtlink/table/table_controller.py` & `qtlink-1.1.2/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.1.2/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/table/table_controller_single_check.py` & `qtlink-1.1.2/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/util.py` & `qtlink-1.1.2/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/widgets/drop_widget.py` & `qtlink-1.1.2/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink/widgets/list_widget.py` & `qtlink-1.1.2/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.1/qtlink.egg-info/PKG-INFO` & `qtlink-1.1.2/qtlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.1.1
+Version: 1.1.2
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.1.1/qtlink.egg-info/SOURCES.txt` & `qtlink-1.1.2/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

