# Comparing `tmp/PyQSPICE-2024.3.18.tar.gz` & `tmp/PyQSPICE-2024.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQSPICE-2024.3.18.tar", last modified: Mon Mar 18 14:20:47 2024, max compression
+gzip compressed data, was "PyQSPICE-2024.4.11.tar", last modified: Thu Apr 11 11:50:28 2024, max compression
```

## Comparing `PyQSPICE-2024.3.18.tar` & `PyQSPICE-2024.4.11.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 14:20:47.197127 PyQSPICE-2024.3.18/
--rw-rw-rw-   0        0        0    16638 2023-10-07 20:41:32.000000 PyQSPICE-2024.3.18/LICENSE
--rw-rw-rw-   0        0        0    23031 2024-03-18 14:20:47.177124 PyQSPICE-2024.3.18/PKG-INFO
--rw-rw-rw-   0        0        0     4992 2023-12-12 01:11:18.000000 PyQSPICE-2024.3.18/README.md
--rw-rw-rw-   0        0        0      622 2024-03-18 14:14:27.000000 PyQSPICE-2024.3.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 14:20:47.198117 PyQSPICE-2024.3.18/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-18 14:20:47.005653 PyQSPICE-2024.3.18/src/
-drwxrwxrwx   0        0        0        0 2024-03-18 14:20:47.073312 PyQSPICE-2024.3.18/src/PyQSPICE/
--rw-rw-rw-   0        0        0       31 2023-10-08 19:35:43.000000 PyQSPICE-2024.3.18/src/PyQSPICE/__init__.py
--rw-rw-rw-   0        0        0    26553 2024-03-18 14:13:06.000000 PyQSPICE-2024.3.18/src/PyQSPICE/qspice.py
-drwxrwxrwx   0        0        0        0 2024-03-18 14:20:47.166119 PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/
--rw-rw-rw-   0        0        0    23031 2024-03-18 14:20:46.000000 PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-03-18 14:20:46.000000 PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 14:20:46.000000 PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-18 14:20:46.000000 PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 14:20:46.000000 PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:28.575276 PyQSPICE-2024.4.11/
+-rw-rw-rw-   0        0        0    16638 2023-10-07 20:41:32.000000 PyQSPICE-2024.4.11/LICENSE
+-rw-rw-rw-   0        0        0    23031 2024-04-11 11:50:28.561275 PyQSPICE-2024.4.11/PKG-INFO
+-rw-rw-rw-   0        0        0     4992 2023-12-12 01:11:18.000000 PyQSPICE-2024.4.11/README.md
+-rw-rw-rw-   0        0        0      622 2024-04-11 11:48:59.000000 PyQSPICE-2024.4.11/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 11:50:28.577292 PyQSPICE-2024.4.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:28.382523 PyQSPICE-2024.4.11/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:28.445071 PyQSPICE-2024.4.11/src/PyQSPICE/
+-rw-rw-rw-   0        0        0       31 2023-10-08 19:35:43.000000 PyQSPICE-2024.4.11/src/PyQSPICE/__init__.py
+-rw-rw-rw-   0        0        0    26784 2024-04-11 11:49:10.000000 PyQSPICE-2024.4.11/src/PyQSPICE/qspice.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:28.543031 PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/
+-rw-rw-rw-   0        0        0    23031 2024-04-11 11:50:28.000000 PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-04-11 11:50:28.000000 PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:50:28.000000 PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 11:50:28.000000 PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 11:50:28.000000 PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/top_level.txt
```

### Comparing `PyQSPICE-2024.3.18/LICENSE` & `PyQSPICE-2024.4.11/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQSPICE-2024.3.18/PKG-INFO` & `PyQSPICE-2024.4.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQSPICE
-Version: 2024.3.18
+Version: 2024.4.11
 Summary: Python Wrapper for QSPICE
 Author: Masashi Nogawa
 License: Qorvo "PyQSPICE" Software License Agreement
         
         This legally binding agreement, for the use of the licensed software installed upon acceptance of this License Agreement, is by and between Qorvo US, Inc, on behalf of itself and its Affiliates and subsidiaries ("Qorvo"), and either an individual or legal entity, including each Affiliate of such, as applicable, on whose behalf you are legally authorized to accept this License Agreement ("Licensee"). As used herein, "you," "your," or "Licensee" shall mean such individual or entity, including Affiliates of such entity.
         
         Licensor is only willing to license the Licensed Software to you on condition that you accept all of the terms in this License Agreement.
```

### Comparing `PyQSPICE-2024.3.18/README.md` & `PyQSPICE-2024.4.11/README.md`

 * *Files identical despite different names*

### Comparing `PyQSPICE-2024.3.18/pyproject.toml` & `PyQSPICE-2024.4.11/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyQSPICE"
-version = "2024.03.18"
+version = "2024.04.11"
 authors = [
     { name="Masashi Nogawa" },
 ]
 description = "Python Wrapper for QSPICE"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

### Comparing `PyQSPICE-2024.3.18/src/PyQSPICE/qspice.py` & `PyQSPICE-2024.4.11/src/PyQSPICE/qspice.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import math
 import cmath
 
 
 
 class clsQSPICE:
 ## Version Number
-    verstr = "2024.03.18"
+    verstr = "2024.04.11"
 
 ## Global (Class) Path Information
     gpath = {}
     gpath['cwd'] = os.getcwd()
     gpath['home'] = expanduser("~")
     usrp = gpath['home'] + "/QSPICE/"
     sysp = r"c:/Program Files/QSPICE/"
@@ -113,14 +113,21 @@
         if self.sim['label'] != 'default': label = self.sim['label']
         if label == "":  add = ""
         else:           add = label + "."
         if self.ts[add + 'cir']:
             subprocess.run([self.gpath['QSPICE64'], self.path[add + 'cir']])
             clsQSPICE.tstime(self, [add + 'qraw'])
 
+    def copy2qraw(self, label = ""):
+        if self.sim['label'] != 'default': label = self.sim['label']
+        if label == "":  add = ""
+        else:           add = label + "."
+        clsQSPICE.tstime(self, [add + 'qraw'])
+
+
     # Load simulation result signals from the simulation results QRAW file
     # Input:  Array of signal strings in the way you specify in ".PLOT" statement
     # Output:  It returns Pandas DataFrame
     #  ==> Pandas supports data loading from the STDOUT-STDIN PIPE/stream (where the Numpy doesn't...temporary file needed)
     def LoadQRAW(self, probe, label = "", Nline = -999):
         if self.sim['label'] != 'default':
             label = self.sim['label']
```

### Comparing `PyQSPICE-2024.3.18/src/PyQSPICE.egg-info/PKG-INFO` & `PyQSPICE-2024.4.11/src/PyQSPICE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQSPICE
-Version: 2024.3.18
+Version: 2024.4.11
 Summary: Python Wrapper for QSPICE
 Author: Masashi Nogawa
 License: Qorvo "PyQSPICE" Software License Agreement
         
         This legally binding agreement, for the use of the licensed software installed upon acceptance of this License Agreement, is by and between Qorvo US, Inc, on behalf of itself and its Affiliates and subsidiaries ("Qorvo"), and either an individual or legal entity, including each Affiliate of such, as applicable, on whose behalf you are legally authorized to accept this License Agreement ("Licensee"). As used herein, "you," "your," or "Licensee" shall mean such individual or entity, including Affiliates of such entity.
         
         Licensor is only willing to license the Licensed Software to you on condition that you accept all of the terms in this License Agreement.
```

