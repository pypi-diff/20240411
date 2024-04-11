# Comparing `tmp/delay_finder-0.1.0.tar.gz` & `tmp/delay_finder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delay_finder-0.1.0.tar", max compression
+gzip compressed data, was "delay_finder-1.0.0.tar", max compression
```

## Comparing `delay_finder-0.1.0.tar` & `delay_finder-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2712 2024-04-09 17:54:26.516044 delay_finder-0.1.0/LICENSE
--rw-r--r--   0        0        0      690 2024-04-09 04:30:17.840852 delay_finder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2504 2024-04-09 17:56:39.983653 delay_finder-0.1.0/README.md
--rw-r--r--   0        0        0      116 2024-04-05 16:27:02.389196 delay_finder-0.1.0/src/delay_finder/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-09 04:38:58.087369 delay_finder-0.1.0/src/delay_finder/data_split.py
--rw-r--r--   0        0        0     1321 2024-04-09 04:55:57.030140 delay_finder-0.1.0/src/delay_finder/filter_columns.py
--rw-r--r--   0        0        0     1104 2024-04-05 17:25:55.340344 delay_finder-0.1.0/src/delay_finder/load_and_save.py
--rw-r--r--   0        0        0     2613 2024-04-04 06:07:48.179090 delay_finder-0.1.0/src/delay_finder/make_histogram.py
--rw-r--r--   0        0        0      828 2024-04-05 16:35:22.773846 delay_finder-0.1.0/src/delay_finder/read.py
--rw-r--r--   0        0        0     2523 2024-04-04 06:07:48.179831 delay_finder-0.1.0/src/delay_finder/replace_value.py
--rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 delay_finder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2724 2024-04-11 00:39:39.425764 delay_finder-1.0.0/LICENSE
+-rw-r--r--   0        0        0      690 2024-04-11 15:54:26.651112 delay_finder-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2883 2024-04-11 00:39:39.427843 delay_finder-1.0.0/README.md
+-rw-r--r--   0        0        0      116 2024-04-05 16:27:02.389196 delay_finder-1.0.0/src/delay_finder/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-09 04:38:58.087369 delay_finder-1.0.0/src/delay_finder/data_split.py
+-rw-r--r--   0        0        0     1321 2024-04-09 04:55:57.030140 delay_finder-1.0.0/src/delay_finder/filter_columns.py
+-rw-r--r--   0        0        0      647 2024-04-11 01:46:35.779000 delay_finder-1.0.0/src/delay_finder/load_and_save.py
+-rw-r--r--   0        0        0     2613 2024-04-04 06:07:48.179090 delay_finder-1.0.0/src/delay_finder/make_histogram.py
+-rw-r--r--   0        0        0      828 2024-04-05 16:35:22.773846 delay_finder-1.0.0/src/delay_finder/read.py
+-rw-r--r--   0        0        0     2523 2024-04-04 06:07:48.179831 delay_finder-1.0.0/src/delay_finder/replace_value.py
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 delay_finder-1.0.0/PKG-INFO
```

### Comparing `delay_finder-0.1.0/LICENSE` & `delay_finder-1.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ## Creative Commons 4.0 License
 For the usage examples file in this repository.
 
 Example Usages © 2024, Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta is licensed under CC BY 4.0
 
 ## MIT License
-GitHub Actions docs workflow template taken from Copyright (c) 2024, Daniel Chen.
+GitHub Actions docs and ci-cd workflow template taken from Copyright (c) 2024, Daniel Chen.
 
 For the portions of the project that are derived from [pycounts-dan]](https://github.com/chendaniely/pycounts-dan).
 Specifically the GitHub Actions docs workflow.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -44,8 +44,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `delay_finder-0.1.0/pyproject.toml` & `delay_finder-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delay_finder"
-version = "0.1.0"
+version = "1.0.0"
 description = "Analyze and predict airline delays!"
 authors = ["Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `delay_finder-0.1.0/README.md` & `delay_finder-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # delay_finder
 
+[![codecov](https://codecov.io/gh/DSCI-310-2024/delay_finder/graph/badge.svg?token=uO4Pe7Dg7w)](https://codecov.io/gh/DSCI-310-2024/delay_finder)
+
+Authors: Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta
+
 `delay_finder` is DSCI 310 Group 17's Python package for analyzing, predicting, and visualizing data related to airline delay.
 
 It has functions to read CSV files into a dataframe, filter dataframe columns, replace a value in a dataframe, split data into 80/20 testing and training sets, save a model as a pickle object and file, and make a histogram visualizing a numeric feature.
 
 This package builds off of [pandas](https://github.com/pandas-dev/pandas), [sci-kit learn](https://github.com/scikit-learn/scikit-learn), [altair](https://github.com/altair-viz/altair) packages and Python's [pickle](https://github.com/python/cpython/blob/main/Lib/pickle.py) library and makes workflow more efficient in analyzing, predicting, and visualizing data related to airline delay.
 
 ## Installation
@@ -42,8 +46,9 @@
 
 `delay_finder` was created by Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta. The code is licensed under the terms of the MIT license.  
 The usage examples file in licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0).
 For more information, please see the license file.
 
 ## Credits
 
-`delay_finder` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+`delay_finder` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).  
+The documentation and ci-cd workflow was adapted from Daniel Chen's [pycounts-dan](https://github.com/chendaniely/pycounts-dan) repository.
```

### Comparing `delay_finder-0.1.0/src/delay_finder/data_split.py` & `delay_finder-1.0.0/src/delay_finder/data_split.py`

 * *Files identical despite different names*

### Comparing `delay_finder-0.1.0/src/delay_finder/filter_columns.py` & `delay_finder-1.0.0/src/delay_finder/filter_columns.py`

 * *Files identical despite different names*

### Comparing `delay_finder-0.1.0/src/delay_finder/load_and_save.py` & `delay_finder-1.0.0/src/delay_finder/load_and_save.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,10 @@
 import pandas as pd
 import pickle
 
-def load_data(file_path):
-    """Load data from a CSV file.
-
-    Parameters:
-    ----------
-    - file_path (str): The path to the CSV file containing the data.
-
-    Returns:
-    -------
-    pandas.DataFrame: The loaded data as a DataFrame.
-
-    Examples:
-    --------
-    >>> import pandas as pd
-    >>> df = load_data('filename.csv') # Replace 'filename.csv' with your desired dataset filename
-    """
-    return pd.read_csv(file_path)
-
 def save_model(model, file_path):
     """Save a trained model to a file using pickle.
 
     Parameters:
     ----------
     - model: The trained model object to be saved.
     - file_path (str): The path to save the model file.
```

### Comparing `delay_finder-0.1.0/src/delay_finder/make_histogram.py` & `delay_finder-1.0.0/src/delay_finder/make_histogram.py`

 * *Files identical despite different names*

### Comparing `delay_finder-0.1.0/src/delay_finder/read.py` & `delay_finder-1.0.0/src/delay_finder/read.py`

 * *Files identical despite different names*

### Comparing `delay_finder-0.1.0/src/delay_finder/replace_value.py` & `delay_finder-1.0.0/src/delay_finder/replace_value.py`

 * *Files identical despite different names*

### Comparing `delay_finder-0.1.0/PKG-INFO` & `delay_finder-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delay_finder
-Version: 0.1.0
+Version: 1.0.0
 Summary: Analyze and predict airline delays!
 License: MIT
 Author: Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +14,18 @@
 Requires-Dist: altair (>=5.2.0)
 Requires-Dist: pandas (>=2.2.0)
 Requires-Dist: scikit-learn (>=1.4.0)
 Description-Content-Type: text/markdown
 
 # delay_finder
 
+[![codecov](https://codecov.io/gh/DSCI-310-2024/delay_finder/graph/badge.svg?token=uO4Pe7Dg7w)](https://codecov.io/gh/DSCI-310-2024/delay_finder)
+
+Authors: Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta
+
 `delay_finder` is DSCI 310 Group 17's Python package for analyzing, predicting, and visualizing data related to airline delay.
 
 It has functions to read CSV files into a dataframe, filter dataframe columns, replace a value in a dataframe, split data into 80/20 testing and training sets, save a model as a pickle object and file, and make a histogram visualizing a numeric feature.
 
 This package builds off of [pandas](https://github.com/pandas-dev/pandas), [sci-kit learn](https://github.com/scikit-learn/scikit-learn), [altair](https://github.com/altair-viz/altair) packages and Python's [pickle](https://github.com/python/cpython/blob/main/Lib/pickle.py) library and makes workflow more efficient in analyzing, predicting, and visualizing data related to airline delay.
 
 ## Installation
@@ -60,9 +64,10 @@
 
 `delay_finder` was created by Siddharth Balodi, Charles Benkard, Mikel Ibarra Gallardo, and Stephanie Ta. The code is licensed under the terms of the MIT license.  
 The usage examples file in licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0).
 For more information, please see the license file.
 
 ## Credits
 
-`delay_finder` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+`delay_finder` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).  
+The documentation and ci-cd workflow was adapted from Daniel Chen's [pycounts-dan](https://github.com/chendaniely/pycounts-dan) repository.
```

