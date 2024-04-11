# Comparing `tmp/qtlink-1.1.2.tar.gz` & `tmp/qtlink-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.1.2.tar", last modified: Wed Apr 10 12:42:36 2024, max compression
+gzip compressed data, was "qtlink-1.1.3.tar", last modified: Thu Apr 11 05:58:35 2024, max compression
```

## Comparing `qtlink-1.1.2.tar` & `qtlink-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.961713 qtlink-1.1.2/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-10 12:42:36.959713 qtlink-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.916189 qtlink-1.1.2/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.1.2/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.949196 qtlink-1.1.2/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.1.2/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.1.2/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.1.2/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1406 2024-04-10 12:21:37.000000 qtlink-1.1.2/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     1086 2024-04-10 11:53:14.000000 qtlink-1.1.2/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.950194 qtlink-1.1.2/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.2/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2042 2024-04-10 12:40:42.000000 qtlink-1.1.2/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.954194 qtlink-1.1.2/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.2/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     6668 2024-04-10 12:00:18.000000 qtlink-1.1.2/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     5455 2024-04-10 11:53:14.000000 qtlink-1.1.2/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     1919 2024-04-10 11:59:10.000000 qtlink-1.1.2/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     3647 2024-04-10 12:00:18.000000 qtlink-1.1.2/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.957713 qtlink-1.1.2/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.1.2/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.1.2/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.1.2/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:42:36.959713 qtlink-1.1.2/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 12:42:36.000000 qtlink-1.1.2/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 12:42:36.961713 qtlink-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-10 12:40:42.000000 qtlink-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.615049 qtlink-1.1.3/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-11 05:58:35.615049 qtlink-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.566782 qtlink-1.1.3/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.1.3/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.600593 qtlink-1.1.3/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.1.3/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.1.3/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0      802 2024-04-11 02:31:03.000000 qtlink-1.1.3/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1406 2024-04-10 12:21:37.000000 qtlink-1.1.3/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     1086 2024-04-10 11:53:14.000000 qtlink-1.1.3/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.615049 qtlink-1.1.3/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.3/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2042 2024-04-10 12:40:42.000000 qtlink-1.1.3/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.615049 qtlink-1.1.3/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.3/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     6668 2024-04-10 12:00:18.000000 qtlink-1.1.3/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     5455 2024-04-10 11:53:14.000000 qtlink-1.1.3/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     1919 2024-04-10 11:59:10.000000 qtlink-1.1.3/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     3791 2024-04-11 05:55:47.000000 qtlink-1.1.3/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.615049 qtlink-1.1.3/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.1.3/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.1.3/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.1.3/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:58:35.615049 qtlink-1.1.3/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-11 05:58:35.000000 qtlink-1.1.3/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-11 05:58:35.000000 qtlink-1.1.3/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 05:58:35.000000 qtlink-1.1.3/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-11 05:58:35.000000 qtlink-1.1.3/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 05:58:35.000000 qtlink-1.1.3/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 05:58:35.615049 qtlink-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-11 05:57:26.000000 qtlink-1.1.3/setup.py
```

### Comparing `qtlink-1.1.2/LICENSE` & `qtlink-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/PKG-INFO` & `qtlink-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.1.2
+Version: 1.1.3
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.1.2/qtlink/dialog/dialog_choice.py` & `qtlink-1.1.3/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/dialog/dialog_info.py` & `qtlink-1.1.3/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/dialog/dialog_table_check.py` & `qtlink-1.1.3/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/dialog/dialog_table_display.py` & `qtlink-1.1.3/qtlink/dialog/dialog_table_display.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.1.3/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/table/table_controller.py` & `qtlink-1.1.3/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.1.3/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/table/table_controller_single_check.py` & `qtlink-1.1.3/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/util.py` & `qtlink-1.1.3/qtlink/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from PySide6.QtCore import QObject, Signal
 
 
+def force_draw():
+    """强制绘制挂起的事件，如弹窗"""
+    from PySide6.QtWidgets import QApplication
+    QApplication.processEvents()
+
+
 def create_signal(signal_type):
     """根据传入类型，创建相应的信号类。"""
 
     class CustomSignal(QObject):
         signal = Signal(signal_type)
 
     return CustomSignal()
 
 
-class ResponseProgressSignal:
-    """需要某个功能类继承它，并连接response_progress_signal方法到某一信号。
+class SlotProgressSignal:
+    """需要某个功能类继承它，并连接slot_progress_signal方法到某一信号。
     然后根据需要实现各种progress_xxx方法，即可根据不同状态自动调用相应的处理方法。"""
 
-    def response_progress_signal(self, state: tuple):
+    def slot_progress_signal(self, state: tuple):
         state_flag, data = state
         if state_flag == ProgressState.flag_start:
             self.progress_start(data)
         elif state_flag == ProgressState.flag_doing:
             self.progress_doing(data)
         elif state_flag == ProgressState.flag_success:
             self.progress_success(data)
```

### Comparing `qtlink-1.1.2/qtlink/widgets/drop_widget.py` & `qtlink-1.1.3/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink/widgets/list_widget.py` & `qtlink-1.1.3/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/qtlink.egg-info/PKG-INFO` & `qtlink-1.1.3/qtlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.1.2
+Version: 1.1.3
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.1.2/qtlink.egg-info/SOURCES.txt` & `qtlink-1.1.3/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.1.2/setup.py` & `qtlink-1.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.1.2",
+    version="1.1.3",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6', 'matplotlib', 'numpy'],
```

