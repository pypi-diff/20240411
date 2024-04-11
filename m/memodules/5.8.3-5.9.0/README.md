# Comparing `tmp/memodules-5.8.3.tar.gz` & `tmp/memodules-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memodules-5.8.3.tar", last modified: Tue Mar 26 05:21:22 2024, max compression
+gzip compressed data, was "memodules-5.9.0.tar", last modified: Thu Apr 11 02:20:16 2024, max compression
```

## Comparing `memodules-5.8.3.tar` & `memodules-5.9.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.395369 memodules-5.8.3/
--rw-rw-rw-   0        0        0      449 2024-03-26 05:21:22.394374 memodules-5.8.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.284750 memodules-5.8.3/memodules/
--rw-rw-rw-   0        0        0       57 2023-11-22 03:59:37.000000 memodules-5.8.3/memodules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.301611 memodules-5.8.3/memodules/alphabet_to_integer/
--rw-rw-rw-   0        0        0     2966 2023-07-03 08:02:29.000000 memodules-5.8.3/memodules/alphabet_to_integer/AlphabetToInteger.py
--rw-rw-rw-   0        0        0       34 2023-07-10 05:00:24.000000 memodules-5.8.3/memodules/alphabet_to_integer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.304601 memodules-5.8.3/memodules/builtins/
--rw-rw-rw-   0        0        0       48 2024-02-27 00:52:47.000000 memodules-5.8.3/memodules/builtins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.309584 memodules-5.8.3/memodules/builtins/tkinter/
--rw-rw-rw-   0        0        0      779 2024-03-26 05:19:27.000000 memodules-5.8.3/memodules/builtins/tkinter/Event.py
--rw-rw-rw-   0        0        0       87 2024-03-26 05:19:42.000000 memodules-5.8.3/memodules/builtins/tkinter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.314560 memodules-5.8.3/memodules/builtins/tkinter/ttk/
--rw-rw-rw-   0        0        0      646 2024-03-26 05:18:53.000000 memodules-5.8.3/memodules/builtins/tkinter/ttk/Event.py
--rw-rw-rw-   0        0        0       65 2024-03-26 05:19:07.000000 memodules-5.8.3/memodules/builtins/tkinter/ttk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.319551 memodules-5.8.3/memodules/cr_exchange_lib/
--rw-rw-rw-   0        0        0       30 2023-07-10 05:00:52.000000 memodules-5.8.3/memodules/cr_exchange_lib/__init__.py
--rw-rw-rw-   0        0        0      528 2023-07-03 07:34:40.000000 memodules-5.8.3/memodules/cr_exchange_lib/crExchangeLib.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.323537 memodules-5.8.3/memodules/cslapp/
--rw-rw-rw-   0        0        0        2 2023-10-31 06:11:53.000000 memodules-5.8.3/memodules/cslapp/__init__.py
--rw-rw-rw-   0        0        0      534 2023-10-31 04:58:15.000000 memodules-5.8.3/memodules/cslapp/calc_source.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.328594 memodules-5.8.3/memodules/debug_tools/
--rw-rw-rw-   0        0        0       87 2024-03-21 06:14:08.000000 memodules-5.8.3/memodules/debug_tools/__init__.py
--rw-rw-rw-   0        0        0     2779 2024-03-21 06:12:58.000000 memodules-5.8.3/memodules/debug_tools/access_viewer.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.336565 memodules-5.8.3/memodules/decorators/
--rw-rw-rw-   0        0        0       70 2023-09-20 07:29:16.000000 memodules-5.8.3/memodules/decorators/PushHF.py
--rw-rw-rw-   0        0        0       83 2023-09-13 06:58:38.000000 memodules-5.8.3/memodules/decorators/__init__.py
--rw-rw-rw-   0        0        0     2571 2023-09-13 05:52:15.000000 memodules-5.8.3/memodules/decorators/debug_dec.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.341477 memodules-5.8.3/memodules/directory/
--rw-rw-rw-   0        0        0       80 2023-11-27 04:09:01.000000 memodules-5.8.3/memodules/directory/__init__.py
--rw-rw-rw-   0        0        0        0 2023-11-27 04:07:08.000000 memodules-5.8.3/memodules/directory/structure.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.345457 memodules-5.8.3/memodules/e_typing/
--rw-rw-rw-   0        0        0     3490 2023-12-13 00:21:50.000000 memodules-5.8.3/memodules/e_typing/__init__.py
--rw-rw-rw-   0        0        0     2342 2023-11-28 05:57:33.000000 memodules-5.8.3/memodules/e_typing/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.350526 memodules-5.8.3/memodules/error_lib/
--rw-rw-rw-   0        0        0      261 2023-07-03 08:01:32.000000 memodules-5.8.3/memodules/error_lib/ErrorLib.py
--rw-rw-rw-   0        0        0       25 2023-07-10 05:01:07.000000 memodules-5.8.3/memodules/error_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.357500 memodules-5.8.3/memodules/inicon/
--rw-rw-rw-   0        0        0      137 2023-11-21 06:53:02.000000 memodules-5.8.3/memodules/inicon/__init__.py
--rw-rw-rw-   0        0        0     9024 2023-11-21 06:49:32.000000 memodules-5.8.3/memodules/inicon/inicon.py
--rw-rw-rw-   0        0        0     7970 2023-11-21 06:52:14.000000 memodules-5.8.3/memodules/inicon/inicon.pyi
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.359490 memodules-5.8.3/memodules/judgment/
--rw-rw-rw-   0        0        0      282 2023-11-22 05:58:18.000000 memodules-5.8.3/memodules/judgment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.378427 memodules-5.8.3/memodules/log/
--rw-rw-rw-   0        0        0     4296 2023-12-18 00:57:53.000000 memodules-5.8.3/memodules/log/Dlog.py
--rw-rw-rw-   0        0        0     1675 2023-12-18 00:57:13.000000 memodules-5.8.3/memodules/log/Dlog.pyi
--rw-rw-rw-   0        0        0      184 2023-12-13 01:08:14.000000 memodules-5.8.3/memodules/log/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-12-18 07:07:23.000000 memodules-5.8.3/memodules/log/cprint.py
--rw-rw-rw-   0        0        0     3199 2023-12-13 01:54:07.000000 memodules-5.8.3/memodules/log/cprint.pyi
--rw-rw-rw-   0        0        0     5385 2023-07-10 23:31:34.000000 memodules-5.8.3/memodules/log/log.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.386398 memodules-5.8.3/memodules/sandbox/
--rw-rw-rw-   0        0        0      168 2024-03-19 04:41:58.000000 memodules-5.8.3/memodules/sandbox/__init__.py
--rw-rw-rw-   0        0        0     1046 2024-03-19 05:22:08.000000 memodules-5.8.3/memodules/sandbox/sqlalchemy.py
--rw-rw-rw-   0        0        0     3078 2024-03-19 07:45:47.000000 memodules-5.8.3/memodules/sandbox/sqlalchemy.pyi
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.392381 memodules-5.8.3/memodules/xl_for_python/
--rw-rw-rw-   0        0        0     2899 2023-07-10 23:30:28.000000 memodules-5.8.3/memodules/xl_for_python/Python_xlTypeLib_Addin.py
--rw-rw-rw-   0        0        0       39 2023-07-10 05:01:49.000000 memodules-5.8.3/memodules/xl_for_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 05:21:22.296619 memodules-5.8.3/memodules.egg-info/
--rw-rw-rw-   0        0        0      449 2024-03-26 05:21:22.000000 memodules-5.8.3/memodules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2024-03-26 05:21:22.000000 memodules-5.8.3/memodules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 05:21:22.000000 memodules-5.8.3/memodules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-26 05:21:22.000000 memodules-5.8.3/memodules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 05:21:22.396367 memodules-5.8.3/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-03-26 05:21:17.000000 memodules-5.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.984761 memodules-5.9.0/
+-rw-rw-rw-   0        0        0      449 2024-04-11 02:20:16.981771 memodules-5.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.786421 memodules-5.9.0/memodules/
+-rw-rw-rw-   0        0        0       57 2023-11-22 03:59:37.000000 memodules-5.9.0/memodules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.811338 memodules-5.9.0/memodules/alphabet_to_integer/
+-rw-rw-rw-   0        0        0     2966 2023-07-03 08:02:29.000000 memodules-5.9.0/memodules/alphabet_to_integer/AlphabetToInteger.py
+-rw-rw-rw-   0        0        0       34 2023-07-10 05:00:24.000000 memodules-5.9.0/memodules/alphabet_to_integer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.815325 memodules-5.9.0/memodules/builtins/
+-rw-rw-rw-   0        0        0       48 2024-02-27 00:52:47.000000 memodules-5.9.0/memodules/builtins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.824295 memodules-5.9.0/memodules/builtins/tkinter/
+-rw-rw-rw-   0        0        0      779 2024-03-26 05:19:27.000000 memodules-5.9.0/memodules/builtins/tkinter/Event.py
+-rw-rw-rw-   0        0        0       87 2024-03-26 05:19:42.000000 memodules-5.9.0/memodules/builtins/tkinter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.831272 memodules-5.9.0/memodules/builtins/tkinter/ttk/
+-rw-rw-rw-   0        0        0      646 2024-03-26 05:18:53.000000 memodules-5.9.0/memodules/builtins/tkinter/ttk/Event.py
+-rw-rw-rw-   0        0        0       65 2024-03-26 05:19:07.000000 memodules-5.9.0/memodules/builtins/tkinter/ttk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.838249 memodules-5.9.0/memodules/cr_exchange_lib/
+-rw-rw-rw-   0        0        0       30 2023-07-10 05:00:52.000000 memodules-5.9.0/memodules/cr_exchange_lib/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-07-03 07:34:40.000000 memodules-5.9.0/memodules/cr_exchange_lib/crExchangeLib.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.845225 memodules-5.9.0/memodules/cslapp/
+-rw-rw-rw-   0        0        0        2 2023-10-31 06:11:53.000000 memodules-5.9.0/memodules/cslapp/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-10-31 04:58:15.000000 memodules-5.9.0/memodules/cslapp/calc_source.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.853199 memodules-5.9.0/memodules/debug_tools/
+-rw-rw-rw-   0        0        0       87 2024-03-21 06:14:08.000000 memodules-5.9.0/memodules/debug_tools/__init__.py
+-rw-rw-rw-   0        0        0     2779 2024-03-21 06:12:58.000000 memodules-5.9.0/memodules/debug_tools/access_viewer.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.866156 memodules-5.9.0/memodules/decorators/
+-rw-rw-rw-   0        0        0       70 2023-09-20 07:29:16.000000 memodules-5.9.0/memodules/decorators/PushHF.py
+-rw-rw-rw-   0        0        0       83 2023-09-13 06:58:38.000000 memodules-5.9.0/memodules/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2571 2023-09-13 05:52:15.000000 memodules-5.9.0/memodules/decorators/debug_dec.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.874129 memodules-5.9.0/memodules/directory/
+-rw-rw-rw-   0        0        0       80 2023-11-27 04:09:01.000000 memodules-5.9.0/memodules/directory/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-11-27 04:07:08.000000 memodules-5.9.0/memodules/directory/structure.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.880109 memodules-5.9.0/memodules/e_typing/
+-rw-rw-rw-   0        0        0     3490 2023-12-13 00:21:50.000000 memodules-5.9.0/memodules/e_typing/__init__.py
+-rw-rw-rw-   0        0        0     2342 2023-11-28 05:57:33.000000 memodules-5.9.0/memodules/e_typing/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.888083 memodules-5.9.0/memodules/error_lib/
+-rw-rw-rw-   0        0        0      261 2023-07-03 08:01:32.000000 memodules-5.9.0/memodules/error_lib/ErrorLib.py
+-rw-rw-rw-   0        0        0       25 2023-07-10 05:01:07.000000 memodules-5.9.0/memodules/error_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.900043 memodules-5.9.0/memodules/inicon/
+-rw-rw-rw-   0        0        0      137 2023-11-21 06:53:02.000000 memodules-5.9.0/memodules/inicon/__init__.py
+-rw-rw-rw-   0        0        0     9024 2023-11-21 06:49:32.000000 memodules-5.9.0/memodules/inicon/inicon.py
+-rw-rw-rw-   0        0        0     7970 2023-11-21 06:52:14.000000 memodules-5.9.0/memodules/inicon/inicon.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.904030 memodules-5.9.0/memodules/judgment/
+-rw-rw-rw-   0        0        0      282 2023-11-22 05:58:18.000000 memodules-5.9.0/memodules/judgment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.945891 memodules-5.9.0/memodules/log/
+-rw-rw-rw-   0        0        0     4296 2023-12-18 00:57:53.000000 memodules-5.9.0/memodules/log/Dlog.py
+-rw-rw-rw-   0        0        0     1675 2023-12-18 00:57:13.000000 memodules-5.9.0/memodules/log/Dlog.pyi
+-rw-rw-rw-   0        0        0      184 2023-12-13 01:08:14.000000 memodules-5.9.0/memodules/log/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-12-18 07:07:23.000000 memodules-5.9.0/memodules/log/cprint.py
+-rw-rw-rw-   0        0        0     3199 2023-12-13 01:54:07.000000 memodules-5.9.0/memodules/log/cprint.pyi
+-rw-rw-rw-   0        0        0     5385 2023-07-10 23:31:34.000000 memodules-5.9.0/memodules/log/log.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.964827 memodules-5.9.0/memodules/sandbox/
+-rw-rw-rw-   0        0        0      168 2024-03-19 04:41:58.000000 memodules-5.9.0/memodules/sandbox/__init__.py
+-rw-rw-rw-   0        0        0     1046 2024-03-19 05:22:08.000000 memodules-5.9.0/memodules/sandbox/sqlalchemy.py
+-rw-rw-rw-   0        0        0     3078 2024-03-19 07:45:47.000000 memodules-5.9.0/memodules/sandbox/sqlalchemy.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.968814 memodules-5.9.0/memodules/sql_pack/
+-rw-rw-rw-   0        0        0      724 2024-04-11 02:18:35.000000 memodules-5.9.0/memodules/sql_pack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.979778 memodules-5.9.0/memodules/xl_for_python/
+-rw-rw-rw-   0        0        0     2899 2023-07-10 23:30:28.000000 memodules-5.9.0/memodules/xl_for_python/Python_xlTypeLib_Addin.py
+-rw-rw-rw-   0        0        0       39 2023-07-10 05:01:49.000000 memodules-5.9.0/memodules/xl_for_python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.801372 memodules-5.9.0/memodules.egg-info/
+-rw-rw-rw-   0        0        0      449 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 02:20:16.984761 memodules-5.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-11 02:20:08.000000 memodules-5.9.0/setup.py
```

### Comparing `memodules-5.8.3/memodules/alphabet_to_integer/AlphabetToInteger.py` & `memodules-5.9.0/memodules/alphabet_to_integer/AlphabetToInteger.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/builtins/tkinter/Event.py` & `memodules-5.9.0/memodules/builtins/tkinter/Event.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/builtins/tkinter/ttk/Event.py` & `memodules-5.9.0/memodules/builtins/tkinter/ttk/Event.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/cr_exchange_lib/crExchangeLib.py` & `memodules-5.9.0/memodules/cr_exchange_lib/crExchangeLib.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/cslapp/calc_source.py` & `memodules-5.9.0/memodules/cslapp/calc_source.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/debug_tools/access_viewer.py` & `memodules-5.9.0/memodules/debug_tools/access_viewer.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/decorators/debug_dec.py` & `memodules-5.9.0/memodules/decorators/debug_dec.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/e_typing/__init__.py` & `memodules-5.9.0/memodules/e_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/e_typing/__init__.pyi` & `memodules-5.9.0/memodules/e_typing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/inicon/inicon.py` & `memodules-5.9.0/memodules/inicon/inicon.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/inicon/inicon.pyi` & `memodules-5.9.0/memodules/inicon/inicon.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/log/Dlog.py` & `memodules-5.9.0/memodules/log/Dlog.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/log/Dlog.pyi` & `memodules-5.9.0/memodules/log/Dlog.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/log/cprint.py` & `memodules-5.9.0/memodules/log/cprint.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/log/cprint.pyi` & `memodules-5.9.0/memodules/log/cprint.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/log/log.py` & `memodules-5.9.0/memodules/log/log.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/sandbox/sqlalchemy.py` & `memodules-5.9.0/memodules/sandbox/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/sandbox/sqlalchemy.pyi` & `memodules-5.9.0/memodules/sandbox/sqlalchemy.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules/xl_for_python/Python_xlTypeLib_Addin.py` & `memodules-5.9.0/memodules/xl_for_python/Python_xlTypeLib_Addin.py`

 * *Files identical despite different names*

### Comparing `memodules-5.8.3/memodules.egg-info/SOURCES.txt` & `memodules-5.9.0/memodules.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,9 +35,10 @@
 memodules/log/__init__.py
 memodules/log/cprint.py
 memodules/log/cprint.pyi
 memodules/log/log.py
 memodules/sandbox/__init__.py
 memodules/sandbox/sqlalchemy.py
 memodules/sandbox/sqlalchemy.pyi
+memodules/sql_pack/__init__.py
 memodules/xl_for_python/Python_xlTypeLib_Addin.py
 memodules/xl_for_python/__init__.py
```

