# Comparing `tmp/nonebot_plugin_kawaii_robot-4.1.0.post1.tar.gz` & `tmp/nonebot_plugin_kawaii_robot-4.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kawaii_robot-4.1.0.post1.tar", last modified: Fri Mar 15 14:33:19 2024, max compression
+gzip compressed data, was "nonebot_plugin_kawaii_robot-4.1.0.post2.tar", last modified: Thu Apr 11 11:22:34 2024, max compression
```

## Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1.tar` & `nonebot_plugin_kawaii_robot-4.1.0.post2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2024-03-15 14:33:05.510238 nonebot_plugin_kawaii_robot-4.1.0.post1/LICENSE
--rw-r--r--   0        0        0     9726 2024-03-15 14:33:05.510238 nonebot_plugin_kawaii_robot-4.1.0.post1/README.md
--rw-r--r--   0        0        0      710 2024-03-15 14:33:05.510238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/__init__.py
--rw-r--r--   0        0        0     6429 2024-03-15 14:33:05.510238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/__main__.py
--rw-r--r--   0        0        0     3629 2024-03-15 14:33:05.510238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/config.py
--rw-r--r--   0        0        0     1419 2024-03-15 14:33:05.514238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/const.py
--rw-r--r--   0        0        0     5167 2024-03-15 14:33:05.514238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/data_source.py
--rw-r--r--   0        0        0    76592 2024-03-15 14:33:05.514238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/resource/data.json
--rw-r--r--   0        0        0    10337 2024-03-15 14:33:05.514238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/resource/leaf.json
--rw-r--r--   0        0        0     4304 2024-03-15 14:33:05.514238 nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/utils.py
--rw-r--r--   0        0        0      866 2024-03-15 14:33:19.342296 nonebot_plugin_kawaii_robot-4.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0    10417 1970-01-01 00:00:00.000000 nonebot_plugin_kawaii_robot-4.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/LICENSE
+-rw-r--r--   0        0        0     9721 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/README.md
+-rw-r--r--   0        0        0      794 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/__init__.py
+-rw-r--r--   0        0        0     6429 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/__main__.py
+-rw-r--r--   0        0        0     3629 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/config.py
+-rw-r--r--   0        0        0     1419 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/const.py
+-rw-r--r--   0        0        0     5167 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/data_source.py
+-rw-r--r--   0        0        0    76592 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/resource/data.json
+-rw-r--r--   0        0        0    10337 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/resource/leaf.json
+-rw-r--r--   0        0        0     4304 2024-04-11 11:22:22.410415 nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/utils.py
+-rw-r--r--   0        0        0      866 2024-04-11 11:22:34.202503 nonebot_plugin_kawaii_robot-4.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0    10412 1970-01-01 00:00:00.000000 nonebot_plugin_kawaii_robot-4.1.0.post2/PKG-INFO
```

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/LICENSE` & `nonebot_plugin_kawaii_robot-4.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/README.md` & `nonebot_plugin_kawaii_robot-4.1.0.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-kawaii-robot
+Version: 4.1.0.post2
+Summary: 使用 Kyomotoi/AnimeThesaurus 的 NoneBot2 的回复（文i）插件
+Home-page: https://github.com/KarisAya/nonebot_plugin_kawaii_robot/
+Author-Email: karisaya <1048827424@qq.com>, student_2333 <lgc2333@126.com>
+License: AGPL-3.0
+Project-URL: Homepage, https://github.com/KarisAya/nonebot_plugin_kawaii_robot/
+Requires-Python: <4.0,>=3.8
+Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot-plugin-alconna>=0.40.1
+Requires-Dist: nonebot-plugin-userinfo>=0.2.2
+Requires-Dist: nonebot-plugin-session>=0.3.1
+Requires-Dist: cookit>=0.1.0
+Requires-Dist: anyio>=3.7.1
+Description-Content-Type: text/markdown
+
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
@@ -245,40 +262,32 @@
 [
   "{username}你好～",
   "{bot_nickname}在哦～"
   // ...
 ]
 ```
 
-<!--
-## 🎉 使用
-
-### 指令表
-
-|  指令  | 权限 | 需要@ | 范围 |   说明   |
-| :----: | :--: | :---: | :--: | :------: |
-| 指令 1 | 主人 |  否   | 私聊 | 指令说明 |
-| 指令 2 | 群员 |  是   | 群聊 | 指令说明 |
-
-### 效果图
-
-如果有效果图的话
--->
-
-<!--
 ## 📞 联系
 
-...
--->
+QQ：3076823485  
+Telegram：[@lgc2333](https://t.me/lgc2333)  
+吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
+邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
 - 插件改编~~抄~~自 [nonebot_plugin_smart_reply](https://github.com/Special-Week/nonebot_plugin_smart_reply)：使用了青云客 api 的的智能~障~回复插件
 - 复读姬借鉴~~抄~~自 [nonebot_plugin_repeater](https://github.com/ninthseason/nonebot-plugin-repeater)：群聊复读机
 
+## 💰 赞助
+
+**[赞助我](https://blog.lgc2333.top/donate)**
+
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
+
 ## 📝 更新日志
 
 ### 4.1.0
 
 - 适配 Pydantic V1 & V2
 - 使用 alconna 支持多平台，词库变量写法变化，新增了几个变量，不再支持 CQ 码
 - 重写了复读的逻辑，添加配置项 `LEAF_FORCE_DIFFERENT_USER`、`LEAF_REPEAT_CONTINUE`
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-kawaii-robot Version: 4.1.0.post2
+Summary: ä½¿ç¨ Kyomotoi/AnimeThesaurus ç NoneBot2 çåå¤ï¼æiï¼æä»¶
+Home-page: https://github.com/KarisAya/nonebot_plugin_kawaii_robot/ Author-
+Email: karisaya <1048827424@qq.com>, student_2333
+126.com> License: AGPL-3.0 Project-URL: Homepage, https://github.com/KarisAya/
+nonebot_plugin_kawaii_robot/ Requires-Python: <4.0,>=3.8 Requires-Dist:
+nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-alconna>=0.40.1 Requires-Dist:
+nonebot-plugin-userinfo>=0.2.2 Requires-Dist: nonebot-plugin-session>=0.3.1
+Requires-Dist: cookit>=0.1.0 Requires-Dist: anyio>=3.7.1 Description-Content-
+Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # NoneBot-Plugin-Kawaii-Robot _â¨ ä½¿ç¨ [Kyomotoi/AnimeThesaurus](https://
   github.com/Kyomotoi/AnimeThesaurus) ç NoneBot2 çåå¤ï¼æ iï¼æä»¶
                            â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð ä»ç» **WARNINGï¼é«äºæ¬¡åæµåº¦è­¦å** ### è¯åºåå¤
@@ -86,20 +96,25 @@
 ä¸­æå¯¹åºçåç½®è¯åºï¼ï¼ - `_hello.json`ï¼ç¨æ·åª at
 äºæºå¨äººï¼æ²¡æå¸¦ä»»ä½å¶ä»ææ¬æ¶æ¯æ¶åå¤çåå®¹ -
 `_poke.json`ï¼ç¨æ·æ³ä¸æ³æºå¨äººæ¶åå¤çææ¬åå®¹ -
 `_unknown.json`ï¼ç¨æ·åéçæ¶æ¯æ²¡æå¹éå°ä»»ä½è¯åºåå®¹æ¶åå¤çæ¶æ¯
 - `_interrupt.json`ï¼ææ­å¤è¯»æ¶åå¤çæ¶æ¯
 è¿äºè¯åºçæ ¼å¼æ¯ä¸ä¸ªææ¬æ°ç»ï¼æ¯ä¸ªåç´ æ¯ä¸æ¡åå¤ï¼åæ ·å¯ä»¥ä½¿ç¨ä¸é¢æå°çåé
 ç¤ºä¾ï¼ ```jsonc [ "{username}ä½ å¥½ï½", "{bot_nickname}å¨å¦ï½" // ... ]
-``` ## ð¡ é¸£è°¢ - æä»¶æ¹ç¼~~æ~~èª [nonebot_plugin_smart_reply](https:
-//github.com/Special-Week/nonebot_plugin_smart_reply)ï¼ä½¿ç¨äºéäºå®¢ api
+``` ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð¡ é¸£è°¢ - æä»¶æ¹ç¼~~æ~~èª [nonebot_plugin_smart_reply]
+(https://github.com/Special-Week/
+nonebot_plugin_smart_reply)ï¼ä½¿ç¨äºéäºå®¢ api
 ççæºè½~é~åå¤æä»¶ - å¤è¯»å§¬åé´~~æ~~èª
 [nonebot_plugin_repeater](https://github.com/ninthseason/nonebot-plugin-
-repeater)ï¼ç¾¤èå¤è¯»æº ## ð æ´æ°æ¥å¿ ### 4.1.0 - éé Pydantic V1
-& V2 - ä½¿ç¨ alconna
+repeater)ï¼ç¾¤èå¤è¯»æº ## ð° èµå© **[èµå©æ](https://
+blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 4.1.0 - éé Pydantic V1 & V2 - ä½¿ç¨ alconna
 æ¯æå¤å¹³å°ï¼è¯åºåéåæ³ååï¼æ°å¢äºå ä¸ªåéï¼ä¸åæ¯æ
 CQ ç  - éåäºå¤è¯»çé»è¾ï¼æ·»å éç½®é¡¹
 `LEAF_FORCE_DIFFERENT_USER`ã`LEAF_REPEAT_CONTINUE` ### 4.0.0 -
 å®å¨éææä»¶ä»£ç ï¼æ´æ¹é¡¹ç®ç»æï¼ä½¿ç¨ `pdm` ç®¡çé¡¹ç® -
 è¯åºä¼åï¼è¯¦è§ [éå è¯åº](#éå è¯åº)ï¼ï¼ -
 å è½½ï¼ç°å¨å¯ä»¥ç´æ¥å¾ `data/kawaii_robot` æä»¶å¤¹éæä½ èªå·±ç
 json è¯åºäº - ç¼åï¼æ¯æäºä¸äºåé -
```

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/__init__.py` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_userinfo")
 require("nonebot_plugin_session")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "4.1.0.post1"
+__version__ = "4.1.0.post2"
 __plugin_meta__ = PluginMetadata(
     name="KawaiiRobot",
     description="使用 Kyomotoi/AnimeThesaurus 的 NoneBot2 的回复（文i）插件",
     usage="Ciallo～(∠・ω< )⌒★",
     type="application",
     homepage="https://github.com/KarisAya/nonebot_plugin_kawaii_robot/",
     config=ConfigModel,
-    supported_adapters=inherit_supported_adapters("nonebot_plugin_alconna"),
+    supported_adapters=inherit_supported_adapters(
+        "nonebot_plugin_alconna",
+        "nonebot_plugin_userinfo",
+        "nonebot_plugin_session",
+    ),
     extra={},
 )
```

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/__main__.py` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/config.py` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/const.py` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/data_source.py` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/resource/data.json` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/resource/data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/resource/leaf.json` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/resource/leaf.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/nonebot_plugin_kawaii_robot/utils.py` & `nonebot_plugin_kawaii_robot-4.1.0.post2/nonebot_plugin_kawaii_robot/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/pyproject.toml` & `nonebot_plugin_kawaii_robot-4.1.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "nonebot-plugin-userinfo>=0.2.2",
     "nonebot-plugin-session>=0.3.1",
     "cookit>=0.1.0",
     "anyio>=3.7.1",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
-version = "4.1.0.post1"
+version = "4.1.0.post2"
 
 [project.license]
 text = "AGPL-3.0"
 
 [project.urls]
 homepage = "https://github.com/KarisAya/nonebot_plugin_kawaii_robot/"
```

### Comparing `nonebot_plugin_kawaii_robot-4.1.0.post1/PKG-INFO` & `nonebot_plugin_kawaii_robot-4.1.0.post2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-kawaii-robot
-Version: 4.1.0.post1
-Summary: 使用 Kyomotoi/AnimeThesaurus 的 NoneBot2 的回复（文i）插件
-Home-page: https://github.com/KarisAya/nonebot_plugin_kawaii_robot/
-Author-Email: karisaya <1048827424@qq.com>, student_2333 <lgc2333@126.com>
-License: AGPL-3.0
-Project-URL: Homepage, https://github.com/KarisAya/nonebot_plugin_kawaii_robot/
-Requires-Python: <4.0,>=3.8
-Requires-Dist: nonebot2>=2.0.0
-Requires-Dist: nonebot-plugin-alconna>=0.40.1
-Requires-Dist: nonebot-plugin-userinfo>=0.2.2
-Requires-Dist: nonebot-plugin-session>=0.3.1
-Requires-Dist: cookit>=0.1.0
-Requires-Dist: anyio>=3.7.1
-Description-Content-Type: text/markdown
-
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
@@ -262,40 +245,32 @@
 [
   "{username}你好～",
   "{bot_nickname}在哦～"
   // ...
 ]
 ```
 
-<!--
-## 🎉 使用
-
-### 指令表
-
-|  指令  | 权限 | 需要@ | 范围 |   说明   |
-| :----: | :--: | :---: | :--: | :------: |
-| 指令 1 | 主人 |  否   | 私聊 | 指令说明 |
-| 指令 2 | 群员 |  是   | 群聊 | 指令说明 |
-
-### 效果图
-
-如果有效果图的话
--->
-
-<!--
 ## 📞 联系
 
-...
--->
+QQ：3076823485  
+Telegram：[@lgc2333](https://t.me/lgc2333)  
+吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
+邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
 - 插件改编~~抄~~自 [nonebot_plugin_smart_reply](https://github.com/Special-Week/nonebot_plugin_smart_reply)：使用了青云客 api 的的智能~障~回复插件
 - 复读姬借鉴~~抄~~自 [nonebot_plugin_repeater](https://github.com/ninthseason/nonebot-plugin-repeater)：群聊复读机
 
+## 💰 赞助
+
+**[赞助我](https://blog.lgc2333.top/donate)**
+
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
+
 ## 📝 更新日志
 
 ### 4.1.0
 
 - 适配 Pydantic V1 & V2
 - 使用 alconna 支持多平台，词库变量写法变化，新增了几个变量，不再支持 CQ 码
 - 重写了复读的逻辑，添加配置项 `LEAF_FORCE_DIFFERENT_USER`、`LEAF_REPEAT_CONTINUE`
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-kawaii-robot Version: 4.1.0.post1
-Summary: ä½¿ç¨ Kyomotoi/AnimeThesaurus ç NoneBot2 çåå¤ï¼æiï¼æä»¶
-Home-page: https://github.com/KarisAya/nonebot_plugin_kawaii_robot/ Author-
-Email: karisaya <1048827424@qq.com>, student_2333
-126.com> License: AGPL-3.0 Project-URL: Homepage, https://github.com/KarisAya/
-nonebot_plugin_kawaii_robot/ Requires-Python: <4.0,>=3.8 Requires-Dist:
-nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-alconna>=0.40.1 Requires-Dist:
-nonebot-plugin-userinfo>=0.2.2 Requires-Dist: nonebot-plugin-session>=0.3.1
-Requires-Dist: cookit>=0.1.0 Requires-Dist: anyio>=3.7.1 Description-Content-
-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # NoneBot-Plugin-Kawaii-Robot _â¨ ä½¿ç¨ [Kyomotoi/AnimeThesaurus](https://
   github.com/Kyomotoi/AnimeThesaurus) ç NoneBot2 çåå¤ï¼æ iï¼æä»¶
                            â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð ä»ç» **WARNINGï¼é«äºæ¬¡åæµåº¦è­¦å** ### è¯åºåå¤
@@ -96,20 +86,25 @@
 ä¸­æå¯¹åºçåç½®è¯åºï¼ï¼ - `_hello.json`ï¼ç¨æ·åª at
 äºæºå¨äººï¼æ²¡æå¸¦ä»»ä½å¶ä»ææ¬æ¶æ¯æ¶åå¤çåå®¹ -
 `_poke.json`ï¼ç¨æ·æ³ä¸æ³æºå¨äººæ¶åå¤çææ¬åå®¹ -
 `_unknown.json`ï¼ç¨æ·åéçæ¶æ¯æ²¡æå¹éå°ä»»ä½è¯åºåå®¹æ¶åå¤çæ¶æ¯
 - `_interrupt.json`ï¼ææ­å¤è¯»æ¶åå¤çæ¶æ¯
 è¿äºè¯åºçæ ¼å¼æ¯ä¸ä¸ªææ¬æ°ç»ï¼æ¯ä¸ªåç´ æ¯ä¸æ¡åå¤ï¼åæ ·å¯ä»¥ä½¿ç¨ä¸é¢æå°çåé
 ç¤ºä¾ï¼ ```jsonc [ "{username}ä½ å¥½ï½", "{bot_nickname}å¨å¦ï½" // ... ]
-``` ## ð¡ é¸£è°¢ - æä»¶æ¹ç¼~~æ~~èª [nonebot_plugin_smart_reply](https:
-//github.com/Special-Week/nonebot_plugin_smart_reply)ï¼ä½¿ç¨äºéäºå®¢ api
+``` ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð¡ é¸£è°¢ - æä»¶æ¹ç¼~~æ~~èª [nonebot_plugin_smart_reply]
+(https://github.com/Special-Week/
+nonebot_plugin_smart_reply)ï¼ä½¿ç¨äºéäºå®¢ api
 ççæºè½~é~åå¤æä»¶ - å¤è¯»å§¬åé´~~æ~~èª
 [nonebot_plugin_repeater](https://github.com/ninthseason/nonebot-plugin-
-repeater)ï¼ç¾¤èå¤è¯»æº ## ð æ´æ°æ¥å¿ ### 4.1.0 - éé Pydantic V1
-& V2 - ä½¿ç¨ alconna
+repeater)ï¼ç¾¤èå¤è¯»æº ## ð° èµå© **[èµå©æ](https://
+blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 4.1.0 - éé Pydantic V1 & V2 - ä½¿ç¨ alconna
 æ¯æå¤å¹³å°ï¼è¯åºåéåæ³ååï¼æ°å¢äºå ä¸ªåéï¼ä¸åæ¯æ
 CQ ç  - éåäºå¤è¯»çé»è¾ï¼æ·»å éç½®é¡¹
 `LEAF_FORCE_DIFFERENT_USER`ã`LEAF_REPEAT_CONTINUE` ### 4.0.0 -
 å®å¨éææä»¶ä»£ç ï¼æ´æ¹é¡¹ç®ç»æï¼ä½¿ç¨ `pdm` ç®¡çé¡¹ç® -
 è¯åºä¼åï¼è¯¦è§ [éå è¯åº](#éå è¯åº)ï¼ï¼ -
 å è½½ï¼ç°å¨å¯ä»¥ç´æ¥å¾ `data/kawaii_robot` æä»¶å¤¹éæä½ èªå·±ç
 json è¯åºäº - ç¼åï¼æ¯æäºä¸äºåé -
```

