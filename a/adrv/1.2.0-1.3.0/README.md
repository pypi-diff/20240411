# Comparing `tmp/adrv-1.2.0.tar.gz` & `tmp/adrv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adrv-1.2.0.tar", max compression
+gzip compressed data, was "adrv-1.3.0.tar", max compression
```

## Comparing `adrv-1.2.0.tar` & `adrv-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    14168 2024-03-30 11:27:00.413807 adrv-1.2.0/adrv/__init__.py
--rw-r--r--   0        0        0     1466 2024-03-19 20:59:47.629936 adrv-1.2.0/adrv/_cls.py
--rw-r--r--   0        0        0     1259 2024-03-19 20:22:55.614192 adrv-1.2.0/adrv/bridge.py
--rw-r--r--   0        0        0     1043 2024-03-02 13:18:04.598600 adrv-1.2.0/adrv/utils.py
--rw-r--r--   0        0        0    35802 2024-02-09 22:09:16.946792 adrv-1.2.0/LICENSE
--rw-r--r--   0        0        0      319 2024-03-30 11:22:46.414889 adrv-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6848 2024-03-19 20:59:42.125789 adrv-1.2.0/README.md
--rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 adrv-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    14592 2024-04-11 17:21:31.670184 adrv-1.3.0/adrv/__init__.py
+-rw-r--r--   0        0        0     1466 2024-03-19 20:59:47.629936 adrv-1.3.0/adrv/_cls.py
+-rw-r--r--   0        0        0     1259 2024-03-19 20:22:55.614192 adrv-1.3.0/adrv/bridge.py
+-rw-r--r--   0        0        0     1043 2024-03-02 13:18:04.598600 adrv-1.3.0/adrv/utils.py
+-rw-r--r--   0        0        0    35802 2024-02-09 22:09:16.946792 adrv-1.3.0/LICENSE
+-rw-r--r--   0        0        0      319 2024-04-11 17:20:52.274932 adrv-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6848 2024-03-19 20:59:42.125789 adrv-1.3.0/README.md
+-rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 adrv-1.3.0/PKG-INFO
```

### Comparing `adrv-1.2.0/adrv/__init__.py` & `adrv-1.3.0/adrv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 import time
 import uuid
 import zipfile
 
 from ._cls import *
 from .utils import *
 
-VERSION = "1.2.0"
-SUPPORTS = "1.0.0"
+VERSION = "1.3.0"
+SUPPORTS = "1.3.0"
 
 class Disk:
     def __init__(self, name: str = 'vDisk', path: str = './', max_size: int = 1000 ** 2):
         """
         Initializes a Disk instance.
 
         Args:
             name (str, optional): The name of the disk. Defaults to 'vDisk'.
             path (str, optional): The path where the disk will be stored. Defaults to './'.
             max_size (int, optional): The maximum size of the disk in bytes. Defaults to 1000000.
         """
         self.name = name.upper()
-        self.path = os.path.join(path, f"{name}.adrv")
+        self.path = os.path.normpath(os.path.join(path, f"{name}.adrv")).replace('\\', '/')
         self.max_size = Size(max_size)
         self.size = Size(0)
 
         if not zipfile.is_zipfile(self.path):
             if not os.path.exists(path):
                 try:
                     os.makedirs(path)
@@ -40,15 +40,15 @@
             self.format_disk()
         
         properties = self.__sys_data('Disk/$Properties')
         self.name = properties[0]
         self.max_size = Size(int(properties[1]))
         self.size = Size(os.path.getsize(self.path))
 
-    def __read(self, _path: str, encoding: str | None = 'UTF-8') -> str:
+    def __read(self, _path: str) -> str:
         """
         Reads content from a file in the disk.
 
         Args:
             _path (str): The path of the file to be read.
             encoding (str | None, optional): The encoding of the file. Defaults to 'UTF-8'.
 
@@ -64,18 +64,18 @@
                     vPath = os.path.normpath(_path)
                     tempPath = os.path.normpath(f"{tempDir}/{vPath}")
 
                     if os.path.exists(tempPath):
                         if os.path.isdir(tempPath):
                             raise FileIsDirectoryError(f"{vPath} is a directory.")
                         else:
-                            with open(tempPath, 'rb', encoding = None) as extracted_file:
+                            with open(tempPath, 'rb') as extracted_file:
                                 content = extracted_file.read()
                                 
-                            return content.decode(encoding)
+                            return content
                     else:
                         raise FileNotFoundError(f"{vPath} was not found.")
                     
     def __write(self, content: str | bytes, _path: str) -> int:
         """
         Writes content to a file in the disk.
 
@@ -142,19 +142,19 @@
             _mode (str, optional): The mode of operation ('r', 'w', 'a'). Defaults to 'r'.
 
         Returns:
             list[str] | None: The system data.
         """
         _path = os.path.join('/.sys/', _name)
         if _mode == 'r':
-            return self.__read(_path, 'UTF-8').replace('\r', '').split('\n')
+            return self.__read(_path).decode('UTF-8').replace('\r', '').split('\n')
         elif _mode == 'w':
             self.__write(_data, _path)
         elif _mode == 'a':
-            data = self.__read(_path, 'UTF-8')
+            data = self.__read(_path).decode('UTF-8')
             if data != '':
                 _data = '\n'.join((data, _data))
             
             self.__write(_data, _path)
 
     def __ls(self) -> list[str]:
         """
@@ -202,16 +202,30 @@
     def extract_all(self, target: str) -> None:
         """
         Extracts all files from the disk to a target directory.
 
         Args:
             target (str): The target directory.
         """
-        with zipfile.ZipFile(self.path) as zip_buffer:
-            zip_buffer.extractall(target)
+
+        registry = self.__sys_data('Disk/$Registry')
+
+        for file in self.__ls():
+            try:
+                _file = [ _item for _item in registry if _item.split('::')[1] == file ][0].split('::')
+            except IndexError:
+                continue
+
+            try:
+                os.makedirs(os.path.dirname(os.path.join(target, _file[0])))
+            except FileExistsError:
+                pass
+
+            with open(os.path.normpath(os.path.join(target, _file[0])), 'wb') as buffer:
+                buffer.write(self.__read(file))
     
     def f_list(self, include_ts: bool = False, sys = False) -> list[str | dict]:
         """
         Lists files in the disk.
 
         Args:
             include_ts (bool, optional): Whether to include timestamps. Defaults to False.
@@ -229,15 +243,14 @@
 
             if include_ts:
                 namelist.append({ 'path': _item.split('::')[0], 'timestamp': _item.split('::')[2] })
             else:
                 namelist.append(_item.split('::')[0])
         
         if sys:
-            print(self.__ls())
             for name in self.__ls():
                 if name.startswith('.sys/') and not name.endswith('/'):
                     if include_ts:
                         namelist.append({'path': name, 'timestamp': 0 })
                     else:
                         namelist.append(name)
```

### Comparing `adrv-1.2.0/adrv/_cls.py` & `adrv-1.3.0/adrv/_cls.py`

 * *Files identical despite different names*

### Comparing `adrv-1.2.0/adrv/bridge.py` & `adrv-1.3.0/adrv/bridge.py`

 * *Files identical despite different names*

### Comparing `adrv-1.2.0/adrv/utils.py` & `adrv-1.3.0/adrv/utils.py`

 * *Files identical despite different names*

### Comparing `adrv-1.2.0/LICENSE` & `adrv-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adrv-1.2.0/README.md` & `adrv-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `adrv-1.2.0/PKG-INFO` & `adrv-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adrv
-Version: 1.2.0
+Version: 1.3.0
 Summary: 
 License: GPL-3.0
 Author: happex
 Author-email: 110610727+okayhappex@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

