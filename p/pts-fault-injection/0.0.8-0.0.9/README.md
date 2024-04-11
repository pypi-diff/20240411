# Comparing `tmp/pts_fault_injection-0.0.8.tar.gz` & `tmp/pts_fault_injection-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fault_injection-0.0.8.tar", last modified: Fri May 12 09:13:28 2023, max compression
+gzip compressed data, was "dist/pts_fault_injection-0.0.9.tar", last modified: Fri Feb  2 11:21:04 2024, max compression
```

## Comparing `pts_fault_injection-0.0.8.tar` & `pts_fault_injection-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 09:13:28.000000 pts_fault_injection-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-12 09:13:28.000000 pts_fault_injection-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 09:13:28.000000 pts_fault_injection-0.0.8/pts_fault_injection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-12 09:13:27.000000 pts_fault_injection-0.0.8/pts_fault_injection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-12 09:13:27.000000 pts_fault_injection-0.0.8/pts_fault_injection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 09:13:27.000000 pts_fault_injection-0.0.8/pts_fault_injection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-12 09:13:27.000000 pts_fault_injection-0.0.8/pts_fault_injection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-05-12 09:13:27.000000 pts_fault_injection-0.0.8/pts_fault_injection.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3470 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 09:13:28.000000 pts_fault_injection-0.0.8/pts_fault_injection/
--rw-rw-rw-   0 root         (0) root         (0)    23696 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/pts_fault_injection/fib_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     6146 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/pts_fault_injection/cmb_box.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/pts_fault_injection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6176 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/pts_fault_injection/load_box.py
--rw-rw-rw-   0 root         (0) root         (0)     7764 2023-05-12 09:13:17.000000 pts_fault_injection-0.0.8/pts_fault_injection/CANFWupdate.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 09:13:28.000000 pts_fault_injection-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection/
+-rw-rw-rw-   0 root         (0) root         (0)    23723 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/fib_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     6146 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/cmb_box.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6176 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/load_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     7764 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/CANFWupdate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/setup.cfg
```

### Comparing `pts_fault_injection-0.0.8/PKG-INFO` & `pts_fault_injection-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fault_injection
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.8/setup.py` & `pts_fault_injection-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fault_injection",
-    version="0.0.8",
+    version="0.0.9",
     author="Pass testing Solutions GmbH",
     description="Fault Injection box Diagnostics package Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/pts-fault-injection-box",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     py_modules=["pts_fault_injection"],
-    install_requires=['python-can==4.0.0', 'dash==2.5.1', 'cantools==37.0.7', 'tabulate==0.8.10', 'uptime==3.0.1',
+    install_requires=['python-can==4.0.0', 'dash==2.5.1', 'cantools>=37.0.7', 'tabulate==0.8.10', 'uptime==3.0.1',
                       'pyserial==3.5'],
     packages=find_packages(include=['pts_fault_injection']),
+    package_data={'pts_fault_injection': ['dbc/*.dbc']},
     include_package_data=True,
 )
```

### Comparing `pts_fault_injection-0.0.8/pts_fault_injection.egg-info/PKG-INFO` & `pts_fault_injection-0.0.9/pts_fault_injection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fault-injection
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.8/LICENSE.txt` & `pts_fault_injection-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.8/README.md` & `pts_fault_injection-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.8/pts_fault_injection/fib_controller.py` & `pts_fault_injection-0.0.9/pts_fault_injection/fib_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,22 +55,23 @@
     """
     Base class for the Fault Injection Box Controller
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%Y-%m-%d %H:%M:%S',
                         level=logging.INFO)
 
-    def __init__(self, dbc_dir="../dbc/"):
+    def __init__(self, dbc_dir=os.path.join(os.path.dirname(__file__))+"/dbc/"):
         self.can_db = cantools.database.Database()
         self.bus = None
-        logging.info(f"Searching for DBCs in {dbc_dir}")
-        for file in os.listdir(dbc_dir):
+        self.dbc_dir = dbc_dir
+        logging.info(f"Searching for DBCs in {self.dbc_dir}")
+        for file in os.listdir(self.dbc_dir):
             if file.endswith(".dbc"):
                 logging.info(f"adding {file}")
-                self.can_db.add_dbc_file(os.path.join(os.getcwd(), dbc_dir + file))
+                self.can_db.add_dbc_file(os.path.join(os.getcwd(), self.dbc_dir + file))
         self.signal_cards = [
             StandardSignalCard(),
             StandardSignalCard(),
             StandardSignalCard(),
             StandardSignalCard(),
             AnalogSignalCard(),
             BusSignalCard(),
@@ -203,22 +204,20 @@
             return [-1, -1]
 
 
 class SignalCard(object):
     """
     Base class for the Signal Cards
     """
-    def __init__(self, dbc_dir="../dbc/"):
+    def __init__(self, dbc_dir=os.path.join(os.path.dirname(__file__))+"/dbc/"):
         self.bus = None
         self.can_db = cantools.database.Database()
         self.dbc_dir = dbc_dir
-        print(f"Searching for DBCs in {self.dbc_dir}")
         for file in os.listdir(self.dbc_dir):
             if file.endswith(".dbc"):
-                print(f"adding {file}")
                 self.can_db.add_dbc_file(os.path.join(os.getcwd(), self.dbc_dir + file))
 
         self.state = 0
         self.cmd_len = None
 
     def can_connection(self, interface, channel, bitrate):
         """
```

### Comparing `pts_fault_injection-0.0.8/pts_fault_injection/cmb_box.py` & `pts_fault_injection-0.0.9/pts_fault_injection/cmb_box.py`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.8/pts_fault_injection/load_box.py` & `pts_fault_injection-0.0.9/pts_fault_injection/load_box.py`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.8/pts_fault_injection/CANFWupdate.py` & `pts_fault_injection-0.0.9/pts_fault_injection/CANFWupdate.py`

 * *Files identical despite different names*

