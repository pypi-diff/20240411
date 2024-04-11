# Comparing `tmp/dissect.jffs-1.2.dev3.tar.gz` & `tmp/dissect.jffs-1.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.jffs-1.2.dev3.tar", last modified: Thu Mar 28 17:22:16 2024, max compression
+gzip compressed data, was "dissect.jffs-1.2.dev4.tar", last modified: Thu Apr 11 11:56:53 2024, max compression
```

## Comparing `dissect.jffs-1.2.dev3.tar` & `dissect.jffs-1.2.dev4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.730053 dissect.jffs-1.2.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.714053 dissect.jffs-1.2.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.718053 dissect.jffs-1.2.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/.github/workflows/dissect-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-28 17:22:16.730053 dissect.jffs-1.2.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.714053 dissect.jffs-1.2.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.718053 dissect.jffs-1.2.dev3/dissect/jffs/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/dissect/jffs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/dissect/jffs/c_jffs2.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/dissect/jffs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/dissect/jffs/jffs2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.730053 dissect.jffs-1.2.dev3/dissect.jffs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-28 17:22:16.000000 dissect.jffs-1.2.dev3/dissect.jffs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-28 17:22:16.000000 dissect.jffs-1.2.dev3/dissect.jffs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:22:16.000000 dissect.jffs-1.2.dev3/dissect.jffs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:22:16.000000 dissect.jffs-1.2.dev3/dissect.jffs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:22:16.000000 dissect.jffs-1.2.dev3/dissect.jffs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-28 17:22:11.000000 dissect.jffs-1.2.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:22:16.730053 dissect.jffs-1.2.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.722053 dissect.jffs-1.2.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-28 17:22:02.000000 dissect.jffs-1.2.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:16.722053 dissect.jffs-1.2.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-28 17:22:04.000000 dissect.jffs-1.2.dev3/tests/data/jffs2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    94574 2024-03-28 17:22:04.000000 dissect.jffs-1.2.dev3/tests/data/jffs2.zlib.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)  7401918 2024-03-28 17:22:04.000000 dissect.jffs-1.2.dev3/tests/data/router.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-28 17:22:03.000000 dissect.jffs-1.2.dev3/tests/test_jffs2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:22:03.000000 dissect.jffs-1.2.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.679379 dissect.jffs-1.2.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.667379 dissect.jffs-1.2.dev4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.667379 dissect.jffs-1.2.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/.github/workflows/dissect-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-11 11:56:53.679379 dissect.jffs-1.2.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.663379 dissect.jffs-1.2.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.667379 dissect.jffs-1.2.dev4/dissect/jffs/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/dissect/jffs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/dissect/jffs/c_jffs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/dissect/jffs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/dissect/jffs/jffs2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.679379 dissect.jffs-1.2.dev4/dissect.jffs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-11 11:56:53.000000 dissect.jffs-1.2.dev4/dissect.jffs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 11:56:53.000000 dissect.jffs-1.2.dev4/dissect.jffs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:53.000000 dissect.jffs-1.2.dev4/dissect.jffs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:53.000000 dissect.jffs-1.2.dev4/dissect.jffs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:53.000000 dissect.jffs-1.2.dev4/dissect.jffs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 11:56:48.000000 dissect.jffs-1.2.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:53.679379 dissect.jffs-1.2.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.667379 dissect.jffs-1.2.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:53.667379 dissect.jffs-1.2.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-11 11:56:45.000000 dissect.jffs-1.2.dev4/tests/data/jffs2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    94574 2024-04-11 11:56:45.000000 dissect.jffs-1.2.dev4/tests/data/jffs2.zlib.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  7401918 2024-04-11 11:56:45.000000 dissect.jffs-1.2.dev4/tests/data/router.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/tests/test_jffs2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:56:44.000000 dissect.jffs-1.2.dev4/tox.ini
```

### Comparing `dissect.jffs-1.2.dev3/.github/workflows/dissect-ci.yml` & `dissect.jffs-1.2.dev4/.github/workflows/dissect-ci.yml`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/LICENSE` & `dissect.jffs-1.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/PKG-INFO` & `dissect.jffs-1.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.jffs
-Version: 1.2.dev3
+Version: 1.2.dev4
 Summary: A Dissect module implementing a parser for the JFFS2 file system, commonly used by router operating systems
 Author-email: JSCU-NL <121175071+JSCU-CNI@users.noreply.github.com>, Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.jffs
 Project-URL: repository, https://github.com/fox-it/dissect.jffs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.jffs-1.2.dev3/README.md` & `dissect.jffs-1.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/dissect/jffs/c_jffs2.py` & `dissect.jffs-1.2.dev4/dissect/jffs/c_jffs2.py`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/dissect/jffs/jffs2.py` & `dissect.jffs-1.2.dev4/dissect/jffs/jffs2.py`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/dissect.jffs.egg-info/PKG-INFO` & `dissect.jffs-1.2.dev4/dissect.jffs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.jffs
-Version: 1.2.dev3
+Version: 1.2.dev4
 Summary: A Dissect module implementing a parser for the JFFS2 file system, commonly used by router operating systems
 Author-email: JSCU-NL <121175071+JSCU-CNI@users.noreply.github.com>, Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.jffs
 Project-URL: repository, https://github.com/fox-it/dissect.jffs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.jffs-1.2.dev3/dissect.jffs.egg-info/SOURCES.txt` & `dissect.jffs-1.2.dev4/dissect.jffs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitattributes
 .gitignore
 COPYRIGHT
 LICENSE
 README.md
 pyproject.toml
 tox.ini
+.github/pull_request_template.md
 .github/workflows/dissect-ci.yml
 dissect.jffs.egg-info/PKG-INFO
 dissect.jffs.egg-info/SOURCES.txt
 dissect.jffs.egg-info/dependency_links.txt
 dissect.jffs.egg-info/requires.txt
 dissect.jffs.egg-info/top_level.txt
 dissect/jffs/__init__.py
```

### Comparing `dissect.jffs-1.2.dev3/pyproject.toml` & `dissect.jffs-1.2.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/tests/data/jffs2.zlib.bin.gz` & `dissect.jffs-1.2.dev4/tests/data/jffs2.zlib.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/tests/data/router.bin.gz` & `dissect.jffs-1.2.dev4/tests/data/router.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/tests/test_jffs2.py` & `dissect.jffs-1.2.dev4/tests/test_jffs2.py`

 * *Files identical despite different names*

### Comparing `dissect.jffs-1.2.dev3/tox.ini` & `dissect.jffs-1.2.dev4/tox.ini`

 * *Files identical despite different names*

