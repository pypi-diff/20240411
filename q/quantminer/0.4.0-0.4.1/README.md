# Comparing `tmp/quantminer-0.4.0.tar.gz` & `tmp/quantminer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.4.0.tar", last modified: Thu Apr 11 15:25:44 2024, max compression
+gzip compressed data, was "quantminer-0.4.1.tar", last modified: Thu Apr 11 20:59:01 2024, max compression
```

## Comparing `quantminer-0.4.0.tar` & `quantminer-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.546450 quantminer-0.4.0/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 15:25:44.546335 quantminer-0.4.0/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.4.0/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.544686 quantminer-0.4.0/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.4.0/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.545817 quantminer-0.4.0/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.4.0/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.4.0/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.4.0/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    21815 2024-04-11 15:25:32.000000 quantminer-0.4.0/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.545210 quantminer-0.4.0/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-11 15:25:44.546486 quantminer-0.4.0/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-11 15:23:37.000000 quantminer-0.4.0/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 20:59:01.739216 quantminer-0.4.1/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 20:59:01.739093 quantminer-0.4.1/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.4.1/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 20:59:01.737398 quantminer-0.4.1/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.4.1/quantminer/__init__.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 20:59:01.738698 quantminer-0.4.1/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.4.1/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.4.1/quantminer/classes/pivot_pip.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.4.1/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    21975 2024-04-11 20:57:45.000000 quantminer-0.4.1/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 20:59:01.737942 quantminer-0.4.1/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 20:59:01.000000 quantminer-0.4.1/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-11 20:59:01.000000 quantminer-0.4.1/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-11 20:59:01.000000 quantminer-0.4.1/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-11 20:59:01.000000 quantminer-0.4.1/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-11 20:59:01.000000 quantminer-0.4.1/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-11 20:59:01.739253 quantminer-0.4.1/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-11 20:57:57.000000 quantminer-0.4.1/setup.py
```

### Comparing `quantminer-0.4.0/quantminer/classes/pivot_pip.py` & `quantminer-0.4.1/quantminer/classes/pivot_pip.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.4.0/quantminer/classes/seqkmeans.py` & `quantminer-0.4.1/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.4.0/quantminer/pipminer.py` & `quantminer-0.4.1/quantminer/pipminer.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         martins = self._compute_performance()
 
         print("Training Complete : ", martins)
 
         # Clean up stored data
         self._cleanup()
 
+        return martins
+
 
     def test(self, data: List[np.ndarray], plot_equity=False):
         # Preprocess Data
         data = self._preprocess_data(data, test_mode=True)
         _returns = np.diff(data, prepend=data[0])
 
         # Generate data windows
@@ -116,29 +118,33 @@
 
         # Implement holding period
         _signals = self.__apply_holding_period(_signals)
 
         # Get the returns, compute martin score
         _returns = _signals * _returns
 
-        print("Test Martin Score : ", self.__compute_martin(_returns))
+        martin_score = self.__compute_martin(_returns)
+
+        print("Test Martin Score : ", martin_score)
 
         if plot_equity:
             plt.plot(np.cumsum(_returns))
             plt.show()
 
         ser = pd.Series(_returns)
 
         print("Profit Factor : ", qt.stats.profit_factor(ser))
         print("Risk of Ruin : ", qt.stats.risk_of_ruin(ser))
         print("Sharpe : ", qt.stats.sharpe(ser))
         print("Avg Win : ", qt.stats.avg_win(ser))
         print("Avg Loss : ", qt.stats.avg_loss(ser))
         print("Avg Return : ", qt.stats.avg_return(ser))
 
+        return martin_score
+
 
     def transform(self, data:Union[List, np.ndarray]):
         """
         Generate labels for a full dataset.
         """
         # Preprocess Data
         data = self._preprocess_data(data, test_mode=True)
@@ -568,14 +574,16 @@
                 new_signals[start_index:end_index] = signal
 
         return new_signals
 
 
     def __compute_martin(self, rets: np.array):
     
+        return qt.stats.ulcer_performance_index(pd.Series(rets))
+    
         rsum = np.sum(rets)
         short = False
         if rsum < 0.0:
             rets *= -1
             rsum *= -1
             short = True
```

### Comparing `quantminer-0.4.0/setup.py` & `quantminer-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='quantminer',
-    version='0.4.0', 
+    version='0.4.1', 
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=[  # List any dependencies here
         "kneed",
         "quantstats",
```

