# Comparing `tmp/mypylib-0.2.0.tar.gz` & `tmp/mypylib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.2.0.tar", last modified: Wed Mar 27 15:23:19 2024, max compression
+gzip compressed data, was "mypylib-0.2.1.tar", last modified: Thu Apr 11 10:20:26 2024, max compression
```

## Comparing `mypylib-0.2.0.tar` & `mypylib-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-03-27 15:23:19.591926 mypylib-0.2.0/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-03-27 15:23:19.591660 mypylib-0.2.0/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.0/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-03-27 15:23:19.587517 mypylib-0.2.0/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    50958 2024-03-27 15:21:30.000000 mypylib-0.2.0/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3417 2024-01-25 14:54:07.000000 mypylib-0.2.0/mypylib/binance.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.0/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.0/mypylib/my_random_proxy.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/rayin.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    10696 2023-12-27 08:14:26.000000 mypylib-0.2.0/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-03-27 15:23:19.591190 mypylib-0.2.0/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.0/mypylib/tmpDevelopment/arping.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.0/mypylib/tmpDevelopment/tmp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.0/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2540 2024-03-19 15:35:40.000000 mypylib-0.2.0/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.0/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     9928 2024-03-24 01:31:48.000000 mypylib-0.2.0/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-03-27 15:23:19.589173 mypylib-0.2.0/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-03-27 15:23:19.000000 mypylib-0.2.0/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-03-27 15:23:19.000000 mypylib-0.2.0/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-03-27 15:23:19.000000 mypylib-0.2.0/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-03-27 15:23:19.000000 mypylib-0.2.0/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-03-27 15:23:19.592019 mypylib-0.2.0/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.0/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.740391 mypylib-0.2.1/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-11 10:20:26.740103 mypylib-0.2.1/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.1/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.735008 mypylib-0.2.1/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    51026 2024-04-11 10:19:20.000000 mypylib-0.2.1/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3417 2024-01-25 14:54:07.000000 mypylib-0.2.1/mypylib/binance.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.1/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.1/mypylib/my_random_proxy.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/rayin.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    10696 2023-12-27 08:14:26.000000 mypylib-0.2.1/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.739558 mypylib-0.2.1/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.1/mypylib/tmpDevelopment/arping.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.1/mypylib/tmpDevelopment/tmp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.1/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2540 2024-03-19 15:35:40.000000 mypylib-0.2.1/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.1/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    10029 2024-04-11 10:19:20.000000 mypylib-0.2.1/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-11 10:20:26.736852 mypylib-0.2.1/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-04-11 10:20:26.000000 mypylib-0.2.1/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-04-11 10:20:26.740472 mypylib-0.2.1/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.1/setup.py
```

### Comparing `mypylib-0.2.0/README.md` & `mypylib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/MP_shioaji_ticks.py` & `mypylib-0.2.1/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/__init__.py` & `mypylib-0.2.1/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,17 +88,18 @@
     '2023/12/27: 0.1.94 all stock info 加入 OTC or TSE',
     '2024/01/02: 0.1.95 Update get_punishment_list()',
     '2024/03/11: 0.1.96 修正處置股資料。必須要看是否在期限內',
     '2024/03/13: 0.1.97 fix get_punishment_list()',
     '2024/03/23: 0.1.98 add warrant_bible_convert_to_c_need()',
     '2024/03/24: 0.1.99 modify warrant_bible_convert_to_c_need() and save warrant_bible.txt',
     '2024/03/27: 0.2.00 fix get_punishment_list() date bug ',
+    '2024/04/11: 0.2.01 fix warrant_bible_convert_to_c_need() bug',
 }
 
-__version__ = '0.2.00'
+__version__ = '0.2.01'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.2.0/mypylib/binance.py` & `mypylib-0.2.1/mypylib/binance.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/binance_copy_bot.py` & `mypylib-0.2.1/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/chdbif.py` & `mypylib-0.2.1/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/crawler.py` & `mypylib-0.2.1/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/crypto.py` & `mypylib-0.2.1/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/finmind.py` & `mypylib-0.2.1/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/libexcel.py` & `mypylib-0.2.1/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/mvp.py` & `mypylib-0.2.1/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/option_test.py` & `mypylib-0.2.1/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/rayin.py` & `mypylib-0.2.1/mypylib/rayin.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/shioaji_history_ticks.py` & `mypylib-0.2.1/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/shioaji_kline.py` & `mypylib-0.2.1/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/shioaji_ticks.py` & `mypylib-0.2.1/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/sjtools.py` & `mypylib-0.2.1/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/tLineNotify.py` & `mypylib-0.2.1/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/ti.py` & `mypylib-0.2.1/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/tmpDevelopment/arping.py` & `mypylib-0.2.1/mypylib/tmpDevelopment/arping.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/tmpDevelopment/tmp.py` & `mypylib-0.2.1/mypylib/tmpDevelopment/tmp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.2.1/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/tplaysound.py` & `mypylib-0.2.1/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/tredis.py` & `mypylib-0.2.1/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/mypylib/warrant.py` & `mypylib-0.2.1/mypylib/warrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,19 @@
     return dict_warrant_to_info, dict_stock_to_warrant
 
 
 def warrant_bible_convert_to_c_need(file_to_convert=None):
     if file_to_convert is None:
         files = os.listdir(f'{expanduser("~")}/warrant')
         files.sort(reverse=True)
-        file_to_convert = f'{expanduser("~")}/warrant/{files[0]}'
+        file = ''
+        for file in files:
+            if file.endswith('.xls'):
+                break
+        file_to_convert = f'{expanduser("~")}/warrant/{file}'
 
     print(f'讀取權證達人寶典: {file_to_convert}')
     dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(file_to_convert)
     date_to_filte = datetime.datetime.today().strftime('%Y/%m/%d')
     list_new_warrants = get_new_warrant_list()
 
     dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
```

### Comparing `mypylib-0.2.0/mypylib.egg-info/SOURCES.txt` & `mypylib-0.2.1/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.0/setup.py` & `mypylib-0.2.1/setup.py`

 * *Files identical despite different names*

