# Comparing `tmp/cn_stats-0.0.8.tar.gz` & `tmp/cn_stats-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cn_stats-0.0.8.tar", last modified: Tue Mar 26 02:01:00 2024, max compression
+gzip compressed data, was "cn_stats-0.0.9.tar", last modified: Thu Apr 11 04:44:41 2024, max compression
```

## Comparing `cn_stats-0.0.8.tar` & `cn_stats-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2024-03-26 02:01:00.218219 cn_stats-0.0.8/
--rw-rw-r--   0 sj        (1000) sj        (1000)     1059 2024-03-26 00:57:49.000000 cn_stats-0.0.8/LICENSE
--rw-rw-r--   0 sj        (1000) sj        (1000)    30127 2024-03-26 02:01:00.218219 cn_stats-0.0.8/PKG-INFO
--rw-rw-r--   0 sj        (1000) sj        (1000)    29667 2024-03-26 01:56:44.000000 cn_stats-0.0.8/README.md
-drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2024-03-26 02:01:00.218219 cn_stats-0.0.8/cn_stats.egg-info/
--rw-rw-r--   0 sj        (1000) sj        (1000)    30127 2024-03-26 02:01:00.000000 cn_stats-0.0.8/cn_stats.egg-info/PKG-INFO
--rw-rw-r--   0 sj        (1000) sj        (1000)      297 2024-03-26 02:01:00.000000 cn_stats-0.0.8/cn_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 sj        (1000) sj        (1000)        1 2024-03-26 02:01:00.000000 cn_stats-0.0.8/cn_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 sj        (1000) sj        (1000)       31 2024-03-26 02:01:00.000000 cn_stats-0.0.8/cn_stats.egg-info/requires.txt
--rw-rw-r--   0 sj        (1000) sj        (1000)        8 2024-03-26 02:01:00.000000 cn_stats-0.0.8/cn_stats.egg-info/top_level.txt
-drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2024-03-26 02:01:00.218219 cn_stats-0.0.8/cnstats/
--rw-rw-r--   0 sj        (1000) sj        (1000)        0 2023-01-06 06:03:41.000000 cn_stats-0.0.8/cnstats/__init__.py
--rw-rw-r--   0 sj        (1000) sj        (1000)     1812 2024-03-26 01:31:45.000000 cn_stats-0.0.8/cnstats/__main__.py
--rw-rw-r--   0 sj        (1000) sj        (1000)     1195 2024-03-26 01:56:21.000000 cn_stats-0.0.8/cnstats/common.py
--rw-rw-r--   0 sj        (1000) sj        (1000)      353 2024-03-26 00:57:49.000000 cn_stats-0.0.8/cnstats/regcode.py
--rw-rw-r--   0 sj        (1000) sj        (1000)     1767 2024-03-26 01:56:33.000000 cn_stats-0.0.8/cnstats/stats.py
--rw-rw-r--   0 sj        (1000) sj        (1000)      273 2024-03-25 05:08:41.000000 cn_stats-0.0.8/cnstats/zbcode.py
--rw-rw-r--   0 sj        (1000) sj        (1000)       38 2024-03-26 02:01:00.218219 cn_stats-0.0.8/setup.cfg
--rw-rw-r--   0 sj        (1000) sj        (1000)     1740 2024-03-26 01:59:50.000000 cn_stats-0.0.8/setup.py
+drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2024-04-11 04:44:41.665107 cn_stats-0.0.9/
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1059 2024-03-25 23:59:30.000000 cn_stats-0.0.9/LICENSE
+-rw-rw-r--   0 sj        (1000) sj        (1000)    30127 2024-04-11 04:44:41.665107 cn_stats-0.0.9/PKG-INFO
+-rw-rw-r--   0 sj        (1000) sj        (1000)    29667 2024-03-27 12:36:12.000000 cn_stats-0.0.9/README.md
+drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2024-04-11 04:44:41.665107 cn_stats-0.0.9/cn_stats.egg-info/
+-rw-rw-r--   0 sj        (1000) sj        (1000)    30127 2024-04-11 04:44:41.000000 cn_stats-0.0.9/cn_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 sj        (1000) sj        (1000)      297 2024-04-11 04:44:41.000000 cn_stats-0.0.9/cn_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 sj        (1000) sj        (1000)        1 2024-04-11 04:44:41.000000 cn_stats-0.0.9/cn_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 sj        (1000) sj        (1000)       31 2024-04-11 04:44:41.000000 cn_stats-0.0.9/cn_stats.egg-info/requires.txt
+-rw-rw-r--   0 sj        (1000) sj        (1000)        8 2024-04-11 04:44:41.000000 cn_stats-0.0.9/cn_stats.egg-info/top_level.txt
+drwxrwxr-x   0 sj        (1000) sj        (1000)        0 2024-04-11 04:44:41.665107 cn_stats-0.0.9/cnstats/
+-rw-rw-r--   0 sj        (1000) sj        (1000)        0 2024-03-24 07:21:14.000000 cn_stats-0.0.9/cnstats/__init__.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1812 2024-03-27 12:36:12.000000 cn_stats-0.0.9/cnstats/__main__.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1195 2024-03-25 22:35:05.000000 cn_stats-0.0.9/cnstats/common.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)      353 2024-03-25 23:33:57.000000 cn_stats-0.0.9/cnstats/regcode.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1767 2024-04-08 00:23:00.000000 cn_stats-0.0.9/cnstats/stats.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)      273 2024-03-25 22:35:05.000000 cn_stats-0.0.9/cnstats/zbcode.py
+-rw-rw-r--   0 sj        (1000) sj        (1000)       38 2024-04-11 04:44:41.665107 cn_stats-0.0.9/setup.cfg
+-rw-rw-r--   0 sj        (1000) sj        (1000)     1740 2024-04-11 04:39:52.000000 cn_stats-0.0.9/setup.py
```

### Comparing `cn_stats-0.0.8/LICENSE` & `cn_stats-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.8/PKG-INFO` & `cn_stats-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn_stats
-Version: 0.0.8
+Version: 0.0.9
 Summary: 获取中国国家统计局网站数据。
 Home-page: https://github.com/songjian/cnstats
 Author: sj
 Author-email: 724385768@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cn_stats-0.0.8/README.md` & `cn_stats-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.8/cn_stats.egg-info/PKG-INFO` & `cn_stats-0.0.9/cn_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn-stats
-Version: 0.0.8
+Version: 0.0.9
 Summary: 获取中国国家统计局网站数据。
 Home-page: https://github.com/songjian/cnstats
 Author: sj
 Author-email: 724385768@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cn_stats-0.0.8/cnstats/__main__.py` & `cn_stats-0.0.9/cnstats/__main__.py`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.8/cnstats/common.py` & `cn_stats-0.0.9/cnstats/common.py`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.8/cnstats/stats.py` & `cn_stats-0.0.9/cnstats/stats.py`

 * *Files identical despite different names*

### Comparing `cn_stats-0.0.8/setup.py` & `cn_stats-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cn_stats",                                     # 包的分发名称，使用字母、数字、_、-
-    version="0.0.8",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="0.0.9",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="sj",                                       # 作者名字
     author_email="724385768@qq.com",                      # 作者邮箱
     description="获取中国国家统计局网站数据。",                            # 包的简介描述
     long_description=long_description,                      # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",          # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/songjian/cnstats",                              # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),                    # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     classifiers=[                                           # 关于包的其他元数据(metadata)
         "Programming Language :: Python :: 3",              # 该软件包仅与Python3兼容
         "License :: OSI Approved :: MIT License",           # 根据MIT许可证开源
         "Operating System :: OS Independent",               # 与操作系统无关
     ],
-    install_requires=['requests==2.28.1', 'pandas==1.4.1'],  # 依赖的包
+    install_requires=['requests>=2.28.1', 'pandas>=1.4.1'],  # 依赖的包
     python_requires='>=3'
 )
```

