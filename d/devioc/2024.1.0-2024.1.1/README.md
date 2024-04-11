# Comparing `tmp/devioc-2024.1.0.tar.gz` & `tmp/devioc-2024.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devioc-2024.1.0.tar", last modified: Wed Feb 21 15:11:50 2024, max compression
+gzip compressed data, was "devioc-2024.1.1.tar", last modified: Thu Apr 11 17:08:01 2024, max compression
```

## Comparing `devioc-2024.1.0.tar` & `devioc-2024.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-02-21 15:11:50.140364 devioc-2024.1.0/
--rw-rw-r--   0 michel   (70005) michel   (70005)     1066 2020-05-10 23:36:10.000000 devioc-2024.1.0/LICENSE
--rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-02-21 15:11:50.140364 devioc-2024.1.0/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      568 2020-05-11 01:30:54.000000 devioc-2024.1.0/README.md
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-02-21 15:11:50.140364 devioc-2024.1.0/bin/
--rwxrwxr-x   0 michel   (70005) michel   (70005)     9465 2022-02-17 18:35:37.000000 devioc-2024.1.0/bin/devioc-startproject
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-02-21 15:11:50.140364 devioc-2024.1.0/devioc/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2020-05-10 23:36:10.000000 devioc-2024.1.0/devioc/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     2819 2020-05-10 23:36:10.000000 devioc-2024.1.0/devioc/log.py
--rw-rw-r--   0 michel   (70005) michel   (70005)    16316 2024-02-21 14:53:19.000000 devioc-2024.1.0/devioc/models.py
--rw-r--r--   0 michel   (70005) michel   (70005)     1366 2020-05-10 23:50:35.000000 devioc-2024.1.0/devioc/version.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-02-21 15:11:50.140364 devioc-2024.1.0/devioc.egg-info/
--rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-02-21 15:11:50.000000 devioc-2024.1.0/devioc.egg-info/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      301 2024-02-21 15:11:50.000000 devioc-2024.1.0/devioc.egg-info/SOURCES.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)        1 2024-02-21 15:11:50.000000 devioc-2024.1.0/devioc.egg-info/dependency_links.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       82 2024-02-21 15:11:50.000000 devioc-2024.1.0/devioc.egg-info/requires.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       12 2024-02-21 15:11:50.000000 devioc-2024.1.0/devioc.egg-info/top_level.txt
--rw-r--r--   0 michel   (70005) michel   (70005)       38 2024-02-21 15:11:50.140364 devioc-2024.1.0/setup.cfg
--rw-rw-r--   0 michel   (70005) michel   (70005)     1018 2022-02-17 18:35:37.000000 devioc-2024.1.0/setup.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-02-21 15:11:50.140364 devioc-2024.1.0/test/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-02-17 18:35:37.000000 devioc-2024.1.0/test/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     4462 2024-02-16 17:57:09.000000 devioc-2024.1.0/test/test_ioc.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1066 2020-05-10 23:36:10.000000 devioc-2024.1.1/LICENSE
+-rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-11 17:08:01.065239 devioc-2024.1.1/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      568 2020-05-11 01:30:54.000000 devioc-2024.1.1/README.md
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.064239 devioc-2024.1.1/bin/
+-rwxrwxr-x   0 michel   (70005) michel   (70005)     9465 2022-02-17 18:35:37.000000 devioc-2024.1.1/bin/devioc-startproject
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/devioc/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2020-05-10 23:36:10.000000 devioc-2024.1.1/devioc/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     2819 2020-05-10 23:36:10.000000 devioc-2024.1.1/devioc/log.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)    16674 2024-04-11 16:55:14.000000 devioc-2024.1.1/devioc/models.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     1366 2020-05-10 23:50:35.000000 devioc-2024.1.1/devioc/version.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/devioc.egg-info/
+-rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      301 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/SOURCES.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)        1 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/dependency_links.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       82 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/requires.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       12 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/top_level.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)       38 2024-04-11 17:08:01.065239 devioc-2024.1.1/setup.cfg
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1018 2022-02-17 18:35:37.000000 devioc-2024.1.1/setup.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/test/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-02-17 18:35:37.000000 devioc-2024.1.1/test/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     4462 2024-02-16 17:57:09.000000 devioc-2024.1.1/test/test_ioc.py
```

### Comparing `devioc-2024.1.0/LICENSE` & `devioc-2024.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.0/PKG-INFO` & `devioc-2024.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devioc
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: Simple Python based EPICS Device IOC Support
 Home-page: https://github.com/michel4j/devioc
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Keywords: epics device ioc development
 Classifier: Intended Audience :: Developers
```

### Comparing `devioc-2024.1.0/README.md` & `devioc-2024.1.1/README.md`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.0/bin/devioc-startproject` & `devioc-2024.1.1/bin/devioc-startproject`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.0/devioc/log.py` & `devioc-2024.1.1/devioc/log.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.0/devioc/models.py` & `devioc-2024.1.1/devioc/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import shutil
 import subprocess
 import sys
 import time
 from collections.abc import Iterable
 from enum import EnumMeta
 from pathlib import Path
+from typing import Tuple
 
 import gepics
 
 from . import log
 
 ENUM_KEYS = [
     'ZR', 'ON', 'TW', 'TH', 'FR', 'FV', 'SX', 'SV',
@@ -443,45 +444,58 @@
     which accepts the active record (pv), the changed value (value) and the ioc instance (ioc). If the Model
     is also the callbacks provider, self, and ioc are identical, otherwise ioc is a reference to the database
     model on which the record resides.
     """
 
     def __init__(self, device_name, callbacks=None, command='softIoc', macros=None):
         self.device_name = device_name
+        self.db_name = self.__class__.__name__
         self.callbacks = callbacks or self
         self.ioc_process = None
         self.macros = {'device': self.device_name}
         if isinstance(macros, dict):
             self.macros.update(**macros)
         self.command = command
         self.ready = False
         self.directory = Path(os.getcwd())
         self.connections = {}
         self.db_cache_dir = self.directory / '__dbcache__'
         self._startup()
         self._setup()
 
-    def _startup(self):
+    def save_db(self) -> Tuple[Path, Path]:
         """
-        Generate the database and start the IOC application in a separate process
+        Save the database and command files
+        :return: Tuple of database and command file paths
         """
+
         if not self.db_cache_dir.exists():
             self.db_cache_dir.mkdir(parents=True, exist_ok=True)
 
-        db_name = self.__class__.__name__
-        with open(self.db_cache_dir / f'{db_name}.db', 'w') as db_file:
+        db_filename = self.db_cache_dir / f'{self.db_name}.db'
+        cmd_filename = self.db_cache_dir / f'{self.db_name}.cmd'
+        with open(db_filename, 'w') as db_file:
             for k, v in self._fields.items():
                 db_file.write(str(v))
 
-        with open(self.db_cache_dir / f'{db_name}.cmd', 'w') as cmd_file:
+        with open(cmd_filename, 'w') as cmd_file:
             macro_text = ','.join(['{}={}'.format(k, v) for k, v in self.macros.items()])
-            cmd_file.write(CMD_TEMPLATE.format(macros=macro_text, db_name=db_name))
+            cmd_file.write(CMD_TEMPLATE.format(macros=macro_text, db_name=self.db_name))
+
+        return db_filename, cmd_filename
+
+    def _startup(self):
+        """
+        Generate the database and start the IOC application in a separate process
+        """
+
+        self.save_db()
 
         os.chdir(self.db_cache_dir)
-        args = [self.command, f'{db_name}.cmd']
+        args = [self.command, f'{self.db_name}.cmd']
 
         self.ioc_process = multiprocessing.Process(
             target=run_softioc,
             args=(args, sys.stdin.fileno(), sys.stdout.fileno()),
         )
         self.ioc_process.daemon = True
         self.ioc_process.start()
```

### Comparing `devioc-2024.1.0/devioc/version.py` & `devioc-2024.1.1/devioc/version.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.0/devioc.egg-info/PKG-INFO` & `devioc-2024.1.1/devioc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devioc
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: Simple Python based EPICS Device IOC Support
 Home-page: https://github.com/michel4j/devioc
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Keywords: epics device ioc development
 Classifier: Intended Audience :: Developers
```

### Comparing `devioc-2024.1.0/setup.py` & `devioc-2024.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.0/test/test_ioc.py` & `devioc-2024.1.1/test/test_ioc.py`

 * *Files identical despite different names*

