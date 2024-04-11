# Comparing `tmp/tokive-1.2.tar.gz` & `tmp/tokive-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokive-1.2.tar", last modified: Mon Apr  1 04:24:35 2024, max compression
+gzip compressed data, was "tokive-1.3.tar", last modified: Thu Apr 11 03:14:09 2024, max compression
```

## Comparing `tokive-1.2.tar` & `tokive-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:24:35.889798 tokive-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 04:24:35.889798 tokive-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 04:24:29.000000 tokive-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 04:24:35.889798 tokive-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-01 04:24:29.000000 tokive-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:24:35.885798 tokive-1.2/tokhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-01 04:24:29.000000 tokive-1.2/tokhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 04:24:29.000000 tokive-1.2/tokhelper/captchaCheck_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-01 04:24:29.000000 tokive-1.2/tokhelper/solve_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    58531 2024-04-01 04:24:29.000000 tokive-1.2/tokhelper/tiktok_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-01 04:24:29.000000 tokive-1.2/tokhelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-01 04:24:29.000000 tokive-1.2/tokive
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:24:35.889798 tokive-1.2/tokive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 04:24:35.000000 tokive-1.2/tokive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-01 04:24:35.000000 tokive-1.2/tokive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 04:24:35.000000 tokive-1.2/tokive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 04:24:35.000000 tokive-1.2/tokive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 04:24:35.000000 tokive-1.2/tokive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:14:09.129630 tokive-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-11 03:14:09.129630 tokive-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 03:14:03.000000 tokive-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:14:09.133630 tokive-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-11 03:14:03.000000 tokive-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:14:09.129630 tokive-1.3/tokhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 03:14:03.000000 tokive-1.3/tokhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 03:14:03.000000 tokive-1.3/tokhelper/captchaCheck_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-11 03:14:03.000000 tokive-1.3/tokhelper/solve_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58572 2024-04-11 03:14:03.000000 tokive-1.3/tokhelper/tiktok_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-11 03:14:03.000000 tokive-1.3/tokhelper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-11 03:14:03.000000 tokive-1.3/tokive
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:14:09.129630 tokive-1.3/tokive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-11 03:14:09.000000 tokive-1.3/tokive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 03:14:09.000000 tokive-1.3/tokive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:14:09.000000 tokive-1.3/tokive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 03:14:09.000000 tokive-1.3/tokive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 03:14:09.000000 tokive-1.3/tokive.egg-info/top_level.txt
```

### Comparing `tokive-1.2/setup.py` & `tokive-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='tokive',
-    version='1.2',
+    version='1.3',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of tokive",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/AutoWinTeam/tokive",
     packages=setuptools.find_packages(),
```

### Comparing `tokive-1.2/tokhelper/captchaCheck_pb2.py` & `tokive-1.3/tokhelper/captchaCheck_pb2.py`

 * *Files identical despite different names*

### Comparing `tokive-1.2/tokhelper/solve_captcha.py` & `tokive-1.3/tokhelper/solve_captcha.py`

 * *Files identical despite different names*

### Comparing `tokive-1.2/tokhelper/tiktok_main.py` & `tokive-1.3/tokhelper/tiktok_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -931,20 +931,21 @@
         domain=get_domain(acc)
         ping_url, ping_params, ping_headers, ping_data, ping_proxiex, ping_cookies = get_room_ping_info(
             acc, domain, room_id, stream_id)
         poll_url, poll_params, poll_headers, poll_data, poll_proxiex, poll_cookies = get_room_poll_info(
             acc, domain, room_id)
         cnt_poll=3
         cnt_captcha=6
-        while True:
+        is_running=True
+        while is_running:
             cnt_poll+=1
             cnt_captcha+=1
             fp_ping(ping_url, ping_params, ping_cookies, ping_headers, ping_data, ping_proxiex)
             if cnt_poll>1:
-                fp_poll(poll_url, poll_params, poll_cookies, poll_headers, poll_data, poll_proxiex)
+                is_running=fp_poll(poll_url, poll_params, poll_cookies, poll_headers, poll_data, poll_proxiex)
                 cnt_poll=0
             if cnt_captcha>5:
                 fp_solve_captcha(acc, id, room_id, cookies, domain)
                 cnt_captcha=0
             time.sleep(5)
     except:
         traceback.print_exc()
```

### Comparing `tokive-1.2/tokhelper/utils.py` & `tokive-1.3/tokhelper/utils.py`

 * *Files identical despite different names*

### Comparing `tokive-1.2/tokive` & `tokive-1.3/tokive`

 * *Files identical despite different names*

