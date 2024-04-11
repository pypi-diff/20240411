# Comparing `tmp/deepecho-0.6.0.tar.gz` & `tmp/deepecho-0.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepecho-0.6.0.tar", last modified: Thu Apr 11 02:18:26 2024, max compression
+gzip compressed data, was "deepecho-0.6.0.dev0.tar", last modified: Tue Apr  9 21:49:21 2024, max compression
```

## Comparing `deepecho-0.6.0.tar` & `deepecho-0.6.0.dev0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-11 02:18:26.575482 deepecho-0.6.0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.6.0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10627 2024-04-11 02:18:26.575213 deepecho-0.6.0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7887 2024-04-11 02:18:22.000000 deepecho-0.6.0/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-11 02:18:26.571854 deepecho-0.6.0/deepecho/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      382 2024-04-11 02:18:22.000000 deepecho-0.6.0/deepecho/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-11 02:18:26.572739 deepecho-0.6.0/deepecho/data/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.6.0/deepecho/data/demo.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2024-04-09 21:41:01.000000 deepecho-0.6.0/deepecho/demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-11 02:18:26.573406 deepecho-0.6.0/deepecho/models/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.6.0/deepecho/models/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10776 2024-04-11 02:18:22.000000 deepecho-0.6.0/deepecho/models/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21539 2024-04-11 02:18:22.000000 deepecho-0.6.0/deepecho/models/basic_gan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    23504 2024-04-11 02:18:22.000000 deepecho-0.6.0/deepecho/models/par.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7142 2024-04-11 02:18:22.000000 deepecho-0.6.0/deepecho/sequences.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-11 02:18:26.573787 deepecho-0.6.0/deepecho.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10627 2024-04-11 02:18:26.000000 deepecho-0.6.0/deepecho.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      398 2024-04-11 02:18:26.000000 deepecho-0.6.0/deepecho.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-04-11 02:18:26.000000 deepecho-0.6.0/deepecho.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      746 2024-04-11 02:18:26.000000 deepecho-0.6.0/deepecho.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2024-04-11 02:18:26.000000 deepecho-0.6.0/deepecho.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4955 2024-04-11 02:18:22.000000 deepecho-0.6.0/pyproject.toml
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2024-04-11 02:18:26.575533 deepecho-0.6.0/setup.cfg
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-11 02:18:26.573573 deepecho-0.6.0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1305 2024-04-11 02:18:22.000000 deepecho-0.6.0/tests/test_tasks.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.534925 deepecho-0.6.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.6.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10632 2024-04-09 21:49:21.534575 deepecho-0.6.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7887 2024-02-12 22:55:24.000000 deepecho-0.6.0.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.530548 deepecho-0.6.0.dev0/deepecho/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      387 2024-04-09 21:47:08.000000 deepecho-0.6.0.dev0/deepecho/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.531345 deepecho-0.6.0.dev0/deepecho/data/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.6.0.dev0/deepecho/data/demo.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.532499 deepecho-0.6.0.dev0/deepecho/models/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.6.0.dev0/deepecho/models/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10776 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/models/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21539 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/models/basic_gan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    23504 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/models/par.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7142 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.532881 deepecho-0.6.0.dev0/deepecho.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10632 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      398 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      746 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4960 2024-04-09 21:48:53.000000 deepecho-0.6.0.dev0/pyproject.toml
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2024-04-09 21:49:21.534997 deepecho-0.6.0.dev0/setup.cfg
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.532677 deepecho-0.6.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1305 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/tests/test_tasks.py
```

### Comparing `deepecho-0.6.0/LICENSE` & `deepecho-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/PKG-INFO` & `deepecho-0.6.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepecho
-Version: 0.6.0
+Version: 0.6.0.dev0
 Summary: Create sequential synthetic data of mixed types using a GAN.
 Author-email: "DataCebo, Inc." <info@sdv.dev>
 License: BSL-1.1
 Project-URL: Source Code, https://github.com/sdv-dev/Deepecho/
 Project-URL: Issue Tracker, https://github.com/sdv-dev/Deepecho/issues
 Project-URL: Twitter, https://twitter.com/sdv_dev
 Project-URL: Chat, https://bit.ly/sdv-slack-invite
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: deepecho Version: 0.6.0 Summary: Create sequential
-synthetic data of mixed types using a GAN. Author-email: "DataCebo, Inc."
+Metadata-Version: 2.1 Name: deepecho Version: 0.6.0.dev0 Summary: Create
+sequential synthetic data of mixed types using a GAN. Author-email: "DataCebo,
+Inc."
 sdv.dev> License: BSL-1.1 Project-URL: Source Code, https://github.com/sdv-dev/
 Deepecho/ Project-URL: Issue Tracker, https://github.com/sdv-dev/Deepecho/
 issues Project-URL: Twitter, https://twitter.com/sdv_dev Project-URL: Chat,
 https://bit.ly/sdv-slack-invite Keywords: deepecho,DeepEcho Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `deepecho-0.6.0/README.md` & `deepecho-0.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/deepecho/data/demo.csv` & `deepecho-0.6.0.dev0/deepecho/data/demo.csv`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/deepecho/models/base.py` & `deepecho-0.6.0.dev0/deepecho/models/base.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/deepecho/models/basic_gan.py` & `deepecho-0.6.0.dev0/deepecho/models/basic_gan.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/deepecho/models/par.py` & `deepecho-0.6.0.dev0/deepecho/models/par.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/deepecho/sequences.py` & `deepecho-0.6.0.dev0/deepecho/sequences.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/deepecho.egg-info/PKG-INFO` & `deepecho-0.6.0.dev0/deepecho.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepecho
-Version: 0.6.0
+Version: 0.6.0.dev0
 Summary: Create sequential synthetic data of mixed types using a GAN.
 Author-email: "DataCebo, Inc." <info@sdv.dev>
 License: BSL-1.1
 Project-URL: Source Code, https://github.com/sdv-dev/Deepecho/
 Project-URL: Issue Tracker, https://github.com/sdv-dev/Deepecho/issues
 Project-URL: Twitter, https://twitter.com/sdv_dev
 Project-URL: Chat, https://bit.ly/sdv-slack-invite
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: deepecho Version: 0.6.0 Summary: Create sequential
-synthetic data of mixed types using a GAN. Author-email: "DataCebo, Inc."
+Metadata-Version: 2.1 Name: deepecho Version: 0.6.0.dev0 Summary: Create
+sequential synthetic data of mixed types using a GAN. Author-email: "DataCebo,
+Inc."
 sdv.dev> License: BSL-1.1 Project-URL: Source Code, https://github.com/sdv-dev/
 Deepecho/ Project-URL: Issue Tracker, https://github.com/sdv-dev/Deepecho/
 issues Project-URL: Twitter, https://twitter.com/sdv_dev Project-URL: Chat,
 https://bit.ly/sdv-slack-invite Keywords: deepecho,DeepEcho Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `deepecho-0.6.0/deepecho.egg-info/requires.txt` & `deepecho-0.6.0.dev0/deepecho.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepecho-0.6.0/pyproject.toml` & `deepecho-0.6.0.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 not_skip = ['__init__.py']
 use_parentheses = true
 
 [tool.pytest.ini_options]
 collect_ignore = ['pyproject.toml']
 
 [tool.bumpversion]
-current_version = "0.6.0"
+current_version = "0.6.0.dev0"
 parse = '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?'
 serialize = [
     '{major}.{minor}.{patch}.{release}{candidate}',
 	'{major}.{minor}.{patch}'
 ]
 search = '{current_version}'
 replace = '{new_version}'
```

### Comparing `deepecho-0.6.0/tests/test_tasks.py` & `deepecho-0.6.0.dev0/tests/test_tasks.py`

 * *Files identical despite different names*

