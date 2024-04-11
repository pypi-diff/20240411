# Comparing `tmp/metamorph-0.0.8.tar.gz` & `tmp/metamorph-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamorph-0.0.8.tar", last modified: Sat Jun  4 23:01:38 2022, max compression
+gzip compressed data, was "metamorph-0.0.9.tar", last modified: Sun Jul 31 11:33:45 2022, max compression
```

## Comparing `metamorph-0.0.8.tar` & `metamorph-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-04 23:01:38.873148 metamorph-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-06-04 23:01:30.000000 metamorph-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2417 2022-06-04 23:01:38.873148 metamorph-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1973 2022-06-04 23:01:30.000000 metamorph-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-04 23:01:38.873148 metamorph-0.0.8/metamorph/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-04 23:01:30.000000 metamorph-0.0.8/metamorph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4363 2022-06-04 23:01:30.000000 metamorph-0.0.8/metamorph/config.py
--rw-r--r--   0 root         (0) root         (0)     5107 2022-06-04 23:01:30.000000 metamorph-0.0.8/metamorph/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-04 23:01:38.873148 metamorph-0.0.8/metamorph.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2417 2022-06-04 23:01:38.000000 metamorph-0.0.8/metamorph.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      286 2022-06-04 23:01:38.000000 metamorph-0.0.8/metamorph.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-04 23:01:38.000000 metamorph-0.0.8/metamorph.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2022-06-04 23:01:38.000000 metamorph-0.0.8/metamorph.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-06-04 23:01:38.000000 metamorph-0.0.8/metamorph.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-06-04 23:01:38.000000 metamorph-0.0.8/metamorph.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-04 23:01:38.873148 metamorph-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1236 2022-06-04 23:01:30.000000 metamorph-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-31 11:33:45.809333 metamorph-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    35149 2022-07-31 11:33:35.000000 metamorph-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2782 2022-07-31 11:33:45.809333 metamorph-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2338 2022-07-31 11:33:35.000000 metamorph-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-31 11:33:45.809333 metamorph-0.0.9/metamorph/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-31 11:33:35.000000 metamorph-0.0.9/metamorph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4363 2022-07-31 11:33:35.000000 metamorph-0.0.9/metamorph/config.py
+-rw-r--r--   0 root         (0) root         (0)     5107 2022-07-31 11:33:35.000000 metamorph-0.0.9/metamorph/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-31 11:33:45.809333 metamorph-0.0.9/metamorph.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2782 2022-07-31 11:33:45.000000 metamorph-0.0.9/metamorph.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      286 2022-07-31 11:33:45.000000 metamorph-0.0.9/metamorph.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-31 11:33:45.000000 metamorph-0.0.9/metamorph.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2022-07-31 11:33:45.000000 metamorph-0.0.9/metamorph.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2022-07-31 11:33:45.000000 metamorph-0.0.9/metamorph.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-07-31 11:33:45.000000 metamorph-0.0.9/metamorph.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-07-31 11:33:45.809333 metamorph-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-07-31 11:33:35.000000 metamorph-0.0.9/setup.py
```

### Comparing `metamorph-0.0.8/LICENSE` & `metamorph-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metamorph-0.0.8/PKG-INFO` & `metamorph-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamorph
-Version: 0.0.8
+Version: 0.0.9
 Summary: auto rewrite text
 Home-page: https://github.com/APN-Pucky/metamorph
 Author: APN
 Author-email: APN-Pucky@no-reply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,18 @@
 
 Doc: `metamorph --help`
 
 (Work-in-progress: Doc: https://apn-pucky.github.io/metamorph/index.html )
 
 [![PyPI version][pypi image]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/metamorph.svg) 
 
-| [Stable][doc release]        | [Dev][doc test]           |
+| [Stable][doc release]        | [Unstable][doc test]           |
 | ------------- |:-------------:|
 | [![workflow][a s image]][a s link]      | [![test][a t image]][a t link]     |
+| -     |[![Codacy Badge][codacy quality image]][codacy quality link] | 
 
 ## Versions
 
 ### Stable
 
 ```sh
 pip install metamorph [--user] [--upgrade]
@@ -89,13 +90,14 @@
 
 [doc release]: https://apn-pucky.github.io/metamorph/index.html
 [doc test]: https://apn-pucky.github.io/metamorph/test/index.html
 
 [pypi image]: https://badge.fury.io/py/metamorph.svg
 [pypi link]: https://pypi.org/project/metamorph/
 
-[a s image]: https://github.com/APN-Pucky/metamorph/actions/workflows/release.yml/badge.svg
-[a s link]: https://github.com/APN-Pucky/metamorph/actions/workflows/release.yml
+[a s image]: https://github.com/APN-Pucky/metamorph/actions/workflows/stable.yml/badge.svg
+[a s link]: https://github.com/APN-Pucky/metamorph/actions/workflows/stable.yml
 [a t link]: https://github.com/APN-Pucky/metamorph/actions/workflows/unstable.yml
 [a t image]: https://github.com/APN-Pucky/metamorph/actions/workflows/unstable.yml/badge.svg
 
-
+[codacy quality image]: https://app.codacy.com/project/badge/Grade/1acfcad112734b1ca875518cf1eeda34
+[codacy quality link]: https://www.codacy.com/gh/APN-Pucky/metamorph/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/metamorph&amp;utm_campaign=Badge_Grade
```

### Comparing `metamorph-0.0.8/README.md` & `metamorph-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 Doc: `metamorph --help`
 
 (Work-in-progress: Doc: https://apn-pucky.github.io/metamorph/index.html )
 
 [![PyPI version][pypi image]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/metamorph.svg) 
 
-| [Stable][doc release]        | [Dev][doc test]           |
+| [Stable][doc release]        | [Unstable][doc test]           |
 | ------------- |:-------------:|
 | [![workflow][a s image]][a s link]      | [![test][a t image]][a t link]     |
+| -     |[![Codacy Badge][codacy quality image]][codacy quality link] | 
 
 ## Versions
 
 ### Stable
 
 ```sh
 pip install metamorph [--user] [--upgrade]
@@ -75,13 +76,14 @@
 
 [doc release]: https://apn-pucky.github.io/metamorph/index.html
 [doc test]: https://apn-pucky.github.io/metamorph/test/index.html
 
 [pypi image]: https://badge.fury.io/py/metamorph.svg
 [pypi link]: https://pypi.org/project/metamorph/
 
-[a s image]: https://github.com/APN-Pucky/metamorph/actions/workflows/release.yml/badge.svg
-[a s link]: https://github.com/APN-Pucky/metamorph/actions/workflows/release.yml
+[a s image]: https://github.com/APN-Pucky/metamorph/actions/workflows/stable.yml/badge.svg
+[a s link]: https://github.com/APN-Pucky/metamorph/actions/workflows/stable.yml
 [a t link]: https://github.com/APN-Pucky/metamorph/actions/workflows/unstable.yml
 [a t image]: https://github.com/APN-Pucky/metamorph/actions/workflows/unstable.yml/badge.svg
 
-
+[codacy quality image]: https://app.codacy.com/project/badge/Grade/1acfcad112734b1ca875518cf1eeda34
+[codacy quality link]: https://www.codacy.com/gh/APN-Pucky/metamorph/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/metamorph&amp;utm_campaign=Badge_Grade
```

### Comparing `metamorph-0.0.8/metamorph/config.py` & `metamorph-0.0.9/metamorph/config.py`

 * *Files identical despite different names*

### Comparing `metamorph-0.0.8/metamorph/main.py` & `metamorph-0.0.9/metamorph/main.py`

 * *Files identical despite different names*

### Comparing `metamorph-0.0.8/metamorph.egg-info/PKG-INFO` & `metamorph-0.0.9/metamorph.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamorph
-Version: 0.0.8
+Version: 0.0.9
 Summary: auto rewrite text
 Home-page: https://github.com/APN-Pucky/metamorph
 Author: APN
 Author-email: APN-Pucky@no-reply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,18 @@
 
 Doc: `metamorph --help`
 
 (Work-in-progress: Doc: https://apn-pucky.github.io/metamorph/index.html )
 
 [![PyPI version][pypi image]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/metamorph.svg) 
 
-| [Stable][doc release]        | [Dev][doc test]           |
+| [Stable][doc release]        | [Unstable][doc test]           |
 | ------------- |:-------------:|
 | [![workflow][a s image]][a s link]      | [![test][a t image]][a t link]     |
+| -     |[![Codacy Badge][codacy quality image]][codacy quality link] | 
 
 ## Versions
 
 ### Stable
 
 ```sh
 pip install metamorph [--user] [--upgrade]
@@ -89,13 +90,14 @@
 
 [doc release]: https://apn-pucky.github.io/metamorph/index.html
 [doc test]: https://apn-pucky.github.io/metamorph/test/index.html
 
 [pypi image]: https://badge.fury.io/py/metamorph.svg
 [pypi link]: https://pypi.org/project/metamorph/
 
-[a s image]: https://github.com/APN-Pucky/metamorph/actions/workflows/release.yml/badge.svg
-[a s link]: https://github.com/APN-Pucky/metamorph/actions/workflows/release.yml
+[a s image]: https://github.com/APN-Pucky/metamorph/actions/workflows/stable.yml/badge.svg
+[a s link]: https://github.com/APN-Pucky/metamorph/actions/workflows/stable.yml
 [a t link]: https://github.com/APN-Pucky/metamorph/actions/workflows/unstable.yml
 [a t image]: https://github.com/APN-Pucky/metamorph/actions/workflows/unstable.yml/badge.svg
 
-
+[codacy quality image]: https://app.codacy.com/project/badge/Grade/1acfcad112734b1ca875518cf1eeda34
+[codacy quality link]: https://www.codacy.com/gh/APN-Pucky/metamorph/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/metamorph&amp;utm_campaign=Badge_Grade
```

### Comparing `metamorph-0.0.8/setup.py` & `metamorph-0.0.9/setup.py`

 * *Files identical despite different names*

