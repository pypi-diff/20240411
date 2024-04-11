# Comparing `tmp/luoguapi-0.1.0.tar.gz` & `tmp/luoguapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luoguapi-0.1.0.tar", last modified: Thu Apr 11 09:26:32 2024, max compression
+gzip compressed data, was "luoguapi-0.1.1.tar", last modified: Thu Apr 11 13:29:43 2024, max compression
```

## Comparing `luoguapi-0.1.0.tar` & `luoguapi-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:26:32.556162 luoguapi-0.1.0/
--rw-rw-rw-   0        0        0    35757 2024-04-11 09:20:08.000000 luoguapi-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      182 2024-04-11 09:26:32.556162 luoguapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      152 2024-04-11 09:17:54.000000 luoguapi-0.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-11 09:26:32.556162 luoguapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      215 2024-04-11 09:23:50.000000 luoguapi-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:26:32.550251 luoguapi-0.1.0/src/
--rw-rw-rw-   0        0        0       17 2024-04-11 09:24:57.000000 luoguapi-0.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:26:32.555771 luoguapi-0.1.0/src/luoguapi.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-11 09:26:32.000000 luoguapi-0.1.0/src/luoguapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-11 09:26:32.000000 luoguapi-0.1.0/src/luoguapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:26:32.000000 luoguapi-0.1.0/src/luoguapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 09:26:32.000000 luoguapi-0.1.0/src/luoguapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8723 2024-04-11 09:12:42.000000 luoguapi-0.1.0/src/luoguapi.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:29:43.754102 luoguapi-0.1.1/
+-rw-rw-rw-   0        0        0    35757 2024-04-11 13:18:58.000000 luoguapi-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      182 2024-04-11 13:29:43.751537 luoguapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2024-04-11 13:18:58.000000 luoguapi-0.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:29:43.755102 luoguapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      215 2024-04-11 13:29:36.000000 luoguapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:29:43.718003 luoguapi-0.1.1/src/
+-rw-rw-rw-   0        0        0       17 2024-04-11 13:18:58.000000 luoguapi-0.1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:29:43.749537 luoguapi-0.1.1/src/luoguapi.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 13:29:43.000000 luoguapi-0.1.1/src/luoguapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8669 2024-04-11 13:28:11.000000 luoguapi-0.1.1/src/luoguapi.py
```

### Comparing `luoguapi-0.1.0/LICENSE.txt` & `luoguapi-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `luoguapi-0.1.0/src/luoguapi.py` & `luoguapi-0.1.1/src/luoguapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 
 def ocr(img: list):
     return requests.post(
         "http://ocr.api.codingoier.work/ocr/file", files={'image': img}).text
 
 
 class session:
+    '''
+    洛谷用户会话
+    '''
 
     def __init__(self):
         self.uid = ''
         self.client = ''
         self.cookie = ''
         self.user = self.user(self)
         self.problem = self.problem(self)
@@ -138,20 +141,18 @@
             尝试使用账号密码登录
             @arg uid: 用户 uid
             @arg passwd: 用户密码
             @return 如果登录成功返回 [True, username] ，登录失败（验证码错误自动重试）后 [False, <Username Or Password Wrong>]
             '''
             self.loginCookie('0', self.makeCookie())
             res = ocr(self.getCaptcha())
-            print(f'Try {res}')
             url = 'https://www.luogu.com.cn/do-auth/password'
-            h = self.session.getHeaders(
-                'https://www.luogu.com.cn/auth/login')
-            response = requests.post(url=url, headers=h, json={
-                                     "username": uid, "password": passwd, "captcha": res})
+            response = requests.post(url=url, headers=self.session.getHeaders(
+                'https://www.luogu.com.cn/auth/login'), json={
+                "username": uid, "password": passwd, "captcha": res})
             if response.status_code == 200:
                 temp = json.loads(response.text)
                 self.loginCookie(uid, self.session.client)
                 return [True, temp['username']]
             else:
                 temp = json.loads(response.text)
                 if (temp['errorType'] == 'LuoguWeb\\Spilopelia\\Exception\\CaptchaNotMatchException'):
@@ -228,16 +229,15 @@
         def solution(self, uid: str):
             '''
             获取指定题目的题解
             @arg uid: 题目编号
             @return 如果成功获取返回 [True, <题解 json 格式数据>], 失败返回原因 [False, <Problem Not Found>]
             '''
             url = f'https://www.luogu.com.cn/problem/solution/{uid}'
-            h = self.session.getHeaders(url)
-            print(h)
-            response = requests.get(url=url, headers=h)
+            response = requests.get(
+                url=url, headers=self.session.getHeaders(url))
             if response.status_code == 404:
                 return [False, 'Problem Not Found']
             response = rmd(
                 response.text, 'JSON.parse(decodeURIComponent("', '"));')
             response = urlDecode(response)
             return [True, response]
```

