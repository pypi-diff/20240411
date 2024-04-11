# Comparing `tmp/startlit-0.0.2.tar.gz` & `tmp/startlit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "startlit-0.0.2.tar", max compression
+gzip compressed data, was "startlit-0.0.3.tar", max compression
```

## Comparing `startlit-0.0.2.tar` & `startlit-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-08 11:02:08.344472 startlit-0.0.2/LICENSE
--rw-r--r--   0        0        0     2716 2024-04-08 11:02:08.344472 startlit-0.0.2/README.md
--rw-r--r--   0        0        0      520 2024-04-08 11:02:08.344472 startlit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-08 11:02:08.344472 startlit-0.0.2/src/startlit/__init__.py
--rw-r--r--   0        0        0     2903 2024-04-08 11:02:08.344472 startlit-0.0.2/src/startlit/start.py
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 startlit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 11:57:07.782928 startlit-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3441 2024-04-11 11:57:07.782928 startlit-0.0.3/README.md
+-rw-r--r--   0        0        0      520 2024-04-11 11:57:07.782928 startlit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      137 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/kill.py
+-rw-r--r--   0        0        0     2323 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/list.py
+-rw-r--r--   0        0        0     2903 2024-04-11 11:57:07.782928 startlit-0.0.3/src/startlit/start.py
+-rw-r--r--   0        0        0     4090 1970-01-01 00:00:00.000000 startlit-0.0.3/PKG-INFO
```

### Comparing `startlit-0.0.2/LICENSE` & `startlit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `startlit-0.0.2/README.md` & `startlit-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # StartLit ⭐
+![PyPI - Version](https://img.shields.io/pypi/v/startlit) ![GitHub repo size](https://img.shields.io/github/repo-size/ineelhere/startlit) ![GitHub License](https://img.shields.io/github/license/ineelhere/startlit) ![example workflow](https://github.com/ineelhere/startlit/actions/workflows/python-publish.yml/badge.svg) 
 
 **Welcome to StartLit!**
 
 StartLit is your gateway to building Streamlit apps with ease. It brings a simple, streamlined way to start your Streamlit projects. Here's what's included in the latest release:
 
 #### Features:
 - **Package Installation**: Now you can easily install StartLit from PYPI using `pip install startlit`.
 - **Simple Usage**: Import the package and run `hello()` to receive a friendly welcome message.
 - **Basic help**: Use the `help()` function to get started with more support
 -  **Starter App**: Use the `starter()` function to download a very simple starter app template, including an `app.py` file and a `requirements.txt` file.
 -  **Multipage App**: Use the `multipage()` function to download an app template for building multipage Streamlit apps. The files/folders will be available in your working directory.
 -  **Fragments App**: Use the `fragments()` function to download an app that allows you to run independent components in the streamlit app.
-
-
+-  **List active streamlit apps** - Use the `list_streamlit_apps()` function to get a list of currently running
+-  **Kill active streamlit apps** - Use the `kill_streamlit_apps(app_id)` function to kill desired running streamlit apps. `app_id` is the app ID you get from the `list_streamlit_apps()` function.
 
 ### Install the package from PYPI
 
 ```python
 pip install startlit
 ```
 ### Import the package
@@ -82,14 +83,20 @@
 
 # Download a multipage app template
 multipage()
 
 # Download a fragment app template
 fragments()
 
+# List all active apps
+list_streamlit_apps()
+
+# Kill a specific app
+kill_streamlit_apps(app_id)
+
 
 ```
 ___
 
 ### Feedback and Contribution:
 Excited to hear your feedback and suggestions for improvements. 
 Feel free to open issues or submit pull requests.
```

### Comparing `startlit-0.0.2/pyproject.toml` & `startlit-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "startlit"
-version = "0.0.2"
+version = "0.0.3"
 description = "Get started with a streamlit app template code in style"
 authors = ["Indraneel Chakraborty"]
 readme = "README.md"
 homepage = "https://github.com/ineelhere/startlit"
 license = "Apache License - Version 2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `startlit-0.0.2/src/startlit/start.py` & `startlit-0.0.3/src/startlit/start.py`

 * *Files identical despite different names*

### Comparing `startlit-0.0.2/PKG-INFO` & `startlit-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: startlit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get started with a streamlit app template code in style
 Home-page: https://github.com/ineelhere/startlit
 License: Apache License - Version 2.0
 Author: Indraneel Chakraborty
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,28 +12,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # StartLit ⭐
+![PyPI - Version](https://img.shields.io/pypi/v/startlit) ![GitHub repo size](https://img.shields.io/github/repo-size/ineelhere/startlit) ![GitHub License](https://img.shields.io/github/license/ineelhere/startlit) ![example workflow](https://github.com/ineelhere/startlit/actions/workflows/python-publish.yml/badge.svg) 
 
 **Welcome to StartLit!**
 
 StartLit is your gateway to building Streamlit apps with ease. It brings a simple, streamlined way to start your Streamlit projects. Here's what's included in the latest release:
 
 #### Features:
 - **Package Installation**: Now you can easily install StartLit from PYPI using `pip install startlit`.
 - **Simple Usage**: Import the package and run `hello()` to receive a friendly welcome message.
 - **Basic help**: Use the `help()` function to get started with more support
 -  **Starter App**: Use the `starter()` function to download a very simple starter app template, including an `app.py` file and a `requirements.txt` file.
 -  **Multipage App**: Use the `multipage()` function to download an app template for building multipage Streamlit apps. The files/folders will be available in your working directory.
 -  **Fragments App**: Use the `fragments()` function to download an app that allows you to run independent components in the streamlit app.
-
-
+-  **List active streamlit apps** - Use the `list_streamlit_apps()` function to get a list of currently running
+-  **Kill active streamlit apps** - Use the `kill_streamlit_apps(app_id)` function to kill desired running streamlit apps. `app_id` is the app ID you get from the `list_streamlit_apps()` function.
 
 ### Install the package from PYPI
 
 ```python
 pip install startlit
 ```
 ### Import the package
@@ -99,14 +100,20 @@
 
 # Download a multipage app template
 multipage()
 
 # Download a fragment app template
 fragments()
 
+# List all active apps
+list_streamlit_apps()
+
+# Kill a specific app
+kill_streamlit_apps(app_id)
+
 
 ```
 ___
 
 ### Feedback and Contribution:
 Excited to hear your feedback and suggestions for improvements. 
 Feel free to open issues or submit pull requests.
```

