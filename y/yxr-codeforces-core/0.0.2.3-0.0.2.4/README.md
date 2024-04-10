# Comparing `tmp/yxr_codeforces_core-0.0.2.3.tar.gz` & `tmp/yxr_codeforces_core-0.0.2.4.tar.gz`

## Comparing `yxr_codeforces_core-0.0.2.3.tar` & `yxr_codeforces_core-0.0.2.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/__init__.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/account.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/constants.py
--rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/contest_list.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/contest_meta.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/contest_register.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/contest_standing.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/httphelper.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/kwargs.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/language.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/logging.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/problem.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/problems.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/py.typed
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/submit.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/url.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/util.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/websocket.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/interfaces/AioHttpHelper.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/codeforces_core/interfaces/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/LICENSE
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/README.md
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/__init__.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/account.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/constants.py
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/contest_list.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/contest_meta.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/contest_register.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/contest_standing.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/httphelper.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/kwargs.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/language.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/logging.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/problem.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/problems.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/py.typed
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/settings.py
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/submit.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/url.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/util.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/websocket.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/interfaces/AioHttpHelper.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/codeforces_core/interfaces/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/LICENSE
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/README.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.4/PKG-INFO
```

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/account.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple
 from random import choice
 from lxml import html
 from lxml.html import HtmlElement
 import logging
 
+from codeforces_core.constants import CF_HOST
+
 from .kwargs import extract_common_kwargs
-from .util import typedxpath
+from .util import calc_tta, typedxpath
 from .interfaces.AioHttpHelper import AioHttpHelperInterface
 
 default_login_url = "/enter?back=%2F"
 
 
 @dataclass
 class LoginResult:
@@ -114,22 +116,26 @@
           await http.close_session()
 
         asyncio.run(demo())
   """
   logger = extract_common_kwargs(**kw).logger
   html_data = await http.async_get(login_url)
   csrf_token, ftaa, bfaa = extract_channel(html_data, logger=logger)[4:7]
+
+  _39ce7 = http.get_cookie(CF_HOST,'39ce7')
+  _tta = calc_tta(_39ce7)
   login_data = {
       'csrf_token': csrf_token,
       'action': 'enter',
       'ftaa': ftaa,
       'bfaa': bfaa,
       'handleOrEmail': handle,
       'password': password,
       'remember': 'on',
+      '_tta':_tta,
   }
   html_data = await http.async_post(login_url, login_data)
   # uc, usmc, cc, pc, csrf_token, ftaa, bfaa = extract_channel(html_data)
   uc, usmc, cc, pc = extract_channel(html_data, logger=logger)[0:4]
 
   success = False
   # if check_login(result.html):
```

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/contest_list.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/contest_list.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/contest_meta.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/contest_meta.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/contest_register.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/contest_register.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,18 +58,18 @@
   url = f'/contestRegistration/{contest_id}'
   resp = await http.async_get(url)
   doc = html.fromstring(resp)
   title = cast(List[_Element], doc.xpath('.//title'))[0].text
   msg = util.show_message(resp)  # AlreadyRegistered
   if msg:
     return RegisterResult(title=title, msg=msg)
-  token = http.get_tokens()
+  tokens = http.get_tokens()
   resp = await http.async_post(
       url,
       data=http.create_form({
-          'csrf_token': token['csrf'],
+          'csrf_token': tokens['csrf'],
           'action': 'formSubmitted',
           'takePartAs': 'personal',  # Take part as individual participant
           'backUrl': '',
       }))
   msg = util.show_message(resp)  # HaveBeenRegistered
   return RegisterResult(title=title, msg=msg)
```

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/contest_standing.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/contest_standing.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/httphelper.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/httphelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, AsyncIterator, Callable, Dict, List, Optional, Tuple, cast
+from typing import Any, AsyncIterator, Callable, Dict, List, Optional, Tuple, Union, cast
 from lxml import html
 from lxml.etree import _Element
 from os import path
 import asyncio
 import aiohttp
 import pyaes
 import json
@@ -14,15 +14,15 @@
 from .kwargs import extract_common_kwargs
 
 default_headers = {
     'Accept': '*/*',
     'Accept-Encoding': 'gzip',
     # 'User-Agent': config.conf['user_agent'], TODO
     'User-Agent':
-    'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36'
+    'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36',
 }
 
 
 class RCPCRedirectionError(Exception):
 
   def __init__(self):
     super().__init__("RCPC redirection detected")
@@ -30,16 +30,21 @@
 
 def add_header(newhdr, headers: Dict[str, str]) -> Dict[str, str]:
   headers.update(newhdr)
   return headers
 
 
 async def on_request_end(session, trace_request_ctx, params):
-  elapsed = asyncio.get_event_loop().time() - trace_request_ctx.start
-  print("[*] Request end : {}".format(elapsed))
+  # https://stackoverflow.com/questions/54185775/dumping-the-request-headers-with-aiohttp
+  # print("Ending %s request for %s. I sent: %s" % (params.method, params.url, params.headers))
+  # print('Sent headers: %s' % params.response.request_info.headers)
+
+  # elapsed = asyncio.get_event_loop().time() - trace_request_ctx.start
+  # print("[*] Request end : {}".format(elapsed))
+  pass
 
 
 class HttpHelper(AioHttpHelperInterface):
   session: Optional[aiohttp.ClientSession] = None
   cookie_jar_path = ''
   cookie_jar: Optional[aiohttp.CookieJar] = None
   token_path = ''
@@ -78,15 +83,19 @@
       else:
         jar.save(file_path=cookie_jar_path)
     return jar
 
   async def open_session(self) -> aiohttp.ClientSession:
     self.cookie_jar = HttpHelper.load_cookie_jar(self.cookie_jar_path)
     self.tokens = HttpHelper.load_tokens(self.token_path)
-    self.session = await aiohttp.ClientSession(cookie_jar=self.cookie_jar).__aenter__()
+
+    trace_config = aiohttp.TraceConfig()
+    trace_config.on_request_end.append(on_request_end)
+
+    self.session = await aiohttp.ClientSession(cookie_jar=self.cookie_jar,trace_configs=[trace_config]).__aenter__()
     return self.session
 
   async def close_session(self) -> None:
     await self.session.__aexit__(None, None, None)
     self.tokens = {}
     self.cookie_jar = None
     self.session = None
@@ -121,39 +130,54 @@
         return await response.text()
     except Exception as e:
       self.logger.error(e)
 
   async def async_post(self, url, data, headers=default_headers, csrf=False, **kwargs: Any):
     if self.session is None:
       raise Exception('Please open_session() before async_get()')
-    if headers == None: headers = default_headers
+    if headers is None: headers = default_headers
     if csrf and 'csrf' in self.tokens:
       headers = add_header({'X-Csrf-Token': self.tokens['csrf']}, headers=headers)
-
+      
     # TODO remove the feature
     if url.startswith('/'): url = self.host + url
     try:
       async with self.session.post(url, headers=headers, data=data, **kwargs) as response:
+        if response.status != 200:
+          self.logger.error('resp:' + str(response))
         assert response.status == 200
         self.check_rcpc(await response.text())
         if self.cookie_jar_path:
           self.cookie_jar.save(file_path=self.cookie_jar_path)
         return await response.text()
     except RCPCRedirectionError:
       async with self.session.post(url, headers=headers, data=data) as response:
         assert response.status == 200
         if self.cookie_jar_path:
           self.cookie_jar.save(file_path=self.cookie_jar_path)
         return await response.text()
     except Exception as e:
       self.logger.error(e)
 
-  def get_tokens(self):
+  def get_tokens(self) -> Dict[str,str]:
     return self.tokens
 
+  def get_cookie(self,host:str,key:str)-> Optional[str]:
+    d = self.cookie_jar.filter_cookies(host)
+    if self.cookie_jar:
+      try:
+        if not d:
+          return None
+        if key in d:
+          return d[key].value
+      except Exception as e:
+        self.logger.exception(e)
+        return None
+    return None
+
   def check_rcpc(self, html_data: str):
     doc = html.fromstring(html_data)
     aesmin = cast(List[_Element], doc.xpath(".//script[@type='text/javascript' and @src='/aes.min.js']"))
     if len(aesmin) > 0:
       print("[+] RCPC redirection detected")
       js = cast(List[_Element], doc.xpath(".//script[not(@type)]"))
       assert len(js) > 0
@@ -165,16 +189,17 @@
           iv = bytes.fromhex(k.split('"')[1])
         elif k[0] == 'c':
           ciphertext = bytes.fromhex(k.split('"')[1])
       assert len(key) == 16 and len(iv) == 16 and len(ciphertext) == 16, 'AES decryption error'
       c = pyaes.AESModeOfOperationCBC(key, iv=iv)
       plaintext = c.decrypt(ciphertext)
       rcpc = plaintext.hex()
-      self.cookie_jar.update_cookies({'RCPC': rcpc})
-      self.cookie_jar.save(file_path=self.cookie_jar_path)
+      if self.cookie_jar:
+        self.cookie_jar.update_cookies({'RCPC': rcpc})
+        self.cookie_jar.save(file_path=self.cookie_jar_path)
       raise RCPCRedirectionError()
 
   def create_form(self, form_data) -> aiohttp.FormData:
     form = aiohttp.FormData()
     for k, v in form_data.items():
       form.add_field(k, v)
     return form
```

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/language.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/language.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/logging.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/logging.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/problem.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/problem.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/problems.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/problems.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/submit.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/submit.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 async def async_submit(http: AioHttpHelperInterface, contest_id: str, level: str, file_path: str, lang_id: str,
                        **kw) -> Tuple[str, str]:
   """
     This method will use ``http`` to post submit
 
-    :param http: AioHttpHelperInterface 
-    :param ws_handler: function to handler messages 
+    :param http: AioHttpHelperInterface
+    :param ws_handler: function to handler messages
 
     :returns: (submission_id, html_text of contest/<contest id>/my )
 
     Examples:
 
     .. code-block::
 
@@ -72,27 +72,50 @@
       'ftaa': token['ftaa'],
       'bfaa': token['bfaa'],
       'action': 'submitSolutionFormSubmitted',
       'submittedProblemIndex': level,
       'programTypeId': lang_id,
   }
   url = '/contest/{}/problem/{}?csrf_token={}'.format(contest_id, level.upper(), token['csrf'])
+  # url = '/contest/{}/submit?csrf_token={}'.format(contest_id, token['csrf'])
   form = http.create_form(submit_form)
   form.add_field('sourceFile', open(file_path, 'rb'), filename=file_path)
+  logger.debug(f"{url},{submit_form}")
   resp = await http.async_post(url, form)  # 正常是 302 -> https://codeforces.com/contest/<contest id>/my
   if not is_user_logged_in(resp):
     logger.error("Login required")
     return '', resp
   doc = html.fromstring(resp)
+  # 重复提交
   for e in typedxpath(doc, './/span[@class="error for__sourceFile"]'):
     if e.text == 'You have submitted exactly the same code before':
       logger.error("[!] " + e.text)
       return '', resp
+  # 可能是 langid 不对!!
+  for e in typedxpath(doc, './/span[@class="error for__programTypeId"]'):
+    logger.error("[!] " + e.text)
+    if e.text == 'Choose valid language':
+        help_text = """
+            Language ID error:
+            Use `oi lang Codeforces` to check newest language id list
+            Use `oi config template list --detail` to check current <template name>
+            Use `oi config template modify Codeforces <template name> --langid <new lang id>` to update langid
+            Modify `lang_id` also in `state.json`: `sed -ie 's/"up_lang": "<old lang id>"/"up_lang": "<new lang id>"/g' state.json`
+        """
+        # TODO remove lang_id in state.json
+        logger.info(help_text)
+    return '', resp
+
+  submit_result_resp_analysed_arr = parse_submit_status(resp)
+  if len(submit_result_resp_analysed_arr) > 0:
+      status = parse_submit_status(resp)[0]
+  else:
+      logger.error("parse_submit_status error")
+      return '',''
 
-  status = parse_submit_status(resp)[0]
   assert status.url.split('/')[-1] == level.upper()
   return status.id, resp
 
 
 # TODO move oiterminal code to here use dataclass
 @dataclass
 class SubmissionPageResult:
@@ -129,15 +152,15 @@
   result = parse_submit_status(html_page)
   return list(filter(lambda o: o.url.endswith(problem_key), result))
 
 
 @dataclass
 class SubmissionWSResult:
   source: Any = field(default_factory=lambda: defaultdict(dict))
-  submit_id: int = 0
+  submit_id: int = 0 # 注意 这个ws返回的是int不是str
   contest_id: int = 0
   title: str = ''
   msg: str = ''
   passed: int = 0
   testcases: int = 0
   ms: int = 0
   mem: int = 0
```

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/url.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/url.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/websocket.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,12 +83,12 @@
   """
   logger = extract_common_kwargs(**kw).logger
   epoch = int(time() * 1000)  # s -> ms
   html_data = await http.async_get(f"/contest/{contest_id}/my")
   cc, pc = extract_channel(html_data, logger)[2:4]
   assert cc and pc
   ws_url = f"wss://pubsub.codeforces.com/ws/s_{pc}/s_{cc}?_={epoch}&tag=&time=&eventid="
-  logger.debug(f"pc = {pc}")  # 似乎和场次有关, 可能包含别人的?
-  logger.debug(f"cc = {cc}")  # 似乎只会包含自己的
+  logger.debug(f"pc = {pc}")  # 似乎只会包含自己的
+  logger.debug(f"cc = {cc}")  # 似乎和场次有关, 可能包含别人的?
   logger.debug(f"ws_url = {ws_url}")
   async for data in http.websockets(ws_url, ws_handler):
     yield data
```

### Comparing `yxr_codeforces_core-0.0.2.3/codeforces_core/interfaces/AioHttpHelper.py` & `yxr_codeforces_core-0.0.2.4/codeforces_core/interfaces/AioHttpHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod
-from typing import Any, Callable, Dict, Protocol, Tuple, AsyncIterator
+from typing import Any, Callable, Dict, Optional, Protocol, Tuple, AsyncIterator
 import aiohttp
 
 
 class AioHttpHelperInterface(Protocol):
 
   @abstractmethod
   def create_form(self, form_data: Dict[str, Any]) -> aiohttp.FormData:
@@ -22,15 +22,19 @@
     raise NotImplementedError
 
   @abstractmethod
   async def open_session(self) -> aiohttp.ClientSession:
     raise NotImplementedError
 
   @abstractmethod
-  def get_tokens(self) -> Any:
+  def get_tokens(self) -> Dict[str,str]:
+    raise NotImplementedError
+
+  @abstractmethod
+  def get_cookie(self,host:str,key:str)-> Optional[str]:
     raise NotImplementedError
 
   @abstractmethod
   async def close_session(self) -> None:
     raise NotImplementedError
 
   # TODO move call back out
```

### Comparing `yxr_codeforces_core-0.0.2.3/.gitignore` & `yxr_codeforces_core-0.0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/LICENSE` & `yxr_codeforces_core-0.0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/README.md` & `yxr_codeforces_core-0.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.3/pyproject.toml` & `yxr_codeforces_core-0.0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 dependencies = [
   "aiohttp",
   "pyaes",
   "requests",
   "beautifulsoup4",
   "lxml",
   "dataclasses-json",
+  "Brotli",
 ]
 [project.urls]
 "Homepage" = "https://github.com/CroMarmot/yxr-codeforces-core"
 "Bug Tracker" = "https://github.com/CroMarmot/yxr-codeforces-core/issues"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `yxr_codeforces_core-0.0.2.3/PKG-INFO` & `yxr_codeforces_core-0.0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: yxr-codeforces-core
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: Simple Codeforces core api
 Project-URL: Homepage, https://github.com/CroMarmot/yxr-codeforces-core
 Project-URL: Bug Tracker, https://github.com/CroMarmot/yxr-codeforces-core/issues
 Author-email: YeXiaoRain <yexiaorain@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 陈鼫RWHTYFZ
@@ -29,14 +29,15 @@
 License-File: LICENSE
 Keywords: api,codeforces,yxr
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: beautifulsoup4
+Requires-Dist: brotli
 Requires-Dist: dataclasses-json
 Requires-Dist: lxml
 Requires-Dist: pyaes
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: toml; extra == 'dev'
```

