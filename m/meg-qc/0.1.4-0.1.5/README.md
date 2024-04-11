# Comparing `tmp/meg_qc-0.1.4.tar.gz` & `tmp/meg_qc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meg_qc-0.1.4.tar", last modified: Tue Apr  9 11:37:34 2024, max compression
+gzip compressed data, was "meg_qc-0.1.5.tar", last modified: Thu Apr 11 13:09:42 2024, max compression
```

## Comparing `meg_qc-0.1.4.tar` & `meg_qc-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.881488 meg_qc-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 11:37:26.000000 meg_qc-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-09 11:37:34.881488 meg_qc-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-09 11:37:26.000000 meg_qc-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.881488 meg_qc-0.1.4/meg_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 11:37:34.881488 meg_qc-0.1.4/meg_qc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20295 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/meg_qc_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/meg_qc_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    20622 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/meg_qc_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.881488 meg_qc-0.1.4/meg_qc/source/
--rw-r--r--   0 runner    (1001) docker     (127)   116244 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/ECG_EOG_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16880 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/Head_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    55779 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/PSD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/Peaks_auto_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18802 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/Peaks_manual_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26313 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/STD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26247 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/initial_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/muscle_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/universal_html_report.py
--rw-r--r--   0 runner    (1001) docker     (127)   116887 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/universal_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.877488 meg_qc-0.1.4/meg_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 11:37:26.000000 meg_qc-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-09 11:37:34.881488 meg_qc-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 11:37:26.000000 meg_qc-0.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-09 11:37:26.000000 meg_qc-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:09:42.743640 meg_qc-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-11 13:09:32.000000 meg_qc-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-11 13:09:42.743640 meg_qc-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-11 13:09:32.000000 meg_qc-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:09:42.743640 meg_qc-0.1.5/meg_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 13:09:32.000000 meg_qc-0.1.5/meg_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-11 13:09:32.000000 meg_qc-0.1.5/meg_qc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 13:09:42.743640 meg_qc-0.1.5/meg_qc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:09:42.743640 meg_qc-0.1.5/meg_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-11 13:09:42.000000 meg_qc-0.1.5/meg_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 13:09:42.000000 meg_qc-0.1.5/meg_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:09:42.000000 meg_qc-0.1.5/meg_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 13:09:42.000000 meg_qc-0.1.5/meg_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 13:09:42.000000 meg_qc-0.1.5/meg_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 13:09:32.000000 meg_qc-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-11 13:09:42.743640 meg_qc-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-11 13:09:32.000000 meg_qc-0.1.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-11 13:09:32.000000 meg_qc-0.1.5/versioneer.py
```

### Comparing `meg_qc-0.1.4/LICENSE` & `meg_qc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.4/PKG-INFO` & `meg_qc-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg_qc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.4/README.md` & `meg_qc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.4/meg_qc/__main__.py` & `meg_qc-0.1.5/meg_qc/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 sys.path.append('./')
-from meg_qc.meg_qc_pipeline import make_derivative_meg_qc
+from meg_qc.calculating.meg_qc_pipeline import make_derivative_meg_qc
 
 #Add initial setup here (offer to install dependencies, etc.)
 
 def main():
 
     print("\nWelcome to MEG QC\n")
```

### Comparing `meg_qc-0.1.4/meg_qc.egg-info/PKG-INFO` & `meg_qc-0.1.5/meg_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg-qc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.4/setup.cfg` & `meg_qc-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.4/setup.py` & `meg_qc-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     with open(REQ_FILE_PATH) as f:
         INSTALL_REQUIRES = list(f.read().splitlines())
     setup(name='meg_qc',
         version= versioneer.get_version(),
         cmdclass=versioneer.get_cmdclass(),
         setup_requires=SETUP_REQUIRES,
         install_requires=INSTALL_REQUIRES,
-        packages=['meg_qc','meg_qc/source'],
+        packages=['meg_qc'],
         url='https://github.com/AaronReer/MEGqc',
         license='MIT',
         author='ANCP',
-        author_email='aaron.reer@uol.de')
+        author_email='aaron.reer@uol.de')
```

### Comparing `meg_qc-0.1.4/versioneer.py` & `meg_qc-0.1.5/versioneer.py`

 * *Files identical despite different names*

