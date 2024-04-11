# Comparing `tmp/thonny-etboard-micropython-firmware-1.0.1.tar.gz` & `tmp/thonny-etboard-micropython-firmware-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-etboard-micropython-firmware-1.0.1.tar", last modified: Tue Aug 31 00:45:12 2021, max compression
+gzip compressed data, was "thonny-etboard-micropython-firmware-1.0.3.tar", last modified: Wed Apr 10 14:47:54 2024, max compression
```

## Comparing `thonny-etboard-micropython-firmware-1.0.1.tar` & `thonny-etboard-micropython-firmware-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.932883 thonny-etboard-micropython-firmware-1.0.1/
--rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      638 2021-08-31 00:45:12.931816 thonny-etboard-micropython-firmware-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       90 2021-07-27 04:20:38.000000 thonny-etboard-micropython-firmware-1.0.1/README.md
--rw-rw-rw-   0        0        0      108 2021-07-26 05:23:52.000000 thonny-etboard-micropython-firmware-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-08-31 00:45:12.932883 thonny-etboard-micropython-firmware-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      943 2021-08-31 00:41:23.000000 thonny-etboard-micropython-firmware-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.903677 thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/
--rw-rw-rw-   0        0        0      638 2021-08-31 00:45:12.000000 thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2021-08-31 00:45:12.000000 thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-31 00:45:12.000000 thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2021-08-31 00:45:12.000000 thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-08-31 00:45:12.000000 thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.876740 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.905662 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/
--rw-rw-rw-   0        0        0     3505 2021-08-31 00:44:48.000000 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.908654 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/__pycache__/
--rw-rw-rw-   0        0        0     3568 2021-07-22 01:02:16.000000 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.881728 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/etboard/
-drwxrwxrwx   0        0        0        0 2021-08-31 00:45:12.923836 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/etboard/firmware/
--rw-rw-rw-   0        0        0  1488656 2021-06-08 08:42:28.000000 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
--rw-rw-rw-   0        0        0  1556784 2021-08-30 07:58:36.000000 thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
+drwxrwxrwx   0        0        0        0 2024-04-10 14:47:54.984849 thonny-etboard-micropython-firmware-1.0.3/
+-rw-rw-rw-   0        0        0     1081 2021-07-26 05:20:04.000000 thonny-etboard-micropython-firmware-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      672 2024-04-10 14:47:54.984849 thonny-etboard-micropython-firmware-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2024-04-10 12:15:53.000000 thonny-etboard-micropython-firmware-1.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-10 09:21:20.000000 thonny-etboard-micropython-firmware-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:47:54.985845 thonny-etboard-micropython-firmware-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      986 2024-04-10 14:47:42.000000 thonny-etboard-micropython-firmware-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:47:54.976875 thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/
+-rw-rw-rw-   0        0        0      672 2024-04-10 14:47:54.000000 thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2024-04-10 14:47:54.000000 thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:47:54.000000 thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 14:47:54.000000 thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 14:47:54.000000 thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:47:54.963244 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/
+drwxrwxrwx   0        0        0        0 2024-04-10 14:47:54.978869 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/
+-rw-rw-rw-   0        0        0     1106 2024-04-10 07:05:59.000000 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:47:54.963244 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/
+drwxrwxrwx   0        0        0        0 2024-04-10 14:47:54.982855 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/firmware/
+-rw-rw-rw-   0        0        0      233 2024-04-10 12:29:43.000000 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/firmware/ReadMe.md
+-rw-rw-rw-   0        0        0  1488656 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
+-rw-rw-rw-   0        0        0  1556784 2024-04-09 09:29:18.000000 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
+-rw-rw-rw-   0        0        0     4218 2024-04-10 12:47:19.000000 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/thonny_v3.py
+-rw-rw-rw-   0        0        0     5173 2024-04-10 14:35:55.000000 thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/thonny_v4.py
```

### Comparing `thonny-etboard-micropython-firmware-1.0.1/LICENSE` & `thonny-etboard-micropython-firmware-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-1.0.1/setup.py` & `thonny-etboard-micropython-firmware-1.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thonny-etboard-micropython-firmware",
-    version="1.0.1",
+    version="1.0.3",
     author="KETRi",
     author_email="ketri3000@gmail.com",
-    description="ET보드 마이크로파이썬 펌웨어",
+    description="이티보드 마이크로파이썬 펌웨어 - Thonny V4 지원",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://et.ketri.re.kr/",
     project_urls={
         "Bug Tracker": "http://et.ketri.re.kr/",
     },
     classifiers=[
@@ -20,8 +20,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=["thonnycontrib.thonny_etboard_firmware"],
     package_data={"thonnycontrib.thonny_etboard_firmware" : ["*", "*/*", "*/*/*", "*/*/*/*", "*/*/*/*/*"]},
     install_requires = ["thonny>=3.3.11"],
     python_requires=">=3.6",
+    license='MIT',
 )
```

### Comparing `thonny-etboard-micropython-firmware-1.0.1/thonny_etboard_micropython_firmware.egg-info/SOURCES.txt` & `thonny-etboard-micropython-firmware-1.0.3/thonny_etboard_micropython_firmware.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 thonny_etboard_micropython_firmware.egg-info/PKG-INFO
 thonny_etboard_micropython_firmware.egg-info/SOURCES.txt
 thonny_etboard_micropython_firmware.egg-info/dependency_links.txt
 thonny_etboard_micropython_firmware.egg-info/requires.txt
 thonny_etboard_micropython_firmware.egg-info/top_level.txt
 thonnycontrib/thonny_etboard_firmware/__init__.py
-thonnycontrib/thonny_etboard_firmware/__pycache__/__init__.cpython-39.pyc
+thonnycontrib/thonny_etboard_firmware/thonny_v3.py
+thonnycontrib/thonny_etboard_firmware/thonny_v4.py
+thonnycontrib/thonny_etboard_firmware/etboard/firmware/ReadMe.md
 thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin
 thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin
```

### Comparing `thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/__init__.py` & `thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/thonny_v3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# ******************************************************************************************
+# FileName     : thonny_v3.py
+# Description  : ETboard MicroPython Firmware 다운로드 플러그인 for Thonny V3
+# Author       : 위대원
+# Created Date : 2021.08.31
+# Reference    :
+# Modified     : SCS : 2024.04.10 : Clean Code a little
+# ******************************************************************************************
+
+# import for global
 import tkinter as tk
 import os
 import time
 from glob import glob
 from thonny import get_workbench, workbench
 from tkinter.messagebox import showinfo
 from thonny import ui_utils
@@ -101,14 +111,18 @@
                                 group=10)
 
         self.workbench.add_command(command_id="et-interpreter",
                                 menu_name="file",
                                 command_label="ET-board 인터프리터 설정",
                                 handler=self.interpreter_select,
                                 group=10)
+       
 
 
-        
-
+#if get_workbench() is not None:
+#    run = ETBoardMenu().load_plugin()
 
-if get_workbench() is not None:
-    run = ETBoardMenu().load_plugin()
+# ==========================================================================================
+#
+#  (주)한국공학기술연구원 http://et.ketri.re.kr
+#
+# ==========================================================================================
```

### Comparing `thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin` & `thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0608_last.bin`

 * *Files identical despite different names*

### Comparing `thonny-etboard-micropython-firmware-1.0.1/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin` & `thonny-etboard-micropython-firmware-1.0.3/thonnycontrib/thonny_etboard_firmware/etboard/firmware/etboard_firmware_micropython_custom_0831_last.bin`

 * *Files identical despite different names*

