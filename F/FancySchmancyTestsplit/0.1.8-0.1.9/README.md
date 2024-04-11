# Comparing `tmp/FancySchmancyTestsplit-0.1.8.tar.gz` & `tmp/FancySchmancyTestsplit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FancySchmancyTestsplit-0.1.8.tar", last modified: Wed Apr 10 09:13:29 2024, max compression
+gzip compressed data, was "FancySchmancyTestsplit-0.1.9.tar", last modified: Thu Apr 11 07:31:22 2024, max compression
```

## Comparing `FancySchmancyTestsplit-0.1.8.tar` & `FancySchmancyTestsplit-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:13:29.608643 FancySchmancyTestsplit-0.1.8/
--rw-rw-rw-   0        0        0     3041 2024-04-10 09:13:29.606642 FancySchmancyTestsplit-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2442 2024-04-10 08:39:22.000000 FancySchmancyTestsplit-0.1.8/README.md
--rw-rw-rw-   0        0        0     1993 2024-04-10 09:11:03.000000 FancySchmancyTestsplit-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 09:13:29.608643 FancySchmancyTestsplit-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 09:13:29.572645 FancySchmancyTestsplit-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 09:13:29.587643 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit/
--rw-rw-rw-   0        0        0      126 2024-04-10 09:12:30.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit/__init__.py
--rw-rw-rw-   0        0        0     4523 2024-04-10 09:13:18.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit/fst.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:13:29.605642 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/
--rw-rw-rw-   0        0        0     3041 2024-04-10 09:13:29.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-10 09:13:29.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:13:29.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-10 09:13:29.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-10 09:13:29.000000 FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 09:13:29.604642 FancySchmancyTestsplit-0.1.8/tests/
--rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.8/tests/test_fancy_schmancy_testsplit.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:31:22.474258 FancySchmancyTestsplit-0.1.9/
+-rw-rw-rw-   0        0        0     3040 2024-04-11 07:31:22.474258 FancySchmancyTestsplit-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2442 2024-04-10 08:39:22.000000 FancySchmancyTestsplit-0.1.9/README.md
+-rw-rw-rw-   0        0        0     1992 2024-04-11 07:30:45.000000 FancySchmancyTestsplit-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 07:31:22.475258 FancySchmancyTestsplit-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 07:31:22.408694 FancySchmancyTestsplit-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 07:31:22.441965 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit/
+-rw-rw-rw-   0        0        0      126 2024-04-10 09:12:30.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-11 07:30:25.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit/fst.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:31:22.473259 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/
+-rw-rw-rw-   0        0        0     3040 2024-04-11 07:31:22.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-11 07:31:22.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 07:31:22.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-11 07:31:22.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-11 07:31:22.000000 FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 07:31:22.471258 FancySchmancyTestsplit-0.1.9/tests/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 21:23:41.000000 FancySchmancyTestsplit-0.1.9/tests/test_fancy_schmancy_testsplit.py
```

### Comparing `FancySchmancyTestsplit-0.1.8/PKG-INFO` & `FancySchmancyTestsplit-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.8
+Version: 0.1.9
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.25.2
 Requires-Dist: pandas==2.1.3
 Requires-Dist: scikit-learn==1.3.2
 
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
```

### Comparing `FancySchmancyTestsplit-0.1.8/README.md` & `FancySchmancyTestsplit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `FancySchmancyTestsplit-0.1.8/pyproject.toml` & `FancySchmancyTestsplit-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 # somewhat static info -----------------------------------------------------------------
 name = "FancySchmancyTestsplit"
 description = "a more in-depth testsplit splitting intercategorical"
 keywords = ["test split", "testsplit", "train test split"]
 
 # variable info ------------------------------------------------------------------------
-version = "0.1.8"
-requires-python = ">=3.11"
+version = "0.1.9"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy==1.25.2",
```

### Comparing `FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit/fst.py` & `FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit/fst.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,12 +129,13 @@
             X_tr, X_te, y_tr, y_te = train_test_split(X, y, test_size = test_split, random_state = seed)
 
             X_train = concat([X_train, X_tr])
             X_test = concat([X_test, X_te])
             y_train = concat([y_train, y_tr])
             y_test = concat([y_test, y_te])
             pass
-        
+
+
         return (X_train, X_test, y_train, y_test)
```

### Comparing `FancySchmancyTestsplit-0.1.8/src/FancySchmancyTestsplit.egg-info/PKG-INFO` & `FancySchmancyTestsplit-0.1.9/src/FancySchmancyTestsplit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: FancySchmancyTestsplit
-Version: 0.1.8
+Version: 0.1.9
 Summary: a more in-depth testsplit splitting intercategorical
 Author-email: Kevin Pohl <pohl.kevin@gmail.com>
 Maintainer-email: Kevin Pohl <pohl.kevin@gmail.com>
 License: MIT
 Keywords: test split,testsplit,train test split
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.25.2
 Requires-Dist: pandas==2.1.3
 Requires-Dist: scikit-learn==1.3.2
 
 # fancy schmancy testsplit
 #### it's like a testsplit, but fancy and also schmancy
```

### Comparing `FancySchmancyTestsplit-0.1.8/tests/test_fancy_schmancy_testsplit.py` & `FancySchmancyTestsplit-0.1.9/tests/test_fancy_schmancy_testsplit.py`

 * *Files identical despite different names*

