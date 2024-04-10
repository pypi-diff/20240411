# Comparing `tmp/auto-qchem-1.3.5.tar.gz` & `tmp/auto-qchem-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto-qchem-1.3.5.tar", last modified: Thu Nov 16 01:05:39 2023, max compression
+gzip compressed data, was "dist/auto-qchem-1.3.6.tar", last modified: Wed Apr 10 21:56:18 2024, max compression
```

## Comparing `auto-qchem-1.3.5.tar` & `auto-qchem-1.3.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/
--rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.5/LICENSE.md
--rw-r--r--   0 mac        (501) staff       (20)      306 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1452 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/auto_qchem.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      306 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/auto_qchem.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      593 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/auto_qchem.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/auto_qchem.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      221 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/auto_qchem.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/auto_qchem.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/autoqchem/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/autoqchem/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    24645 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/autoqchem/db_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.5/autoqchem/descriptor_functions.py
--rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.5/autoqchem/draw_utils.py
--rw-r--r--   0 mac        (501) staff       (20)     6445 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/autoqchem/gaussian_input_generator.py
--rw-r--r--   0 mac        (501) staff       (20)    19324 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/autoqchem/gaussian_log_extractor.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2023-10-17 04:18:23.000000 auto-qchem-1.3.5/autoqchem/helper_classes.py
--rw-r--r--   0 mac        (501) staff       (20)     4234 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/autoqchem/helper_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2700 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/autoqchem/molecule.py
--rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.5/autoqchem/openbabel_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    11508 2023-10-17 04:18:23.000000 auto-qchem-1.3.5/autoqchem/rdkit_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    28471 2023-11-16 01:05:05.000000 auto-qchem-1.3.5/autoqchem/sge_manager.py
--rw-r--r--   0 mac        (501) staff       (20)    26054 2023-10-17 04:18:23.000000 auto-qchem-1.3.5/autoqchem/slurm_manager.py
--rw-r--r--   0 mac        (501) staff       (20)     1374 2023-08-18 17:24:25.000000 auto-qchem-1.3.5/autoqchem/test.py
--rw-r--r--   0 mac        (501) staff       (20)      211 2023-10-17 04:18:07.000000 auto-qchem-1.3.5/config.yml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-11-16 01:05:39.000000 auto-qchem-1.3.5/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1089 2023-11-16 01:05:27.000000 auto-qchem-1.3.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/
+-rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.6/LICENSE.md
+-rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1452 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      593 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      221 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/autoqchem/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    24645 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/db_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.6/autoqchem/descriptor_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.6/autoqchem/draw_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)     6445 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/gaussian_input_generator.py
+-rw-r--r--   0 mac        (501) staff       (20)    19324 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/gaussian_log_extractor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/helper_classes.py
+-rw-r--r--   0 mac        (501) staff       (20)     4234 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/helper_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2700 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/molecule.py
+-rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.6/autoqchem/openbabel_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    11508 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/rdkit_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    28471 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/sge_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)    26054 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/slurm_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)     1374 2023-08-18 17:24:25.000000 auto-qchem-1.3.6/autoqchem/test.py
+-rw-r--r--   0 mac        (501) staff       (20)      211 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/config.yml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1089 2024-04-10 21:56:10.000000 auto-qchem-1.3.6/setup.py
```

### Comparing `auto-qchem-1.3.5/LICENSE.md` & `auto-qchem-1.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/README.md` & `auto-qchem-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/auto_qchem.egg-info/SOURCES.txt` & `auto-qchem-1.3.6/auto_qchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/db_functions.py` & `auto-qchem-1.3.6/autoqchem/db_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/descriptor_functions.py` & `auto-qchem-1.3.6/autoqchem/descriptor_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/draw_utils.py` & `auto-qchem-1.3.6/autoqchem/draw_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/gaussian_input_generator.py` & `auto-qchem-1.3.6/autoqchem/gaussian_input_generator.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/gaussian_log_extractor.py` & `auto-qchem-1.3.6/autoqchem/gaussian_log_extractor.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/helper_classes.py` & `auto-qchem-1.3.6/autoqchem/helper_classes.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/helper_functions.py` & `auto-qchem-1.3.6/autoqchem/helper_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/molecule.py` & `auto-qchem-1.3.6/autoqchem/molecule.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/openbabel_utils.py` & `auto-qchem-1.3.6/autoqchem/openbabel_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/rdkit_utils.py` & `auto-qchem-1.3.6/autoqchem/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/sge_manager.py` & `auto-qchem-1.3.6/autoqchem/sge_manager.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/slurm_manager.py` & `auto-qchem-1.3.6/autoqchem/slurm_manager.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/autoqchem/test.py` & `auto-qchem-1.3.6/autoqchem/test.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.5/setup.py` & `auto-qchem-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='auto-qchem',
-    version='1.3.5',
+    version='1.3.6',
     packages=['autoqchem'],
     data_files=['config.yml'],
     url='https://github.com/doyle-lab-ucla/auto-qchem',
     license='GPL',
     author='Andrzej Zuranski, Benjamin Shields, Jason Wang, Winston Gee',
     description='auto-qchem',
     long_description='automated dft calculation management software',
```

