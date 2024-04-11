# Comparing `tmp/nonebot_plugin_picstatus-2.0.0.post2.tar.gz` & `tmp/nonebot_plugin_picstatus-2.0.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_picstatus-2.0.0.post2.tar", last modified: Mon Mar 18 05:35:48 2024, max compression
+gzip compressed data, was "nonebot_plugin_picstatus-2.0.0.post3.tar", last modified: Wed Apr 10 14:23:23 2024, max compression
```

## Comparing `nonebot_plugin_picstatus-2.0.0.post2.tar` & `nonebot_plugin_picstatus-2.0.0.post3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/LICENSE
--rw-r--r--   0        0        0    10412 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/README.md
--rw-r--r--   0        0        0     1319 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/__init__.py
--rw-r--r--   0        0        0     1345 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/__main__.py
--rw-r--r--   0        0        0     3439 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/bg_provider.py
--rw-r--r--   0        0        0     5363 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/__init__.py
--rw-r--r--   0        0        0     2649 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/bot.py
--rw-r--r--   0        0        0     1338 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/cpu.py
--rw-r--r--   0        0        0     3019 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/disk.py
--rw-r--r--   0        0        0      505 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/mem.py
--rw-r--r--   0        0        0     3539 2024-03-18 05:35:36.174585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/misc.py
--rw-r--r--   0        0        0     3126 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/network.py
--rw-r--r--   0        0        0     1570 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/process.py
--rw-r--r--   0        0        0     2891 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/config.py
--rw-r--r--   0        0        0    10798 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/assets/default_avatar.webp
--rw-r--r--   0        0        0   197506 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/assets/default_bg.webp
--rw-r--r--   0        0        0       69 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/js/globalThis.d.ts
--rw-r--r--   0        0        0       25 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/js/init-global.js
--rw-r--r--   0        0        0     1993 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/js/lazy-load.js
--rw-r--r--   0        0        0      189 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/js/load-plugin.js
--rw-r--r--   0        0        0     3511 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/statistics.py
--rw-r--r--   0        0        0     2171 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/__init__.py
--rw-r--r--   0        0        0     1903 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/__init__.py
--rw-r--r--   0        0        0     7561 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/index.css
--rw-r--r--   0        0        0       35 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/no-blur.css
--rw-r--r--   0        0        0       57 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/no-radius.css
--rw-r--r--   0        0        0       36 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/no-shadow.css
--rw-r--r--   0        0        0      670 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/theme-dark.css
--rw-r--r--   0        0        0     1294 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/templates/index.html.jinja
--rw-r--r--   0        0        0     4745 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/templates/macros.html.jinja
--rw-r--r--   0        0        0     6104 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/pw_render.py
--rw-r--r--   0        0        0      819 2024-03-18 05:35:36.178585 nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/util.py
--rw-r--r--   0        0        0      967 2024-03-18 05:35:48.646704 nonebot_plugin_picstatus-2.0.0.post2/pyproject.toml
--rw-r--r--   0        0        0    11279 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-2.0.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/LICENSE
+-rw-r--r--   0        0        0    10236 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/README.md
+-rw-r--r--   0        0        0     1369 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/__init__.py
+-rw-r--r--   0        0        0     1345 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/__main__.py
+-rw-r--r--   0        0        0     3439 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/bg_provider.py
+-rw-r--r--   0        0        0     5363 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/__init__.py
+-rw-r--r--   0        0        0     2649 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/bot.py
+-rw-r--r--   0        0        0     1338 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/cpu.py
+-rw-r--r--   0        0        0     3019 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/disk.py
+-rw-r--r--   0        0        0      505 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/mem.py
+-rw-r--r--   0        0        0     3539 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/misc.py
+-rw-r--r--   0        0        0     3126 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/network.py
+-rw-r--r--   0        0        0     1570 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/process.py
+-rw-r--r--   0        0        0     2891 2024-04-10 14:23:08.222802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/config.py
+-rw-r--r--   0        0        0    10798 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/assets/default_avatar.webp
+-rw-r--r--   0        0        0   197506 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/assets/default_bg.webp
+-rw-r--r--   0        0        0       69 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/js/globalThis.d.ts
+-rw-r--r--   0        0        0       25 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/js/init-global.js
+-rw-r--r--   0        0        0     1993 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/js/lazy-load.js
+-rw-r--r--   0        0        0      189 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/js/load-plugin.js
+-rw-r--r--   0        0        0     3511 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/statistics.py
+-rw-r--r--   0        0        0     2171 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/__init__.py
+-rw-r--r--   0        0        0     1903 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/__init__.py
+-rw-r--r--   0        0        0     7561 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/index.css
+-rw-r--r--   0        0        0       35 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/no-blur.css
+-rw-r--r--   0        0        0       57 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/no-radius.css
+-rw-r--r--   0        0        0       36 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/no-shadow.css
+-rw-r--r--   0        0        0      670 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/theme-dark.css
+-rw-r--r--   0        0        0     1294 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/templates/index.html.jinja
+-rw-r--r--   0        0        0     4745 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/templates/macros.html.jinja
+-rw-r--r--   0        0        0     6104 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/pw_render.py
+-rw-r--r--   0        0        0      819 2024-04-10 14:23:08.226802 nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/util.py
+-rw-r--r--   0        0        0      967 2024-04-10 14:23:23.834906 nonebot_plugin_picstatus-2.0.0.post3/pyproject.toml
+-rw-r--r--   0        0        0    11103 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-2.0.0.post3/PKG-INFO
```

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/LICENSE` & `nonebot_plugin_picstatus-2.0.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/README.md` & `nonebot_plugin_picstatus-2.0.0.post3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -151,23 +151,17 @@
 
 ### [故梦 API](https://api.gumengya.com) & [LoliApi](https://docs.loliapi.com/) & [Lolicon API](https://api.lolicon.app/)
 
 - 背景图来源
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
-
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
-
-  </details>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 ## 📝 更新日志
 
 ### 2.0.0
 
 - 代码重构，现在开发者可以更自由灵活的添加新状态图片样式
 - 配置项变动：
```

#### html2text {}

```diff
@@ -28,19 +28,17 @@
 126.com> ## ð¡ é¸£è°¢ ### [nonebot/plugin-alconna](https://github.com/
 nonebot/plugin-alconna) - å¼ºå¤§çå½ä»¤è§£æåºï¼åå¤å¹³å°ééæ¹æ¡
 ### [noneplugin/nonebot-plugin-userinfo](https://github.com/noneplugin/nonebot-
 plugin-userinfo) - å¤å¹³å°ç¨æ·ä¿¡æ¯è·åæ¹æ¡ ### [kexue-z/nonebot-
 plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - HTML
 æ¸²ææ¹æ¡ ### [ææ¢¦ API](https://api.gumengya.com) & [LoliApi](https://
 docs.loliapi.com/) & [Lolicon API](https://api.lolicon.app/) - èæ¯å¾æ¥æº
-## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 2.0.0 -
+## ð° èµå© **[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 2.0.0 -
 ä»£ç éæï¼ç°å¨å¼åèå¯ä»¥æ´èªç±çµæ´»çæ·»å æ°ç¶æå¾çæ ·å¼
 - éç½®é¡¹åå¨ï¼ - æ°å¢ `PS_TEMPLATE` - æ°å¢ `PS_COLLECT_INTERVAL` -
 æ°å¢ `PS_DEFAULT_COLLECT_CACHE_SIZE` - æ°å¢ `PS_COLLECT_CACHE_SIZE` -
 æ°å¢ `PS_COUNT_MESSAGE_SENT_EVENT` - æ°å¢ `PS_DISCONNECT_RESET_COUNTER` -
 éå½å `PS_COMPONENTS` -> `PS_DEFAULT_COMPONENTS` - éå½å
 `PS_ADDITIONAL_CSS` -> `PS_DEFAULT_ADDITIONAL_CSS` - éå½å
 `PS_ADDITIONAL_SCRIPT` -> `PS_DEFAULT_ADDITIONAL_SCRIPT` vv11
```

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/__init__.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,18 +23,21 @@
 
 usage = f"指令：{' / '.join(config.ps_command)}"
 if config.ps_need_at:
     usage += "\n注意：使用指令时需要@机器人"
 if config.ps_only_su:
     usage += "\n注意：仅SuperUser可以使用此指令"
 
-__version__ = "2.0.0.post2"
+__version__ = "2.0.0.post3"
 __plugin_meta__ = PluginMetadata(
     name="PicStatus",
     description="以图片形式显示当前设备的运行状态",
     usage=usage,
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus",
     config=ConfigModel,
-    supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
+    supported_adapters=inherit_supported_adapters(
+        "nonebot_plugin_alconna",
+        "nonebot_plugin_userinfo",
+    ),
     extra={"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/__main__.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/bg_provider.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/bg_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/__init__.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/bot.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/cpu.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/cpu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/disk.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/disk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/misc.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/misc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/network.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/network.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/collectors/process.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/collectors/process.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/config.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/assets/default_avatar.webp` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/assets/default_avatar.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/assets/default_bg.webp` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/assets/default_bg.webp`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/res/js/lazy-load.js` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/res/js/lazy-load.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/statistics.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/statistics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/__init__.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/__init__.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/index.css` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/index.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/css/theme-dark.css` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/css/theme-dark.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/templates/index.html.jinja` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/templates/index.html.jinja`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/default/res/templates/macros.html.jinja` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/default/res/templates/macros.html.jinja`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/templates/pw_render.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/templates/pw_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/nonebot_plugin_picstatus/util.py` & `nonebot_plugin_picstatus-2.0.0.post3/nonebot_plugin_picstatus/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/pyproject.toml` & `nonebot_plugin_picstatus-2.0.0.post3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "anyio>=3.6.2",
     "httpx>=0.25.0",
     "jinja2>=3.1.2",
     "yarl>=1.9.4",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "2.0.0.post2"
+version = "2.0.0.post3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus"
```

### Comparing `nonebot_plugin_picstatus-2.0.0.post2/PKG-INFO` & `nonebot_plugin_picstatus-2.0.0.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picstatus
-Version: 2.0.0.post2
+Version: 2.0.0.post3
 Summary: A NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
@@ -174,23 +174,17 @@
 
 ### [故梦 API](https://api.gumengya.com) & [LoliApi](https://docs.loliapi.com/) & [Lolicon API](https://api.lolicon.app/)
 
 - 背景图来源
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
-
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
-
-  </details>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 ## 📝 更新日志
 
 ### 2.0.0
 
 - 代码重构，现在开发者可以更自由灵活的添加新状态图片样式
 - 配置项变动：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 2.0.0.post2
+Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 2.0.0.post3
 Summary: A NoneBot2 plugin generates a picture which shows the status of
 current device Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-
 picstatus Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-picstatus Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-apscheduler>=0.4.0 Requires-Dist:
 nonebot-plugin-alconna>=0.40.1 Requires-Dist: nonebot-plugin-userinfo>=0.1.3
@@ -41,19 +41,17 @@
 126.com> ## ð¡ é¸£è°¢ ### [nonebot/plugin-alconna](https://github.com/
 nonebot/plugin-alconna) - å¼ºå¤§çå½ä»¤è§£æåºï¼åå¤å¹³å°ééæ¹æ¡
 ### [noneplugin/nonebot-plugin-userinfo](https://github.com/noneplugin/nonebot-
 plugin-userinfo) - å¤å¹³å°ç¨æ·ä¿¡æ¯è·åæ¹æ¡ ### [kexue-z/nonebot-
 plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - HTML
 æ¸²ææ¹æ¡ ### [ææ¢¦ API](https://api.gumengya.com) & [LoliApi](https://
 docs.loliapi.com/) & [Lolicon API](https://api.lolicon.app/) - èæ¯å¾æ¥æº
-## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 2.0.0 -
+## ð° èµå© **[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 2.0.0 -
 ä»£ç éæï¼ç°å¨å¼åèå¯ä»¥æ´èªç±çµæ´»çæ·»å æ°ç¶æå¾çæ ·å¼
 - éç½®é¡¹åå¨ï¼ - æ°å¢ `PS_TEMPLATE` - æ°å¢ `PS_COLLECT_INTERVAL` -
 æ°å¢ `PS_DEFAULT_COLLECT_CACHE_SIZE` - æ°å¢ `PS_COLLECT_CACHE_SIZE` -
 æ°å¢ `PS_COUNT_MESSAGE_SENT_EVENT` - æ°å¢ `PS_DISCONNECT_RESET_COUNTER` -
 éå½å `PS_COMPONENTS` -> `PS_DEFAULT_COMPONENTS` - éå½å
 `PS_ADDITIONAL_CSS` -> `PS_DEFAULT_ADDITIONAL_CSS` - éå½å
 `PS_ADDITIONAL_SCRIPT` -> `PS_DEFAULT_ADDITIONAL_SCRIPT` vv11
```

