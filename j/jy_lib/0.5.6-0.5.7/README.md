# Comparing `tmp/jy_lib-0.5.6.tar.gz` & `tmp/jy_lib-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.5.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.5.6.tar` & `jy_lib-0.5.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.5.6/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.5.6/.pypirc
--rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.5.6/.vscode/launch.json
--rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.5.6/.vscode/settings.json
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.5.6/LICENSE
--rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.5.6/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.5.6/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.5.6/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.5.6/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-11 01:36:03.611613 jy_lib-0.5.6/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.5.6/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.5.6/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.5.6/jy_lib/base.py
--rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.5.6/jy_lib/cache.py
--rw-r--r--   0        0        0     3120 2024-04-11 01:28:25.532231 jy_lib-0.5.6/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.5.6/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.5.6/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.5.6/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.5.6/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.5.6/jy_lib/decorator.py
--rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.5.6/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.5.6/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.5.6/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.5.6/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.5.6/jy_lib/nav.py
--rw-r--r--   0        0        0    17343 2024-04-02 02:09:29.527247 jy_lib-0.5.6/jy_lib/smb_client.py
--rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.5.6/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.5.6/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.5.6/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.5.6/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.5.6/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.5.6/publish-test.sh
--rw-r--r--   0        0        0      553 2024-03-22 03:15:49.048497 jy_lib-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-11 01:28:25.533916 jy_lib-0.5.6/requirements.txt
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 jy_lib-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.5.7/.gitignore
+-rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.5.7/.pypirc
+-rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.5.7/.vscode/launch.json
+-rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.5.7/.vscode/settings.json
+-rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.5.7/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.5.7/Pipfile
+-rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.5.7/Pipfile.lock
+-rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.5.7/README.md
+-rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.5.7/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-11 07:53:20.897598 jy_lib-0.5.7/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.5.7/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.5.7/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.5.7/jy_lib/base.py
+-rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.5.7/jy_lib/cache.py
+-rw-r--r--   0        0        0     3120 2024-04-11 01:28:25.532231 jy_lib-0.5.7/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.5.7/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.5.7/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.5.7/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.5.7/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.5.7/jy_lib/decorator.py
+-rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.5.7/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.5.7/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.5.7/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.5.7/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.5.7/jy_lib/nav.py
+-rw-r--r--   0        0        0    17343 2024-04-02 02:09:29.527247 jy_lib-0.5.7/jy_lib/smb_client.py
+-rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.5.7/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.5.7/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.5.7/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.5.7/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.5.7/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.5.7/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-11 01:28:25.533916 jy_lib-0.5.7/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.5.7/PKG-INFO
```

### Comparing `jy_lib-0.5.6/.gitignore` & `jy_lib-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/.vscode/settings.json` & `jy_lib-0.5.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/LICENSE` & `jy_lib-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/Pipfile` & `jy_lib-0.5.7/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/Pipfile.lock` & `jy_lib-0.5.7/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/__init__.py` & `jy_lib-0.5.7/jy_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     WarrantsType,
     BlockType,
     SpotType,
     SymbolType,
     SymbolFlag,
 )
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
```

### Comparing `jy_lib-0.5.6/jy_lib/auth_client.py` & `jy_lib-0.5.7/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/bank.py` & `jy_lib-0.5.7/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/base.py` & `jy_lib-0.5.7/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/cache.py` & `jy_lib-0.5.7/jy_lib/cache.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/clickhouse.py` & `jy_lib-0.5.7/jy_lib/clickhouse.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/compressor.py` & `jy_lib-0.5.7/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/country.py` & `jy_lib-0.5.7/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/currency.py` & `jy_lib-0.5.7/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/date.py` & `jy_lib-0.5.7/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/decorator.py` & `jy_lib-0.5.7/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/exchange.py` & `jy_lib-0.5.7/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/interrupt_protect.py` & `jy_lib-0.5.7/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/lock.py` & `jy_lib-0.5.7/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/math.py` & `jy_lib-0.5.7/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/nav.py` & `jy_lib-0.5.7/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/smb_client.py` & `jy_lib-0.5.7/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/symbol.py` & `jy_lib-0.5.7/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/symbol_em.py` & `jy_lib-0.5.7/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.6/jy_lib/time.py` & `jy_lib-0.5.7/jy_lib/time.py`

 * *Files identical despite different names*

