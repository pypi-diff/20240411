# Comparing `tmp/fyplot-2.0.tar.gz` & `tmp/fyplot-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fyplot-2.0.tar", last modified: Tue Jun  9 19:30:41 2020, max compression
+gzip compressed data, was "fyplot-2.1.tar", last modified: Thu Apr 11 08:00:16 2024, max compression
```

## Comparing `fyplot-2.0.tar` & `fyplot-2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-09 19:30:41.000000 fyplot-2.0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      641 2020-06-09 18:48:43.000000 fyplot-2.0/setup.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      455 2020-06-08 20:28:11.000000 fyplot-2.0/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2020-06-09 19:30:41.000000 fyplot-2.0/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      317 2020-06-09 19:30:41.000000 fyplot-2.0/PKG-INFO
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        7 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      263 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      317 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       10 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot.egg-info/requires.txt
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-09 19:30:41.000000 fyplot-2.0/bin/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1268 2020-06-09 19:27:32.000000 fyplot-2.0/bin/fyplot_demo2
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1577 2020-06-09 19:17:36.000000 fyplot-2.0/bin/fyplot_demo
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-09 19:30:41.000000 fyplot-2.0/fyplot/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3355 2020-06-09 19:16:56.000000 fyplot-2.0/fyplot/function_plot.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3621 2020-06-09 19:26:52.000000 fyplot-2.0/fyplot/dict_plot.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-06-09 19:17:05.000000 fyplot-2.0/fyplot/__init__.py
+drwxr-xr-x   0 vberenz   (5950) is        (1040)        0 2024-04-11 08:00:16.369330 fyplot-2.1/
+-rw-r--r--   0 vberenz   (5950) is        (1040)      317 2024-04-11 08:00:16.365330 fyplot-2.1/PKG-INFO
+-rw-r--r--   0 vberenz   (5950) is        (1040)      455 2024-04-11 07:49:48.000000 fyplot-2.1/README.md
+drwxr-xr-x   0 vberenz   (5950) is        (1040)        0 2024-04-11 08:00:16.365330 fyplot-2.1/bin/
+-rw-r--r--   0 vberenz   (5950) is        (1040)     1577 2024-04-11 07:49:48.000000 fyplot-2.1/bin/fyplot_demo
+-rw-r--r--   0 vberenz   (5950) is        (1040)     1268 2024-04-11 07:49:48.000000 fyplot-2.1/bin/fyplot_demo2
+drwxr-xr-x   0 vberenz   (5950) is        (1040)        0 2024-04-11 08:00:16.365330 fyplot-2.1/fyplot/
+-rw-r--r--   0 vberenz   (5950) is        (1040)        0 2024-04-11 07:49:48.000000 fyplot-2.1/fyplot/__init__.py
+-rw-r--r--   0 vberenz   (5950) is        (1040)     3644 2024-04-11 07:49:48.000000 fyplot-2.1/fyplot/dict_plot.py
+-rw-r--r--   0 vberenz   (5950) is        (1040)     3355 2024-04-11 07:49:48.000000 fyplot-2.1/fyplot/function_plot.py
+drwxr-xr-x   0 vberenz   (5950) is        (1040)        0 2024-04-11 08:00:16.365330 fyplot-2.1/fyplot.egg-info/
+-rw-r--r--   0 vberenz   (5950) is        (1040)      317 2024-04-11 08:00:16.000000 fyplot-2.1/fyplot.egg-info/PKG-INFO
+-rw-r--r--   0 vberenz   (5950) is        (1040)      263 2024-04-11 08:00:16.000000 fyplot-2.1/fyplot.egg-info/SOURCES.txt
+-rw-r--r--   0 vberenz   (5950) is        (1040)        1 2024-04-11 08:00:16.000000 fyplot-2.1/fyplot.egg-info/dependency_links.txt
+-rw-r--r--   0 vberenz   (5950) is        (1040)       10 2024-04-11 08:00:16.000000 fyplot-2.1/fyplot.egg-info/requires.txt
+-rw-r--r--   0 vberenz   (5950) is        (1040)        7 2024-04-11 08:00:16.000000 fyplot-2.1/fyplot.egg-info/top_level.txt
+-rw-r--r--   0 vberenz   (5950) is        (1040)       38 2024-04-11 08:00:16.369330 fyplot-2.1/setup.cfg
+-rw-r--r--   0 vberenz   (5950) is        (1040)      641 2024-04-11 07:49:48.000000 fyplot-2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fyplot-2.0/setup.py` & `fyplot-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `fyplot-2.0/bin/fyplot_demo2` & `fyplot-2.1/bin/fyplot_demo2`

 * *Files identical despite different names*

### Comparing `fyplot-2.0/bin/fyplot_demo` & `fyplot-2.1/bin/fyplot_demo`

 * *Files identical despite different names*

### Comparing `fyplot-2.0/fyplot/function_plot.py` & `fyplot-2.1/fyplot/function_plot.py`

 * *Files identical despite different names*

### Comparing `fyplot-2.0/fyplot/dict_plot.py` & `fyplot-2.1/fyplot/dict_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright(c) 2020  Max Planck Gesellschaft
 # Author: Vincent Berenz
 
-from pyqtgraph.Qt import QtGui, QtCore, QtWidgets
+from pyqtgraph.Qt import QtCore, QtWidgets
 import pyqtgraph as pg
 from collections import deque
 import threading,math,time
 
 pg.setConfigOptions(antialias=True)
 
 class Config:
@@ -17,16 +17,16 @@
         self.data_size = 200
         self.title = "untitled"
         self.windows_size = [800,800]
         self.start = False
         self.limits = {}
 
         
-_APPLICATION = QtGui.QApplication([])
-_WIN = pg.GraphicsWindow(title="pasta")
+_APPLICATION = QtWidgets.QApplication([])
+_WIN = pg.GraphicsLayoutWidget(title="pasta")
 _WIN.resize(1,1)
 _WIN.setWindowTitle("")
 
 
 _FIRST_ITERATION = True
 _CHANNELS = {}
 _PLOTS = {} # key : channel , value : {slot:(plot,curve)}
@@ -88,14 +88,15 @@
             curves = {}
             for slot in _CONFIG.slots[channel]:
                 curve = p.plot(pen=_CONFIG.slots_colors[slot],name=slot)
                 curves[slot]=(p,curve)
             _PLOTS[channel]=curves
         _WIN.nextRow()
 
+    _WIN.show()
     _CONFIG.start = True
 
     
 def set_data(data):
     global _CHANNELS
     for channel,d in data.items():
         _CHANNELS[channel].update(d)
@@ -127,13 +128,13 @@
     
 def start_plotting(config,target_function):
     global _CONFIG
     _CONFIG = config
     _start(target_function)
     import sys
     if (sys.flags.interactive != 1) or not hasattr(QtCore, 'PYQT_VERSION'):
-        QtGui.QApplication.instance().exec_()
+        QtWidgets.QApplication.instance().exec_()
```

