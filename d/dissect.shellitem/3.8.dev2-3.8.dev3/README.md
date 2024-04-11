# Comparing `tmp/dissect.shellitem-3.8.dev2.tar.gz` & `tmp/dissect.shellitem-3.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.shellitem-3.8.dev2.tar", last modified: Thu Mar 21 10:17:05 2024, max compression
+gzip compressed data, was "dissect.shellitem-3.8.dev3.tar", last modified: Thu Mar 28 17:22:27 2024, max compression
```

## Comparing `dissect.shellitem-3.8.dev2.tar` & `dissect.shellitem-3.8.dev3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.089584 dissect.shellitem-3.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-21 10:17:05.089584 dissect.shellitem-3.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.081584 dissect.shellitem-3.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.081584 dissect.shellitem-3.8.dev2/dissect/shellitem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/dissect/shellitem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.085584 dissect.shellitem-3.8.dev2/dissect/shellitem/lnk/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/dissect/shellitem/lnk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39685 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/dissect/shellitem/lnk/c_lnk.py
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/dissect/shellitem/lnk/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.085584 dissect.shellitem-3.8.dev2/dissect/shellitem/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/dissect/shellitem/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/dissect/shellitem/tools/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.085584 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-21 10:17:05.000000 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-21 10:17:05.000000 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:17:05.000000 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-21 10:17:05.000000 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:17:05.000000 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:17:05.000000 dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-21 10:16:59.000000 dissect.shellitem-3.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:17:05.089584 dissect.shellitem-3.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.085584 dissect.shellitem-3.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.085584 dissect.shellitem-3.8.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/data/downloads.win81.lnk
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/data/local.directory.seven.lnk
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/data/modified_remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/data/remote.directory.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/data/remote.file.xp.lnk
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/data/vista.idlist.lnk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:05.085584 dissect.shellitem-3.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tests/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 10:16:53.000000 dissect.shellitem-3.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.490174 dissect.shellitem-3.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-28 17:22:27.490174 dissect.shellitem-3.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.482174 dissect.shellitem-3.8.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.486174 dissect.shellitem-3.8.dev3/dissect/shellitem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/dissect/shellitem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.486174 dissect.shellitem-3.8.dev3/dissect/shellitem/lnk/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/dissect/shellitem/lnk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39685 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/dissect/shellitem/lnk/c_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/dissect/shellitem/lnk/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.486174 dissect.shellitem-3.8.dev3/dissect/shellitem/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/dissect/shellitem/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/dissect/shellitem/tools/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.490174 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-28 17:22:27.000000 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-28 17:22:27.000000 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:22:27.000000 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 17:22:27.000000 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:22:27.000000 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:22:27.000000 dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-28 17:22:21.000000 dissect.shellitem-3.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:22:27.490174 dissect.shellitem-3.8.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.486174 dissect.shellitem-3.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.486174 dissect.shellitem-3.8.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/data/downloads.win81.lnk
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/data/local.directory.seven.lnk
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/data/modified_remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/data/remote.directory.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/data/remote.file.xp.lnk
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/data/vista.idlist.lnk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:27.490174 dissect.shellitem-3.8.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tests/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:22:10.000000 dissect.shellitem-3.8.dev3/tox.ini
```

### Comparing `dissect.shellitem-3.8.dev2/LICENSE` & `dissect.shellitem-3.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/PKG-INFO` & `dissect.shellitem-3.8.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.shellitem-3.8.dev2/README.md` & `dissect.shellitem-3.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/dissect/shellitem/lnk/c_lnk.py` & `dissect.shellitem-3.8.dev3/dissect/shellitem/lnk/c_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/dissect/shellitem/lnk/lnk.py` & `dissect.shellitem-3.8.dev3/dissect/shellitem/lnk/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/dissect/shellitem/tools/lnk.py` & `dissect.shellitem-3.8.dev3/dissect/shellitem/tools/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/PKG-INFO` & `dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.shellitem-3.8.dev2/dissect.shellitem.egg-info/SOURCES.txt` & `dissect.shellitem-3.8.dev3/dissect.shellitem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/pyproject.toml` & `dissect.shellitem-3.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/conftest.py` & `dissect.shellitem-3.8.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/data/downloads.win81.lnk` & `dissect.shellitem-3.8.dev3/tests/data/downloads.win81.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/data/local.directory.seven.lnk` & `dissect.shellitem-3.8.dev3/tests/data/local.directory.seven.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/data/modified_remote.file.xp.lnk` & `dissect.shellitem-3.8.dev3/tests/data/modified_remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/data/remote.directory.xp.lnk` & `dissect.shellitem-3.8.dev3/tests/data/remote.directory.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/data/remote.file.xp.lnk` & `dissect.shellitem-3.8.dev3/tests/data/remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/data/vista.idlist.lnk` & `dissect.shellitem-3.8.dev3/tests/data/vista.idlist.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/docs/Makefile` & `dissect.shellitem-3.8.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/docs/conf.py` & `dissect.shellitem-3.8.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tests/test_lnk.py` & `dissect.shellitem-3.8.dev3/tests/test_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.8.dev2/tox.ini` & `dissect.shellitem-3.8.dev3/tox.ini`

 * *Files identical despite different names*

