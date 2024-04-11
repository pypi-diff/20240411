# Comparing `tmp/nonebot-plugin-orangejuice-0.9.0.tar.gz` & `tmp/nonebot-plugin-orangejuice-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-orangejuice-0.9.0.tar", last modified: Wed Apr 10 04:04:11 2024, max compression
+gzip compressed data, was "nonebot-plugin-orangejuice-0.9.1.tar", last modified: Thu Apr 11 12:35:30 2024, max compression
```

## Comparing `nonebot-plugin-orangejuice-0.9.0.tar` & `nonebot-plugin-orangejuice-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 04:04:11.774775 nonebot-plugin-orangejuice-0.9.0/
--rw-rw-rw-   0        0        0     1091 2024-03-10 10:09:46.000000 nonebot-plugin-orangejuice-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     4959 2024-04-10 04:04:11.772782 nonebot-plugin-orangejuice-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3000 2024-03-18 02:27:28.000000 nonebot-plugin-orangejuice-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 04:04:11.731794 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/
--rw-rw-rw-   0        0        0     7334 2024-04-10 04:01:14.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Card.py
--rw-rw-rw-   0        0        0      581 2024-04-09 10:25:58.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Config.py
--rw-rw-rw-   0        0        0      879 2024-03-14 06:19:14.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Deck.py
--rw-rw-rw-   0        0        0     1010 2024-04-09 07:53:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Emote.py
--rw-rw-rw-   0        0        0    10337 2024-04-09 10:22:07.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Ess.py
--rw-rw-rw-   0        0        0     9075 2024-04-10 02:39:25.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Le.py
--rw-rw-rw-   0        0        0     3044 2024-03-27 04:25:49.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Mixer.py
--rw-rw-rw-   0        0        0    12144 2024-04-10 04:01:59.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Stats.py
--rw-rw-rw-   0        0        0     2408 2024-04-10 04:03:49.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:04:11.769775 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/
--rw-rw-rw-   0        0        0     4959 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      200 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-10 04:04:11.000000 nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      977 2024-04-10 04:03:56.000000 nonebot-plugin-orangejuice-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 04:04:11.776301 nonebot-plugin-orangejuice-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 12:35:30.533697 nonebot-plugin-orangejuice-0.9.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-10 10:09:46.000000 nonebot-plugin-orangejuice-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     4959 2024-04-11 12:35:30.530684 nonebot-plugin-orangejuice-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3000 2024-03-18 02:27:28.000000 nonebot-plugin-orangejuice-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 12:35:30.504461 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/
+-rw-rw-rw-   0        0        0     7340 2024-04-11 11:38:37.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Card.py
+-rw-rw-rw-   0        0        0      581 2024-04-09 10:25:58.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Config.py
+-rw-rw-rw-   0        0        0      879 2024-03-14 06:19:14.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Deck.py
+-rw-rw-rw-   0        0        0     1010 2024-04-09 07:53:11.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Emote.py
+-rw-rw-rw-   0        0        0    10337 2024-04-09 10:22:07.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Ess.py
+-rw-rw-rw-   0        0        0    10555 2024-04-10 09:11:26.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Le.py
+-rw-rw-rw-   0        0        0     3044 2024-03-27 04:25:49.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Mixer.py
+-rw-rw-rw-   0        0        0    12144 2024-04-10 04:01:59.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Stats.py
+-rw-rw-rw-   0        0        0     2408 2024-04-11 12:34:47.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 12:35:30.528685 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/
+-rw-rw-rw-   0        0        0     4959 2024-04-11 12:35:30.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2024-04-11 12:35:30.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 12:35:30.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      200 2024-04-11 12:35:30.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-11 12:35:30.000000 nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-04-11 12:34:49.000000 nonebot-plugin-orangejuice-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 12:35:30.534356 nonebot-plugin-orangejuice-0.9.1/setup.cfg
```

### Comparing `nonebot-plugin-orangejuice-0.9.0/LICENSE` & `nonebot-plugin-orangejuice-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/PKG-INFO` & `nonebot-plugin-orangejuice-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orangejuice
-Version: 0.9.0
+Version: 0.9.1
 Summary: Sorabot Implemention
 Author-email: Polaris_Light <995905922@qq.com>
 License: MIT License
         
         Copyright (c) 2024 Polaris Light
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.9.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.9.1 Summary:
 Sorabot Implemention Author-email: Polaris_Light <995905922@qq.com> License:
 MIT License Copyright (c) 2024 Polaris Light Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `nonebot-plugin-orangejuice-0.9.0/README.md` & `nonebot-plugin-orangejuice-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Card.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Card.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                     target_group = groups[arg]
                 elif arg in groups.values():
                     target_group = arg
                 elif arg in tables:
                     target_table = arg
             
             for regex, key in self.regex.items():
-               if re.match(regex, name):
+               if re.match(regex, name, re.I):
                    name = key        
             
             for table in tables:
                 if target_table and target_table != table:
                     continue
                 table_attr: BaseClass = getattr(self, table)
                 for tuple in table_attr:
```

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Config.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Deck.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Deck.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Emote.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Emote.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Ess.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Ess.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Le.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Le.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 except Exception:
     scheduler = None
     logger.warning("未安装定时插件依赖")
 
 from .Config import plugin_config
 
 from .Ess import ess
-from .Card import card
 
 
 class Check: 
     def __init__(self) -> None:
         self.cd = plugin_config.le_cd
         self.max_count = plugin_config.le_max
         self.user_cd = {}
@@ -136,22 +135,26 @@
         
         if check.check(event):
             return None
 
         text = arg.extract_plain_text()
         num = min(int(text), 9) if (text := text[:1]).isdigit() and int(text) else 4
     
-        ordinary_list = []
-        for tuple in card.cardHyper:
-            if tuple[3] == 'ordinary':
-                ordinary_list.append(tuple)
-    
+        mw_list = ["平安的旅途","风信鸡的指引","烹饪时间","极速装置","束发魔女","主角的特权","甜点守护者","愤怒狂暴","湛蓝乌鸦·再临","给你的礼物",
+            "反射外装","决杀手术","奇迹红豆冰淇淋","星之再生","金蛋","三角力场","变化无常的风车","亚空间通道","阴谋机器人出动！","恶魔之手",
+            "阴谋的间谍行动～预备","坚实魔女","空间的跳跃(标记)","特别舞台","飞艇轰炸","束缚之锁","情报官","魔法狱火","记录重现","荒唐的性能",
+            "阴谋的操纵者","兔子模玩店","扩散光子步枪","永恒的观测者","浮游炮展开","融化的记忆","圣诞小姐的工作","海贼在天上飞？","店铺扩张战略","天使之手",
+            "超能模式！","永久流放","修罗场模式","玩偶使","白色圣诞大粉碎","赌博！","涡轮满载","×16大火箭","大爆炸铃","脱衣","隐身启动","劲敌","杀戮魔法",
+            "神出鬼没","兽之魔女","不动之物体","艾莉的奇迹","爆燃！","自爆","火箭炮","大火箭炮","乔纳桑·速袭","另一个最终兵器","露露的幸运蛋","星球的导火线",
+            "才气觉醒","水晶障壁","统治者","急速的亚莉希安罗妮","圣露眼","拜托了厨师长！","升档","炽热的商人之魂","月夜之舞","社交界亮相","黄昏色的梦",
+            "小麦格农炮","梦寐以求的世界","星星收集者","甜点天堂","甜点制作者的魔法","甜点成堆大作战","假想越狱","露露是厄运之龙","母亲之力","艾莉的超能奇迹","前主角的光辉时刻"]
+
         result = []
         for i in range(0, num):
-            result.append('「' + random.choice(ordinary_list)[1] + '」')
+            result.append('「' + random.choice(mw_list) + '」')
         await matcher.finish(f'奇迹漫步结果：\n{", ".join(result)}')
 
     async def divination(self, bot: Bot, matcher: Matcher, event: Union[GroupMessageEvent, PrivateMessageEvent], arg: Message = CommandArg()) -> None:
         if isinstance(event, GroupMessageEvent) and event.group_id in ess.config['modules']['Le']:
             return None
         
         if check.check(event):
```

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Mixer.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Mixer.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/Stats.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/Stats.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice/__init__.py` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     usage= r'See Sorabot Docs.',
     type="application",
     supported_adapters={"~onebot.v11"},
     homepage="https://github.com/FDCraft/nonebot-plugin-orangejuice",
     config=Config,
     extra={
         'author': 'Polaris_Light',
-        'version': '0.9.0',
+        'version': '0.9.1',
         'priority': 10
     }
 )
 
 import re
 
 from nonebot import on_command, on_regex
```

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orangejuice
-Version: 0.9.0
+Version: 0.9.1
 Summary: Sorabot Implemention
 Author-email: Polaris_Light <995905922@qq.com>
 License: MIT License
         
         Copyright (c) 2024 Polaris Light
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.9.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.9.1 Summary:
 Sorabot Implemention Author-email: Polaris_Light <995905922@qq.com> License:
 MIT License Copyright (c) 2024 Polaris Light Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `nonebot-plugin-orangejuice-0.9.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt` & `nonebot-plugin-orangejuice-0.9.1/nonebot_plugin_orangejuice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.9.0/pyproject.toml` & `nonebot-plugin-orangejuice-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-orangejuice"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.0.0-beta.1",
     "nonebot-plugin-apscheduler>=0.4.0",
     "cachetools>=5.0.0",
     "aiohttp>=3.8.0",
     "aiosqlite>=0.20.0",
```

