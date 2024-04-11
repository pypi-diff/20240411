# Comparing `tmp/acquire-3.9.dev8.tar.gz` & `tmp/acquire-3.9.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.9.dev8.tar", last modified: Mon Aug 28 10:07:14 2023, max compression
+gzip compressed data, was "acquire-3.9.dev9.tar", last modified: Mon Aug 28 14:05:40 2023, max compression
```

## Comparing `acquire-3.9.dev8.tar` & `acquire-3.9.dev9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/
--rw-r--r--   0 runner    (1001) docker     (999)      294 2023-08-28 10:07:01.000000 acquire-3.9.dev8/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (999)    34523 2023-08-28 10:07:01.000000 acquire-3.9.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       48 2023-08-28 10:07:01.000000 acquire-3.9.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     3846 2023-08-28 10:07:14.928903 acquire-3.9.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2772 2023-08-28 10:07:01.000000 acquire-3.9.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.924903 acquire-3.9.dev8/acquire/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    83940 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (999)    21652 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (999)     3948 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.924903 acquire-3.9.dev8/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1878 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (999)      290 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)     8447 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (999)     1946 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (999)     7226 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (999)     6568 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (999)     2612 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (999)     7276 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (999)     3426 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (999)      210 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3282 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (999)      838 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (999)     2709 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    15901 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1745 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (999)     1911 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (999)     3053 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (999)    13666 2023-08-28 10:07:01.000000 acquire-3.9.dev8/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)      168 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.924903 acquire-3.9.dev8/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3846 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1322 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       96 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      129 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-28 10:07:14.000000 acquire-3.9.dev8/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1724 2023-08-28 10:07:05.000000 acquire-3.9.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 10:07:14.928903 acquire-3.9.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      938 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:07:14.928903 acquire-3.9.dev8/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (999)      749 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (999)      785 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1056 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_acquire_modules.py
--rw-r--r--   0 runner    (1001) docker     (999)    10608 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (999)      757 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (999)     1010 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (999)      808 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (999)     2695 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (999)     1306 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_misc_users.py
--rw-r--r--   0 runner    (1001) docker     (999)     1130 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (999)    10147 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     1794 2023-08-28 10:07:01.000000 acquire-3.9.dev8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.051999 acquire-3.9.dev9/
+-rw-r--r--   0 runner    (1001) docker     (999)      294 2023-08-28 14:05:25.000000 acquire-3.9.dev9/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (999)    34523 2023-08-28 14:05:25.000000 acquire-3.9.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)       48 2023-08-28 14:05:25.000000 acquire-3.9.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     3846 2023-08-28 14:05:40.051999 acquire-3.9.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2772 2023-08-28 14:05:25.000000 acquire-3.9.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    83957 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (999)    21652 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3948 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1878 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (999)      290 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8447 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1946 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7226 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6568 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2612 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7276 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3426 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (999)      210 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3282 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (999)      838 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2709 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15901 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1745 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1911 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3053 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13666 2023-08-28 14:05:25.000000 acquire-3.9.dev9/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)      168 2023-08-28 14:05:39.000000 acquire-3.9.dev9/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.047999 acquire-3.9.dev9/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3846 2023-08-28 14:05:40.000000 acquire-3.9.dev9/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1322 2023-08-28 14:05:40.000000 acquire-3.9.dev9/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 14:05:40.000000 acquire-3.9.dev9/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       96 2023-08-28 14:05:40.000000 acquire-3.9.dev9/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      129 2023-08-28 14:05:40.000000 acquire-3.9.dev9/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-28 14:05:40.000000 acquire-3.9.dev9/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     1724 2023-08-28 14:05:30.000000 acquire-3.9.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 14:05:40.051999 acquire-3.9.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.051999 acquire-3.9.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      938 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:05:40.051999 acquire-3.9.dev9/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (999)      749 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (999)      785 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     1056 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_acquire_modules.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10608 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (999)      757 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1010 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (999)      808 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2695 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1306 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_misc_users.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1130 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10147 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1794 2023-08-28 14:05:25.000000 acquire-3.9.dev9/tox.ini
```

### Comparing `acquire-3.9.dev8/LICENSE` & `acquire-3.9.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/PKG-INFO` & `acquire-3.9.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.9.dev8
+Version: 3.9.dev9
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.9.dev8/README.md` & `acquire-3.9.dev9/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/acquire.py` & `acquire-3.9.dev9/acquire/acquire.py`

 * *Files 0% similar despite different names*

```diff
@@ -2023,14 +2023,15 @@
             Misc,
             NTDS,
             ActiveDirectory,
             QuarantinedFiles,
             RemoteAccess,
             WindowsNotifications,
             SSH,
+            IIS,
         ],
         "linux": [
             Etc,
             Boot,
             Home,
             History,
             SSH,
```

### Comparing `acquire-3.9.dev8/acquire/collector.py` & `acquire-3.9.dev9/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/crypt.py` & `acquire-3.9.dev9/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/dynamic/windows/collect.py` & `acquire-3.9.dev9/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/dynamic/windows/handles.py` & `acquire-3.9.dev9/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/dynamic/windows/named_objects.py` & `acquire-3.9.dev9/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/dynamic/windows/ntdll.py` & `acquire-3.9.dev9/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/dynamic/windows/types.py` & `acquire-3.9.dev9/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/esxi.py` & `acquire-3.9.dev9/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/hashes.py` & `acquire-3.9.dev9/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/log.py` & `acquire-3.9.dev9/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/outputs/base.py` & `acquire-3.9.dev9/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/outputs/dir.py` & `acquire-3.9.dev9/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/outputs/tar.py` & `acquire-3.9.dev9/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/tools/decrypter.py` & `acquire-3.9.dev9/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/uploaders/minio.py` & `acquire-3.9.dev9/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/uploaders/plugin.py` & `acquire-3.9.dev9/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/uploaders/plugin_registry.py` & `acquire-3.9.dev9/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire/utils.py` & `acquire-3.9.dev9/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/acquire.egg-info/PKG-INFO` & `acquire-3.9.dev9/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.9.dev8
+Version: 3.9.dev9
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.9.dev8/acquire.egg-info/SOURCES.txt` & `acquire-3.9.dev9/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/pyproject.toml` & `acquire-3.9.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/conftest.py` & `acquire-3.9.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/docs/Makefile` & `acquire-3.9.dev9/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/docs/conf.py` & `acquire-3.9.dev9/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_acquire_command.py` & `acquire-3.9.dev9/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_acquire_modules.py` & `acquire-3.9.dev9/tests/test_acquire_modules.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_collector.py` & `acquire-3.9.dev9/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_decryptor_funcs.py` & `acquire-3.9.dev9/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_esxi_memory.py` & `acquire-3.9.dev9/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_file_sorting.py` & `acquire-3.9.dev9/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_minio_uploader.py` & `acquire-3.9.dev9/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_misc_users.py` & `acquire-3.9.dev9/tests/test_misc_users.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_plugin.py` & `acquire-3.9.dev9/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tests/test_utils.py` & `acquire-3.9.dev9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.9.dev8/tox.ini` & `acquire-3.9.dev9/tox.ini`

 * *Files identical despite different names*

