# Comparing `tmp/jy_lib-0.5.5.tar.gz` & `tmp/jy_lib-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.5.5.tar` & `jy_lib-0.5.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.5.5/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.5.5/.pypirc
--rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.5.5/.vscode/launch.json
--rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.5.5/.vscode/settings.json
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.5.5/LICENSE
--rw-r--r--   0        0        0      279 2023-10-23 03:28:56.135347 jy_lib-0.5.5/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.5.5/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.5.5/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.5.5/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-02 02:09:46.217825 jy_lib-0.5.5/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.5.5/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.5.5/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.5.5/jy_lib/base.py
--rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.5.5/jy_lib/cache.py
--rw-r--r--   0        0        0     4391 2024-02-29 10:03:32.680087 jy_lib-0.5.5/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.5.5/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.5.5/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.5.5/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.5.5/jy_lib/decorator.py
--rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.5.5/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.5.5/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.5.5/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.5.5/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.5.5/jy_lib/nav.py
--rw-r--r--   0        0        0    17343 2024-04-02 02:09:29.527247 jy_lib-0.5.5/jy_lib/smb_client.py
--rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.5.5/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.5.5/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.5.5/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.5.5/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.5.5/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.5.5/publish-test.sh
--rw-r--r--   0        0        0      553 2024-03-22 03:15:49.048497 jy_lib-0.5.5/pyproject.toml
--rw-r--r--   0        0        0       63 2024-03-04 00:45:32.639570 jy_lib-0.5.5/requirements.txt
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 jy_lib-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.5.6/.gitignore
+-rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.5.6/.pypirc
+-rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.5.6/.vscode/launch.json
+-rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.5.6/.vscode/settings.json
+-rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.5.6/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.5.6/Pipfile
+-rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.5.6/Pipfile.lock
+-rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.5.6/README.md
+-rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.5.6/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-11 01:36:03.611613 jy_lib-0.5.6/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.5.6/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.5.6/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.5.6/jy_lib/base.py
+-rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.5.6/jy_lib/cache.py
+-rw-r--r--   0        0        0     3120 2024-04-11 01:28:25.532231 jy_lib-0.5.6/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.5.6/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.5.6/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.5.6/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.5.6/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.5.6/jy_lib/decorator.py
+-rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.5.6/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.5.6/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.5.6/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.5.6/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.5.6/jy_lib/nav.py
+-rw-r--r--   0        0        0    17343 2024-04-02 02:09:29.527247 jy_lib-0.5.6/jy_lib/smb_client.py
+-rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.5.6/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.5.6/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.5.6/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.5.6/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.5.6/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.5.6/publish-test.sh
+-rw-r--r--   0        0        0      553 2024-03-22 03:15:49.048497 jy_lib-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-11 01:28:25.533916 jy_lib-0.5.6/requirements.txt
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 jy_lib-0.5.6/PKG-INFO
```

### Comparing `jy_lib-0.5.5/.gitignore` & `jy_lib-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/.vscode/settings.json` & `jy_lib-0.5.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/LICENSE` & `jy_lib-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/Pipfile.lock` & `jy_lib-0.5.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/__init__.py` & `jy_lib-0.5.6/jy_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     WarrantsType,
     BlockType,
     SpotType,
     SymbolType,
     SymbolFlag,
 )
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
```

### Comparing `jy_lib-0.5.5/jy_lib/auth_client.py` & `jy_lib-0.5.6/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/bank.py` & `jy_lib-0.5.6/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/base.py` & `jy_lib-0.5.6/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/cache.py` & `jy_lib-0.5.6/jy_lib/cache.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/compressor.py` & `jy_lib-0.5.6/jy_lib/compressor.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,26 +28,26 @@
         elif self == self.BR:
             return brotli.Compressor()
         elif self == self.ZSTD:
             return zstandard.ZstdCompressor(level)
 
 
 class ZstdStreamCompressor:
-    def __init__(self, size: int = -1, interval: int = -1, threads: int = 0):
+    def __init__(self, size: int = -1, interval: int = -1, threads: int = 0, level: int = zstandard.STRATEGY_BTULTRA2):
         """
         with ZstdStreamCompressor(size=len(data1) + len(data2), interval=1024*1024) as sc:
             sc.update(data=data1)
             sc.update(data=data2)
             return sc.stream
         """
         self.stream: io.BytesIO = io.BytesIO()
         self.size: int = size
         self.interval: int = interval
         self.interval_count: int = 0
-        self.compressor = zstandard.ZstdCompressor(level=zstandard.STRATEGY_BTULTRA2, threads=threads)
+        self.compressor = zstandard.ZstdCompressor(level=level, threads=threads)
         self.chunker = self.compressor.chunker(size=self.size)
         self._origin_size: int = 0
 
     def update(self, data: bytes):
         """对原始数据流进行流式压缩"""
         assert isinstance(data, bytes)
         buffer = io.BytesIO(data)
```

### Comparing `jy_lib-0.5.5/jy_lib/country.py` & `jy_lib-0.5.6/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/currency.py` & `jy_lib-0.5.6/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/date.py` & `jy_lib-0.5.6/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/decorator.py` & `jy_lib-0.5.6/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/exchange.py` & `jy_lib-0.5.6/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/interrupt_protect.py` & `jy_lib-0.5.6/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/lock.py` & `jy_lib-0.5.6/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/math.py` & `jy_lib-0.5.6/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/nav.py` & `jy_lib-0.5.6/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/smb_client.py` & `jy_lib-0.5.6/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/symbol.py` & `jy_lib-0.5.6/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/symbol_em.py` & `jy_lib-0.5.6/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/jy_lib/time.py` & `jy_lib-0.5.6/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.5.5/pyproject.toml` & `jy_lib-0.5.6/pyproject.toml`

 * *Files identical despite different names*

