# Comparing `tmp/dissect.executable-1.6.dev3.tar.gz` & `tmp/dissect.executable-1.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.executable-1.6.dev3.tar", last modified: Thu Mar 28 17:21:53 2024, max compression
+gzip compressed data, was "dissect.executable-1.6.dev4.tar", last modified: Thu Apr 11 11:56:44 2024, max compression
```

## Comparing `dissect.executable-1.6.dev3.tar` & `dissect.executable-1.6.dev4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.651033 dissect.executable-1.6.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.655033 dissect.executable-1.6.dev3/dissect/executable/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.655033 dissect.executable-1.6.dev3/dissect/executable/elf/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/elf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/elf/c_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/elf/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.655033 dissect.executable-1.6.dev3/dissect/executable/macho/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/macho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.655033 dissect.executable-1.6.dev3/dissect/executable/pe/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/dissect/executable/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/dissect.executable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-28 17:21:53.000000 dissect.executable-1.6.dev3/dissect.executable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-28 17:21:53.000000 dissect.executable-1.6.dev3/dissect.executable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:53.000000 dissect.executable-1.6.dev3/dissect.executable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:21:53.000000 dissect.executable-1.6.dev3/dissect.executable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:53.000000 dissect.executable-1.6.dev3/dissect.executable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-28 17:21:48.000000 dissect.executable-1.6.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    16608 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/data/hello_world.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    14416 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/data/hello_world.stripped.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.659033 dissect.executable-1.6.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/test_segment_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:43.000000 dissect.executable-1.6.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.734944 dissect.executable-1.6.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-11 11:56:44.734944 dissect.executable-1.6.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.726944 dissect.executable-1.6.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.730944 dissect.executable-1.6.dev4/dissect/executable/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.730944 dissect.executable-1.6.dev4/dissect/executable/elf/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/elf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/elf/c_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/elf/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.730944 dissect.executable-1.6.dev4/dissect/executable/macho/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/macho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.730944 dissect.executable-1.6.dev4/dissect/executable/pe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/dissect/executable/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.734944 dissect.executable-1.6.dev4/dissect.executable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-11 11:56:44.000000 dissect.executable-1.6.dev4/dissect.executable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 11:56:44.000000 dissect.executable-1.6.dev4/dissect.executable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:44.000000 dissect.executable-1.6.dev4/dissect.executable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:44.000000 dissect.executable-1.6.dev4/dissect.executable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:44.000000 dissect.executable-1.6.dev4/dissect.executable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-11 11:56:40.000000 dissect.executable-1.6.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:44.734944 dissect.executable-1.6.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.730944 dissect.executable-1.6.dev4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.734944 dissect.executable-1.6.dev4/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16608 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/data/hello_world.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14416 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/data/hello_world.stripped.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:44.734944 dissect.executable-1.6.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/test_segment_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:56:32.000000 dissect.executable-1.6.dev4/tox.ini
```

### Comparing `dissect.executable-1.6.dev3/LICENSE` & `dissect.executable-1.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/PKG-INFO` & `dissect.executable-1.6.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.6.dev3
+Version: 1.6.dev4
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.executable-1.6.dev3/README.md` & `dissect.executable-1.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/dissect/executable/elf/c_elf.py` & `dissect.executable-1.6.dev4/dissect/executable/elf/c_elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/dissect/executable/elf/elf.py` & `dissect.executable-1.6.dev4/dissect/executable/elf/elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/dissect.executable.egg-info/PKG-INFO` & `dissect.executable-1.6.dev4/dissect.executable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.6.dev3
+Version: 1.6.dev4
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.executable-1.6.dev3/dissect.executable.egg-info/SOURCES.txt` & `dissect.executable-1.6.dev4/dissect.executable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/pyproject.toml` & `dissect.executable-1.6.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/data/hello_world.out` & `dissect.executable-1.6.dev4/tests/data/hello_world.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/data/hello_world.stripped.out` & `dissect.executable-1.6.dev4/tests/data/hello_world.stripped.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/docs/Makefile` & `dissect.executable-1.6.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/docs/conf.py` & `dissect.executable-1.6.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/test_dump.py` & `dissect.executable-1.6.dev4/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/test_section.py` & `dissect.executable-1.6.dev4/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/test_segment.py` & `dissect.executable-1.6.dev4/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tests/test_segment_table.py` & `dissect.executable-1.6.dev4/tests/test_segment_table.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.6.dev3/tox.ini` & `dissect.executable-1.6.dev4/tox.ini`

 * *Files identical despite different names*

