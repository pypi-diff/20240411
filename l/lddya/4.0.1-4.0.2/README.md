# Comparing `tmp/lddya-4.0.1.tar.gz` & `tmp/lddya-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lddya-4.0.1.tar", last modified: Sun Nov 12 14:15:23 2023, max compression
+gzip compressed data, was "lddya-4.0.2.tar", last modified: Thu Apr 11 13:03:05 2024, max compression
```

## Comparing `lddya-4.0.1.tar` & `lddya-4.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-11-12 14:15:23.102214 lddya-4.0.1/
--rw-rw-rw-   0        0        0      310 2023-11-12 14:15:23.102214 lddya-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       74 2021-12-03 06:05:24.000000 lddya-4.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-11-12 14:15:23.099214 lddya-4.0.1/lddya/
--rw-rw-rw-   0        0        0    22096 2023-09-07 03:20:10.000000 lddya-4.0.1/lddya/Algorithm.py
--rw-rw-rw-   0        0        0     7851 2022-11-01 06:31:16.000000 lddya-4.0.1/lddya/Data.py
--rw-rw-rw-   0        0        0     1444 2022-01-21 14:37:00.000000 lddya-4.0.1/lddya/DataFrame.py
--rw-rw-rw-   0        0        0     2272 2023-10-30 08:59:16.000000 lddya-4.0.1/lddya/Draw.py
--rw-rw-rw-   0        0        0     4893 2022-10-21 12:41:30.000000 lddya-4.0.1/lddya/Map.py
--rw-rw-rw-   0        0        0    16714 2021-12-03 06:05:24.000000 lddya-4.0.1/lddya/Optimizer.py
--rw-rw-rw-   0        0        0       54 2023-09-07 03:17:02.000000 lddya-4.0.1/lddya/__init__.py
--rw-rw-rw-   0        0        0      393 2021-12-03 06:05:24.000000 lddya-4.0.1/lddya/tool.py
-drwxrwxrwx   0        0        0        0 2023-11-12 14:15:23.101214 lddya-4.0.1/lddya.egg-info/
--rw-rw-rw-   0        0        0      310 2023-11-12 14:15:23.000000 lddya-4.0.1/lddya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-11-12 14:15:23.000000 lddya-4.0.1/lddya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-12 14:15:23.000000 lddya-4.0.1/lddya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-11-12 14:15:23.000000 lddya-4.0.1/lddya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-12 14:15:23.000000 lddya-4.0.1/lddya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-12 14:15:23.102214 lddya-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0      781 2023-11-12 14:15:16.000000 lddya-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:03:05.934377 lddya-4.0.2/
+-rw-rw-rw-   0        0        0      310 2024-04-11 13:03:05.934377 lddya-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2021-12-03 06:05:24.000000 lddya-4.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 13:03:05.930288 lddya-4.0.2/lddya/
+-rw-rw-rw-   0        0        0    22096 2023-09-07 03:20:10.000000 lddya-4.0.2/lddya/Algorithm.py
+-rw-rw-rw-   0        0        0     7851 2022-11-01 06:31:16.000000 lddya-4.0.2/lddya/Data.py
+-rw-rw-rw-   0        0        0     1444 2022-01-21 14:37:00.000000 lddya-4.0.2/lddya/DataFrame.py
+-rw-rw-rw-   0        0        0     2372 2024-04-11 02:41:50.000000 lddya-4.0.2/lddya/Draw.py
+-rw-rw-rw-   0        0        0     4893 2022-10-21 12:41:30.000000 lddya-4.0.2/lddya/Map.py
+-rw-rw-rw-   0        0        0    16714 2021-12-03 06:05:24.000000 lddya-4.0.2/lddya/Optimizer.py
+-rw-rw-rw-   0        0        0       54 2023-09-07 03:17:02.000000 lddya-4.0.2/lddya/__init__.py
+-rw-rw-rw-   0        0        0      393 2021-12-03 06:05:24.000000 lddya-4.0.2/lddya/tool.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:03:05.933374 lddya-4.0.2/lddya.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:03:05.934377 lddya-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-04-11 13:02:41.000000 lddya-4.0.2/setup.py
```

### Comparing `lddya-4.0.1/lddya/Algorithm.py` & `lddya-4.0.2/lddya/Algorithm.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.1/lddya/Data.py` & `lddya-4.0.2/lddya/Data.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.1/lddya/DataFrame.py` & `lddya-4.0.2/lddya/DataFrame.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.1/lddya/Draw.py` & `lddya-4.0.2/lddya/Draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 import matplotlib.patches as pat
 import numpy as np
 
 class ShanGeTu():
-    def __init__(self,map_data) -> None:
+    def __init__(self,map_data,x_label = '',y_label = '') -> None:
         self.map_size = len(map_data)
         self.fig = plt.figure(figsize=(7,7))
         self.ax1 = self.fig.add_subplot(1,1,1)
         self.ax1.set_xbound(0,len(map_data))
         self.ax1.set_ybound(0,len(map_data))
         rect_pat = []
         for ki,i in enumerate(map_data):
@@ -15,14 +15,16 @@
                 if j == 1:
                     rect_pat.append(pat.Rectangle((kj,ki),1,1,color = 'k'))
                 else:
                     rect_pat.append(pat.Rectangle((kj,ki),1,1,fill = False,edgecolor = 'k',linewidth = 1))
         for i in rect_pat:
             self.ax1.add_patch(i)
         x = np.array([i for i in range(len(map_data))])
+        self.ax1.set_xlabel(x_label)
+        self.ax1.set_ylabel(y_label)
         self.ax1.set_xticks(x+0.5,x+1)
         self.ax1.set_yticks(x+0.5,x+1)
 
     def draw_way(self,way_data,style = None):
         '''
         绘制一条路线，way_data为路径经过的节点坐标。坐标格式为[y,x],这是为了对接现有的算法标准，style同plt.plot中的style
         '''
```

### Comparing `lddya-4.0.1/lddya/Map.py` & `lddya-4.0.2/lddya/Map.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.1/lddya/Optimizer.py` & `lddya-4.0.2/lddya/Optimizer.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.1/setup.py` & `lddya-4.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 ############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "lddya",
-    version = "4.0.1",
+    version = "4.0.2",
     keywords = {"pip", "license","licensetool", "tool", "gm"},
     description = "新增了优化器类别",
     long_description = "具体功能，请自行挖掘。",
     license = "MIT Licence",
 
     url = "https://github.com/not_define/please_wait",
     author = "lidongdong",
     author_email = "927052521@qq.com",
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    install_requires = ['chardet']
+    install_requires = ['numpy','matplotlib','pygame','pandas']
 )
```

