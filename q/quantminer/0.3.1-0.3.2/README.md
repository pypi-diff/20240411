# Comparing `tmp/quantminer-0.3.1.tar.gz` & `tmp/quantminer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.3.1.tar", last modified: Wed Apr 10 21:17:35 2024, max compression
+gzip compressed data, was "quantminer-0.3.2.tar", last modified: Thu Apr 11 02:05:26 2024, max compression
```

## Comparing `quantminer-0.3.1.tar` & `quantminer-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.655459 quantminer-0.3.1/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:17:35.655284 quantminer-0.3.1/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.3.1/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.649689 quantminer-0.3.1/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.3.1/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.654357 quantminer-0.3.1/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.3.1/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.3.1/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.3.1/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    18877 2024-04-10 21:16:30.000000 quantminer-0.3.1/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.650722 quantminer-0.3.1/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 21:17:35.655677 quantminer-0.3.1/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 21:16:43.000000 quantminer-0.3.1/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.517655 quantminer-0.3.2/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 02:05:26.517538 quantminer-0.3.2/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.3.2/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.515715 quantminer-0.3.2/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.3.2/quantminer/__init__.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.517215 quantminer-0.3.2/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.3.2/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.3.2/quantminer/classes/pivot_pip.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.3.2/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    18864 2024-04-11 02:04:50.000000 quantminer-0.3.2/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.516620 quantminer-0.3.2/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-11 02:05:26.517699 quantminer-0.3.2/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-11 02:04:39.000000 quantminer-0.3.2/setup.py
```

### Comparing `quantminer-0.3.1/quantminer/classes/pivot_pip.py` & `quantminer-0.3.2/quantminer/classes/pivot_pip.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.3.1/quantminer/classes/seqkmeans.py` & `quantminer-0.3.2/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.3.1/quantminer/pipminer.py` & `quantminer-0.3.2/quantminer/pipminer.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,27 +179,26 @@
             if _l in self._cluster_labels_short
             else 0
         )
 
         return signal, list(np.squeeze(_pivots))
 
 
-    @staticmethod
-    def save_model(path:Union[Path, str]):
+    def save_model(self, path:Union[Path, str]):
         # Convert path to Path object, and check if it exists
         if not isinstance(path, Path):
             path = Path(str)
             
             if not path.exists():
                 raise FileNotFoundError(f"File not found: {path}")
             
         # Save model
         with open(path, 'wb') as f:
             try:
-                pickle.dump(miner, f)
+                pickle.dump(self, f)
                 print(f'Model saved at {path}')
             except Exception as e:
                 raise e
     
     @staticmethod
     def load_model(path:Union[Path, str]):
         # Convert path to Path object, and check if it exists
```

### Comparing `quantminer-0.3.1/setup.py` & `quantminer-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='quantminer',
-    version='0.3.1', 
+    version='0.3.2', 
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=[  # List any dependencies here
         "kneed",
         "quantstats",
```

