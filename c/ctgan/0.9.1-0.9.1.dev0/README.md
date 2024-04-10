# Comparing `tmp/ctgan-0.9.1.tar.gz` & `tmp/ctgan-0.9.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctgan-0.9.1.tar", last modified: Thu Mar 14 15:03:42 2024, max compression
+gzip compressed data, was "ctgan-0.9.1.dev0.tar", last modified: Thu Mar 14 11:59:58 2024, max compression
```

## Comparing `ctgan-0.9.1.tar` & `ctgan-0.9.1.dev0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 15:03:42.215076 ctgan-0.9.1/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2023-01-20 22:22:05.000000 ctgan-0.9.1/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11197 2024-03-14 15:03:42.214899 ctgan-0.9.1/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7294 2023-10-05 21:41:39.000000 ctgan-0.9.1/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 15:03:42.209947 ctgan-0.9.1/ctgan/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      314 2024-03-14 15:03:39.000000 ctgan-0.9.1/ctgan/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4415 2022-10-07 17:29:33.000000 ctgan-0.9.1/ctgan/__main__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2457 2022-08-17 21:26:32.000000 ctgan-0.9.1/ctgan/data.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6169 2024-03-14 15:03:38.000000 ctgan-0.9.1/ctgan/data_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10533 2023-10-05 21:41:39.000000 ctgan-0.9.1/ctgan/data_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2023-05-09 17:51:59.000000 ctgan-0.9.1/ctgan/demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 15:03:42.211674 ctgan-0.9.1/ctgan/synthesizers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      258 2022-10-07 17:29:33.000000 ctgan-0.9.1/ctgan/synthesizers/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5287 2023-02-25 01:28:14.000000 ctgan-0.9.1/ctgan/synthesizers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19815 2024-03-14 15:03:38.000000 ctgan-0.9.1/ctgan/synthesizers/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8167 2024-03-14 15:03:38.000000 ctgan-0.9.1/ctgan/synthesizers/tvae.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 15:03:42.212122 ctgan-0.9.1/ctgan.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11197 2024-03-14 15:03:42.000000 ctgan-0.9.1/ctgan.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2024-03-14 15:03:42.000000 ctgan-0.9.1/ctgan.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-03-14 15:03:42.000000 ctgan-0.9.1/ctgan.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2024-03-14 15:03:42.000000 ctgan-0.9.1/ctgan.egg-info/entry_points.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1195 2024-03-14 15:03:42.000000 ctgan-0.9.1/ctgan.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2024-03-14 15:03:42.000000 ctgan-0.9.1/ctgan.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2024-03-14 15:03:39.000000 ctgan-0.9.1/pyproject.toml
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      482 2024-03-14 15:03:42.215336 ctgan-0.9.1/setup.cfg
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 15:03:42.211887 ctgan-0.9.1/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1332 2024-03-14 15:03:38.000000 ctgan-0.9.1/tests/test_tasks.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 11:59:58.817715 ctgan-0.9.1.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4816 2023-01-20 22:22:05.000000 ctgan-0.9.1.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11202 2024-03-14 11:59:58.817583 ctgan-0.9.1.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7294 2023-10-05 21:41:39.000000 ctgan-0.9.1.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 11:59:58.812263 ctgan-0.9.1.dev0/ctgan/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      319 2024-02-29 23:50:05.000000 ctgan-0.9.1.dev0/ctgan/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4415 2022-10-07 17:29:33.000000 ctgan-0.9.1.dev0/ctgan/__main__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2457 2022-08-17 21:26:32.000000 ctgan-0.9.1.dev0/ctgan/data.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6169 2024-02-12 22:54:12.000000 ctgan-0.9.1.dev0/ctgan/data_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10533 2023-10-05 21:41:39.000000 ctgan-0.9.1.dev0/ctgan/data_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2023-05-09 17:51:59.000000 ctgan-0.9.1.dev0/ctgan/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 11:59:58.814372 ctgan-0.9.1.dev0/ctgan/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      258 2022-10-07 17:29:33.000000 ctgan-0.9.1.dev0/ctgan/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5287 2023-02-25 01:28:14.000000 ctgan-0.9.1.dev0/ctgan/synthesizers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19815 2024-03-14 00:57:07.000000 ctgan-0.9.1.dev0/ctgan/synthesizers/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8167 2023-11-21 22:24:26.000000 ctgan-0.9.1.dev0/ctgan/synthesizers/tvae.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 11:59:58.814913 ctgan-0.9.1.dev0/ctgan.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11202 2024-03-14 11:59:58.000000 ctgan-0.9.1.dev0/ctgan.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2024-03-14 11:59:58.000000 ctgan-0.9.1.dev0/ctgan.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-03-14 11:59:58.000000 ctgan-0.9.1.dev0/ctgan.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2024-03-14 11:59:58.000000 ctgan-0.9.1.dev0/ctgan.egg-info/entry_points.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1195 2024-03-14 11:59:58.000000 ctgan-0.9.1.dev0/ctgan.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2024-03-14 11:59:58.000000 ctgan-0.9.1.dev0/ctgan.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4821 2024-03-14 11:17:57.000000 ctgan-0.9.1.dev0/pyproject.toml
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      482 2024-03-14 11:59:58.817937 ctgan-0.9.1.dev0/setup.cfg
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-14 11:59:58.814654 ctgan-0.9.1.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1332 2024-03-14 00:57:07.000000 ctgan-0.9.1.dev0/tests/test_tasks.py
```

### Comparing `ctgan-0.9.1/LICENSE` & `ctgan-0.9.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/PKG-INFO` & `ctgan-0.9.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctgan
-Version: 0.9.1
+Version: 0.9.1.dev0
 Summary: Create tabular synthetic data using a conditional GAN
 Author-email: "DataCebo, Inc." <info@sdv.dev>
 License: BSL-1.1
 Project-URL: Source Code, https://github.com/sdv-dev/CTGAN/
 Project-URL: Issue Tracker, https://github.com/sdv-dev/CTGAN/issues
 Project-URL: Changes, https://github.com/sdv-dev/CTGAN/blob/main/HISTORY.md
 Project-URL: Twitter, https://twitter.com/sdv_dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctgan Version: 0.9.1 Summary: Create tabular
+Metadata-Version: 2.1 Name: ctgan Version: 0.9.1.dev0 Summary: Create tabular
 synthetic data using a conditional GAN Author-email: "DataCebo, Inc."
 sdv.dev> License: BSL-1.1 Project-URL: Source Code, https://github.com/sdv-dev/
 CTGAN/ Project-URL: Issue Tracker, https://github.com/sdv-dev/CTGAN/issues
 Project-URL: Changes, https://github.com/sdv-dev/CTGAN/blob/main/HISTORY.md
 Project-URL: Twitter, https://twitter.com/sdv_dev Project-URL: Chat, https://
 bit.ly/sdv-slack-invite Keywords: ctgan,CTGAN Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: License
```

### Comparing `ctgan-0.9.1/README.md` & `ctgan-0.9.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/__main__.py` & `ctgan-0.9.1.dev0/ctgan/__main__.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/data.py` & `ctgan-0.9.1.dev0/ctgan/data.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/data_sampler.py` & `ctgan-0.9.1.dev0/ctgan/data_sampler.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/data_transformer.py` & `ctgan-0.9.1.dev0/ctgan/data_transformer.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/synthesizers/base.py` & `ctgan-0.9.1.dev0/ctgan/synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/synthesizers/ctgan.py` & `ctgan-0.9.1.dev0/ctgan/synthesizers/ctgan.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan/synthesizers/tvae.py` & `ctgan-0.9.1.dev0/ctgan/synthesizers/tvae.py`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/ctgan.egg-info/PKG-INFO` & `ctgan-0.9.1.dev0/ctgan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctgan
-Version: 0.9.1
+Version: 0.9.1.dev0
 Summary: Create tabular synthetic data using a conditional GAN
 Author-email: "DataCebo, Inc." <info@sdv.dev>
 License: BSL-1.1
 Project-URL: Source Code, https://github.com/sdv-dev/CTGAN/
 Project-URL: Issue Tracker, https://github.com/sdv-dev/CTGAN/issues
 Project-URL: Changes, https://github.com/sdv-dev/CTGAN/blob/main/HISTORY.md
 Project-URL: Twitter, https://twitter.com/sdv_dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ctgan Version: 0.9.1 Summary: Create tabular
+Metadata-Version: 2.1 Name: ctgan Version: 0.9.1.dev0 Summary: Create tabular
 synthetic data using a conditional GAN Author-email: "DataCebo, Inc."
 sdv.dev> License: BSL-1.1 Project-URL: Source Code, https://github.com/sdv-dev/
 CTGAN/ Project-URL: Issue Tracker, https://github.com/sdv-dev/CTGAN/issues
 Project-URL: Changes, https://github.com/sdv-dev/CTGAN/blob/main/HISTORY.md
 Project-URL: Twitter, https://twitter.com/sdv_dev Project-URL: Chat, https://
 bit.ly/sdv-slack-invite Keywords: ctgan,CTGAN Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: License
```

### Comparing `ctgan-0.9.1/ctgan.egg-info/requires.txt` & `ctgan-0.9.1.dev0/ctgan.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ctgan-0.9.1/pyproject.toml` & `ctgan-0.9.1.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 convention = 'google'
 add-ignore = ['D107', 'D407', 'D417']
 
 [tool.pytest.ini_options]
 collect_ignore = ['pyproject.toml']
 
 [tool.bumpversion]
-current_version = "0.9.1"
+current_version = '0.9.1.dev0'
 parse = '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?'
 serialize = [
     '{major}.{minor}.{patch}.{release}{candidate}',
 	'{major}.{minor}.{patch}'
 ]
 search = '{current_version}'
 replace = '{new_version}'
```

### Comparing `ctgan-0.9.1/tests/test_tasks.py` & `ctgan-0.9.1.dev0/tests/test_tasks.py`

 * *Files identical despite different names*

