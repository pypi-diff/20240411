# Comparing `tmp/scrapy-util-0.0.9.tar.gz` & `tmp/scrapy-util-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapy-util-0.0.9.tar", last modified: Mon Feb  8 07:00:13 2021, max compression
+gzip compressed data, was "dist/scrapy-util-1.0.2.tar", last modified: Thu Apr 11 07:31:53 2024, max compression
```

## Comparing `scrapy-util-0.0.9.tar` & `scrapy-util-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/
--rwxr-xr-x   0 hina       (501) staff       (20)      276 2021-01-26 13:50:50.000000 scrapy-util-0.0.9/MANIFEST.in
--rw-r--r--   0 hina       (501) staff       (20)     2242 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)     1384 2021-01-27 05:35:54.000000 scrapy-util-0.0.9/README.md
--rwxr-xr-x   0 hina       (501) staff       (20)       16 2021-01-26 11:01:20.000000 scrapy-util-0.0.9/requirements.txt
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/scrapy_util/
--rw-r--r--   0 hina       (501) staff       (20)       24 2021-01-26 13:46:50.000000 scrapy-util-0.0.9/scrapy_util/__init__.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/scrapy_util/extensions/
--rw-r--r--   0 hina       (501) staff       (20)      200 2021-01-27 04:14:16.000000 scrapy-util-0.0.9/scrapy_util/extensions/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      480 2021-01-27 03:10:48.000000 scrapy-util-0.0.9/scrapy_util/extensions/localtime_core_stats.py
--rw-r--r--   0 hina       (501) staff       (20)     1126 2021-01-27 04:13:26.000000 scrapy-util-0.0.9/scrapy_util/extensions/show_duration_extension.py
--rw-r--r--   0 hina       (501) staff       (20)     2166 2021-02-08 03:23:46.000000 scrapy-util-0.0.9/scrapy_util/extensions/stats_collector_extension.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/scrapy_util/items/
--rw-r--r--   0 hina       (501) staff       (20)       59 2021-01-26 09:24:20.000000 scrapy-util-0.0.9/scrapy_util/items/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      129 2021-01-26 09:12:30.000000 scrapy-util-0.0.9/scrapy_util/items/trick_item.py
--rw-r--r--   0 hina       (501) staff       (20)       77 2021-01-26 10:26:11.000000 scrapy-util-0.0.9/scrapy_util/logger.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/scrapy_util/middlewares/
--rw-r--r--   0 hina       (501) staff       (20)      105 2021-01-26 09:24:28.000000 scrapy-util-0.0.9/scrapy_util/middlewares/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      573 2021-01-27 04:01:46.000000 scrapy-util-0.0.9/scrapy_util/middlewares/dont_request_downloader_middleware.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/scrapy_util/spiders/
--rw-r--r--   0 hina       (501) staff       (20)       65 2021-01-26 09:24:41.000000 scrapy-util-0.0.9/scrapy_util/spiders/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)     1521 2021-01-27 03:47:08.000000 scrapy-util-0.0.9/scrapy_util/spiders/script_spider.py
--rw-r--r--   0 hina       (501) staff       (20)      616 2021-01-27 04:15:50.000000 scrapy-util-0.0.9/scrapy_util/utils.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/scrapy_util.egg-info/
--rw-r--r--   0 hina       (501) staff       (20)     2242 2021-02-08 07:00:12.000000 scrapy-util-0.0.9/scrapy_util.egg-info/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)      731 2021-02-08 07:00:12.000000 scrapy-util-0.0.9/scrapy_util.egg-info/SOURCES.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2021-02-08 07:00:12.000000 scrapy-util-0.0.9/scrapy_util.egg-info/dependency_links.txt
--rw-r--r--   0 hina       (501) staff       (20)       16 2021-02-08 07:00:12.000000 scrapy-util-0.0.9/scrapy_util.egg-info/requires.txt
--rw-r--r--   0 hina       (501) staff       (20)       12 2021-02-08 07:00:12.000000 scrapy-util-0.0.9/scrapy_util.egg-info/top_level.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2021-02-08 07:00:12.000000 scrapy-util-0.0.9/scrapy_util.egg-info/zip-safe
--rw-r--r--   0 hina       (501) staff       (20)       38 2021-02-08 07:00:13.000000 scrapy-util-0.0.9/setup.cfg
--rwxr-xr-x   0 hina       (501) staff       (20)     1696 2021-02-08 03:26:03.000000 scrapy-util-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/localtime_core_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/show_duration_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/stats_collector_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/items/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/items/mongo_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/items/trick_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/middlewares/dont_request_downloader_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/pipelines/mongo_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/spiders/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/list_next_request_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/list_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/script_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1911 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/tests/test_hello.py
```

### Comparing `scrapy-util-0.0.9/scrapy_util/extensions/show_duration_extension.py` & `scrapy-util-1.0.2/scrapy_util/extensions/show_duration_extension.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-0.0.9/scrapy_util/extensions/stats_collector_extension.py` & `scrapy-util-1.0.2/scrapy_util/extensions/stats_collector_extension.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # @Date    : 2018-12-12
 # @Author  : Peng Shiyu
 
 import requests
 from scrapy import signals
 
 from scrapy_util.logger import logger
-from scrapy_util.utils import ScrapydUtil
-
+import os
 
 class StatsCollectorExtension(object):
     """
     日志记录扩展
     """
     DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -35,21 +34,18 @@
     def spider_closed(self, spider, reason):
         stats = spider.crawler.stats.get_stats()
 
         # 获取数据
         start_time = stats.get("start_time")
         finish_time = stats.get("finish_time")
         duration = (finish_time - start_time).seconds
-
         # 保存收集到的信息
-        result = ScrapydUtil.parse_log_file(self.log_file)
-
         item = {
-            "job_id": result.get('job_id', ''),
-            "project": result.get('project', ''),
+            "job_id": os.environ.get("SCRAPYD_JOB",""),
+            "project": os.environ.get("SCRAPY_PROJECT",""),
             "spider": spider.name,
             "item_scraped_count": stats.get("item_scraped_count", 0),
             "item_dropped_count": stats.get("item_dropped_count", 0),
             "start_time": start_time.strftime(self.DATETIME_FORMAT),
             "finish_time": finish_time.strftime(self.DATETIME_FORMAT),
             "duration": duration,
             "finish_reason": stats.get("finish_reason"),
```

### Comparing `scrapy-util-0.0.9/scrapy_util/middlewares/dont_request_downloader_middleware.py` & `scrapy-util-1.0.2/scrapy_util/middlewares/dont_request_downloader_middleware.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-0.0.9/scrapy_util/spiders/script_spider.py` & `scrapy-util-1.0.2/scrapy_util/spiders/script_spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from scrapy import Spider
 
 from scrapy_util.items.trick_item import TrickItem
 
 
 class ScriptSpider(Spider):
     """继承该类，用于仅做脚本执行，Request 不请求网络"""
-    name = 'base_script'
-
     start_urls = ['https://www.baidu.com/']
 
     custom_settings = {
         'DOWNLOADER_MIDDLEWARES': {
             # 脚本直接返回，不进行网络请求 Middleware
             'scrapy_util.middlewares.DontRequestDownloaderMiddleware': 100,
```

### Comparing `scrapy-util-0.0.9/scrapy_util/utils.py` & `scrapy-util-1.0.2/scrapy_util/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
-
+import os
 
 class ScrapydUtil(object):
 
     @classmethod
     def parse_log_file(cls, log_file):
         """
         通过scrapyd调度才会有 LOG_FILE 参数
 
         LOG_FILE: logs/project/spider/e007e2085fe011ebab89acde48001122.log
         :return:
         """
         if log_file:
-            _, project, spider, filename = log_file.split('/')
-            job_id, _ = filename.split('.')
+            _, project, spider, filename = log_file.split(os.sep)
+            job_id, _ = os.path.spiltext(filename)
 
         else:
             project = ''
             spider = ''
             job_id = ''
 
         return {
```

### Comparing `scrapy-util-0.0.9/scrapy_util.egg-info/SOURCES.txt` & `scrapy-util-1.0.2/scrapy_util.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 scrapy_util/__init__.py
 scrapy_util/logger.py
 scrapy_util/utils.py
+scrapy_util/version.py
 scrapy_util.egg-info/PKG-INFO
 scrapy_util.egg-info/SOURCES.txt
 scrapy_util.egg-info/dependency_links.txt
 scrapy_util.egg-info/requires.txt
 scrapy_util.egg-info/top_level.txt
 scrapy_util.egg-info/zip-safe
 scrapy_util/extensions/__init__.py
 scrapy_util/extensions/localtime_core_stats.py
 scrapy_util/extensions/show_duration_extension.py
 scrapy_util/extensions/stats_collector_extension.py
 scrapy_util/items/__init__.py
+scrapy_util/items/mongo_item.py
 scrapy_util/items/trick_item.py
 scrapy_util/middlewares/__init__.py
 scrapy_util/middlewares/dont_request_downloader_middleware.py
+scrapy_util/pipelines/__init__.py
+scrapy_util/pipelines/mongo_pipeline.py
 scrapy_util/spiders/__init__.py
-scrapy_util/spiders/script_spider.py
+scrapy_util/spiders/list_next_request_spider.py
+scrapy_util/spiders/list_spider.py
+scrapy_util/spiders/script_spider.py
+tests/__init__.py
+tests/test_hello.py
```

### Comparing `scrapy-util-0.0.9/setup.py` & `scrapy-util-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 
 # @Date    : 2019-06-26
 # @Author  : Peng Shiyu
-
+import glob
 import io
 import os
 
+import six
 from setuptools import setup, find_packages
 
 """
 ## 本地测试
 安装测试
 python setup.py install 
-python setup.py develop 
+python setup.py develop
+
+python setup.py develop --uninstall 
 
 卸载
 pip uninstall scrapy-util -y
 
 
 ## 打包上传
 先升级打包工具
@@ -45,30 +48,36 @@
 打包的用的setup必须引入
 
 参考：
 https://packaging.python.org/guides/making-a-pypi-friendly-readme/
 
 """
 
-base_dir = os.path.dirname(os.path.abspath(__file__))
+# 版本号
+version_file = glob.glob("*/version.py", recursive=True)[0]
 
-version = '0.0.9'
+with io.open(version_file, 'rb') as f:
+    version_var = {}
+    six.exec_(f.read(), version_var)
+    VERSION = version_var['VERSION']
 
+# 说明
 with io.open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
+# 依赖
 with io.open("requirements.txt", 'r') as f:
-    install_requires = f.read().split(os.sep)
+    install_requires = f.read().split(os.linesep)
 
 setup(
     name='scrapy-util',
-    version=version,
+    version=VERSION,
     description="scrapy util",
 
-    keywords='spider admin',
+    keywords='spider,admin',
     author='Peng Shiyu',
     author_email='pengshiyuyx@gmail.com',
     license='MIT',
     url="https://github.com/mouday/scrapy-util",
 
     long_description=long_description,
     long_description_content_type='text/markdown',
```

