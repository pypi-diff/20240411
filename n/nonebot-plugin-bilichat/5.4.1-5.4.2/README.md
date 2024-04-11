# Comparing `tmp/nonebot_plugin_bilichat-5.4.1.tar.gz` & `tmp/nonebot_plugin_bilichat-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.4.1.tar", last modified: Mon Apr  8 08:58:07 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.4.2.tar", last modified: Thu Apr 11 08:29:41 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.4.1.tar` & `nonebot_plugin_bilichat-5.4.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    34523 2024-04-08 08:58:03.764665 nonebot_plugin_bilichat-5.4.1/LICENSE
--rw-r--r--   0        0        0    17759 2024-04-08 08:58:03.764665 nonebot_plugin_bilichat-5.4.1/README.md
--rw-r--r--   0        0        0     2674 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2232 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1656 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2686 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7793 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      942 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3895 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5230 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9273 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3166 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4233 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3942 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      518 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6192 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      437 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1160 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7333 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3796 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3115 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1732 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1788 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     4033 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      568 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      833 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      341 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3019 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1040 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0     1163 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-08 08:58:03.784664 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     2623 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7217 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    15576 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4931 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2268 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1615 2024-04-08 08:58:03.788665 nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1754 2024-04-08 08:58:07.080700 nonebot_plugin_bilichat-5.4.1/pyproject.toml
--rw-r--r--   0        0        0    19454 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-11 08:29:35.533645 nonebot_plugin_bilichat-5.4.2/LICENSE
+-rw-r--r--   0        0        0    17759 2024-04-11 08:29:35.533645 nonebot_plugin_bilichat-5.4.2/README.md
+-rw-r--r--   0        0        0     2674 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2232 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1656 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2686 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7799 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      942 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3895 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5230 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9273 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3166 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4233 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3942 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      518 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6192 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      437 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1160 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7333 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3796 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3115 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1732 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1788 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     4033 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      568 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      833 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      341 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3019 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1040 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0     1163 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     2623 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7217 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    15576 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4931 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2268 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1615 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1754 2024-04-11 08:29:41.597682 nonebot_plugin_bilichat-5.4.2/pyproject.toml
+-rw-r--r--   0        0        0    19454 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.4.1/LICENSE` & `nonebot_plugin_bilichat-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/README.md` & `nonebot_plugin_bilichat-5.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             _msgs = msg
     except Exception:
         _msgs = msg
 
     bililink = None
     for _msg in _msgs[Text] + _msgs[Hyper]:
         # b23 格式的链接
-        _msg_str = str(_msg)
+        _msg_str = _msg.__repr__()
         if "b23" in _msg_str:
             if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", _msg_str):  # type: ignore
                 bililink = await b23_extract(list(b23.groups()))
                 break
         # av bv cv 格式和动态的链接
         for seg in ("av", "bv", "cv", "dynamic", "opus", "t.bilibili.com"):
             if seg in _msg_str.lower():
```

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.1/pyproject.toml` & `nonebot_plugin_bilichat-5.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.4.1"
+version = "5.4.2"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
```

### Comparing `nonebot_plugin_bilichat-5.4.1/PKG-INFO` & `nonebot_plugin_bilichat-5.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.4.1
+Version: 5.4.2
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.4.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.4.2 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
```

