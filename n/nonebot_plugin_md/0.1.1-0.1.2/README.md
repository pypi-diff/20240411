# Comparing `tmp/nonebot_plugin_md-0.1.1.tar.gz` & `tmp/nonebot_plugin_md-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_md-0.1.1.tar", last modified: Thu Mar 21 12:15:38 2024, max compression
+gzip compressed data, was "nonebot_plugin_md-0.1.2.tar", last modified: Thu Apr 11 05:58:48 2024, max compression
```

## Comparing `nonebot_plugin_md-0.1.1.tar` & `nonebot_plugin_md-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/LICENSE
--rw-r--r--   0        0        0     3087 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/README.md
--rw-r--r--   0        0        0      671 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/__init__.py
--rw-r--r--   0        0        0     1024 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/__main__.py
--rw-r--r--   0        0        0    11519 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/b30.py
--rw-r--r--   0        0        0      192 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/config.py
--rw-r--r--   0        0        0     2851 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/image.py
--rw-r--r--   0        0        0      946 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/message.py
--rw-r--r--   0        0        0      769 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/nonebot_plugin_md/utils.py
--rw-r--r--   0        0        0      889 2024-03-21 12:15:38.411520 nonebot_plugin_md-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    52752 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/tests/1.png
--rw-r--r--   0        0        0        0 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2836 2024-03-21 12:15:25.047657 nonebot_plugin_md-0.1.1/tests/image.py
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 nonebot_plugin_md-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3088 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/README.md
+-rw-r--r--   0        0        0      666 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/__main__.py
+-rw-r--r--   0        0        0    11519 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/b30.py
+-rw-r--r--   0        0        0      192 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/config.py
+-rw-r--r--   0        0        0     2851 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/image.py
+-rw-r--r--   0        0        0      946 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/message.py
+-rw-r--r--   0        0        0      769 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/nonebot_plugin_md/utils.py
+-rw-r--r--   0        0        0      882 2024-04-11 05:58:48.343881 nonebot_plugin_md-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    52752 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/tests/1.png
+-rw-r--r--   0        0        0        0 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2836 2024-04-11 05:58:32.743903 nonebot_plugin_md-0.1.2/tests/image.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 nonebot_plugin_md-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_md-0.1.1/LICENSE` & `nonebot_plugin_md-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/README.md` & `nonebot_plugin_md-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```bash
-nb plugin install nonebot-plugin-md
+nb plugin install nonebot_plugin_md
 ```
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
@@ -99,8 +99,8 @@
 - 如果本插件对你有帮助，不要忘了点个Star~
 - 本项目仅供学习使用，请勿用于商业用途
 - [更新日志](./docs/update.md)
 - [AGPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_md/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
 
 ## 🌐 感谢
 
-- [MDbot](https://github.com/Doctorade/MDBot)- 源代码来源
+- [MDbot](https://github.com/Doctorade/MDBot)- 源代码来源
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 ## è¯´æ
 ä½¿ç¨ä»MuseDash.moeæ¸æ¥çæ°æ®åapiå¼åçåµæ¯æ¥åbotï¼å¯ä»¥å®ç°ç»å®qqåmdè´¦å·ãæ¥è¯¢b30ãæ¥è¯¢æ²ç®ä¿¡æ¯ãæ¥è¯¢é¾åº¦æè¡ç­åè½
 æ¯ænonebot_plugin_saaææ¯æçææééå¨ ## ä¸»è¦åè½ - 1.
 åå§å åé`md update` - 2. ç»å® åé`md bindname xxx` æè `md
 binduid xxx` - 3. b30 ## å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯
 [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
-plugin install nonebot-plugin-md ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+plugin install nonebot_plugin_md ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip ```bash pip install nonebot-plugin-md ``` pdm
 ```bash pdm add nonebot-plugin-md ``` poetry ```bash poetry add nonebot-plugin-
 md ``` conda ```bash conda install nonebot-plugin-md ``` ## å¶ä» -
 æ¬é¡¹ç®åå æ¯å ä¹æ¾ä¸å°å¼æºçmdæ¥è¯¢æä»¶ï¼å æ­¤èªå·±åä¸ªå¼æºçï¼æ¬¢è¿å¤§ä½¬æissåpr
 - å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [æ´æ°æ¥å¿](./docs/
```

### Comparing `nonebot_plugin_md-0.1.1/nonebot_plugin_md/__init__.py` & `nonebot_plugin_md-0.1.2/nonebot_plugin_md/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
 __version__ = "0.1.1"
 __plugin_meta__ = PluginMetadata(
-    name="Sekai Stickers",
+    name="Muse Dash",
     description="基于 NoneBot2 的 MUSE DASH查询插件",
     usage="",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_md",
     config=ConfigModel,
     supported_adapters=inherit_supported_adapters("nonebot_plugin_saa"),
     extra={
```

### Comparing `nonebot_plugin_md-0.1.1/nonebot_plugin_md/__main__.py` & `nonebot_plugin_md-0.1.2/nonebot_plugin_md/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/nonebot_plugin_md/b30.py` & `nonebot_plugin_md-0.1.2/nonebot_plugin_md/b30.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/nonebot_plugin_md/image.py` & `nonebot_plugin_md-0.1.2/nonebot_plugin_md/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/nonebot_plugin_md/message.py` & `nonebot_plugin_md-0.1.2/nonebot_plugin_md/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/nonebot_plugin_md/utils.py` & `nonebot_plugin_md-0.1.2/nonebot_plugin_md/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/pyproject.toml` & `nonebot_plugin_md-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "nonebot_plugin_md"
-version = "0.1.1"
+version = "0.1.2"
 description = "muse dash for nonebot2"
 authors = [
     { name = "Agnes Digital", email = "Z735803792@163.com" },
 ]
 dependencies = [
     "nonebot2>=2.1.1",
     "nonebot-plugin-send-anything-anywhere>=0.3.2",
     "aiohttp>=3.8.1",
     "fuzzywuzzy>=0.18.0",
     "lxml>=4.9.1",
 ]
-requires-python = ">=3.9,<=3.12"
+requires-python = ">=3.9"
 keywords = [
     "md",
     "nonebot2",
     "plugin",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `nonebot_plugin_md-0.1.1/tests/1.png` & `nonebot_plugin_md-0.1.2/tests/1.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/tests/image.py` & `nonebot_plugin_md-0.1.2/tests/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_md-0.1.1/PKG-INFO` & `nonebot_plugin_md-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_md
-Version: 0.1.1
+Version: 0.1.2
 Summary: muse dash for nonebot2
 Keywords: md nonebot2 plugin
 Author-Email: Agnes Digital <Z735803792@163.com>
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: <=3.12,>=3.9
+Requires-Python: >=3.9
 Requires-Dist: nonebot2>=2.1.1
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.3.2
 Requires-Dist: aiohttp>=3.8.1
 Requires-Dist: fuzzywuzzy>=0.18.0
 Requires-Dist: lxml>=4.9.1
 Description-Content-Type: text/markdown
 
@@ -68,15 +68,15 @@
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```bash
-nb plugin install nonebot-plugin-md
+nb plugin install nonebot_plugin_md
 ```
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
@@ -121,8 +121,8 @@
 - 如果本插件对你有帮助，不要忘了点个Star~
 - 本项目仅供学习使用，请勿用于商业用途
 - [更新日志](./docs/update.md)
 - [AGPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_md/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
 
 ## 🌐 感谢
 
-- [MDbot](https://github.com/Doctorade/MDBot)- 源代码来源
+- [MDbot](https://github.com/Doctorade/MDBot)- 源代码来源
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_md Version: 0.1.1 Summary: muse dash
+Metadata-Version: 2.1 Name: nonebot_plugin_md Version: 0.1.2 Summary: muse dash
 for nonebot2 Keywords: md nonebot2 plugin Author-Email: Agnes Digital
 163.com> License: AGPL-3.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Requires-Python:
-<=3.12,>=3.9 Requires-Dist: nonebot2>=2.1.1 Requires-Dist: nonebot-plugin-send-
+>=3.9 Requires-Dist: nonebot2>=2.1.1 Requires-Dist: nonebot-plugin-send-
 anything-anywhere>=0.3.2 Requires-Dist: aiohttp>=3.8.1 Requires-Dist:
 fuzzywuzzy>=0.18.0 Requires-Dist: lxml>=4.9.1 Description-Content-Type: text/
 markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_md _â¨æ¸¸æææ¯å¿«è·(muse dash)æ¥è¯¢â¨__[_G_i_t_H_u_b_ _s_t_a_r_s_]
              _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]_[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]_[_p_y_p_i_][python][NoneBot]
 ## è¯´æ
 ä½¿ç¨ä»MuseDash.moeæ¸æ¥çæ°æ®åapiå¼åçåµæ¯æ¥åbotï¼å¯ä»¥å®ç°ç»å®qqåmdè´¦å·ãæ¥è¯¢b30ãæ¥è¯¢æ²ç®ä¿¡æ¯ãæ¥è¯¢é¾åº¦æè¡ç­åè½
 æ¯ænonebot_plugin_saaææ¯æçææééå¨ ## ä¸»è¦åè½ - 1.
 åå§å åé`md update` - 2. ç»å® åé`md bindname xxx` æè `md
 binduid xxx` - 3. b30 ## å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯
 [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
-plugin install nonebot-plugin-md ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+plugin install nonebot_plugin_md ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip ```bash pip install nonebot-plugin-md ``` pdm
 ```bash pdm add nonebot-plugin-md ``` poetry ```bash poetry add nonebot-plugin-
 md ``` conda ```bash conda install nonebot-plugin-md ``` ## å¶ä» -
 æ¬é¡¹ç®åå æ¯å ä¹æ¾ä¸å°å¼æºçmdæ¥è¯¢æä»¶ï¼å æ­¤èªå·±åä¸ªå¼æºçï¼æ¬¢è¿å¤§ä½¬æissåpr
 - å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [æ´æ°æ¥å¿](./docs/
```

