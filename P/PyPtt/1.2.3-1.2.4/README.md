# Comparing `tmp/PyPtt-1.2.3.tar.gz` & `tmp/PyPtt-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPtt-1.2.3.tar", last modified: Sun Mar 31 03:53:59 2024, max compression
+gzip compressed data, was "PyPtt-1.2.4.tar", last modified: Thu Apr 11 03:41:55 2024, max compression
```

## Comparing `PyPtt-1.2.3.tar` & `PyPtt-1.2.4.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:53:59.609747 PyPtt-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-31 03:53:51.000000 PyPtt-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-31 03:53:51.000000 PyPtt-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-31 03:53:59.609747 PyPtt-1.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:53:59.605747 PyPtt-1.2.3/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (127)    32091 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-31 03:53:59.000000 PyPtt-1.2.3/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    21201 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:53:59.605747 PyPtt-1.2.3/PyPtt/lang/
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/lang/en_US.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/lang/zh_TW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    55000 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-03-31 03:53:51.000000 PyPtt-1.2.3/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 03:53:59.609747 PyPtt-1.2.3/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-31 03:53:59.000000 PyPtt-1.2.3/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-31 03:53:59.000000 PyPtt-1.2.3/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 03:53:59.000000 PyPtt-1.2.3/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 03:53:59.000000 PyPtt-1.2.3/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 03:53:59.000000 PyPtt-1.2.3/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-31 03:53:51.000000 PyPtt-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 03:53:59.609747 PyPtt-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-31 03:53:51.000000 PyPtt-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:41:55.721691 PyPtt-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-11 03:41:50.000000 PyPtt-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 03:41:50.000000 PyPtt-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-11 03:41:55.721691 PyPtt-1.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:41:55.717691 PyPtt-1.2.4/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    32091 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-11 03:41:55.000000 PyPtt-1.2.4/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:41:55.721691 PyPtt-1.2.4/PyPtt/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/lang/en_US.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/lang/zh_TW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:41:55.721691 PyPtt-1.2.4/PyPtt/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/ssl/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-11 03:41:50.000000 PyPtt-1.2.4/PyPtt/ssl/key.pem
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:41:55.721691 PyPtt-1.2.4/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-11 03:41:55.000000 PyPtt-1.2.4/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 03:41:55.000000 PyPtt-1.2.4/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:41:55.000000 PyPtt-1.2.4/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 03:41:55.000000 PyPtt-1.2.4/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 03:41:55.000000 PyPtt-1.2.4/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-11 03:41:50.000000 PyPtt-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:41:55.721691 PyPtt-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-11 03:41:50.000000 PyPtt-1.2.4/setup.py
```

### Comparing `PyPtt-1.2.3/LICENSE` & `PyPtt-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PKG-INFO` & `PyPtt-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.3
+Version: 1.2.4
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.2.3/PyPtt/PTT.py` & `PyPtt-1.2.4/PyPtt/PTT.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_bucket.py` & `PyPtt-1.2.4/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_call_status.py` & `PyPtt-1.2.4/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_change_pw.py` & `PyPtt-1.2.4/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_comment.py` & `PyPtt-1.2.4/PyPtt/_api_comment.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_del_post.py` & `PyPtt-1.2.4/PyPtt/_api_del_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_board_info.py` & `PyPtt-1.2.4/PyPtt/_api_get_board_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # print('nuser', nuser)
     # print('------------------------')
     if '[靜]' in nuser:
         online_user = 0
     else:
         if '編號' not in nuser or '人氣' not in nuser:
             raise exceptions.NoSuchBoard(api.config, board)
-        pattern = re.compile('[\d]+')
+        pattern = re.compile(r'[\d]+')
         r = pattern.search(nuser)
         if r is None:
             raise exceptions.NoSuchBoard(api.config, board)
         # 減一是把自己本身拿掉
         online_user = int(r.group(0)) - 1
 
     logger.debug('人氣', online_user)
@@ -70,31 +70,31 @@
     api.connect_core.send(
         'i',
         target_list)
 
     ori_screen = api.connect_core.get_screen_queue()[-1]
     # print(ori_screen)
 
-    p = re.compile('《(.+)》看板設定')
+    p = re.compile(r'《(.+)》看板設定')
     r = p.search(ori_screen)
     if r is not None:
         boardname = r.group(0)[1:-5].strip()
 
     logger.debug('看板名稱', boardname, board)
 
     if boardname.lower() != board.lower():
         raise exceptions.NoSuchBoard(api.config, board)
 
-    p = re.compile('中文敘述: (.+)')
+    p = re.compile(r'中文敘述: (.+)')
     r = p.search(ori_screen)
     if r is not None:
         chinese_des = r.group(0)[5:].strip()
     logger.debug('中文敘述', chinese_des)
 
-    p = re.compile('板主名單: (.+)')
+    p = re.compile(r'板主名單: (.+)')
     r = p.search(ori_screen)
     if r is not None:
         moderator_line = r.group(0)[5:].strip()
         if '(無)' in moderator_line:
             moderators = []
         else:
             moderators = moderator_line.split('/')
@@ -127,15 +127,15 @@
     # 限制 快速連推文章, 最低間隔時間: 5 秒
     # 開放 快速連推文章
 
     fast_push = ('開放 快速連推文章' in ori_screen)
     logger.debug('快速連推文章', fast_push)
 
     if not fast_push:
-        p = re.compile('最低間隔時間: [\d]+')
+        p = re.compile(r'最低間隔時間: [\d]+')
         r = p.search(ori_screen)
         if r is not None:
             min_interval = r.group(0)[7:].strip()
             min_interval = int(min_interval)
         else:
             min_interval = 0
         logger.debug('最低間隔時間', min_interval)
@@ -162,24 +162,24 @@
 
     cool_mode = ('未 設為冷靜模式' not in ori_screen)
     logger.debug('冷靜模式', cool_mode)
 
     require18 = ('禁止 未滿十八歲進入' in ori_screen)
     logger.debug('禁止未滿十八歲進入', require18)
 
-    p = re.compile('登入次數 [\d]+ 次以上')
+    p = re.compile(r'登入次數 [\d]+ 次以上')
     r = p.search(ori_screen)
     if r is not None:
         require_login_time = r.group(0).split(' ')[1]
         require_login_time = int(require_login_time)
     else:
         require_login_time = 0
     logger.debug('發文限制登入次數', require_login_time)
 
-    p = re.compile('退文篇數 [\d]+ 篇以下')
+    p = re.compile(r'退文篇數 [\d]+ 篇以下')
     r = p.search(ori_screen)
     if r is not None:
         require_illegal_post = r.group(0).split(' ')[1]
         require_illegal_post = int(require_illegal_post)
     else:
         require_illegal_post = 0
     logger.debug('發文限制退文篇數', require_illegal_post)
@@ -208,15 +208,15 @@
             # no post permission
 
         ori_screen = api.connect_core.get_screen_queue()[-1]
         screen_lines = ori_screen.split('\n')
 
         for i in screen_lines:
             if '種類：' in i:
-                type_pattern = re.compile('\d\.([^\ ]*)')
+                type_pattern = re.compile(r'\d\.([^\ ]*)')
                 # 0 is not present any type that the key hold None object
                 kind_list = type_pattern.findall(i)
                 break
 
         # Clear post status
         cmd_list = []
         cmd_list.append(command.ctrl_c)
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_board_list.py` & `PyPtt-1.2.4/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_bottom_post_list.py` & `PyPtt-1.2.4/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_favourite_board.py` & `PyPtt-1.2.4/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_newest_index.py` & `PyPtt-1.2.4/PyPtt/_api_get_newest_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         ]
 
         def get_index(api):
             current_capacity, _ = _api_util.get_mailbox_capacity(api)
             last_screen = api.connect_core.get_screen_queue()[-1]
             cursor_line = [x for x in last_screen.split('\n') if x.strip().startswith(api.cursor)][0]
 
-            list_index = int(re.compile('(\d+)').search(cursor_line).group(0))
+            list_index = int(re.compile(r'(\d+)').search(cursor_line).group(0))
 
             if search_type == 0 and search_list is None:
                 if list_index > current_capacity:
                     newest_index = list_index
                 else:
                     newest_index = current_capacity
             else:
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_post.py` & `PyPtt-1.2.4/PyPtt/_api_get_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,28 +161,28 @@
 
         if len(cursor_line) != 1:
             raise exceptions.UnknownError(ori_screen)
 
         cursor_line = cursor_line[0]
         log.logger.debug('CursorLine', cursor_line)
 
-        pattern = re.compile('[\d]+\/[\d]+')
+        pattern = re.compile(r'[\d]+\/[\d]+')
         pattern_result = pattern.search(cursor_line)
         if pattern_result is None:
             list_date = None
         else:
             list_date = pattern_result.group(0)
             list_date = list_date[-5:]
 
-        pattern = re.compile('\[[\w]+\]')
+        pattern = re.compile(r'\[[\w]+\]')
         pattern_result = pattern.search(cursor_line)
         if pattern_result is not None:
             post_del_status = data_type.PostStatus.DELETED_BY_AUTHOR
         else:
-            pattern = re.compile('<[\w]+>')
+            pattern = re.compile(r'<[\w]+>')
             pattern_result = pattern.search(cursor_line)
             post_del_status = data_type.PostStatus.DELETED_BY_MODERATOR
 
         # > 79843     9/11 -             □ (本文已被吃掉)<
         # > 76060     8/28 -             □ (本文已被刪除) [weida7332]
         # print(f'O=>{CursorLine}<')
         if pattern_result is not None:
@@ -258,17 +258,17 @@
             PostField.has_control_code: has_control_code,
             PostField.pass_format_check: False,
             PostField.push_number: push_number,
             PostField.is_unconfirmed: api.Unconfirmed
         })
         return post
 
-    post_author_pattern_new = re.compile('作者  (.+) 看板')
-    post_author_pattern_old = re.compile('作者  (.+)')
-    board_pattern = re.compile('看板  (.+)')
+    post_author_pattern_new = re.compile(r'作者  (.+) 看板')
+    post_author_pattern_old = re.compile(r'作者  (.+)')
+    board_pattern = re.compile(r'看板  (.+)')
 
     post_date = None
     post_content = None
     ip = None
     location = None
     push_list = []
 
@@ -319,15 +319,15 @@
             return post
         post_author = pattern_result.group(0)
         post_author = post_author[:post_author.rfind(')') + 1]
     post_author = post_author[4:].strip()
 
     log.logger.debug(i18n.author, post_author)
 
-    post_title_pattern = re.compile('標題  (.+)')
+    post_title_pattern = re.compile(r'標題  (.+)')
 
     title_line = origin_post_lines[1]
     pattern_result = post_title_pattern.search(title_line)
     if pattern_result is None:
         log.logger.info(i18n.substandard_post, i18n.title)
 
         post.update({
@@ -352,15 +352,15 @@
 
         return post
     post_title = pattern_result.group(0)
     post_title = post_title[4:].strip()
 
     log.logger.debug(i18n.title, post_title)
 
-    post_date_pattern = re.compile('時間  .{24}')
+    post_date_pattern = re.compile(r'時間  .{24}')
     date_line = origin_post_lines[2]
     pattern_result = post_date_pattern.search(date_line)
     if pattern_result is None:
         log.logger.info(i18n.substandard_post, i18n.date)
 
         post.update({
             PostField.board: board,
@@ -435,16 +435,16 @@
 
         return post
 
     log.logger.debug(i18n.content, post_content)
 
     info_lines = [line for line in origin_post_lines if line.startswith('※') or line.startswith('◆')]
 
-    pattern = re.compile('[\d]+\.[\d]+\.[\d]+\.[\d]+')
-    pattern_p2 = re.compile('[\d]+-[\d]+-[\d]+-[\d]+')
+    pattern = re.compile(r'[\d]+\.[\d]+\.[\d]+\.[\d]+')
+    pattern_p2 = re.compile(r'[\d]+-[\d]+-[\d]+-[\d]+')
     for line in reversed(info_lines):
 
         log.logger.debug('IP Line', line)
 
         # type 1
         # ※ 編輯: CodingMan (111.243.146.98 臺灣)
         # ※ 發信站: 批踢踢實業坊(ptt.cc), 來自: 111.243.146.98 (臺灣)
@@ -502,17 +502,17 @@
                 PostField.push_number: push_number,
                 PostField.full_content: origin_post,
                 PostField.is_unconfirmed: api.Unconfirmed, })
 
             return post
     log.logger.debug('IP', ip)
 
-    push_author_pattern = re.compile('[推|噓|→] [\w| ]+:')
-    push_date_pattern = re.compile('[\d]+/[\d]+ [\d]+:[\d]+')
-    push_ip_pattern = re.compile('[\d]+\.[\d]+\.[\d]+\.[\d]+')
+    push_author_pattern = re.compile(r'[推|噓|→] [\w| ]+:')
+    push_date_pattern = re.compile(r'[\d]+/[\d]+ [\d]+:[\d]+')
+    push_ip_pattern = re.compile(r'[\d]+\.[\d]+\.[\d]+\.[\d]+')
 
     push_list = []
 
     for line in origin_post_lines:
         if line.startswith('推'):
             comment_type = data_type.CommentType.PUSH
         elif line.startswith('噓 '):
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_post_index.py` & `PyPtt-1.2.4/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_time.py` & `PyPtt-1.2.4/PyPtt/_api_get_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from . import command
 from . import connect_core
 from . import exceptions
 from . import i18n
 from . import log
 from . import screens
 
-pattern = re.compile('[\d]+:[\d][\d]')
+pattern = re.compile(r'[\d]+:[\d][\d]')
 
 
 def get_time(api) -> str:
     _api_util.one_thread(api)
     if not api._is_login:
         raise exceptions.RequireLogin(i18n.require_login)
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_get_user.py` & `PyPtt-1.2.4/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_give_money.py` & `PyPtt-1.2.4/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_has_new_mail.py` & `PyPtt-1.2.4/PyPtt/_api_has_new_mail.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     cmd_list.append(command.ctrl_z)
     cmd_list.append('m')
     # cmd_list.append('1')
     # cmd_list.append(command.enter)
     cmd = ''.join(cmd_list)
     current_capacity = None
     plus_count = 0
-    index_pattern = re.compile('(\d+)')
+    index_pattern = re.compile(r'(\d+)')
     checked_index_list = []
     break_detect = False
 
     target_list = [
         connect_core.TargetUnit(screens.Target.InMailBox, log_level=log.DEBUG, break_detect=True)
     ]
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_loginout.py` & `PyPtt-1.2.4/PyPtt/_api_loginout.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     #     log.log(
     #         api.config,
     #         LogLevel.INFO,
     #         i18n.MailBoxFull)
     #     api.is_mailbox_full = True
 
     def register_processing(screen):
-        pattern = re.compile('[\d]+')
+        pattern = re.compile(r'[\d]+')
         api.process_picks = int(pattern.search(screen).group(0))
 
     if len(ptt_pw) > 8:
         ptt_pw = ptt_pw[:8]
 
     ptt_id = ptt_id.strip()
     ptt_pw = ptt_pw.strip()
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_mail.py` & `PyPtt-1.2.4/PyPtt/_api_mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,18 @@
 # --
 # ※ 發信站: 批踢踢實業坊(ptt.cc)
 # ◆ From: 220.142.14.95
 content_start = '───────────────────────────────────────'
 content_end = '--\n※ 發信站: 批踢踢實業坊(ptt.cc)'
 content_ip_old = '◆ From: '
 
-mail_author_pattern = re.compile('作者  (.+)')
-mail_title_pattern = re.compile('標題  (.+)')
-mail_date_pattern = re.compile('時間  (.+)')
-ip_pattern = re.compile('[\d]+\.[\d]+\.[\d]+\.[\d]+')
+mail_author_pattern = re.compile(r'作者  (.+)')
+mail_title_pattern = re.compile(r'標題  (.+)')
+mail_date_pattern = re.compile(r'時間  (.+)')
+ip_pattern = re.compile(r'[\d]+\.[\d]+\.[\d]+\.[\d]+')
 
 
 def get_mail(api, index: int, search_type: Optional[data_type.SearchType] = None,
              search_condition: Optional[str] = None,
              search_list: Optional[list] = None) -> Dict:
     _api_util.one_thread(api)
```

### Comparing `PyPtt-1.2.3/PyPtt/_api_mark_post.py` & `PyPtt-1.2.4/PyPtt/_api_mark_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_post.py` & `PyPtt-1.2.4/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_reply_post.py` & `PyPtt-1.2.4/PyPtt/_api_reply_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_search_user.py` & `PyPtt-1.2.4/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_set_board_title.py` & `PyPtt-1.2.4/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/_api_util.py` & `PyPtt-1.2.4/PyPtt/_api_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         connect_core.TargetUnit(screens.Target.InPost, log_level=log.DEBUG, break_detect=True),
         connect_core.TargetUnit(screens.Target.PostNoContent, log_level=log.DEBUG, break_detect=True),
         # 動畫文章
         connect_core.TargetUnit(screens.Target.Animation, response=command.go_main_menu_type_q,
                                 break_detect_after_send=True),
     ]
 
-    line_from_pattern = re.compile('[\d]+~[\d]+')
+    line_from_pattern = re.compile(r'[\d]+~[\d]+')
 
     has_control_code = False
     control_code_mode = False
     push_start = False
     content_start_exist = False
     content_start_jump = False
     content_start_jump_set = False
@@ -188,15 +188,15 @@
         return mail_capacity
 
     last_screen = api.connect_core.get_screen_queue()[-1]
     capacity_line = last_screen.split('\n')[2]
 
     log.logger.debug('capacity_line', capacity_line)
 
-    pattern_result = re.compile('(\d+)/(\d+)').search(capacity_line)
+    pattern_result = re.compile(r'(\d+)/(\d+)').search(capacity_line)
     if pattern_result is not None:
         current_capacity = int(pattern_result.group(0).split('/')[0])
         max_capacity = int(pattern_result.group(0).split('/')[1])
 
         log.logger.debug('current_capacity', current_capacity)
         log.logger.debug('max_capacity', max_capacity)
 
@@ -250,51 +250,51 @@
 
     aid_line = [line for line in ori_screen.split(
         '\n') if line.startswith('│ 文章代碼(AID)')]
 
     post_aid = None
     if len(aid_line) == 1:
         aid_line = aid_line[0]
-        pattern = re.compile('#[\w|-]+')
+        pattern = re.compile(r'#[\w|-]+')
         pattern_result = pattern.search(aid_line)
         post_aid = pattern_result.group(0)[1:]
 
-    pattern = re.compile('文章網址: https:[\S]+html')
+    pattern = re.compile(r'文章網址: https:[\S]+html')
     pattern_result = pattern.search(ori_screen_temp)
 
     if pattern_result is None:
         post_web = None
     else:
         post_web = pattern_result.group(0)[6:]
 
-    pattern = re.compile('這一篇文章值 [\d]+ Ptt幣')
+    pattern = re.compile(r'這一篇文章值 [\d]+ Ptt幣')
     pattern_result = pattern.search(ori_screen_temp)
     if pattern_result is None:
         # 特殊文章無價格
         post_money = -1
     else:
         post_money = pattern_result.group(0)[7:]
         post_money = post_money[:post_money.find(' ')]
         post_money = int(post_money)
 
-    pattern = re.compile('[\d]+\/[\d]+')
+    pattern = re.compile(r'[\d]+\/[\d]+')
     pattern_result = pattern.search(cursor_line)
     if pattern_result is None:
         list_date = None
     else:
         list_date = pattern_result.group(0)
         list_date = list_date[-5:]
     # print(list_date)
 
     # >  7485   9 8/09 CodingMan    □ [閒聊] PTT Library 更新
     # > 79189 M 1 9/17 LittleCalf   □ [公告] 禁言退文公告
     # >781508 +爆 9/17 jodojeda     □ [新聞] 國人吃魚少 學者：應把吃魚當成輕鬆愉快
     # >781406 +X1 9/17 kingofage111 R: [申請] ReDmango 請辭Gossiping板主職務
 
-    pattern = re.compile('[\d]+')
+    pattern = re.compile(r'[\d]+')
     pattern_result = pattern.search(cursor_line)
     post_index = 0
     if pattern_result is not None:
         post_index = int(pattern_result.group(0))
 
     push_number = cursor_line
     push_number = push_number[7:11]
```

### Comparing `PyPtt-1.2.3/PyPtt/check_value.py` & `PyPtt-1.2.4/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/command.py` & `PyPtt-1.2.4/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/config.py` & `PyPtt-1.2.4/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/connect_core.py` & `PyPtt-1.2.4/PyPtt/connect_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import os.path
 import ssl
 import telnetlib
 import threading
 import time
 import traceback
 import warnings
 from typing import Any
@@ -19,15 +20,19 @@
 from . import exceptions
 from . import i18n
 from . import log
 from . import screens
 
 websockets.http.USER_AGENT += f' PyPtt/{PyPtt.__version__}'
 
+_script_path = os.path.dirname(os.path.abspath(__file__))
+
 ssl_context = ssl.create_default_context()
+ssl_context.load_cert_chain(certfile=f"{_script_path}/ssl/cert.pem", keyfile=f"{_script_path}/ssl/key.pem")
+ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
 
 
 class TargetUnit:
     def __init__(self, detect_target, log_level: log.LogLevel = None, response: [Any | str] = '', break_detect=False,
                  break_detect_after_send=False, exceptions_=None, refresh=True, secret=False, handler=None,
                  max_match: int = 0):
```

### Comparing `PyPtt-1.2.3/PyPtt/data_type.py` & `PyPtt-1.2.4/PyPtt/data_type.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/exceptions.py` & `PyPtt-1.2.4/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/i18n.py` & `PyPtt-1.2.4/PyPtt/i18n.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/lang/en_US.yaml` & `PyPtt-1.2.4/PyPtt/lang/en_US.yaml`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/lang/zh_TW.yaml` & `PyPtt-1.2.4/PyPtt/lang/zh_TW.yaml`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/lib_util.py` & `PyPtt-1.2.4/PyPtt/lib_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 def get_aid_from_url(url: str) -> Tuple[str, str]:
     # 檢查是否為字串
     check_value.check_type(url, str, 'url')
 
     # 檢查是否符合 PTT BOARD 文章網址格式
-    pattern = re.compile('https://www.ptt.cc/bbs/[-.\w]+/M.[\d]+.A[.\w]*.html')
+    pattern = re.compile(r'https://www.ptt.cc/bbs/[-.\w]+/M.[\d]+.A[.\w]*.html')
     r = pattern.search(url)
     if r is None:
         raise ValueError('wrong parameter url must be www.ptt.cc post url')
 
     board = url[23:]
     board = board[:board.find('/')]
```

### Comparing `PyPtt-1.2.3/PyPtt/log.py` & `PyPtt-1.2.4/PyPtt/log.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt/screens.py` & `PyPtt-1.2.4/PyPtt/screens.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,16 +187,16 @@
 
         print('len:' + str(len(screen_queue)))
     if function_name is not None:
         print('錯誤在 ' + function_name + ' 函式發生')
     print('-' * 50)
 
 
-xy_pattern_h = re.compile('^=ESC=\[[\d]+;[\d]+H')
-xy_pattern_s = re.compile('^=ESC=\[[\d]+;[\d]+s')
+xy_pattern_h = re.compile(r'^=ESC=\[[\d]+;[\d]+H')
+xy_pattern_s = re.compile(r'^=ESC=\[[\d]+;[\d]+s')
 
 
 class VT100Parser:
     def _h(self):
         self._cursor_x = 0
         self._cursor_y = 0
 
@@ -226,26 +226,20 @@
         self._cursor_y = 0
         self.screen = [''] * 24
         self.screen_length = dict()
 
         data = bytes_data.decode(encoding, errors='replace')
 
         # remove color
-        data = re.sub('\x1B\[[\d+;]*m', '', data)
+        data = re.sub(r'\x1B\[[\d+;]*m', '', data)
         data = re.sub(r'[\x1B]', '=ESC=', data)
         data = re.sub(r'[\r]', '', data)
         while ' \x08' in data:
             data = re.sub(r' \x08', '', data)
 
-        # print('---' * 8)
-        # print(encoding)
-        # print(bytes_data)
-        # print(data)
-        # print('---' * 8)
-
         if '=ESC=[2J' in data:
             data = data[data.rfind('=ESC=[2J') + len('=ESC=[2J'):]
 
         count = 0
         while data:
             count += 1
             while True:
```

### Comparing `PyPtt-1.2.3/PyPtt/service.py` & `PyPtt-1.2.4/PyPtt/service.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/PyPtt.egg-info/PKG-INFO` & `PyPtt-1.2.4/PyPtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.3
+Version: 1.2.4
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.2.3/PyPtt.egg-info/SOURCES.txt` & `PyPtt-1.2.4/PyPtt.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -41,8 +41,10 @@
 PyPtt/service.py
 PyPtt.egg-info/PKG-INFO
 PyPtt.egg-info/SOURCES.txt
 PyPtt.egg-info/dependency_links.txt
 PyPtt.egg-info/requires.txt
 PyPtt.egg-info/top_level.txt
 PyPtt/lang/en_US.yaml
-PyPtt/lang/zh_TW.yaml
+PyPtt/lang/zh_TW.yaml
+PyPtt/ssl/cert.pem
+PyPtt/ssl/key.pem
```

### Comparing `PyPtt-1.2.3/README.md` & `PyPtt-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.3/setup.py` & `PyPtt-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,10 +119,13 @@
         'websockets',
         'uao',
         'requests',
         'AutoStrEnum',
         'PyYAML',
     ],
     package_data={
-        'PyPtt': ['lang/*.yaml'],
+        'PyPtt': [
+            'lang/*.yaml',
+            'ssl/*.pem',
+        ],
     }
 )
```

