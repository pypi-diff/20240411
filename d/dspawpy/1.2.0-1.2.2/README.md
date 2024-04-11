# Comparing `tmp/dspawpy-1.2.0.tar.gz` & `tmp/dspawpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspawpy-1.2.0.tar", last modified: Wed Apr  3 03:28:37 2024, max compression
+gzip compressed data, was "dspawpy-1.2.2.tar", last modified: Thu Apr 11 08:22:12 2024, max compression
```

## Comparing `dspawpy-1.2.0.tar` & `dspawpy-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.102995 dspawpy-1.2.0/
--rw-r--r--   0 zzl       (1000) zzl       (1000)     1055 2024-01-26 06:56:39.000000 dspawpy-1.2.0/LICENSE.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-03 03:28:37.101997 dspawpy-1.2.0/PKG-INFO
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11295 2024-04-03 02:00:28.000000 dspawpy-1.2.0/README.md
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.069995 dspawpy-1.2.0/dspawpy/
--rw-r--r--   0 zzl       (1000) zzl       (1000)       46 2024-04-03 03:27:54.000000 dspawpy-1.2.0/dspawpy/__init__.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.079993 dspawpy-1.2.0/dspawpy/analysis/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.0/dspawpy/analysis/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    29688 2024-03-27 08:59:24.000000 dspawpy-1.2.0/dspawpy/analysis/aimdtools.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    19672 2024-03-27 09:01:23.000000 dspawpy-1.2.0/dspawpy/analysis/vacf.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.083994 dspawpy-1.2.0/dspawpy/cli/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2024-01-26 06:56:39.000000 dspawpy-1.2.0/dspawpy/cli/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    63725 2024-03-28 10:00:18.000000 dspawpy-1.2.0/dspawpy/cli/cli.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    63408 2024-03-28 10:01:36.000000 dspawpy-1.2.0/dspawpy/cli/cli_en.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.089997 dspawpy-1.2.0/dspawpy/diffusion/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.0/dspawpy/diffusion/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)     3718 2024-03-27 02:02:22.000000 dspawpy-1.2.0/dspawpy/diffusion/neb.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    60374 2024-03-28 02:11:43.000000 dspawpy-1.2.0/dspawpy/diffusion/nebtools.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    10749 2024-03-27 09:26:05.000000 dspawpy-1.2.0/dspawpy/diffusion/pathfinder.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.095999 dspawpy-1.2.0/dspawpy/io/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.0/dspawpy/io/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    62177 2024-04-03 02:00:11.000000 dspawpy-1.2.0/dspawpy/io/read.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    26244 2024-03-27 09:31:14.000000 dspawpy-1.2.0/dspawpy/io/structure.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    33242 2024-03-27 09:28:27.000000 dspawpy-1.2.0/dspawpy/io/utils.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    27196 2024-03-27 09:29:46.000000 dspawpy-1.2.0/dspawpy/io/write.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    48744 2024-04-03 02:35:54.000000 dspawpy-1.2.0/dspawpy/plot.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.097998 dspawpy-1.2.0/dspawpy.egg-info/
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/PKG-INFO
--rw-r--r--   0 zzl       (1000) zzl       (1000)      626 2024-04-03 03:28:37.000000 dspawpy-1.2.0/dspawpy.egg-info/SOURCES.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)        1 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/dependency_links.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       76 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/entry_points.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       64 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/requires.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)        8 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/top_level.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       38 2024-04-03 03:28:37.102995 dspawpy-1.2.0/setup.cfg
--rw-r--r--   0 zzl       (1000) zzl       (1000)     1308 2024-04-03 03:28:00.000000 dspawpy-1.2.0/setup.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.338863 dspawpy-1.2.2/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)     1055 2024-01-26 06:56:39.000000 dspawpy-1.2.2/LICENSE.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-11 08:22:12.336866 dspawpy-1.2.2/PKG-INFO
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    11526 2024-04-11 08:13:27.000000 dspawpy-1.2.2/README.md
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.294652 dspawpy-1.2.2/dspawpy/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       46 2024-04-11 08:22:10.000000 dspawpy-1.2.2/dspawpy/__init__.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.308867 dspawpy-1.2.2/dspawpy/analysis/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.2/dspawpy/analysis/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    29688 2024-03-27 08:59:24.000000 dspawpy-1.2.2/dspawpy/analysis/aimdtools.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    19672 2024-03-27 09:01:23.000000 dspawpy-1.2.2/dspawpy/analysis/vacf.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.312867 dspawpy-1.2.2/dspawpy/cli/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2024-01-26 06:56:39.000000 dspawpy-1.2.2/dspawpy/cli/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    65500 2024-04-11 08:13:27.000000 dspawpy-1.2.2/dspawpy/cli/cli.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    65297 2024-04-11 08:13:27.000000 dspawpy-1.2.2/dspawpy/cli/cli_en.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.321865 dspawpy-1.2.2/dspawpy/diffusion/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.2/dspawpy/diffusion/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)     3718 2024-03-27 02:02:22.000000 dspawpy-1.2.2/dspawpy/diffusion/neb.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    60374 2024-03-28 02:11:43.000000 dspawpy-1.2.2/dspawpy/diffusion/nebtools.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    10749 2024-03-27 09:26:05.000000 dspawpy-1.2.2/dspawpy/diffusion/pathfinder.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.331862 dspawpy-1.2.2/dspawpy/io/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.2/dspawpy/io/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    62058 2024-04-10 09:19:19.000000 dspawpy-1.2.2/dspawpy/io/read.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    26244 2024-03-27 09:31:14.000000 dspawpy-1.2.2/dspawpy/io/structure.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    33242 2024-03-27 09:28:27.000000 dspawpy-1.2.2/dspawpy/io/utils.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    27196 2024-03-27 09:29:46.000000 dspawpy-1.2.2/dspawpy/io/write.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    48744 2024-04-11 08:13:21.000000 dspawpy-1.2.2/dspawpy/plot.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.332863 dspawpy-1.2.2/dspawpy.egg-info/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/PKG-INFO
+-rw-r--r--   0 zzl       (1000) zzl       (1000)      626 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/SOURCES.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        1 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/dependency_links.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       76 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/entry_points.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       64 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/requires.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        8 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/top_level.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       38 2024-04-11 08:22:12.338863 dspawpy-1.2.2/setup.cfg
+-rw-r--r--   0 zzl       (1000) zzl       (1000)     1308 2024-04-11 08:22:10.000000 dspawpy-1.2.2/setup.py
```

### Comparing `dspawpy-1.2.0/LICENSE.txt` & `dspawpy-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/PKG-INFO` & `dspawpy-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.2.0
+Version: 1.2.2
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dspawpy-1.2.0/README.md` & `dspawpy-1.2.2/dspawpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: dspawpy
+Version: 1.2.2
+Summary: Tools for dspaw
+Home-page: http://www.hzwtech.com/
+Author: Hzwtech
+Author-email: ZhengZhilin@hzwtech.com
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pymatgen>=2022.2.7
+Requires-Dist: statsmodels
+Requires-Dist: h5py
+Requires-Dist: monty
+Requires-Dist: prompt_toolkit
+Requires-Dist: loguru
+
 ![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
 ![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
 ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # Introduction （简介）
 
 dspawpy is a post-processing tool mainly for DFT package [DS-PAW](https://cloud.hzwtech.com/web/product-service?id=10), providing some functions of data capture, conversion, structure conversion, and drawing. （dspawpy 主要是 [DS-PAW](https://cloud.hzwtech.com/web/product-service?id=10) 软件的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能）
```

### Comparing `dspawpy-1.2.0/dspawpy/analysis/aimdtools.py` & `dspawpy-1.2.2/dspawpy/analysis/aimdtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/analysis/vacf.py` & `dspawpy-1.2.2/dspawpy/analysis/vacf.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/cli/cli.py` & `dspawpy-1.2.2/dspawpy/cli/cli.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1775 +1,1775 @@
-# -*- coding: utf-8 -*-
-import time
-
-main_menu = """
-1: dspawpy更新 
-2: structure结构转化
-3: volumetricData数据处理
-4: band能带数据处理
-5: dos态密度数据处理
-6: bandDos能带和态密度共同显示
-7: optical光学性质数据处理
-8: neb过渡态计算数据处理
-9: phonon声子计算数据处理
-10: aimd分子动力学模拟数据处理
-11: Polarization铁电极化数据处理
-12: ZPE零点振动能数据处理
-13: TS的热校正能
---> 输入数字后回车选择功能："""
-
-menu3 = """
-=== 3 volumetricData数据处理 ===
-
-  1: volumetricData可视化
-  2: 差分volumetricData可视化
-  3: volumetricData面平均
-  
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-
-menu4 = """
-=== 4 band能带数据处理 ===
-
-  1: 普通能带
-  2: 将能带投影到每一种元素分别作图，数据点大小表示该元素对该轨道的贡献
-  3: 能带投影到不同元素的不同轨道
-  4: 将能带投影到不同原子的不同轨道
-  5: 能带反折叠处理
-  6. band-compare能带对比图处理
-  
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-menu5 = """
-=== 5 dos态密度数据处理 ===
-
-  1: 总的态密度
-  2: 将态密度投影到不同的轨道上
-  3: 将态密度投影到不同的元素上
-  4: 将态密度投影到不同原子的不同轨道上
-  5: 将态密度投影到不同原子的分裂d轨道(t2g, eg)上
-  6: d-带中心分析
-  
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-menu6 = """
-=== 6 bandDos能带和态密度共同显示 ===
-
-  1: 将能带和态密度显示在一张图上
-  2: 将能带和投影态密度显示在一张图上
-
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-menu8 = """
-=== 8 neb过渡态计算数据处理 ===
-
-  1: 输入文件之生成中间构型
-  2: 绘制能垒图
-  3: 过渡态计算概览
-  4: NEB链可视化
-  5: 计算构型间距
-  6: neb续算
-
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-menu9 = """
-=== 9 phonon声子计算数据处理 ===
-
-  1: 声子能带数据处理
-  2: 声子态密度数据处理
-  3: 声子热力学数据处理
-
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-menu10 = """
-=== 10 aimd分子动力学模拟数据处理 ===
-
-  1: 轨迹文件转换格式为.xyz或.dump
-  2: 动力学过程中能量、温度等变化曲线
-  3: 均方位移（MSD）
-  4. 均方根偏差（RMSD）
-  5. 径向分布函数（RDF）
-
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-menu13 = """
-=== 13 TS的热校正能 ===
-
-  1: 吸附质
-  2: 理想气体
-
-  0: 返回主菜单
-  --> 输入数字后回车选择功能："""
-
-import os  # noqa: E402
-from argparse import ArgumentParser  # noqa: E402
-
-argparser = ArgumentParser("dspawpy命令行交互小工具")
-argparser.add_argument(
-    "-q", "--quick", action="store_true", help="不联网检查dspawpy版本"
-)
-argparser.add_argument(
-    "-c", "--clean", action="store_true", help="不显示dspawpy_logo，直接显示菜单"
-)
-args = argparser.parse_args()
-
-
-def online_check(dv, df):
-    latest_version = None
-    try:  # 如果正常导入dspawpy，应当有 requests库（pymatgen和mp-api的依赖）
-        print("正在联网检查dspawpy版本... 使用 -q 参数启动此程序可跳过检查")
-        response = get("https://pypi.org/pypi/dspawpy/json", timeout=3)
-        latest_version = response.json()["info"]["version"]
-        error_message = None
-    except ImportError:
-        error_message = "无法导入 requests 库"
-    except exceptions.Timeout:
-        error_message = "requests联网检查dspawpy版本超时"
-    except exceptions.RequestException as e:
-        error_message = f"requests联网检查dspawpy版本时出现异常: {e}"
-    except Exception as e:
-        error_message = f"联网检查dspawpy版本失败: {e}"
-    finally:
-        if latest_version:
-            if latest_version != dv:
-                print(
-                    f"\n 成功导入 {dv}（不是最新版本 {latest_version}），可尝试使用功能1升级"
-                )
-                print(
-                    f" 导入的dspawpy模块文件路径为（如果不符合预期，请检查环境变量)：\n {df}\n"
-                )
-            else:
-                print(f"\n         成功导入 {dv}（最新版）dspawpy\n")
-
-            with open(os.path.expanduser("~/.dspawpy_latest_version"), "w") as fin:
-                fin.write(latest_version)
-        else:
-            print(f"\n         成功导入 {dv}（无法联网检查最新版本）dspawpy\n")
-
-    return error_message
-
-
-def verify_dspawpy_version(skip=False):
-    error_message = None
-    try:
-        import dspawpy
-
-        try:
-            dv = dspawpy.__version__
-        except Exception:  # 老版本没有__version__属性
-            dv = "??? 版本过老，无法检测"
-        finally:
-            df = os.path.dirname(dspawpy.__file__)
-
-        if skip:
-            print(f"\n         成功导入 dspawpy={dv}\n")
-        else:
-            # 检查是否存在 ~/.dspawpy_latest_version 文件，存在则读取其中写的版本号信息
-            # 如果不存在，或者读取失败，则联网检查最新版本，并在检查成功后写入 ~/.dspawpy_latest_version 文件
-            if os.path.isfile(os.path.expanduser("~/.dspawpy_latest_version")):
-                with open(os.path.expanduser("~/.dspawpy_latest_version"), "r") as fin:
-                    latest_version = fin.read().strip()
-                if dv == latest_version:
-                    print(f"\n         成功导入 {dv}（最新版）dspawpy\n")
-                else:
-                    error_message = online_check(dv, df)
-            else:
-                error_message = online_check(dv, df)
-
-    except ImportError:
-        print("     我们检测到您并未安装dspawpy，试试菜单1快速安装吧     ")
-    except Exception as e:
-        error_message = f"导入dspawpy失败: {e}"
-
-    print("********这是dspawpy命令行交互小工具，预祝您使用愉快********")
-    if error_message is not None:
-        print(error_message)
-
-
-def collect_user_input() -> list:
-    """让用户选择功能，这一步不用记录日志，直接打印提示信息"""
-
-    if args.clean:  # 不显示 dspawpy_logo
-        dspawpy_logo = ""
-    else:
-        dspawpy_logo = r"""
-********这是dspawpy命令行交互小工具，预祝您使用愉快********
-    ( )
-   _| |  ___  _ _      _ _  _   _   _  _ _    _   _
- /'_` |/',__)( '_`\  /'_` )( ) ( ) ( )( '_`\ ( ) ( )
-( (_| |\__, \| (_) )( (_| || \_/ \_/ || (_) )| (_) |
-`\__,_)(____/| ,__/'`\__,_)`\___x___/'| ,__/'`\__, |
-             | |                      | |    ( )_| |
-             (_)                      (_)    `\___/'
-"""
-    print(dspawpy_logo)
-
-    if args.quick:
-        iskip = True
-    else:
-        iskip = False
-
-    verify_dspawpy_version(skip=iskip)
-
-    while True:  # 主菜单选择
-        n = input(main_menu)
-        if n == "1":  # 环境部署比较特殊，不要进入主程序
-            cmd = "pip install dspawpy --user -i https://pypi.tuna.tsinghua.edu.cn/simple && pip install -U dspawpy -i https://pypi.org/simple --user"
-            while True:
-                yn = input(f"更新dspawpy将执行\n {cmd}\n (y/n)? ")
-                if yn.lower() == "y":
-                    if os.system(cmd) == 0:
-                        print(">>>>>> 执行成功")
-                        print("请重新运行程序，使安装生效")
-                    else:
-                        print("!!!!!! 执行失败")
-                    break
-                elif yn.lower() == "n":
-                    print("###### 放弃执行")
-                    break
-                else:
-                    print("!!! 输入错误，请重试")
-                    continue
-
-        elif n == "2":
-            return 2, 0
-
-        elif n == "3":
-            while True:
-                n = input(menu3)
-                if n not in ["0", "1", "2", "3"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 3, 1
-                elif n == "2":
-                    return 3, 2
-                elif n == "3":
-                    return 3, 3
-                else:
-                    break
-            if n == "0":
-                continue
-            break
-
-        elif n == "4":
-            while True:
-                n = input(menu4)
-                if n not in ["0", "1", "2", "3", "4", "5", "6"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 4, 1
-                elif n == "2":
-                    return 4, 2
-                elif n == "3":
-                    return 4, 3
-                elif n == "4":
-                    return 4, 4
-                elif n == "5":
-                    return 4, 5
-                elif n == "6":
-                    return 4, 6
-                else:
-                    break
-            if n == "0":
-                continue
-            break
-
-        elif n == "5":
-            while True:
-                n = input(menu5)
-                if n not in ["0", "1", "2", "3", "4", "5", "6"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 5, 1
-                elif n == "2":
-                    return 5, 2
-                elif n == "3":
-                    return 5, 3
-                elif n == "4":
-                    return 5, 4
-                elif n == "5":
-                    return 5, 5
-                elif n == "6":
-                    return 5, 6
-                else:
-                    break
-
-            if n == "0":
-                continue
-            break
-
-        elif n == "6":
-            while True:
-                n = input(menu6)
-                if n not in ["0", "1", "2"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 6, 1
-                elif n == "2":
-                    return 6, 2
-                else:
-                    break
-            if n == "0":
-                continue
-            break
-
-        elif n == "7":
-            return 7, 0
-        elif n == "8":
-            while True:
-                n = input(menu8)
-                if n not in ["0", "1", "2", "3", "4", "5", "6"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":  # 插值
-                    return 8, 1
-                elif n == "2":  # 能垒图
-                    return 8, 2
-                elif n == "3":  # 总结
-                    return 8, 3
-                elif n == "4":  # 可视化链
-                    return 8, 4
-                elif n == "5":  # 计算距离
-                    return 8, 5
-                elif n == "6":  # 重启
-                    return 8, 6
-                else:
-                    break
-            if n == "0":
-                continue
-            break
-
-        elif n == "9":
-            while True:
-                n = input(menu9)
-                if n not in ["0", "1", "2", "3"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 9, 1
-                elif n == "2":
-                    return 9, 2
-                elif n == "3":
-                    return 9, 3
-                else:
-                    break
-
-            if n == "0":
-                continue
-            break
-
-        elif n == "10":
-            while True:
-                n = input(menu10)
-                if n not in ["0", "1", "2", "3", "4", "5"]:
-                    print("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 10, 1
-                elif n == "2":
-                    return 10, 2
-                elif n == "3":
-                    return 10, 3
-                elif n == "4":
-                    return 10, 4
-                elif n == "5":
-                    return 10, 5
-                else:
-                    break
-
-            if n == "0":
-                continue
-            break
-
-        elif n == "11":
-            return 11, 0
-
-        elif n == "12":
-            return 12, 0
-
-        elif n == "13":
-            while True:
-                n = input(menu13)
-                if n not in ["0", "1", "2"]:
-                    logger.error("!!! 输入错误，请重试")
-                    continue
-                elif n == "1":
-                    return 13, 1
-                elif n == "2":
-                    return 13, 2
-                else:
-                    break
-            if n == "0":
-                continue
-            break
-
-        else:
-            print("XXXXXX 输入错误，请重试 XXXXXX")
-            continue
-
-
-from multiprocessing.pool import ThreadPool  # noqa: E402
-
-from requests import exceptions, get  # noqa: E402
-
-pool = ThreadPool(processes=1)
-async_result = pool.apply_async(collect_user_input)
-
-
-def main():
-    """run specific task by user selected task number"""
-    # print('entering main...') # uncomment this to see the speed impact
-    task_number = async_result.get()
-    time.sleep(3)
-    pool.close()
-    # print('got task number') # uncomment this to see the speed impact
-    tasks = Tasks()
-    if task_number[0] == 2:
-        tasks.s2()
-
-    elif task_number == (3, 1):
-        tasks.s3_1()
-    elif task_number == (3, 2):
-        tasks.s3_2()
-    elif task_number == (3, 3):
-        tasks.s3_3()
-
-    elif task_number[0] == 4:  # band
-        if task_number[1] != 6:
-            infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-            ylims = check_lims(
-                "输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）："
-            )
-            outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
-        if task_number[1] == 1:  # band
-            tasks.s4_1(infile, ylims, outfile)
-        elif task_number[1] == 2:  # band-proj
-            tasks.s4_2(infile, ylims, outfile)
-        elif task_number[1] == 3:  # band-proj-element
-            tasks.s4_3(infile, ylims, outfile)
-        elif task_number[1] == 4:  # band-proj-site
-            tasks.s4_4(infile, ylims, outfile)
-        elif task_number[1] == 5:  # band-unfold
-            tasks.s4_5(infile, ylims, outfile)
-        elif task_number[1] == 6:  # band-compare
-            tasks.s4_6()
-
-    elif task_number[0] == 5:  # dos
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        from dspawpy.io.read import get_dos_data
-
-        dosdata = get_dos_data(infile)
-        from pymatgen.electronic_structure.plotter import DosPlotter
-
-        dos_plotter = DosPlotter(stack=False, zero_at_efermi=True)
-        if task_number[1] != 6:
-            xlims = check_lims(
-                "输入x轴范围（先小后大，以空格分隔，直接回车可跳过设置）："
-            )
-            ylims = check_lims(
-                "输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）："
-            )
-            outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
-        if task_number[1] == 1:  # tdos
-            tasks.s5_1(dosdata, dos_plotter, xlims, ylims, outfile)
-        elif task_number[1] == 2:
-            tasks.s5_2(dosdata, dos_plotter, xlims, ylims, outfile)
-        elif task_number[1] == 3:
-            tasks.s5_3(dosdata, dos_plotter, xlims, ylims, outfile)
-        elif task_number[1] == 4:
-            tasks.s5_4(dosdata, dos_plotter, xlims, ylims, outfile)
-        elif task_number[1] == 5:
-            tasks.s5_5(dosdata, dos_plotter, xlims, ylims, outfile)
-        elif task_number[1] == 6:
-            tasks.s5_6(dosdata)
-
-    elif task_number[0] == 6:
-        infile1 = prompt("待解析能带band文件路径（包含文件名）：", completer=pc)
-        infile2 = prompt("待解析态密度dos文件路径（包含文件名）：", completer=pc)
-        ylims = check_lims("输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）：")
-        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
-        if task_number[1] == 1:
-            tasks.s6_1(infile1, infile2, ylims, outfile)
-        else:
-            tasks.s6_2(infile1, infile2, ylims, outfile)
-
-    elif task_number[0] == 7:
-        tasks.s7()
-
-    elif task_number[0] == 8:
-        if task_number[1] == 1:
-            tasks.s8_1()
-        elif task_number[1] == 2:
-            tasks.s8_2()
-        elif task_number[1] == 3:
-            tasks.s8_3()
-        elif task_number[1] == 4:
-            tasks.s8_4()
-        elif task_number[1] == 5:
-            tasks.s8_5()
-        elif task_number[1] == 6:
-            tasks.s8_6()
-
-    elif task_number[0] == 9:
-        if task_number[1] == 1:
-            tasks.s9_1()
-        elif task_number[1] == 2:
-            tasks.s9_2()
-        elif task_number[1] == 3:
-            tasks.s9_3()
-
-    elif task_number[0] == 10:
-        if task_number[1] == 1:
-            tasks.s10_1()
-        elif task_number[1] == 2:
-            tasks.s10_2()
-        elif task_number[1] == 3:
-            tasks.s10_3()
-        elif task_number[1] == 4:
-            tasks.s10_4()
-        elif task_number[1] == 5:
-            tasks.s10_5()
-
-    elif task_number[0] == 11:
-        tasks.s11()
-
-    elif task_number[0] == 12:
-        tasks.s12()
-
-    elif task_number[0] == 13:
-        if task_number[1] == 1:
-            tasks.s13_1()
-        elif task_number[1] == 2:
-            tasks.s13_2()
-
-
-import matplotlib  # noqa: E402
-import matplotlib.pyplot as plt  # noqa: E402
-
-matplotlib.use("agg")  # to avoid qt error on some linux servers.
-import sys  # noqa: E402
-
-from prompt_toolkit import prompt  # noqa: E402
-from prompt_toolkit.completion import PathCompleter, WordCompleter, FuzzyCompleter  # noqa: E402
-
-pc = FuzzyCompleter(PathCompleter(expanduser=True))
-
-from loguru import logger  # noqa: E402
-
-logger.remove()
-logger.add(
-    sys.stderr,
-    level="INFO",
-    format="<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <cyan>{message}</cyan>",
-)
-logger.add(
-    ".dspawpycli-debug.log",
-    level="DEBUG",
-    format="{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}",
-)
-
-
-def until_give_valid_input(user_prompt, valid_input, completer=None, allow_empty=False):
-    while True:
-        ns = prompt(user_prompt, completer=completer).strip().split()
-        if allow_empty and len(ns) == 0:
-            return valid_input
-        else:
-            valid = True
-            for n in ns:
-                if n not in valid_input:
-                    print("!!! 输入错误，请重试")
-                    valid = False
-                    break
-            if valid:
-                return ns
-            else:
-                continue
-
-
-def check_lims(user_prompt):
-    # return None or [float, float]
-    while True:
-        userInput = input(user_prompt).strip()
-        if userInput == "":
-            return None
-        else:
-            if " " not in userInput:
-                logger.warning(f"!!! {userInput}没有以空格分隔，请重试")
-                continue
-            elif len(userInput.split(" ")) != 2:
-                logger.warning(f"!!! {userInput}参数长度不为2")
-                continue
-            else:
-                try:
-                    float(userInput.split(" ")[0])
-                    float(userInput.split(" ")[1])
-                    return userInput.split(" ")  # return '1_2'
-                except Exception:
-                    logger.warning(f"!!! {userInput}不全是数字，请重试")
-                    continue
-
-
-class HiddenPrints:
-    def __enter__(self):
-        self._original_stdout = sys.stdout
-        sys.stdout = open(os.devnull, "w")
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        sys.stdout.close()
-        sys.stdout = self._original_stdout
-
-
-class Tasks:
-    @logger.catch
-    def s2(
-        self,
-    ):
-        infile = prompt(
-            "待解析文件路径（包含文件名，支持h5, json, pdb, as, hzw等格式）：",
-            completer=pc,
-        )
-        outfile = prompt(
-            "输出文件路径（包含文件名，支持pdb, xyz, dump, json, as, hzw等格式）：",
-            completer=pc,
-        )
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.structure import convert
-
-        convert(infile=infile, outfile=outfile)
-
-    @logger.catch
-    def s3_1(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
-        task = until_give_valid_input(
-            f"任务类型{_list}：",
-            _list,
-            completer=WordCompleter(_list),
-        )
-
-        subtype = None
-        if task == "potential":
-            if infile.endswith(".h5"):
-                from dspawpy.io.read import load_h5
-
-                data = load_h5(infile)
-                keys = [
-                    k.split("/")[-1] for k in data.keys() if k.startswith("/Potential")
-                ]
-
-                if len(keys) == 0:
-                    raise ValueError(
-                        f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
-                    )
-                elif len(keys) == 1:
-                    subtype = keys[0]
-                else:
-                    subtype = until_give_valid_input(
-                        f"检测到 {keys} 数据集，请选择其中之一：",
-                        keys,
-                        completer=WordCompleter(keys),
-                    )
-
-            elif infile.endswith(".json"):
-                import json
-
-                with open(infile, "r") as fin:
-                    data = json.load(fin)
-                    if "Potential" not in data.keys():
-                        raise ValueError(
-                            f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
-                        )
-                    keys = [k for k in data["Potential"].keys()]
-
-                if len(keys) == 1:
-                    subtype = keys[0]
-                else:
-                    subtype = until_give_valid_input(
-                        f"检测到 {keys} 数据集，请选择其中之一：",
-                        keys,
-                        completer=WordCompleter(keys),
-                    )
-            else:
-                raise ValueError(
-                    f"仅支持h5和json格式，不支持{infile.split('.')[-1]}格式的数据文件！"
-                )
-
-        outfile = prompt(
-            "输出文件路径（包含文件名，支持.cube和.vasp格式）：", completer=pc
-        )
-        if outfile.split(".")[-1].lower() == "cube":
-            cube_or_vasp = "cube"
-        elif (
-            outfile.split(".")[-1].lower() == "vesta"
-            or outfile.split(".")[-1].lower() == "vasp"
-        ):
-            cube_or_vasp = "vesta"
-        else:
-            cube_or_vasp = until_give_valid_input(
-                "请指定输出文件格式（cube, vasp）：", ["cube", "vesta", "vasp"]
-            )
-
-        logger.info("正在处理，请稍等...")
-        from dspawpy.io.write import write_VESTA
-
-        write_VESTA(
-            in_filename=infile,
-            data_type=task,
-            out_filename=outfile,
-            subtype=subtype,
-            format=cube_or_vasp,
-        )
-        logger.info("可直接使用VESTA软件打开")
-
-    @logger.catch
-    def s3_2(
-        self,
-    ):
-        total = prompt("体系总电荷密度文件路径（包含文件名）:", completer=pc)
-        individuals = []
-        while True:
-            individual = prompt(
-                "体系各组分电荷密度文件路径，(包含文件名，直接回车表示停止输入）:",
-                completer=pc,
-            )
-            if individual == "":
-                break
-            individuals.append(individual)
-
-        outfile = prompt(
-            "输出文件路径（包含文件名，支持.cube和.vasp格式）：", completer=pc
-        )
-
-        if outfile.split(".")[-1].lower() == "cube":
-            cube_or_vasp = "cube"
-        elif (
-            outfile.split(".")[-1].lower() == "vesta"
-            or outfile.split(".")[-1].lower() == "vasp"
-        ):
-            cube_or_vasp = "vesta"
-        else:
-            cube_or_vasp = until_give_valid_input(
-                "请指定输出文件格式（cube, vesta）：", ["cube", "vesta", "vasp"]
-            )
-
-        logger.info("正在处理，请稍等...")
-        from dspawpy.io.write import write_delta_rho_vesta
-
-        write_delta_rho_vesta(
-            total=total, individuals=individuals, output=outfile, format=cube_or_vasp
-        )
-        logger.info("可直接使用VESTA软件打开")
-
-    @logger.catch
-    def s3_3(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        axes = until_give_valid_input("沿哪些轴平均（0, 1, 2）：", ["0", "1", "2"])
-        _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
-        task = until_give_valid_input(
-            f"任务类型{_list}：",
-            _list,
-            completer=WordCompleter(_list),
-        )
-        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
-
-        subtype = None
-        if task == "rho":
-            k = "TotalCharge"
-        elif task == "potential":
-            if infile.endswith(".h5"):
-                from dspawpy.io.read import load_h5
-
-                data = load_h5(infile)
-                keys = [
-                    k.split("/")[-1] for k in data.keys() if k.startswith("/Potential")
-                ]
-
-                if len(keys) == 0:
-                    raise ValueError(
-                        f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
-                    )
-                elif len(keys) == 1:
-                    subtype = keys[0]
-                else:
-                    subtype = until_give_valid_input(
-                        f"检测到 {keys} 数据集，请选择其中之一：",
-                        keys,
-                        completer=WordCompleter(keys),
-                    )
-
-            elif infile.endswith(".json"):
-                import json
-
-                with open(infile, "r") as fin:
-                    data = json.load(fin)
-                    if "Potential" not in data.keys():
-                        raise ValueError(
-                            f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
-                        )
-                    keys = [k for k in data["Potential"].keys()]
-
-                if len(keys) == 1:
-                    subtype = keys[0]
-                else:
-                    subtype = until_give_valid_input(
-                        f"检测到 {keys} 数据集，请选择其中之一：",
-                        keys,
-                        completer=WordCompleter(keys),
-                    )
-            else:
-                raise ValueError(
-                    f"仅支持h5和json格式，不支持{infile.split('.')[-1]}格式的数据文件！"
-                )
-            k = subtype
-        elif task == "elf":
-            k = "TotalELF"
-        elif task == "pcharge":
-            k = "TotalCharge"
-        elif task == "rhoBound":
-            k = "Rho"
-        else:
-            raise ValueError(f"Unknown task: {task}")
-
-        logger.info("正在处理，请稍等...")
-        axes_indices = [int(i) for i in axes.split()]
-        for ai in axes_indices:
-            from dspawpy.plot import average_along_axis
-
-            average_along_axis(infile, axis=ai, label=f"axis{ai}", subtype=subtype)
-        if len(axes_indices) > 1:
-            plt.legend()
-
-        plt.xlabel("Grid Index")
-        plt.ylabel(k)
-        absfile = os.path.abspath(outfile)
-        os.makedirs(os.path.dirname(os.path.abspath(absfile)), exist_ok=True)
-        plt.savefig(absfile, dpi=300)
-
-    @logger.catch
-    def s4_1(self, infile, ylims, outfile):
-        from dspawpy.io.read import get_band_data
-        from pymatgen.electronic_structure.plotter import BSPlotter
-
-        band_data = get_band_data(infile)
-        is_metal = band_data.is_metal()
-        if is_metal:
-            logger.info("正在处理，请稍等...")
-            bsp = BSPlotter(band_data)
-            bsp.get_plot(ylim=ylims)
-        else:
-            while True:
-                shift = input(
-                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
-                )
-                if shift.lower().startswith("y"):
-                    logger.info("正在处理，请稍等...")
-                    from dspawpy.io.read import get_band_data
-
-                    band_data = get_band_data(infile, zero_to_efermi=True)
-                    bsp = BSPlotter(band_data)
-                    bsp.get_plot(False, ylim=ylims)
-                    break
-                elif shift.lower().startswith("n"):
-                    logger.info("正在处理，请稍等...")
-                    bsp = BSPlotter(band_data)
-                    bsp.get_plot(ylim=ylims)
-                    break
-                else:
-                    print("输入有误，请重新输入！")
-                    continue
-
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s4_2(self, infile, ylims, outfile):
-        from dspawpy.io.read import get_band_data
-        from pymatgen.electronic_structure.plotter import BSPlotterProjected
-
-        band_data = get_band_data(infile)
-        is_metal = band_data.is_metal()
-        if is_metal:
-            logger.info("正在处理，请稍等...")
-            bsp = BSPlotterProjected(band_data)
-            bsp.get_elt_projected_plots(ylim=ylims)
-        else:
-            while True:
-                shift = input(
-                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
-                )
-                if shift.lower().startswith("y"):
-                    logger.info("正在处理，请稍等...")
-                    band_data = get_band_data(infile, zero_to_efermi=True)
-                    bsp = BSPlotterProjected(band_data)
-                    bsp.get_elt_projected_plots(False, ylim=ylims)
-                    break
-                elif shift.lower().startswith("n"):
-                    logger.info("正在处理，请稍等...")
-                    bsp = BSPlotterProjected(band_data)
-                    bsp.get_elt_projected_plots(ylim=ylims)
-                    break
-                else:
-                    print("输入有误，请重新输入！")
-                    continue
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s4_3(self, infile, ylims, outfile):
-        from dspawpy.io.read import get_band_data
-        from pymatgen.electronic_structure.plotter import BSPlotterProjected
-
-        band_data = get_band_data(infile)
-        # 获取元素和轨道列表
-        es = band_data.structure.composition.elements
-        for e in es:
-            print("可选元素:", str(e))
-            available_orbitals = ["s"]
-            orbitals = e.atomic_orbitals
-            for o in orbitals:
-                if "p" in o:
-                    available_orbitals.append("p")
-                elif "d" in o:
-                    available_orbitals.append("d")
-                elif "f" in o:
-                    available_orbitals.append("f")
-            unique_orbitals = list(set(available_orbitals))
-            print(f"{str(e)}元素的可选轨道: ", unique_orbitals)
-
-        dictio = {}
-        while True:
-            _e = input("选择一种元素（直接回车表示选择结束）: ")
-            if _e == "":
-                break
-            _o = input(f"选择{_e}元素的原子轨道（用空格分隔）: ")
-            _os = _o.split(" ")
-            dict_eo = {_e: _os}
-            # update dictio
-            dictio.update(dict_eo)
-
-        print("选定的轨道元素字典: ", dictio)
-
-        is_metal = band_data.is_metal()
-        if is_metal:
-            logger.info("正在处理，请稍等...")
-            bsp = BSPlotterProjected(band_data)
-            bsp.get_projected_plots_dots(dictio)
-        else:
-            while True:
-                shift = input(
-                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
-                )
-                if shift.lower().startswith("y"):
-                    logger.info("正在处理，请稍等...")
-                    band_data = get_band_data(infile, zero_to_efermi=True)
-                    bsp = BSPlotterProjected(band_data)
-                    bsp.get_projected_plots_dots(dictio, False, ylim=ylims)
-                    break
-                elif shift.lower().startswith("n"):
-                    logger.info("正在处理，请稍等...")
-                    bsp = BSPlotterProjected(band_data)
-                    bsp.get_projected_plots_dots(dictio, ylim=ylims)
-                    break
-                else:
-                    print("输入有误，请重新输入！")
-                    continue
-
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s4_4(self, infile, ylims, outfile):
-        from dspawpy.io.read import get_band_data
-        from pymatgen.electronic_structure.plotter import BSPlotterProjected
-
-        band_data = get_band_data(infile)
-        print(band_data.structure)
-        es = band_data.structure.composition.elements
-        for e in es:
-            available_orbitals = ["s"]
-            orbitals = e.atomic_orbitals
-            for o in orbitals:
-                if "p" in o:
-                    available_orbitals.append("p")
-                    available_orbitals.append("px")
-                    available_orbitals.append("py")
-                    available_orbitals.append("pz")
-                elif "d" in o:
-                    available_orbitals.append("d")
-                    available_orbitals.append("dxy")
-                    available_orbitals.append("dyz")
-                    available_orbitals.append("dxz")
-                    available_orbitals.append("dx2")
-                    available_orbitals.append("dz2")
-                elif "f" in o:
-                    available_orbitals.append("f")
-                    available_orbitals.append("f_3")
-                    available_orbitals.append("f_2")
-                    available_orbitals.append("f_1")
-                    available_orbitals.append("f0")
-                    available_orbitals.append("f1")
-                    available_orbitals.append("f2")
-                    available_orbitals.append("f3")
-
-            unique_orbitals = list(set(available_orbitals))
-            print(f"{str(e)}元素的可选轨道: ", unique_orbitals)
-
-        dictio = {}
-        while True:
-            _n = input("--> 请选择一个原子序号（直接回车表示不再输入）: ")
-            if _n == "":
-                break
-            _e = band_data.structure.sites[int(_n)].species_string
-            dictpa = {_e: [int(_n) + 1]}
-            _o = input(f" 请选择第{_n}号原子（{_e}）的轨道（用空格分隔）: ")
-            _os = _o.split(" ")
-            dict_eo = {_e: _os}
-            # update dictio
-            dictio.update(dict_eo)
-
-        logger.info("------------------------------------")
-        logger.info("选定的轨道元素字典: ", dictio)
-        logger.info(" dictpa_d number 从1开始，而不是0")
-
-        is_metal = band_data.is_metal()
-        if is_metal:
-            logger.info("正在处理，请稍等...")
-            bsp = BSPlotterProjected(band_data)
-            bsp.get_projected_plots_dots_patom_pmorb(dictio, dictpa, ylim=ylims)
-        else:
-            while True:
-                shift = input(
-                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
-                )
-                if shift.lower().startswith("y"):
-                    logger.info("正在处理，请稍等...")
-                    band_data = get_band_data(infile, zero_to_efermi=True)
-                    bsp = BSPlotterProjected(band_data)
-                    bsp.get_projected_plots_dots_patom_pmorb(
-                        dictio, dictpa, zero_to_efermi=False, ylim=ylims
-                    )
-                    break
-                elif shift.lower().startswith("n"):
-                    logger.info("正在处理，请稍等...")
-                    bsp = BSPlotterProjected(band_data)
-                    bsp.get_projected_plots_dots_patom_pmorb(dictio, dictpa, ylim=ylims)
-                    break
-                else:
-                    print("输入有误，请重新输入！")
-                    continue
-
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s4_5(self, infile, ylims, outfile):
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.plot import plot_bandunfolding
-
-        plot_bandunfolding(infile)
-        plt.ylim(ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s4_6(
-        self,
-    ):
-        infile1 = prompt("待解析瓦尼尔能带文件路径（包含文件名）：", completer=pc)
-        infile2 = prompt("待解析普通能带文件路径（包含文件名）：", completer=pc)
-        if infile1.endswith(".json"):
-            infile3 = prompt(
-                "待解析system.json文件路径（与wannier.json所在文件夹一致，包含文件名）：",
-                completer=pc,
-            )
-            infile1 = [infile1, infile3]
-        ylims = check_lims("输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）：")
-        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.read import get_band_data
-        from pymatgen.electronic_structure.plotter import BSPlotter
-
-        if isinstance(infile1, list):  # wannier
-            bd1 = get_band_data(infile1[0], infile1[1])
-        else:  # str
-            bd1 = get_band_data(infile1)
-        bsp = BSPlotter(bs=bd1)
-        bd2 = get_band_data(infile2)  # dft
-        bsp2 = BSPlotter(bs=bd2)
-        bsp.add_bs(bsp2._bs)
-        bsp.get_plot(bs_labels=["wannier interpolated", "DFT"], ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s5_1(self, dos_data, dos_plotter, xlims, ylims, outfile):
-        """暂不支持修改绘图风格"""
-        logger.info("正在处理，请稍等...")
-        dos_plotter.add_dos("total dos", dos=dos_data)
-        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s5_2(self, dos_data, dos_plotter, xlims, ylims, outfile):
-        logger.info("正在处理，请稍等...")
-        dos_plotter.add_dos_dict(dos_data.get_spd_dos())
-        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s5_3(self, dos_data, dos_plotter, xlims, ylims, outfile):
-        logger.info("正在处理，请稍等...")
-        dos_plotter.add_dos_dict(dos_data.get_element_dos())
-        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s5_4(self, dos_data, dos_plotter, xlims, ylims, outfile):
-        iShift = input("是否平移费米能级？（y/n）：")
-        while True:
-            if iShift.lower().startswith("y"):
-                break
-            elif iShift.lower().startswith("n"):
-                from pymatgen.electronic_structure.plotter import DosPlotter
-
-                dos_plotter = DosPlotter(stack=False, zero_at_efermi=False)
-                break
-            else:
-                iShift = input("输入错误，请重新输入：")
-                continue
-
-        # 获取元素和轨道列表
-        print(dos_data.structure)
-        es = dos_data.structure.composition.elements
-        for e in es:
-            available_orbitals = ["s"]
-            orbitals = e.atomic_orbitals
-            for o in orbitals:
-                if "p" in o:
-                    available_orbitals.append("p")
-                    available_orbitals.append("px")
-                    available_orbitals.append("py")
-                    available_orbitals.append("pz")
-                elif "d" in o:
-                    available_orbitals.append("d")
-                    available_orbitals.append("dxy")
-                    available_orbitals.append("dyz")
-                    available_orbitals.append("dxz")
-                    available_orbitals.append("dx2")
-                    available_orbitals.append("dz2")
-                elif "f" in o:
-                    available_orbitals.append("f")
-                    available_orbitals.append("f_3")
-                    available_orbitals.append("f_2")
-                    available_orbitals.append("f_1")
-                    available_orbitals.append("f0")
-                    available_orbitals.append("f1")
-                    available_orbitals.append("f2")
-                    available_orbitals.append("f3")
-            unique_orbitals = list(set(available_orbitals))
-            print(f"{str(e)}元素的可选轨道: ", unique_orbitals)
-
-        ns = []
-        oss = []
-        while True:
-            _n = input("--> 请选择一个原子序号（直接回车表示不再输入）: ")
-            if _n == "":
-                break
-            _e = dos_data.structure.sites[int(_n)].species_string
-            _o = input(f" 请选择第{_n}号原子（{_e}）的轨道（用空格分隔）: ")
-            _os = _o.split(" ")
-            ns.append(_n)
-            oss.append(_os)
-
-        logger.info("正在处理，请稍等...")
-        from pymatgen.electronic_structure.core import Orbital
-
-        for _n, _os in zip(ns, oss):
-            for _orb in _os:
-                print(f"atom-{_n} {_orb}")
-                dos_plotter.add_dos(
-                    f"{_e}(atom-{_n}) {_orb}",  # label
-                    dos_data.get_site_orbital_dos(
-                        dos_data.structure[int(_n)], getattr(Orbital, _orb)
-                    ),
-                )
-        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s5_5(self, dos_data, dos_plotter, xlims, ylims, outfile):
-        iShift = input("是否平移费米能级？（y/n）：")
-        while True:
-            if iShift.lower().startswith("y"):
-                break
-            elif iShift.lower().startswith("n"):
-                from pymatgen.electronic_structure.plotter import DosPlotter
-
-                dos_plotter = DosPlotter(stack=False, zero_at_efermi=False)
-                break
-            else:
-                iShift = input("输入错误，请重新输入：")
-                continue
-
-        print(dos_data.structure)
-        ais = input("选择原子序号（用空格分隔）: ")
-        logger.info("正在处理，请稍等...")
-
-        atom_indices = [int(ai) for ai in ais.split()]
-        for atom_index in atom_indices:
-            dos_plotter.add_dos_dict(
-                dos_data.get_site_t2g_eg_resolved_dos(dos_data.structure[atom_index])
-            )
-
-        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s5_6(self, dos_data):
-        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.utils import d_band
-
-        os.makedirs(os.path.dirname(os.path.abspath(outfile)), exist_ok=True)
-        with open(outfile, "w") as f:
-            for spin in dos_data.densities:
-                # up, down = (1, -1)
-                if spin.value == 1:
-                    s = "up"
-                elif spin.value == -1:
-                    s = "down"
-                print("spin=", s)
-                f.write(f"spin={s}\n")
-                c = d_band(spin, dos_data)
-                f.write(str(c) + "\n")
-                print(c)
-
-    @logger.catch
-    def s6_1(self, bfile, dfile, ylims, outfile):
-        logger.info("正在处理，请稍等...")
-        from dspawpy.io.read import get_band_data, get_dos_data
-
-        band_data = get_band_data(bfile)
-        dos_data = get_dos_data(dfile)
-        from pymatgen.electronic_structure.plotter import BSDOSPlotter
-
-        bdp = BSDOSPlotter(dos_projection=None)
-        from dspawpy.plot import pltbd
-
-        pltbd(bdp, band_data, dos_data, ylim=ylims, filename=outfile)
-
-    @logger.catch
-    def s6_2(self, bfile, dfile, ylims, outfile):
-        logger.info("正在处理，请稍等...")
-        from dspawpy.io.read import get_band_data, get_dos_data
-
-        band_data = get_band_data(bfile)
-        dos_data = get_dos_data(dfile)
-        from pymatgen.electronic_structure.plotter import BSDOSPlotter
-
-        bdp = BSDOSPlotter(dos_projection="element")
-        from dspawpy.plot import pltbd
-
-        pltbd(bdp, band_data, dos_data, ylim=ylims, filename=outfile)
-
-    @logger.catch
-    def s7(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        _list = [
-            "AbsorptionCoefficient",
-            "ExtinctionCoefficient",
-            "RefractiveIndex",
-            "Reflectance",
-        ]
-        keys = until_give_valid_input(
-            f"数据类型（可选 {_list}）：",
-            _list,
-            completer=WordCompleter(_list),
-            allow_empty=True,
-        )
-        _list2 = ["X", "Y", "Z", "XY", "YZ", "ZX"]
-        label = until_give_valid_input(
-            f"指定数据 {_list2}：",
-            _list2,
-            completer=WordCompleter(_list2),
-            allow_empty=True,
-        )
-
-        outdir = prompt("输出文件路径：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.plot import plot_optical
-
-        if outdir.strip() != "":
-            os.makedirs(outdir, exist_ok=True)
-        plot_optical(datafile=infile, keys=keys, axes=label, prefix=outdir)
-
-    @logger.catch
-    def s8_1(
-        self,
-    ):
-        """插值NEB链"""
-        inis = prompt("初态构型文件路径（包含文件名）：", completer=pc)
-        fins = prompt("末态构型文件路径（包含文件名）：", completer=pc)
-        nmiddle = int(input("初末态之间插入几个构型："))
-        method = until_give_valid_input("插值方法（IDPP/Linear）：", ["IDPP", "Linear"])
-        outdir = prompt("输出文件夹（直接回车表示当前文件夹）：", completer=pc)
-        if outdir == "":
-            outdir = "."
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.diffusion.neb import NEB, write_neb_structures
-        from dspawpy.io.structure import read
-
-        init_struct = read(inis)[0]
-        final_struct = read(fins)[0]
-
-        neb = NEB(init_struct, final_struct, nmiddle + 2)
-        if method == "Linear":
-            structures = neb.linear_interpolate()  # 线性插值
-        elif method == "IDPP":
-            try:
-                structures = neb.idpp_interpolate()  # idpp插值
-            except Exception:
-                logger.error("  IDPP插值失败，请检查构型是否合理！")
-                structures = neb.linear_interpolate()
-                logger.warning("  已自动转为线性插值！")
-        else:
-            raise ValueError("Unknown interpolation method: {}".format(method))
-        # 保存 as 结构文件到 dest 路径下
-        absdir = os.path.abspath(outdir)
-        os.makedirs(os.path.dirname(absdir), exist_ok=True)
-        write_neb_structures(structures, fmt="as", path=absdir)
-        logger.info(f"已将插值后的构型保存到{absdir}路径下")
-
-        while True:
-            yn = input("是否预览插值链？（y/n）")
-            if yn.lower().startswith("y"):
-                from dspawpy.diffusion.nebtools import write_json_chain
-
-                write_json_chain(preview=True, directory=absdir)
-                break
-            elif yn.lower().startswith("n"):
-                break
-            else:
-                print("输入错误，请重新输入！")
-                continue
-
-    @logger.catch
-    def s8_2(
-        self,
-    ):
-        """绘制NEB势垒"""
-        infile = prompt(
-            "待解析neb.h5/neb.json路径（包含文件名）或NEB文件夹：", completer=pc
-        )
-        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
-        logger.info("插值方法默认使用pchip，如果要用其他方法，请使用独立脚本")
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.diffusion.nebtools import plot_barrier
-
-        if os.path.isdir(infile):
-            plot_barrier(directory=infile, figname=outfile, show=False)
-        elif os.path.isfile(infile):
-            plot_barrier(datafile=infile, figname=outfile, show=False)
-        else:
-            raise ValueError(f"{infile} 必须是文件或文件夹路径")
-
-    @logger.catch
-    def s8_3(
-        self,
-    ):
-        """输出NEB计算结果"""
-        datafolder = prompt("NEB计算文件夹：", completer=pc)
-        outdir = prompt("输出到文件夹（直接回车表示当前文件夹）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.diffusion.nebtools import summary
-
-        assert os.path.isdir(datafolder), f"{datafolder} 必须是文件夹路径"
-        absdir = os.path.abspath(outdir)
-        os.makedirs(os.path.dirname(absdir), exist_ok=True)
-        summary(
-            directory=datafolder,
-            outdir=absdir,
-            figname=f"{absdir}/neb_summary.png",
-            show=False,
-        )
-
-    @logger.catch
-    def s8_4(
-        self,
-    ):
-        """输出插值链"""
-        preview = until_give_valid_input(
-            "预览插值生成的NEB链（无需完成计算）（y/n）：", ["y", "n"]
-        )
-        directory = prompt("NEB计算文件夹：", completer=pc)
-        if preview == "y":
-            step = 0
-        else:
-            step = int(input("第几个离子步（从1开始计数，-1表示最新构型）："))
-        dst = prompt("输出到文件夹（直接回车表示当前文件夹）：", completer=pc)
-        json_or_xyz = until_give_valid_input(
-            "输出文件格式（json/xyz）：", ["json", "xyz"]
-        )
-        logger.info("正在处理，请稍等...")
-
-        if json_or_xyz.startswith("xyz"):
-            from dspawpy.diffusion.nebtools import write_xyz_chain
-
-            write_xyz_chain(False, directory, step, dst)
-        else:
-            from dspawpy.diffusion.nebtools import write_json_chain
-
-            write_json_chain(False, directory, step, dst)
-
-    @logger.catch
-    def s8_5(
-        self,
-    ):
-        """计算两个构型的距离"""
-        infile1 = prompt("第一个构型路径（包含文件名）：", completer=pc)
-        infile2 = prompt("第二个构型路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.structure import read
-
-        s1 = read(infile1)[0]
-        s2 = read(infile2)[0]
-        from dspawpy.diffusion.nebtools import get_distance
-
-        dist = get_distance(
-            s1.frac_coords, s2.frac_coords, s1.lattice.matrix, s2.lattice.matrix
-        )
-        logger.info(f"两个构型的距离为：{dist} Angstrom")
-
-    @logger.catch
-    def s8_6(
-        self,
-    ):
-        """续算"""
-        dataFolder = prompt("NEB计算文件夹：", completer=pc)
-        outdir = prompt("备份文件夹：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.diffusion.nebtools import restart
-
-        restart(dataFolder, outdir)
-
-    @logger.catch
-    def s9_1(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        ylims = check_lims("输入y轴范围（先小后大，空格分隔，直接回车可跳过）：")
-        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.read import get_phonon_band_data
-
-        band_data = get_phonon_band_data(infile)  # 读取声子能带
-
-        with HiddenPrints():
-            from pymatgen.phonon.plotter import PhononBSPlotter
-
-        bsp = PhononBSPlotter(band_data)
-        bsp.get_plot(ylim=ylims)
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s9_2(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        xlims = check_lims("输入x轴范围（先小后大，空格分隔，直接回车可跳过）：")
-        ylims = check_lims("输入y轴范围（先小后大，空格分隔，直接回车可跳过）：")
-        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.read import get_phonon_dos_data
-
-        dos = get_phonon_dos_data(infile)  # 读取声子能带
-        with HiddenPrints():
-            from pymatgen.phonon.plotter import PhononDosPlotter
-        dp = PhononDosPlotter(stack=False, sigma=None)
-        dp.add_dos(label="Phonon", dos=dos)
-        dp.get_plot(
-            xlim=xlims,  # x轴范围
-            ylim=ylims,  # y轴范围
-            units="thz",  # 单位
-        )
-
-        save_figure_dpi300(outfile)
-
-    @logger.catch
-    def s9_3(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.plot import plot_phonon_thermal
-
-        plot_phonon_thermal(infile, outfile, False)
-
-    @logger.catch
-    def s10_1(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        outfile = prompt("输出文件路径（包含.xyz或.dump文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.structure import convert
-
-        convert(infile, outfile=outfile)
-
-    @logger.catch
-    def s10_2(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.plot import plot_aimd
-
-        plot_aimd(infile, show=False, figname=outfile)
-
-    @logger.catch
-    def s10_3(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        outfile = prompt("MSD图片输出路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.analysis.aimdtools import MSD, _get_time_step, plot_msd
-        from dspawpy.io.structure import read
-
-        structures = read(infile)
-        elements = [str(i) for i in structures[0].species]
-        unique_elements = list(set(elements))
-        select_str = input(
-            f"元素列表\n{elements}\n去重后\n{unique_elements}\n选择原子或元素（以空格隔开）："
-        )
-        boss = select_str.strip()
-        if boss == "":
-            select = "all"
-        else:
-            if ":" in boss:  # slice, '1:3', '1:3:2'
-                select = boss
-            elif " " in boss:  # list of symbols or atom indices, '1 2 3', 'H He Li'
-                raw_list = boss.split()
-                if all([i.isdigit() for i in raw_list]):
-                    select = [int(i) for i in raw_list]
-                elif all([i in unique_elements for i in raw_list]):
-                    select = raw_list
-                else:
-                    raise ValueError(f"Invalid input for select_str={select_str}")
-            else:
-                # single symbol or atom index
-                # boss may be H1, must remove digit before checking
-                if boss in unique_elements:
-                    select = boss  # symbol
-                elif boss.isdigit():
-                    select = int(boss)  # atom index
-                else:
-                    raise ValueError(f"Invalid input for select_str={select_str}")
-
-        print(select)
-        msd_type = until_give_valid_input(
-            "计算MSD的类型，可选xyz,xy,xz,yz,x,y,z，（直接回车等同于'xyz'，表示计算所有分量）",
-            ["xyz", "xy", "xz", "yz", "x", "y", "z", ""],
-        )
-        timestep = input(
-            f"输入时间步长（fs），直接回车将尝试从{infile}中自动读取，失败则此数值将设为1.0："
-        )
-        xlims = check_lims("输入x轴下限和上限，用空格分隔，直接回车将自动设置")
-        ylims = check_lims("输入y轴下限和上限，用空格分隔，直接回车将自动设置")
-
-        if msd_type == "":
-            msd_type = "xyz"
-
-        if timestep == "":
-            if isinstance(infile, str) or len(infile) == 1:
-                ts = _get_time_step(infile)
-            else:
-                logger.warning(
-                    "For multiple datafiles, you must manually specify the timestep. It will default to 1.0fs."
-                )
-                ts = 1.0
-        else:
-            ts = float(timestep)
-
-        msd_calculator = MSD(structures, select, msd_type)
-        msd = msd_calculator.run()
-
-        import numpy as np
-
-        xs = np.arange(msd_calculator.n_frames) * ts
-        plot_msd(xs, msd, xlims, ylims, figname=outfile, show=False)
-
-    @logger.catch
-    def s10_4(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        timestep = input(
-            f"输入时间步长（fs），直接回车将尝试从{infile}中自动读取，失败则此数值将设为1.0："
-        )
-        if timestep == "":
-            timestep = None
-        else:
-            timestep = float(timestep)
-        xlims = check_lims("输入x轴下限和上限，用空格分隔，直接回车将自动设置")
-        ylims = check_lims("输入y轴下限和上限，用空格分隔，直接回车将自动设置")
-        outfile = prompt("RMSD图片输出路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
-
-        lagtime, rmsd = get_lagtime_rmsd(infile, timestep)
-        plot_rmsd(lagtime, rmsd, xlims, ylims, outfile, False)
-
-    @logger.catch
-    def s10_5(
-        self,
-    ):
-        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-        from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
-        from dspawpy.io.structure import read
-
-        strs = read(datafile=infile)
-        elements = [str(i) for i in strs[0].species]
-        unique_elements = list(set(elements))
-        print(f" 元素列表：{elements}\n 去重后：{unique_elements}")
-        ele1 = until_give_valid_input("--> 请选择一个中心元素：", unique_elements)
-        ele2 = until_give_valid_input("--> 请选择一个对象元素：", unique_elements)
-
-        rmin = input("请输入最小半径, Å （默认0）:")
-        if rmin == "":
-            rmin = 0
-        else:
-            rmin = float(rmin)
-
-        rmax = input("请输入最大半径, Å（默认10）:")
-        if rmax == "":
-            rmax = 10
-        else:
-            rmax = float(rmax)
-
-        ngrid = input("请输入网格数（默认101，包含端点）:")
-        if ngrid == "":
-            ngrid = 101
-        else:
-            ngrid = int(ngrid)
-
-        sigma = input("请输入sigma值（用于一维高斯函数平滑处理，默认0，不处理）:")
-        if sigma == "":
-            sigma = 0
-        else:
-            sigma = float(sigma)
-
-        xlims = [rmin, rmax]
-        ylims = check_lims("请依次输入y轴下限与上限，用空格分隔（默认不指定）:")
-        outfile = prompt("RDF图片输出路径（包含文件名）：", completer=pc)
-
-        rs, rdfs = get_rs_rdfs(infile, ele1, ele2, rmin, rmax, ngrid, sigma)
-        plot_rdf(rs, rdfs, ele1, ele2, xlims, ylims, outfile, False)
-
-    @logger.catch
-    def s11(
-        self,
-    ):  # --> pol.png
-        infile = prompt("已完成铁电极化计算任务的文件夹：", completer=pc)
-        repetition = int(input("请输入数据点绘图时重复次数（默认2）："))
-        if repetition == "":
-            repetition = 2
-        outfile = prompt("图片输出路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.plot import plot_polarization_figure
-
-        plot_polarization_figure(infile, repetition, figname=outfile, show=False)
-
-    @logger.catch
-    def s12(
-        self,
-    ):
-        infile = prompt("待解析frequency.txt文件路径（包含文件名）：", completer=pc)
-        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.utils import getZPE
-
-        print(getZPE(infile, outfile))
-
-    @logger.catch
-    def s13_1(
-        self,
-    ):
-        infile = prompt("待解析frequency.txt文件路径（包含文件名）：", completer=pc)
-        temperature = float(input("请输入温度(K)："))
-        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.utils import getTSads
-
-        TSads = getTSads(infile, temperature, outfile)
-        print("Entropy contribution, T*S (eV): ", TSads)
-
-    @logger.catch
-    def s13_2(
-        self,
-    ):
-        fretxt = prompt("待解析frequency.txt文件路径（包含文件名）：", completer=pc)
-        infile = prompt("待解析h5/json文件路径（包含文件名）：", completer=pc)
-        temperature = float(input("请输入温度(K)："))
-        pressure = float(input("请输入压强(Pa)："))
-        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
-        logger.info("如果要设置更多参数，请参考手册相应章节的独立脚本")
-        logger.info("正在处理，请稍等...")
-
-        from dspawpy.io.utils import getTSgas
-
-        TSgas = getTSgas(
-            fretxt=fretxt,
-            datafile=infile,
-            temperature=temperature,
-            pressure=pressure,
-            outfile=outfile,
-        )
-        print("--> T*S (eV): ", TSgas)
-
-
-@logger.catch
-def save_figure_dpi300(outfile):
-    absfile = os.path.abspath(outfile)
-    os.makedirs(os.path.dirname(absfile), exist_ok=True)
-    plt.tight_layout()
-    plt.savefig(absfile, dpi=300)
-    print(f"--> {absfile}")
-
-
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+import time
+
+main_menu = """
+1: dspawpy更新 
+2: structure结构转化
+3: volumetricData数据处理
+4: band能带数据处理
+5: dos态密度数据处理
+6: bandDos能带和态密度共同显示
+7: optical光学性质数据处理
+8: neb过渡态计算数据处理
+9: phonon声子计算数据处理
+10: aimd分子动力学模拟数据处理
+11: Polarization铁电极化数据处理
+12: ZPE零点振动能数据处理
+13: TS的热校正能
+--> 输入数字后回车选择功能："""
+
+menu3 = """
+=== 3 volumetricData数据处理 ===
+
+  1: volumetricData可视化
+  2: 差分volumetricData可视化
+  3: volumetricData面平均
+  
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+
+menu4 = """
+=== 4 band能带数据处理 ===
+
+  1: 普通能带
+  2: 将能带投影到每一种元素分别作图，数据点大小表示该元素对该轨道的贡献
+  3: 能带投影到不同元素的不同轨道
+  4: 将能带投影到不同原子的不同轨道
+  5: 能带反折叠处理
+  6. band-compare能带对比图处理
+  
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+menu5 = """
+=== 5 dos态密度数据处理 ===
+
+  1: 总的态密度
+  2: 将态密度投影到不同的轨道上
+  3: 将态密度投影到不同的元素上
+  4: 将态密度投影到不同原子的不同轨道上
+  5: 将态密度投影到不同原子的分裂d轨道(t2g, eg)上
+  6: d-带中心分析
+  
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+menu6 = """
+=== 6 bandDos能带和态密度共同显示 ===
+
+  1: 将能带和态密度显示在一张图上
+  2: 将能带和投影态密度显示在一张图上
+
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+menu8 = """
+=== 8 neb过渡态计算数据处理 ===
+
+  1: 输入文件之生成中间构型
+  2: 绘制能垒图
+  3: 过渡态计算概览
+  4: NEB链可视化
+  5: 计算构型间距
+  6: neb续算
+
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+menu9 = """
+=== 9 phonon声子计算数据处理 ===
+
+  1: 声子能带数据处理
+  2: 声子态密度数据处理
+  3: 声子热力学数据处理
+
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+menu10 = """
+=== 10 aimd分子动力学模拟数据处理 ===
+
+  1: 轨迹文件转换格式为.xyz或.dump
+  2: 动力学过程中能量、温度等变化曲线
+  3: 均方位移（MSD）
+  4. 均方根偏差（RMSD）
+  5. 径向分布函数（RDF）
+
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+menu13 = """
+=== 13 TS的热校正能 ===
+
+  1: 吸附质
+  2: 理想气体
+
+  0: 返回主菜单
+  --> 输入数字后回车选择功能："""
+
+import os  # noqa: E402
+from argparse import ArgumentParser  # noqa: E402
+
+argparser = ArgumentParser("dspawpy命令行交互小工具")
+argparser.add_argument(
+    "-q", "--quick", action="store_true", help="不联网检查dspawpy版本"
+)
+argparser.add_argument(
+    "-c", "--clean", action="store_true", help="不显示dspawpy_logo，直接显示菜单"
+)
+args = argparser.parse_args()
+
+
+def online_check(dv, df):
+    latest_version = None
+    try:  # 如果正常导入dspawpy，应当有 requests库（pymatgen和mp-api的依赖）
+        print("正在联网检查dspawpy版本... 使用 -q 参数启动此程序可跳过检查")
+        response = get("https://pypi.org/pypi/dspawpy/json", timeout=3)
+        latest_version = response.json()["info"]["version"]
+        error_message = None
+    except ImportError:
+        error_message = "无法导入 requests 库"
+    except exceptions.Timeout:
+        error_message = "requests联网检查dspawpy版本超时"
+    except exceptions.RequestException as e:
+        error_message = f"requests联网检查dspawpy版本时出现异常: {e}"
+    except Exception as e:
+        error_message = f"联网检查dspawpy版本失败: {e}"
+    finally:
+        if latest_version:
+            if latest_version != dv:
+                print(
+                    f"\n 成功导入 {dv}（不是最新版本 {latest_version}），可尝试使用功能1升级"
+                )
+                print(
+                    f" 导入的dspawpy模块文件路径为（如果不符合预期，请检查环境变量)：\n {df}\n"
+                )
+            else:
+                print(f"\n         成功导入 {dv}（最新版）dspawpy\n")
+
+            with open(os.path.expanduser("~/.dspawpy_latest_version"), "w") as fin:
+                fin.write(latest_version)
+        else:
+            print(f"\n         成功导入 {dv}（无法联网检查最新版本）dspawpy\n")
+
+    return error_message
+
+
+def verify_dspawpy_version(skip=False):
+    error_message = None
+    try:
+        import dspawpy
+
+        try:
+            dv = dspawpy.__version__
+        except Exception:  # 老版本没有__version__属性
+            dv = "??? 版本过老，无法检测"
+        finally:
+            df = os.path.dirname(dspawpy.__file__)
+
+        if skip:
+            print(f"\n         成功导入 dspawpy={dv}\n")
+        else:
+            # 检查是否存在 ~/.dspawpy_latest_version 文件，存在则读取其中写的版本号信息
+            # 如果不存在，或者读取失败，则联网检查最新版本，并在检查成功后写入 ~/.dspawpy_latest_version 文件
+            if os.path.isfile(os.path.expanduser("~/.dspawpy_latest_version")):
+                with open(os.path.expanduser("~/.dspawpy_latest_version"), "r") as fin:
+                    latest_version = fin.read().strip()
+                if dv == latest_version:
+                    print(f"\n         成功导入 {dv}（最新版）dspawpy\n")
+                else:
+                    error_message = online_check(dv, df)
+            else:
+                error_message = online_check(dv, df)
+
+    except ImportError:
+        print("     我们检测到您并未安装dspawpy，试试菜单1快速安装吧     ")
+    except Exception as e:
+        error_message = f"导入dspawpy失败: {e}"
+
+    print("********这是dspawpy命令行交互小工具，预祝您使用愉快********")
+    if error_message is not None:
+        print(error_message)
+
+
+def collect_user_input() -> list:
+    """让用户选择功能，这一步不用记录日志，直接打印提示信息"""
+
+    if args.clean:  # 不显示 dspawpy_logo
+        dspawpy_logo = ""
+    else:
+        dspawpy_logo = r"""
+********这是dspawpy命令行交互小工具，预祝您使用愉快********
+    ( )
+   _| |  ___  _ _      _ _  _   _   _  _ _    _   _
+ /'_` |/',__)( '_`\  /'_` )( ) ( ) ( )( '_`\ ( ) ( )
+( (_| |\__, \| (_) )( (_| || \_/ \_/ || (_) )| (_) |
+`\__,_)(____/| ,__/'`\__,_)`\___x___/'| ,__/'`\__, |
+             | |                      | |    ( )_| |
+             (_)                      (_)    `\___/'
+"""
+    print(dspawpy_logo)
+
+    if args.quick:
+        iskip = True
+    else:
+        iskip = False
+
+    verify_dspawpy_version(skip=iskip)
+
+    while True:  # 主菜单选择
+        n = input(main_menu)
+        if n == "1":  # 环境部署比较特殊，不要进入主程序
+            cmd = "pip install dspawpy --user -i https://pypi.tuna.tsinghua.edu.cn/simple && pip install -U dspawpy -i https://pypi.org/simple --user"
+            while True:
+                yn = input(f"更新dspawpy将执行\n {cmd}\n (y/n)? ")
+                if yn.lower() == "y":
+                    if os.system(cmd) == 0:
+                        print(">>>>>> 执行成功")
+                        print("请重新运行程序，使安装生效")
+                    else:
+                        print("!!!!!! 执行失败")
+                    break
+                elif yn.lower() == "n":
+                    print("###### 放弃执行")
+                    break
+                else:
+                    print("!!! 输入错误，请重试")
+                    continue
+
+        elif n == "2":
+            return 2, 0
+
+        elif n == "3":
+            while True:
+                n = input(menu3)
+                if n not in ["0", "1", "2", "3"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 3, 1
+                elif n == "2":
+                    return 3, 2
+                elif n == "3":
+                    return 3, 3
+                else:
+                    break
+            if n == "0":
+                continue
+            break
+
+        elif n == "4":
+            while True:
+                n = input(menu4)
+                if n not in ["0", "1", "2", "3", "4", "5", "6"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 4, 1
+                elif n == "2":
+                    return 4, 2
+                elif n == "3":
+                    return 4, 3
+                elif n == "4":
+                    return 4, 4
+                elif n == "5":
+                    return 4, 5
+                elif n == "6":
+                    return 4, 6
+                else:
+                    break
+            if n == "0":
+                continue
+            break
+
+        elif n == "5":
+            while True:
+                n = input(menu5)
+                if n not in ["0", "1", "2", "3", "4", "5", "6"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 5, 1
+                elif n == "2":
+                    return 5, 2
+                elif n == "3":
+                    return 5, 3
+                elif n == "4":
+                    return 5, 4
+                elif n == "5":
+                    return 5, 5
+                elif n == "6":
+                    return 5, 6
+                else:
+                    break
+
+            if n == "0":
+                continue
+            break
+
+        elif n == "6":
+            while True:
+                n = input(menu6)
+                if n not in ["0", "1", "2"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 6, 1
+                elif n == "2":
+                    return 6, 2
+                else:
+                    break
+            if n == "0":
+                continue
+            break
+
+        elif n == "7":
+            return 7, 0
+        elif n == "8":
+            while True:
+                n = input(menu8)
+                if n not in ["0", "1", "2", "3", "4", "5", "6"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":  # 插值
+                    return 8, 1
+                elif n == "2":  # 能垒图
+                    return 8, 2
+                elif n == "3":  # 总结
+                    return 8, 3
+                elif n == "4":  # 可视化链
+                    return 8, 4
+                elif n == "5":  # 计算距离
+                    return 8, 5
+                elif n == "6":  # 重启
+                    return 8, 6
+                else:
+                    break
+            if n == "0":
+                continue
+            break
+
+        elif n == "9":
+            while True:
+                n = input(menu9)
+                if n not in ["0", "1", "2", "3"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 9, 1
+                elif n == "2":
+                    return 9, 2
+                elif n == "3":
+                    return 9, 3
+                else:
+                    break
+
+            if n == "0":
+                continue
+            break
+
+        elif n == "10":
+            while True:
+                n = input(menu10)
+                if n not in ["0", "1", "2", "3", "4", "5"]:
+                    print("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 10, 1
+                elif n == "2":
+                    return 10, 2
+                elif n == "3":
+                    return 10, 3
+                elif n == "4":
+                    return 10, 4
+                elif n == "5":
+                    return 10, 5
+                else:
+                    break
+
+            if n == "0":
+                continue
+            break
+
+        elif n == "11":
+            return 11, 0
+
+        elif n == "12":
+            return 12, 0
+
+        elif n == "13":
+            while True:
+                n = input(menu13)
+                if n not in ["0", "1", "2"]:
+                    logger.error("!!! 输入错误，请重试")
+                    continue
+                elif n == "1":
+                    return 13, 1
+                elif n == "2":
+                    return 13, 2
+                else:
+                    break
+            if n == "0":
+                continue
+            break
+
+        else:
+            print("XXXXXX 输入错误，请重试 XXXXXX")
+            continue
+
+
+from multiprocessing.pool import ThreadPool  # noqa: E402
+
+from requests import exceptions, get  # noqa: E402
+
+pool = ThreadPool(processes=1)
+async_result = pool.apply_async(collect_user_input)
+
+
+def main():
+    """run specific task by user selected task number"""
+    # print('entering main...') # uncomment this to see the speed impact
+    task_number = async_result.get()
+    time.sleep(3)
+    pool.close()
+    # print('got task number') # uncomment this to see the speed impact
+    tasks = Tasks()
+    if task_number[0] == 2:
+        tasks.s2()
+
+    elif task_number == (3, 1):
+        tasks.s3_1()
+    elif task_number == (3, 2):
+        tasks.s3_2()
+    elif task_number == (3, 3):
+        tasks.s3_3()
+
+    elif task_number[0] == 4:  # band
+        if task_number[1] != 6:
+            infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+            ylims = check_lims(
+                "输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）："
+            )
+            outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
+        if task_number[1] == 1:  # band
+            tasks.s4_1(infile, ylims, outfile)
+        elif task_number[1] == 2:  # band-proj
+            tasks.s4_2(infile, ylims, outfile)
+        elif task_number[1] == 3:  # band-proj-element
+            tasks.s4_3(infile, ylims, outfile)
+        elif task_number[1] == 4:  # band-proj-site
+            tasks.s4_4(infile, ylims, outfile)
+        elif task_number[1] == 5:  # band-unfold
+            tasks.s4_5(infile, ylims, outfile)
+        elif task_number[1] == 6:  # band-compare
+            tasks.s4_6()
+
+    elif task_number[0] == 5:  # dos
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        from dspawpy.io.read import get_dos_data
+
+        dosdata = get_dos_data(infile)
+        from pymatgen.electronic_structure.plotter import DosPlotter
+
+        dos_plotter = DosPlotter(stack=False, zero_at_efermi=True)
+        if task_number[1] != 6:
+            xlims = check_lims(
+                "输入x轴范围（先小后大，以空格分隔，直接回车可跳过设置）："
+            )
+            ylims = check_lims(
+                "输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）："
+            )
+            outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
+        if task_number[1] == 1:  # tdos
+            tasks.s5_1(dosdata, dos_plotter, xlims, ylims, outfile)
+        elif task_number[1] == 2:
+            tasks.s5_2(dosdata, dos_plotter, xlims, ylims, outfile)
+        elif task_number[1] == 3:
+            tasks.s5_3(dosdata, dos_plotter, xlims, ylims, outfile)
+        elif task_number[1] == 4:
+            tasks.s5_4(dosdata, dos_plotter, xlims, ylims, outfile)
+        elif task_number[1] == 5:
+            tasks.s5_5(dosdata, dos_plotter, xlims, ylims, outfile)
+        elif task_number[1] == 6:
+            tasks.s5_6(dosdata)
+
+    elif task_number[0] == 6:
+        infile1 = prompt("待解析能带band文件路径（包含文件名）：", completer=pc)
+        infile2 = prompt("待解析态密度dos文件路径（包含文件名）：", completer=pc)
+        ylims = check_lims("输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）：")
+        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
+        if task_number[1] == 1:
+            tasks.s6_1(infile1, infile2, ylims, outfile)
+        else:
+            tasks.s6_2(infile1, infile2, ylims, outfile)
+
+    elif task_number[0] == 7:
+        tasks.s7()
+
+    elif task_number[0] == 8:
+        if task_number[1] == 1:
+            tasks.s8_1()
+        elif task_number[1] == 2:
+            tasks.s8_2()
+        elif task_number[1] == 3:
+            tasks.s8_3()
+        elif task_number[1] == 4:
+            tasks.s8_4()
+        elif task_number[1] == 5:
+            tasks.s8_5()
+        elif task_number[1] == 6:
+            tasks.s8_6()
+
+    elif task_number[0] == 9:
+        if task_number[1] == 1:
+            tasks.s9_1()
+        elif task_number[1] == 2:
+            tasks.s9_2()
+        elif task_number[1] == 3:
+            tasks.s9_3()
+
+    elif task_number[0] == 10:
+        if task_number[1] == 1:
+            tasks.s10_1()
+        elif task_number[1] == 2:
+            tasks.s10_2()
+        elif task_number[1] == 3:
+            tasks.s10_3()
+        elif task_number[1] == 4:
+            tasks.s10_4()
+        elif task_number[1] == 5:
+            tasks.s10_5()
+
+    elif task_number[0] == 11:
+        tasks.s11()
+
+    elif task_number[0] == 12:
+        tasks.s12()
+
+    elif task_number[0] == 13:
+        if task_number[1] == 1:
+            tasks.s13_1()
+        elif task_number[1] == 2:
+            tasks.s13_2()
+
+
+import matplotlib  # noqa: E402
+import matplotlib.pyplot as plt  # noqa: E402
+
+matplotlib.use("agg")  # to avoid qt error on some linux servers.
+import sys  # noqa: E402
+
+from prompt_toolkit import prompt  # noqa: E402
+from prompt_toolkit.completion import PathCompleter, WordCompleter, FuzzyCompleter  # noqa: E402
+
+pc = FuzzyCompleter(PathCompleter(expanduser=True))
+
+from loguru import logger  # noqa: E402
+
+logger.remove()
+logger.add(
+    sys.stderr,
+    level="INFO",
+    format="<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <cyan>{message}</cyan>",
+)
+logger.add(
+    ".dspawpycli-debug.log",
+    level="DEBUG",
+    format="{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}",
+)
+
+
+def until_give_valid_input(user_prompt, valid_input, completer=None, allow_empty=False):
+    while True:
+        ns = prompt(user_prompt, completer=completer).strip().split()
+        if allow_empty and len(ns) == 0:
+            return valid_input
+        else:
+            valid = True
+            for n in ns:
+                if n not in valid_input:
+                    print("!!! 输入错误，请重试")
+                    valid = False
+                    break
+            if valid:
+                return ns
+            else:
+                continue
+
+
+def check_lims(user_prompt):
+    # return None or [float, float]
+    while True:
+        userInput = input(user_prompt).strip()
+        if userInput == "":
+            return None
+        else:
+            if " " not in userInput:
+                logger.warning(f"!!! {userInput}没有以空格分隔，请重试")
+                continue
+            elif len(userInput.split(" ")) != 2:
+                logger.warning(f"!!! {userInput}参数长度不为2")
+                continue
+            else:
+                try:
+                    float(userInput.split(" ")[0])
+                    float(userInput.split(" ")[1])
+                    return userInput.split(" ")  # return '1_2'
+                except Exception:
+                    logger.warning(f"!!! {userInput}不全是数字，请重试")
+                    continue
+
+
+class HiddenPrints:
+    def __enter__(self):
+        self._original_stdout = sys.stdout
+        sys.stdout = open(os.devnull, "w")
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        sys.stdout.close()
+        sys.stdout = self._original_stdout
+
+
+class Tasks:
+    @logger.catch
+    def s2(
+        self,
+    ):
+        infile = prompt(
+            "待解析文件路径（包含文件名，支持h5, json, pdb, as, hzw等格式）：",
+            completer=pc,
+        )
+        outfile = prompt(
+            "输出文件路径（包含文件名，支持pdb, xyz, dump, json, as, hzw等格式）：",
+            completer=pc,
+        )
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.structure import convert
+
+        convert(infile=infile, outfile=outfile)
+
+    @logger.catch
+    def s3_1(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
+        task = until_give_valid_input(
+            f"任务类型{_list}：",
+            _list,
+            completer=WordCompleter(_list),
+        )
+
+        subtype = None
+        if task == "potential":
+            if infile.endswith(".h5"):
+                from dspawpy.io.read import load_h5
+
+                data = load_h5(infile)
+                keys = [
+                    k.split("/")[-1] for k in data.keys() if k.startswith("/Potential")
+                ]
+
+                if len(keys) == 0:
+                    raise ValueError(
+                        f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
+                    )
+                elif len(keys) == 1:
+                    subtype = keys[0]
+                else:
+                    subtype = until_give_valid_input(
+                        f"检测到 {keys} 数据集，请选择其中之一：",
+                        keys,
+                        completer=WordCompleter(keys),
+                    )
+
+            elif infile.endswith(".json"):
+                import json
+
+                with open(infile, "r") as fin:
+                    data = json.load(fin)
+                    if "Potential" not in data.keys():
+                        raise ValueError(
+                            f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
+                        )
+                    keys = [k for k in data["Potential"].keys()]
+
+                if len(keys) == 1:
+                    subtype = keys[0]
+                else:
+                    subtype = until_give_valid_input(
+                        f"检测到 {keys} 数据集，请选择其中之一：",
+                        keys,
+                        completer=WordCompleter(keys),
+                    )
+            else:
+                raise ValueError(
+                    f"仅支持h5和json格式，不支持{infile.split('.')[-1]}格式的数据文件！"
+                )
+
+        outfile = prompt(
+            "输出文件路径（包含文件名，支持.cube和.vasp格式）：", completer=pc
+        )
+        if outfile.split(".")[-1].lower() == "cube":
+            cube_or_vasp = "cube"
+        elif (
+            outfile.split(".")[-1].lower() == "vesta"
+            or outfile.split(".")[-1].lower() == "vasp"
+        ):
+            cube_or_vasp = "vesta"
+        else:
+            cube_or_vasp = until_give_valid_input(
+                "请指定输出文件格式（cube, vasp）：", ["cube", "vesta", "vasp"]
+            )
+
+        logger.info("正在处理，请稍等...")
+        from dspawpy.io.write import write_VESTA
+
+        write_VESTA(
+            in_filename=infile,
+            data_type=task,
+            out_filename=outfile,
+            subtype=subtype,
+            format=cube_or_vasp,
+        )
+        logger.info("可直接使用VESTA软件打开")
+
+    @logger.catch
+    def s3_2(
+        self,
+    ):
+        total = prompt("体系总电荷密度文件路径（包含文件名）:", completer=pc)
+        individuals = []
+        while True:
+            individual = prompt(
+                "体系各组分电荷密度文件路径，(包含文件名，直接回车表示停止输入）:",
+                completer=pc,
+            )
+            if individual == "":
+                break
+            individuals.append(individual)
+
+        outfile = prompt(
+            "输出文件路径（包含文件名，支持.cube和.vasp格式）：", completer=pc
+        )
+
+        if outfile.split(".")[-1].lower() == "cube":
+            cube_or_vasp = "cube"
+        elif (
+            outfile.split(".")[-1].lower() == "vesta"
+            or outfile.split(".")[-1].lower() == "vasp"
+        ):
+            cube_or_vasp = "vesta"
+        else:
+            cube_or_vasp = until_give_valid_input(
+                "请指定输出文件格式（cube, vesta）：", ["cube", "vesta", "vasp"]
+            )
+
+        logger.info("正在处理，请稍等...")
+        from dspawpy.io.write import write_delta_rho_vesta
+
+        write_delta_rho_vesta(
+            total=total, individuals=individuals, output=outfile, format=cube_or_vasp
+        )
+        logger.info("可直接使用VESTA软件打开")
+
+    @logger.catch
+    def s3_3(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        axes = until_give_valid_input("沿哪些轴平均（0, 1, 2）：", ["0", "1", "2"])
+        _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
+        task = until_give_valid_input(
+            f"任务类型{_list}：",
+            _list,
+            completer=WordCompleter(_list),
+        )
+        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
+
+        subtype = None
+        if task == "rho":
+            k = "TotalCharge"
+        elif task == "potential":
+            if infile.endswith(".h5"):
+                from dspawpy.io.read import load_h5
+
+                data = load_h5(infile)
+                keys = [
+                    k.split("/")[-1] for k in data.keys() if k.startswith("/Potential")
+                ]
+
+                if len(keys) == 0:
+                    raise ValueError(
+                        f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
+                    )
+                elif len(keys) == 1:
+                    subtype = keys[0]
+                else:
+                    subtype = until_give_valid_input(
+                        f"检测到 {keys} 数据集，请选择其中之一：",
+                        keys,
+                        completer=WordCompleter(keys),
+                    )
+
+            elif infile.endswith(".json"):
+                import json
+
+                with open(infile, "r") as fin:
+                    data = json.load(fin)
+                    if "Potential" not in data.keys():
+                        raise ValueError(
+                            f"未检测到数据集，请检查文件{infile}路径或者任务类型是否正确！"
+                        )
+                    keys = [k for k in data["Potential"].keys()]
+
+                if len(keys) == 1:
+                    subtype = keys[0]
+                else:
+                    subtype = until_give_valid_input(
+                        f"检测到 {keys} 数据集，请选择其中之一：",
+                        keys,
+                        completer=WordCompleter(keys),
+                    )
+            else:
+                raise ValueError(
+                    f"仅支持h5和json格式，不支持{infile.split('.')[-1]}格式的数据文件！"
+                )
+            k = subtype
+        elif task == "elf":
+            k = "TotalELF"
+        elif task == "pcharge":
+            k = "TotalCharge"
+        elif task == "rhoBound":
+            k = "Rho"
+        else:
+            raise ValueError(f"Unknown task: {task}")
+
+        logger.info("正在处理，请稍等...")
+        axes_indices = [int(i) for i in axes.split()]
+        for ai in axes_indices:
+            from dspawpy.plot import average_along_axis
+
+            average_along_axis(infile, axis=ai, label=f"axis{ai}", subtype=subtype)
+        if len(axes_indices) > 1:
+            plt.legend()
+
+        plt.xlabel("Grid Index")
+        plt.ylabel(k)
+        absfile = os.path.abspath(outfile)
+        os.makedirs(os.path.dirname(os.path.abspath(absfile)), exist_ok=True)
+        plt.savefig(absfile, dpi=300)
+
+    @logger.catch
+    def s4_1(self, infile, ylims, outfile):
+        from dspawpy.io.read import get_band_data
+        from pymatgen.electronic_structure.plotter import BSPlotter
+
+        band_data = get_band_data(infile)
+        is_metal = band_data.is_metal()
+        if is_metal:
+            logger.info("正在处理，请稍等...")
+            bsp = BSPlotter(band_data)
+            bsp.get_plot(ylim=ylims)
+        else:
+            while True:
+                shift = input(
+                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
+                )
+                if shift.lower().startswith("y"):
+                    logger.info("正在处理，请稍等...")
+                    from dspawpy.io.read import get_band_data
+
+                    band_data = get_band_data(infile, zero_to_efermi=True)
+                    bsp = BSPlotter(band_data)
+                    bsp.get_plot(False, ylim=ylims)
+                    break
+                elif shift.lower().startswith("n"):
+                    logger.info("正在处理，请稍等...")
+                    bsp = BSPlotter(band_data)
+                    bsp.get_plot(ylim=ylims)
+                    break
+                else:
+                    print("输入有误，请重新输入！")
+                    continue
+
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s4_2(self, infile, ylims, outfile):
+        from dspawpy.io.read import get_band_data
+        from pymatgen.electronic_structure.plotter import BSPlotterProjected
+
+        band_data = get_band_data(infile)
+        is_metal = band_data.is_metal()
+        if is_metal:
+            logger.info("正在处理，请稍等...")
+            bsp = BSPlotterProjected(band_data)
+            bsp.get_elt_projected_plots(ylim=ylims)
+        else:
+            while True:
+                shift = input(
+                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
+                )
+                if shift.lower().startswith("y"):
+                    logger.info("正在处理，请稍等...")
+                    band_data = get_band_data(infile, zero_to_efermi=True)
+                    bsp = BSPlotterProjected(band_data)
+                    bsp.get_elt_projected_plots(False, ylim=ylims)
+                    break
+                elif shift.lower().startswith("n"):
+                    logger.info("正在处理，请稍等...")
+                    bsp = BSPlotterProjected(band_data)
+                    bsp.get_elt_projected_plots(ylim=ylims)
+                    break
+                else:
+                    print("输入有误，请重新输入！")
+                    continue
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s4_3(self, infile, ylims, outfile):
+        from dspawpy.io.read import get_band_data
+        from pymatgen.electronic_structure.plotter import BSPlotterProjected
+
+        band_data = get_band_data(infile)
+        # 获取元素和轨道列表
+        es = band_data.structure.composition.elements
+        for e in es:
+            print("可选元素:", str(e))
+            available_orbitals = ["s"]
+            orbitals = e.atomic_orbitals
+            for o in orbitals:
+                if "p" in o:
+                    available_orbitals.append("p")
+                elif "d" in o:
+                    available_orbitals.append("d")
+                elif "f" in o:
+                    available_orbitals.append("f")
+            unique_orbitals = list(set(available_orbitals))
+            print(f"{str(e)}元素的可选轨道: ", unique_orbitals)
+
+        dictio = {}
+        while True:
+            _e = input("选择一种元素（直接回车表示选择结束）: ")
+            if _e == "":
+                break
+            _o = input(f"选择{_e}元素的原子轨道（用空格分隔）: ")
+            _os = _o.split(" ")
+            dict_eo = {_e: _os}
+            # update dictio
+            dictio.update(dict_eo)
+
+        print("选定的轨道元素字典: ", dictio)
+
+        is_metal = band_data.is_metal()
+        if is_metal:
+            logger.info("正在处理，请稍等...")
+            bsp = BSPlotterProjected(band_data)
+            bsp.get_projected_plots_dots(dictio)
+        else:
+            while True:
+                shift = input(
+                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
+                )
+                if shift.lower().startswith("y"):
+                    logger.info("正在处理，请稍等...")
+                    band_data = get_band_data(infile, zero_to_efermi=True)
+                    bsp = BSPlotterProjected(band_data)
+                    bsp.get_projected_plots_dots(dictio, False, ylim=ylims)
+                    break
+                elif shift.lower().startswith("n"):
+                    logger.info("正在处理，请稍等...")
+                    bsp = BSPlotterProjected(band_data)
+                    bsp.get_projected_plots_dots(dictio, ylim=ylims)
+                    break
+                else:
+                    print("输入有误，请重新输入！")
+                    continue
+
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s4_4(self, infile, ylims, outfile):
+        from dspawpy.io.read import get_band_data
+        from pymatgen.electronic_structure.plotter import BSPlotterProjected
+
+        band_data = get_band_data(infile)
+        print(band_data.structure)
+        es = band_data.structure.composition.elements
+        for e in es:
+            available_orbitals = ["s"]
+            orbitals = e.atomic_orbitals
+            for o in orbitals:
+                if "p" in o:
+                    available_orbitals.append("p")
+                    available_orbitals.append("px")
+                    available_orbitals.append("py")
+                    available_orbitals.append("pz")
+                elif "d" in o:
+                    available_orbitals.append("d")
+                    available_orbitals.append("dxy")
+                    available_orbitals.append("dyz")
+                    available_orbitals.append("dxz")
+                    available_orbitals.append("dx2")
+                    available_orbitals.append("dz2")
+                elif "f" in o:
+                    available_orbitals.append("f")
+                    available_orbitals.append("f_3")
+                    available_orbitals.append("f_2")
+                    available_orbitals.append("f_1")
+                    available_orbitals.append("f0")
+                    available_orbitals.append("f1")
+                    available_orbitals.append("f2")
+                    available_orbitals.append("f3")
+
+            unique_orbitals = list(set(available_orbitals))
+            print(f"{str(e)}元素的可选轨道: ", unique_orbitals)
+
+        dictio = {}
+        while True:
+            _n = input("--> 请选择一个原子序号（直接回车表示不再输入）: ")
+            if _n == "":
+                break
+            _e = band_data.structure.sites[int(_n)].species_string
+            dictpa = {_e: [int(_n) + 1]}
+            _o = input(f" 请选择第{_n}号原子（{_e}）的轨道（用空格分隔）: ")
+            _os = _o.split(" ")
+            dict_eo = {_e: _os}
+            # update dictio
+            dictio.update(dict_eo)
+
+        logger.info("------------------------------------")
+        logger.info("选定的轨道元素字典: ", dictio)
+        logger.info(" dictpa_d number 从1开始，而不是0")
+
+        is_metal = band_data.is_metal()
+        if is_metal:
+            logger.info("正在处理，请稍等...")
+            bsp = BSPlotterProjected(band_data)
+            bsp.get_projected_plots_dots_patom_pmorb(dictio, dictpa, ylim=ylims)
+        else:
+            while True:
+                shift = input(
+                    "此为非金属体系，是否要将能量零点从价带顶平移至费米能级？(y/n)"
+                )
+                if shift.lower().startswith("y"):
+                    logger.info("正在处理，请稍等...")
+                    band_data = get_band_data(infile, zero_to_efermi=True)
+                    bsp = BSPlotterProjected(band_data)
+                    bsp.get_projected_plots_dots_patom_pmorb(
+                        dictio, dictpa, zero_to_efermi=False, ylim=ylims
+                    )
+                    break
+                elif shift.lower().startswith("n"):
+                    logger.info("正在处理，请稍等...")
+                    bsp = BSPlotterProjected(band_data)
+                    bsp.get_projected_plots_dots_patom_pmorb(dictio, dictpa, ylim=ylims)
+                    break
+                else:
+                    print("输入有误，请重新输入！")
+                    continue
+
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s4_5(self, infile, ylims, outfile):
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.plot import plot_bandunfolding
+
+        plot_bandunfolding(infile)
+        plt.ylim(ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s4_6(
+        self,
+    ):
+        infile1 = prompt("待解析瓦尼尔能带文件路径（包含文件名）：", completer=pc)
+        infile2 = prompt("待解析普通能带文件路径（包含文件名）：", completer=pc)
+        if infile1.endswith(".json"):
+            infile3 = prompt(
+                "待解析system.json文件路径（与wannier.json所在文件夹一致，包含文件名）：",
+                completer=pc,
+            )
+            infile1 = [infile1, infile3]
+        ylims = check_lims("输入y轴范围（先小后大，以空格分隔，直接回车可跳过设置）：")
+        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.read import get_band_data
+        from pymatgen.electronic_structure.plotter import BSPlotter
+
+        if isinstance(infile1, list):  # wannier
+            bd1 = get_band_data(infile1[0], infile1[1])
+        else:  # str
+            bd1 = get_band_data(infile1)
+        bsp = BSPlotter(bs=bd1)
+        bd2 = get_band_data(infile2)  # dft
+        bsp2 = BSPlotter(bs=bd2)
+        bsp.add_bs(bsp2._bs)
+        bsp.get_plot(bs_labels=["wannier interpolated", "DFT"], ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s5_1(self, dos_data, dos_plotter, xlims, ylims, outfile):
+        """暂不支持修改绘图风格"""
+        logger.info("正在处理，请稍等...")
+        dos_plotter.add_dos("total dos", dos=dos_data)
+        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s5_2(self, dos_data, dos_plotter, xlims, ylims, outfile):
+        logger.info("正在处理，请稍等...")
+        dos_plotter.add_dos_dict(dos_data.get_spd_dos())
+        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s5_3(self, dos_data, dos_plotter, xlims, ylims, outfile):
+        logger.info("正在处理，请稍等...")
+        dos_plotter.add_dos_dict(dos_data.get_element_dos())
+        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s5_4(self, dos_data, dos_plotter, xlims, ylims, outfile):
+        iShift = input("是否平移费米能级？（y/n）：")
+        while True:
+            if iShift.lower().startswith("y"):
+                break
+            elif iShift.lower().startswith("n"):
+                from pymatgen.electronic_structure.plotter import DosPlotter
+
+                dos_plotter = DosPlotter(stack=False, zero_at_efermi=False)
+                break
+            else:
+                iShift = input("输入错误，请重新输入：")
+                continue
+
+        # 获取元素和轨道列表
+        print(dos_data.structure)
+        es = dos_data.structure.composition.elements
+        for e in es:
+            available_orbitals = ["s"]
+            orbitals = e.atomic_orbitals
+            for o in orbitals:
+                if "p" in o:
+                    available_orbitals.append("p")
+                    available_orbitals.append("px")
+                    available_orbitals.append("py")
+                    available_orbitals.append("pz")
+                elif "d" in o:
+                    available_orbitals.append("d")
+                    available_orbitals.append("dxy")
+                    available_orbitals.append("dyz")
+                    available_orbitals.append("dxz")
+                    available_orbitals.append("dx2")
+                    available_orbitals.append("dz2")
+                elif "f" in o:
+                    available_orbitals.append("f")
+                    available_orbitals.append("f_3")
+                    available_orbitals.append("f_2")
+                    available_orbitals.append("f_1")
+                    available_orbitals.append("f0")
+                    available_orbitals.append("f1")
+                    available_orbitals.append("f2")
+                    available_orbitals.append("f3")
+            unique_orbitals = list(set(available_orbitals))
+            print(f"{str(e)}元素的可选轨道: ", unique_orbitals)
+
+        ns = []
+        oss = []
+        while True:
+            _n = input("--> 请选择一个原子序号（直接回车表示不再输入）: ")
+            if _n == "":
+                break
+            _e = dos_data.structure.sites[int(_n)].species_string
+            _o = input(f" 请选择第{_n}号原子（{_e}）的轨道（用空格分隔）: ")
+            _os = _o.split(" ")
+            ns.append(_n)
+            oss.append(_os)
+
+        logger.info("正在处理，请稍等...")
+        from pymatgen.electronic_structure.core import Orbital
+
+        for _n, _os in zip(ns, oss):
+            for _orb in _os:
+                print(f"atom-{_n} {_orb}")
+                dos_plotter.add_dos(
+                    f"{_e}(atom-{_n}) {_orb}",  # label
+                    dos_data.get_site_orbital_dos(
+                        dos_data.structure[int(_n)], getattr(Orbital, _orb)
+                    ),
+                )
+        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s5_5(self, dos_data, dos_plotter, xlims, ylims, outfile):
+        iShift = input("是否平移费米能级？（y/n）：")
+        while True:
+            if iShift.lower().startswith("y"):
+                break
+            elif iShift.lower().startswith("n"):
+                from pymatgen.electronic_structure.plotter import DosPlotter
+
+                dos_plotter = DosPlotter(stack=False, zero_at_efermi=False)
+                break
+            else:
+                iShift = input("输入错误，请重新输入：")
+                continue
+
+        print(dos_data.structure)
+        ais = input("选择原子序号（用空格分隔）: ")
+        logger.info("正在处理，请稍等...")
+
+        atom_indices = [int(ai) for ai in ais.split()]
+        for atom_index in atom_indices:
+            dos_plotter.add_dos_dict(
+                dos_data.get_site_t2g_eg_resolved_dos(dos_data.structure[atom_index])
+            )
+
+        dos_plotter.get_plot(xlim=xlims, ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s5_6(self, dos_data):
+        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.utils import d_band
+
+        os.makedirs(os.path.dirname(os.path.abspath(outfile)), exist_ok=True)
+        with open(outfile, "w") as f:
+            for spin in dos_data.densities:
+                # up, down = (1, -1)
+                if spin.value == 1:
+                    s = "up"
+                elif spin.value == -1:
+                    s = "down"
+                print("spin=", s)
+                f.write(f"spin={s}\n")
+                c = d_band(spin, dos_data)
+                f.write(str(c) + "\n")
+                print(c)
+
+    @logger.catch
+    def s6_1(self, bfile, dfile, ylims, outfile):
+        logger.info("正在处理，请稍等...")
+        from dspawpy.io.read import get_band_data, get_dos_data
+
+        band_data = get_band_data(bfile)
+        dos_data = get_dos_data(dfile)
+        from pymatgen.electronic_structure.plotter import BSDOSPlotter
+
+        bdp = BSDOSPlotter(dos_projection=None)
+        from dspawpy.plot import pltbd
+
+        pltbd(bdp, band_data, dos_data, ylim=ylims, filename=outfile)
+
+    @logger.catch
+    def s6_2(self, bfile, dfile, ylims, outfile):
+        logger.info("正在处理，请稍等...")
+        from dspawpy.io.read import get_band_data, get_dos_data
+
+        band_data = get_band_data(bfile)
+        dos_data = get_dos_data(dfile)
+        from pymatgen.electronic_structure.plotter import BSDOSPlotter
+
+        bdp = BSDOSPlotter(dos_projection="element")
+        from dspawpy.plot import pltbd
+
+        pltbd(bdp, band_data, dos_data, ylim=ylims, filename=outfile)
+
+    @logger.catch
+    def s7(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        _list = [
+            "AbsorptionCoefficient",
+            "ExtinctionCoefficient",
+            "RefractiveIndex",
+            "Reflectance",
+        ]
+        keys = until_give_valid_input(
+            f"数据类型（可选 {_list}）：",
+            _list,
+            completer=WordCompleter(_list),
+            allow_empty=True,
+        )
+        _list2 = ["X", "Y", "Z", "XY", "YZ", "ZX"]
+        label = until_give_valid_input(
+            f"指定数据 {_list2}：",
+            _list2,
+            completer=WordCompleter(_list2),
+            allow_empty=True,
+        )
+
+        outdir = prompt("输出文件路径：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.plot import plot_optical
+
+        if outdir.strip() != "":
+            os.makedirs(outdir, exist_ok=True)
+        plot_optical(datafile=infile, keys=keys, axes=label, prefix=outdir)
+
+    @logger.catch
+    def s8_1(
+        self,
+    ):
+        """插值NEB链"""
+        inis = prompt("初态构型文件路径（包含文件名）：", completer=pc)
+        fins = prompt("末态构型文件路径（包含文件名）：", completer=pc)
+        nmiddle = int(input("初末态之间插入几个构型："))
+        method = until_give_valid_input("插值方法（IDPP/Linear）：", ["IDPP", "Linear"])
+        outdir = prompt("输出文件夹（直接回车表示当前文件夹）：", completer=pc)
+        if outdir == "":
+            outdir = "."
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.diffusion.neb import NEB, write_neb_structures
+        from dspawpy.io.structure import read
+
+        init_struct = read(inis)[0]
+        final_struct = read(fins)[0]
+
+        neb = NEB(init_struct, final_struct, nmiddle + 2)
+        if method == "Linear":
+            structures = neb.linear_interpolate()  # 线性插值
+        elif method == "IDPP":
+            try:
+                structures = neb.idpp_interpolate()  # idpp插值
+            except Exception:
+                logger.error("  IDPP插值失败，请检查构型是否合理！")
+                structures = neb.linear_interpolate()
+                logger.warning("  已自动转为线性插值！")
+        else:
+            raise ValueError("Unknown interpolation method: {}".format(method))
+        # 保存 as 结构文件到 dest 路径下
+        absdir = os.path.abspath(outdir)
+        os.makedirs(os.path.dirname(absdir), exist_ok=True)
+        write_neb_structures(structures, fmt="as", path=absdir)
+        logger.info(f"已将插值后的构型保存到{absdir}路径下")
+
+        while True:
+            yn = input("是否预览插值链？（y/n）")
+            if yn.lower().startswith("y"):
+                from dspawpy.diffusion.nebtools import write_json_chain
+
+                write_json_chain(preview=True, directory=absdir)
+                break
+            elif yn.lower().startswith("n"):
+                break
+            else:
+                print("输入错误，请重新输入！")
+                continue
+
+    @logger.catch
+    def s8_2(
+        self,
+    ):
+        """绘制NEB势垒"""
+        infile = prompt(
+            "待解析neb.h5/neb.json路径（包含文件名）或NEB文件夹：", completer=pc
+        )
+        outfile = prompt("输出图片路径（包含文件名）：", completer=pc)
+        logger.info("插值方法默认使用pchip，如果要用其他方法，请使用独立脚本")
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.diffusion.nebtools import plot_barrier
+
+        if os.path.isdir(infile):
+            plot_barrier(directory=infile, figname=outfile, show=False)
+        elif os.path.isfile(infile):
+            plot_barrier(datafile=infile, figname=outfile, show=False)
+        else:
+            raise ValueError(f"{infile} 必须是文件或文件夹路径")
+
+    @logger.catch
+    def s8_3(
+        self,
+    ):
+        """输出NEB计算结果"""
+        datafolder = prompt("NEB计算文件夹：", completer=pc)
+        outdir = prompt("输出到文件夹（直接回车表示当前文件夹）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.diffusion.nebtools import summary
+
+        assert os.path.isdir(datafolder), f"{datafolder} 必须是文件夹路径"
+        absdir = os.path.abspath(outdir)
+        os.makedirs(os.path.dirname(absdir), exist_ok=True)
+        summary(
+            directory=datafolder,
+            outdir=absdir,
+            figname=f"{absdir}/neb_summary.png",
+            show=False,
+        )
+
+    @logger.catch
+    def s8_4(
+        self,
+    ):
+        """输出插值链"""
+        preview = until_give_valid_input(
+            "预览插值生成的NEB链（无需完成计算）（y/n）：", ["y", "n"]
+        )
+        directory = prompt("NEB计算文件夹：", completer=pc)
+        if preview == "y":
+            step = 0
+        else:
+            step = int(input("第几个离子步（从1开始计数，-1表示最新构型）："))
+        dst = prompt("输出到文件夹（直接回车表示当前文件夹）：", completer=pc)
+        json_or_xyz = until_give_valid_input(
+            "输出文件格式（json/xyz）：", ["json", "xyz"]
+        )
+        logger.info("正在处理，请稍等...")
+
+        if json_or_xyz.startswith("xyz"):
+            from dspawpy.diffusion.nebtools import write_xyz_chain
+
+            write_xyz_chain(False, directory, step, dst)
+        else:
+            from dspawpy.diffusion.nebtools import write_json_chain
+
+            write_json_chain(False, directory, step, dst)
+
+    @logger.catch
+    def s8_5(
+        self,
+    ):
+        """计算两个构型的距离"""
+        infile1 = prompt("第一个构型路径（包含文件名）：", completer=pc)
+        infile2 = prompt("第二个构型路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.structure import read
+
+        s1 = read(infile1)[0]
+        s2 = read(infile2)[0]
+        from dspawpy.diffusion.nebtools import get_distance
+
+        dist = get_distance(
+            s1.frac_coords, s2.frac_coords, s1.lattice.matrix, s2.lattice.matrix
+        )
+        logger.info(f"两个构型的距离为：{dist} Angstrom")
+
+    @logger.catch
+    def s8_6(
+        self,
+    ):
+        """续算"""
+        dataFolder = prompt("NEB计算文件夹：", completer=pc)
+        outdir = prompt("备份文件夹：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.diffusion.nebtools import restart
+
+        restart(dataFolder, outdir)
+
+    @logger.catch
+    def s9_1(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        ylims = check_lims("输入y轴范围（先小后大，空格分隔，直接回车可跳过）：")
+        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.read import get_phonon_band_data
+
+        band_data = get_phonon_band_data(infile)  # 读取声子能带
+
+        with HiddenPrints():
+            from pymatgen.phonon.plotter import PhononBSPlotter
+
+        bsp = PhononBSPlotter(band_data)
+        bsp.get_plot(ylim=ylims)
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s9_2(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        xlims = check_lims("输入x轴范围（先小后大，空格分隔，直接回车可跳过）：")
+        ylims = check_lims("输入y轴范围（先小后大，空格分隔，直接回车可跳过）：")
+        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.read import get_phonon_dos_data
+
+        dos = get_phonon_dos_data(infile)  # 读取声子能带
+        with HiddenPrints():
+            from pymatgen.phonon.plotter import PhononDosPlotter
+        dp = PhononDosPlotter(stack=False, sigma=None)
+        dp.add_dos(label="Phonon", dos=dos)
+        dp.get_plot(
+            xlim=xlims,  # x轴范围
+            ylim=ylims,  # y轴范围
+            units="thz",  # 单位
+        )
+
+        save_figure_dpi300(outfile)
+
+    @logger.catch
+    def s9_3(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.plot import plot_phonon_thermal
+
+        plot_phonon_thermal(infile, outfile, False)
+
+    @logger.catch
+    def s10_1(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        outfile = prompt("输出文件路径（包含.xyz或.dump文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.structure import convert
+
+        convert(infile, outfile=outfile)
+
+    @logger.catch
+    def s10_2(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        outfile = prompt("输出文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.plot import plot_aimd
+
+        plot_aimd(infile, show=False, figname=outfile)
+
+    @logger.catch
+    def s10_3(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        outfile = prompt("MSD图片输出路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.analysis.aimdtools import MSD, _get_time_step, plot_msd
+        from dspawpy.io.structure import read
+
+        structures = read(infile)
+        elements = [str(i) for i in structures[0].species]
+        unique_elements = list(set(elements))
+        select_str = input(
+            f"元素列表\n{elements}\n去重后\n{unique_elements}\n选择原子或元素（以空格隔开）："
+        )
+        boss = select_str.strip()
+        if boss == "":
+            select = "all"
+        else:
+            if ":" in boss:  # slice, '1:3', '1:3:2'
+                select = boss
+            elif " " in boss:  # list of symbols or atom indices, '1 2 3', 'H He Li'
+                raw_list = boss.split()
+                if all([i.isdigit() for i in raw_list]):
+                    select = [int(i) for i in raw_list]
+                elif all([i in unique_elements for i in raw_list]):
+                    select = raw_list
+                else:
+                    raise ValueError(f"Invalid input for select_str={select_str}")
+            else:
+                # single symbol or atom index
+                # boss may be H1, must remove digit before checking
+                if boss in unique_elements:
+                    select = boss  # symbol
+                elif boss.isdigit():
+                    select = int(boss)  # atom index
+                else:
+                    raise ValueError(f"Invalid input for select_str={select_str}")
+
+        print(select)
+        msd_type = until_give_valid_input(
+            "计算MSD的类型，可选xyz,xy,xz,yz,x,y,z，（直接回车等同于'xyz'，表示计算所有分量）",
+            ["xyz", "xy", "xz", "yz", "x", "y", "z", ""],
+        )
+        timestep = input(
+            f"输入时间步长（fs），直接回车将尝试从{infile}中自动读取，失败则此数值将设为1.0："
+        )
+        xlims = check_lims("输入x轴下限和上限，用空格分隔，直接回车将自动设置")
+        ylims = check_lims("输入y轴下限和上限，用空格分隔，直接回车将自动设置")
+
+        if msd_type == "":
+            msd_type = "xyz"
+
+        if timestep == "":
+            if isinstance(infile, str) or len(infile) == 1:
+                ts = _get_time_step(infile)
+            else:
+                logger.warning(
+                    "For multiple datafiles, you must manually specify the timestep. It will default to 1.0fs."
+                )
+                ts = 1.0
+        else:
+            ts = float(timestep)
+
+        msd_calculator = MSD(structures, select, msd_type)
+        msd = msd_calculator.run()
+
+        import numpy as np
+
+        xs = np.arange(msd_calculator.n_frames) * ts
+        plot_msd(xs, msd, xlims, ylims, figname=outfile, show=False)
+
+    @logger.catch
+    def s10_4(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        timestep = input(
+            f"输入时间步长（fs），直接回车将尝试从{infile}中自动读取，失败则此数值将设为1.0："
+        )
+        if timestep == "":
+            timestep = None
+        else:
+            timestep = float(timestep)
+        xlims = check_lims("输入x轴下限和上限，用空格分隔，直接回车将自动设置")
+        ylims = check_lims("输入y轴下限和上限，用空格分隔，直接回车将自动设置")
+        outfile = prompt("RMSD图片输出路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
+
+        lagtime, rmsd = get_lagtime_rmsd(infile, timestep)
+        plot_rmsd(lagtime, rmsd, xlims, ylims, outfile, False)
+
+    @logger.catch
+    def s10_5(
+        self,
+    ):
+        infile = prompt("待解析文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+        from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
+        from dspawpy.io.structure import read
+
+        strs = read(datafile=infile)
+        elements = [str(i) for i in strs[0].species]
+        unique_elements = list(set(elements))
+        print(f" 元素列表：{elements}\n 去重后：{unique_elements}")
+        ele1 = until_give_valid_input("--> 请选择一个中心元素：", unique_elements)
+        ele2 = until_give_valid_input("--> 请选择一个对象元素：", unique_elements)
+
+        rmin = input("请输入最小半径, Å （默认0）:")
+        if rmin == "":
+            rmin = 0
+        else:
+            rmin = float(rmin)
+
+        rmax = input("请输入最大半径, Å（默认10）:")
+        if rmax == "":
+            rmax = 10
+        else:
+            rmax = float(rmax)
+
+        ngrid = input("请输入网格数（默认101，包含端点）:")
+        if ngrid == "":
+            ngrid = 101
+        else:
+            ngrid = int(ngrid)
+
+        sigma = input("请输入sigma值（用于一维高斯函数平滑处理，默认0，不处理）:")
+        if sigma == "":
+            sigma = 0
+        else:
+            sigma = float(sigma)
+
+        xlims = [rmin, rmax]
+        ylims = check_lims("请依次输入y轴下限与上限，用空格分隔（默认不指定）:")
+        outfile = prompt("RDF图片输出路径（包含文件名）：", completer=pc)
+
+        rs, rdfs = get_rs_rdfs(infile, ele1, ele2, rmin, rmax, ngrid, sigma)
+        plot_rdf(rs, rdfs, ele1, ele2, xlims, ylims, outfile, False)
+
+    @logger.catch
+    def s11(
+        self,
+    ):  # --> pol.png
+        infile = prompt("已完成铁电极化计算任务的文件夹：", completer=pc)
+        repetition = int(input("请输入数据点绘图时重复次数（默认2）："))
+        if repetition == "":
+            repetition = 2
+        outfile = prompt("图片输出路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.plot import plot_polarization_figure
+
+        plot_polarization_figure(infile, repetition, figname=outfile, show=False)
+
+    @logger.catch
+    def s12(
+        self,
+    ):
+        infile = prompt("待解析frequency.txt文件路径（包含文件名）：", completer=pc)
+        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.utils import getZPE
+
+        print(getZPE(infile, outfile))
+
+    @logger.catch
+    def s13_1(
+        self,
+    ):
+        infile = prompt("待解析frequency.txt文件路径（包含文件名）：", completer=pc)
+        temperature = float(input("请输入温度(K)："))
+        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.utils import getTSads
+
+        TSads = getTSads(infile, temperature, outfile)
+        print("Entropy contribution, T*S (eV): ", TSads)
+
+    @logger.catch
+    def s13_2(
+        self,
+    ):
+        fretxt = prompt("待解析frequency.txt文件路径（包含文件名）：", completer=pc)
+        infile = prompt("待解析h5/json文件路径（包含文件名）：", completer=pc)
+        temperature = float(input("请输入温度(K)："))
+        pressure = float(input("请输入压强(Pa)："))
+        outfile = prompt("输出文本文件路径（包含文件名）：", completer=pc)
+        logger.info("如果要设置更多参数，请参考手册相应章节的独立脚本")
+        logger.info("正在处理，请稍等...")
+
+        from dspawpy.io.utils import getTSgas
+
+        TSgas = getTSgas(
+            fretxt=fretxt,
+            datafile=infile,
+            temperature=temperature,
+            pressure=pressure,
+            outfile=outfile,
+        )
+        print("--> T*S (eV): ", TSgas)
+
+
+@logger.catch
+def save_figure_dpi300(outfile):
+    absfile = os.path.abspath(outfile)
+    os.makedirs(os.path.dirname(absfile), exist_ok=True)
+    plt.tight_layout()
+    plt.savefig(absfile, dpi=300)
+    print(f"--> {absfile}")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dspawpy-1.2.0/dspawpy/diffusion/neb.py` & `dspawpy-1.2.2/dspawpy/diffusion/neb.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/diffusion/nebtools.py` & `dspawpy-1.2.2/dspawpy/diffusion/nebtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/diffusion/pathfinder.py` & `dspawpy-1.2.2/dspawpy/diffusion/pathfinder.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/read.py` & `dspawpy-1.2.2/dspawpy/io/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1151,15 +1151,15 @@
 
 
 def _get_total_dos(dos: dict):
     # h5 -> Dos Obj
     energies = np.asarray(dos["/DosInfo/DosEnergy"])
     from pymatgen.electronic_structure.core import Spin
 
-    if dos["/DosInfo/SpinType"][0] == "none":
+    if dos["/DosInfo/SpinType"][0] != "collinear":
         densities = {Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"])}
     else:
         densities = {
             Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"]),
             Spin.down: np.asarray(dos["/DosInfo/Spin2/Dos"]),
         }
 
@@ -1171,15 +1171,15 @@
 
 
 def _get_total_dos_json(dos: dict):
     # json -> Dos Obj
     energies = np.asarray(dos["DosInfo"]["DosEnergy"])
     from pymatgen.electronic_structure.core import Spin
 
-    if dos["DosInfo"]["SpinType"] == "none":
+    if dos["DosInfo"]["SpinType"] != "collinear":
         densities = {Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"])}
     else:
         densities = {
             Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"]),
             Spin.down: np.asarray(dos["DosInfo"]["Spin2"]["Dos"]),
         }
     efermi = dos["DosInfo"]["EFermi"]
@@ -1297,18 +1297,15 @@
 def _get_band_data_h5(band: dict, iwan=False, zero_to_efermi=False):
     if iwan:
         bd = "WannBandInfo"
     else:
         bd = "BandInfo"
     number_of_band = band[f"/{bd}/NumberOfBand"][0]
     number_of_kpoints = band[f"/{bd}/NumberOfKpoints"][0]
-    if (
-        band[f"/{bd}/SpinType"][0] == "none"
-        or band[f"/{bd}/SpinType"][0] == "non-collinear"
-    ):
+    if band[f"/{bd}/SpinType"][0] != "collinear":
         number_of_spin = 1
     else:
         number_of_spin = 2
 
     symmetry_kPoints_index = band[f"/{bd}/SymmetryKPointsIndex"]
 
     efermi = band[f"/{bd}/EFermi"][0]
@@ -1390,73 +1387,73 @@
         bd = "WannBandInfo"
         structure = _get_structure_json(syst["AtomInfo"])
         efermi = syst["Energy"]["EFermi"]
     else:
         bd = "BandInfo"
         structure = _get_structure_json(band["AtomInfo"])
 
-    number_of_band = band[f"{bd}"]["NumberOfBand"]
-    number_of_kpoints = band[f"{bd}"]["NumberOfKpoints"]
-    if "Spin2" in band[f"{bd}"]:
-        number_of_spin = 2
-    else:
+    number_of_band = band[bd]["NumberOfBand"]
+    number_of_kpoints = band[bd]["NumberOfKpoints"]
+    if band[bd]['SpinType'][0] != 'collinear':
         number_of_spin = 1
+    else:
+        number_of_spin = 2
 
-    symmetry_kPoints_index = band[f"{bd}"]["SymmetryKPointsIndex"]
+    symmetry_kPoints_index = band[bd]["SymmetryKPointsIndex"]
 
-    if "EFermi" in band[f"{bd}"]:
-        efermi = band[f"{bd}"]["EFermi"]
+    if "EFermi" in band[bd]:
+        efermi = band[bd]["EFermi"]
 
     eigenvals = {}
     from pymatgen.electronic_structure.core import Spin
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
 
-        if "BandEnergies" in band[f"{bd}"][spin_key]:
-            data = band[f"{bd}"][spin_key]["BandEnergies"]
-        elif "Band" in band[f"{bd}"][spin_key]:
-            data = band[f"{bd}"][spin_key]["Band"]
+        if "BandEnergies" in band[bd][spin_key]:
+            data = band[bd][spin_key]["BandEnergies"]
+        elif "Band" in band[bd][spin_key]:
+            data = band[bd][spin_key]["Band"]
         else:
             print("Band key error")
             return
 
         band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
 
         if zero_to_efermi:
             eigenvals[spin] = band_data - efermi
 
         else:
             eigenvals[spin] = band_data
 
-    kpoints = np.asarray(band[f"{bd}"]["CoordinatesOfKPoints"]).reshape(
+    kpoints = np.asarray(band[bd]["CoordinatesOfKPoints"]).reshape(
         number_of_kpoints, 3
     )
 
     labels_dict = {}
 
-    for i, s in enumerate(band[f"{bd}"]["SymmetryKPoints"]):
+    for i, s in enumerate(band[bd]["SymmetryKPoints"]):
         labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
 
     # read projection data
     projections = None
-    if "IsProject" in band[f"{bd}"].keys():
-        if band[f"{bd}"]["IsProject"]:
+    if "IsProject" in band[bd].keys():
+        if band[bd]["IsProject"]:
             projections = {}
-            number_of_orbit = len(band[f"{bd}"]["Orbit"])
+            number_of_orbit = len(band[bd]["Orbit"])
             projection = np.zeros(
                 (number_of_band, number_of_kpoints, number_of_orbit, len(structure))
             )
 
             for i in range(number_of_spin):
                 spin_key = "Spin" + str(i + 1)
                 spin = Spin.up if i == 0 else Spin.down
 
-                data = band[f"{bd}"][spin_key]["ProjectBand"]
+                data = band[bd][spin_key]["ProjectBand"]
                 for d in data:
                     orbit_index = d["OrbitIndex"] - 1
                     atom_index = d["AtomIndex"] - 1
                     project_data = d["Contribution"]
                     projection[:, :, orbit_index, atom_index] = (
                         np.asarray(project_data)
                         .reshape((number_of_kpoints, number_of_band))
```

### Comparing `dspawpy-1.2.0/dspawpy/io/structure.py` & `dspawpy-1.2.2/dspawpy/io/structure.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/utils.py` & `dspawpy-1.2.2/dspawpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/write.py` & `dspawpy-1.2.2/dspawpy/io/write.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/plot.py` & `dspawpy-1.2.2/dspawpy/plot.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy.egg-info/PKG-INFO` & `dspawpy-1.2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,249 +1,231 @@
-Metadata-Version: 2.1
-Name: dspawpy
-Version: 1.2.0
-Summary: Tools for dspaw
-Home-page: http://www.hzwtech.com/
-Author: Hzwtech
-Author-email: ZhengZhilin@hzwtech.com
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pymatgen>=2022.2.7
-Requires-Dist: statsmodels
-Requires-Dist: h5py
-Requires-Dist: monty
-Requires-Dist: prompt_toolkit
-Requires-Dist: loguru
-
-![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
-![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
-![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
-
-# Introduction （简介）
-
-dspawpy is a post-processing tool mainly for DFT package [DS-PAW](https://cloud.hzwtech.com/web/product-service?id=10), providing some functions of data capture, conversion, structure conversion, and drawing. （dspawpy 主要是 [DS-PAW](https://cloud.hzwtech.com/web/product-service?id=10) 软件的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能）
-
-## Installation （安装）
-
-Either by pip: （通过pip安装）
-
-```bash
-pip install dspawpy -U --user
-```
-
-Or by conda: （通过conda安装）
-
-```bash
-conda install -c conda-forge dspawpy
-```
-
-## CHANGELOG （版本更新简述）
-
-### 1.2.0
-
-- 体验优化： 将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
-- 体验优化： cli增加模糊匹配功能
-- 体验优化： optical绘图默认绘制全部数据以便查看
-- 体验优化： neb备份时如果目标文件夹已存在，将原先的改名成附加时间戳的文件夹
-- BUG修复： dos非线性自旋时无法读取h5/json数据
-
-
-### 1.1.9
-
-- BUG修复： 修复cli的一些已知bug
-
-### 1.1.8
-
-- 功能强化： 体数据（volumetric data）支持自定义网格插值（调用scipy的RegularGridInterpolator插值器）；增加 txt 格式支持，每行包含格点的 xyz 坐标和具体数值
-
-### 1.1.7
-
-- BUG修复： 修复conda install dspawpy后cli没有同步安装导致无法唤起的故障
-- BUG修复： 移除 plot_dos 函数中 xlim、ylim两个参数类型提示，以避免python<3.9的运行错误
-- BUG修复： 老版本python, pymatgen, monty等第三方库的兼容性问题
-
-### 1.1.6
-
-- 重要变更： cli 环境部署模块改成dspawpy更新模块，因为现在cli内置于dspawpy中，在hzw机器上唤起cli必定已经source环境了，不再需要原先的1.1功能；仅保留原先的1.2功能，即升级dspawpy
-- BUG修复： 移除 plot_dos 函数中 xlim、ylim两个参数类型提示时使用的 | 符号（需要python3.10支持），以避免python<3.10的运行错误
-
-### 1.1.5
-
-- 功能强化： 从pmg中提取plot_dos函数，增加raw参数用于输出投影态密度绘图坐标点数据到dos_raw.csv，使用案例请参考辅助工具使用教程——dos部分
-
-### 1.1.4
-
-- BUG修复： cli 5-6 d带中心参数传递错误
-- BUG修复： cli 7-1 内部传参错误
-- BUG修复： structure结构写成文件时应采用元素符号而不是带电荷的species
-- BUG修复： __init__.py 中版本号未及时更新(影响1.1.2和1.1.3两个版本)
-
-### 1.1.3
-
-- BUG修复： 增加cli所需两个依赖，移除python3.12的语法警告
-
-### 1.1.2
-
-- 功能强化： cli 默认调用 agg 作为matplotlib的绘图后端，避免在某些linux服务器上由于X11转发未设置导致的QT相关问题
-- 功能强化： cli 优化NEB链功能提示语
-- BUG修复： 兼容python3.12和numpy>1.24
-- BUG修复： 用户脚本兼容新旧pymatgen
-- BUG修复： NEB续算默认备份文件夹改名成backup
-
-### 1.1.1
-
-- 重要变更： cli并入dspapwy，不需要再去官网下载cli了
-- 功能强化： cli多处细节优化，提升交互体验
-- 功能强化： 增加 dump_bs_raw() 和 dump_dos_raw() 函数，功能有限
-
-### 1.1.0
-
-- BUG修复： io.write.write_VESTA() 和 io.write.write_delta_rho_vesta() 增加 inorm 参数，用于控制是否归一化（默认关闭）
-- 功能强化： io.write.write_VESTA() 和 io.write.write_delta_rho_vesta() 增加 compact 参数，可以在不影响VESTA显示效果的前提下，减小写出的文件（如 .cube ）体积（默认关闭）
-- 功能强化： 新增 bdplot() 函数（基于pymatgen的BSDOSPlotter类的get_plot函数优化），用于绘制能带态密度图，详见手册说明
-
-### 1.0.9
-
-- BUG修复： as结构文件中的原子自由度标签可以将 Fix_x Fix_y Fix_z 缩写为 Fix，其他内容不变
-- 重要变更： 使用 diffusion.nebtools.write_json_chain/write_xyz_chain() 生成NEB链时如果step=-1，则优先读取 latestStructureXX.as，失败后尝试 nebXX.h5，最后尝试 nebXX.json；可以使用 ignorels 参数忽略 latestStructureXX.as
-
-### 1.0.8
-
-- BUG修复： 准备弃用的 build_Structures_from_datafile() 未返回结构，read() 不受影响；其他调用 build_Structures_from_datafile() 的函数改为调用 read
-- BUG修复： 修复 io.read.get_band_data() 考虑自旋且设置了zero_to_efermi时，自旋向下能带数据解析错误的问题
-- 功能强化： io.structure模块新增 read() 代替 build_Structures_from_datafile()，write() 代替 io.write.to_file()，convert() 封装 read() 和 write() 函数，便于快速调用
-
-### 1.0.5
-
-- 功能强化： to_file() 写pdb文件时，结构可以不含晶胞信息
-
-### 1.0.4
-
-- BUG修复： build_Structures_from_datafile()选择原子序号时上限设置，h5文件里最后一个离子步信息改成尝试读取
-- 功能强化： build_Structures_from_datafile()支持读取pdb格式
-- 细节修改： AIMD读不到PressureKinetic信息时增加相应警告
-
-### 1.0.3
-
-- BUG修复： 解决浮点数过大时volumetricData相关文件浮点数粘在一起的问题
-- BUG修复： plot_barrier()读取neb.h5/json绘制能垒图时，反应坐标依旧累加
-- BUG修复： plot_bandunfolding()能带反折叠费米能级被默认置零
-- 功能强化： 新增cube格式用于保存volumetricData
-- 功能强化： 全局支持相对路径与绝对路径混写
-- 功能强化： datafile参数以及io.read以及diffusion.nebtools模块中的相应参数，可以是文件位置，也可以是文件所在的文件夹路径
-- 功能强化： build_Structures_from_datafile()增加task参数，用于配合datafile为文件夹路径的情况
-- 重要变更： 移除中文提示语句，精简提示信息
-- 重要变更： volumetricData默认使用cube格式写入
-- 重要变更： 移除thermo_correction()，一个单纯的外包装函数
-- 细节修改： 保存图片或文件时，统一使用 ==> 标记文件绝对路径
-
-### 1.0.2
-
-- BUG修复：  当存在Fix或Mag信息时，structure.as 坐标类型可能解析错误的问题
-- 功能强化： 预览NEB链条函数改名 write_xyz(json)_chain，增加dst参数制定保存路径
-- 功能强化： potential 中数据集不预作限制
-- 功能强化： get_lagtime_msd, get_lagtime_rmsd 自动从数据文件中读取timestep（以前必须手动指定）
-- 细节修改： 优化部分提示语句
-
-### 1.0.1
-
-- BUG修复： to_file绑定filename参数，避免老版本pymatgen的兼容性问题
-- BUG修复： average_along_axis的task参数改成大小写敏感，避免rhoBound任务类型解析错误
-- 功能强化： 将文件存入不存在的目录前，先创建（支持相对路径）
-- 功能强化： write_VESTA和average_along_axis增加subtype参数，指定TotalLocalPotential数据
-
-### 1.0.0
-
-- BUG修复： 文件开头增加utf8编码声明
-- 功能强化： 电荷密度差分支持更多组分（不限二元）
-- 重要变更： io.utils的getZPE、getTSads、getTSgas函数，增加参数用于将计算结果存入文件
-- 重要变更： io.write.write_VESTA() data_type参数可选值从boundcharge改成rhoBound，且大小写敏感，从而保持与DS-PAW输出文件名相同
-
-### 0.9.9
-
-- BUG修复： 修复新版numpy不支持混用array和list生成数组的问题
-- BUG修复： 修复从json文件读能带时zero_to_efermi不生效的问题
-- 新增功能： build_Structures_from_datafile模块支持读取 neb.h5 和 phonon.h5 文件
-- 重要变更： 移除io模块中冗余的 _json.py （相关功能已整合进其他模块中并有所加强）
-- 重要变更： 删除 setup.py 中不需要的 joblib 依赖库
-
-### 0.9.8
-
-- BUG修复： to_file 和 build_Structures_from_datafile 接口统一
-- BUG修复： io.write模块涉及的保存文件操作，当目标路径上层文件夹不存在时将自动创建
-- BUG修复： io.read.get_band_data的zero_to_efermi参数设置为True时，数据的处理逻辑
-- BUG修复： io.read.get_sinfo读取relax.json不再因FixLattice而报错
-- 新增选项： nebtools的summary函数，新增show_converge用于控制是否显示收敛图，outdir用于指定收敛图的路径
-- 新增功能： 写文件涉及的操作，支持传入路径，而不单是文件名
-- 新增功能： nebtools的restart函数支持在Windows机器上操作，不必在旧NEB路径执行，备份路径可随意指定
-- 新增功能： nebtools的get_neb_subfolder函数新增return_abs参数，用于返回子文件夹的绝对路径
-- 重要变更： nebtools的restart函数删除inputin参数，采用压缩较快的zip方法，将生成zip压缩包而不是tar.xz
-- 重要变更： io.read.get_band_data的zero_to_fermi参数改名zero_to_efermi
-
-### 0.9.7
-
-- BUG修复： get_rdf 元素对自己计算RDF时的索引
-- 新增选项：to_file 增加 si 参数，支持读入单个structure以及Structure列表
-
-### 0.9.6
-
-- BUG修复： pymatgen支持的几类结构文件的读取接口
-
-### 0.9.5
-
-- 重要变更： get_band_data 的 shift_efermi 参数改名为 zero_to_fermi
-
-### 0.9.4
-
-- 新增功能： get_band_data 增加 shift_efermi 参数
-- BUG修复： 电荷密度差分函数移除 numpy 多维数组的 shape 参数
-- BUG修复： Fe_1 -> Fe+, Fe_2 -> Fe2+ 用于能带、态密度绘图
-
-### 0.9.3
-
-- 新增功能： 接入pymatgen支持的几类结构文件的读写操作
-- 新增功能： 支持通过 `dspawpy.__version__` 查看版本号
-- 重要变更： write_xyz_traj, write_dump_traj 并入 to_file 函数
-- 细节优化： 大幅提高RDF计算效率
-
-### 0.9.2
-
-- 新增功能： 支持从as文件中解析磁矩和FIX信息
-- 新增功能： 从h5/json文件中读取数据时支持指定读取的离子步（从1开始）
-
-### 0.9.1
-
-- 重要变更： 精简合并多个函数，统一调用方法
-- 新增功能： 支持合并多个xyz和dump文件
-- 细节优化： 读取h5或json文件后若无错误，不再打印空行
-- 细节优化： 耗时的RDF计算显示进度百分比
-
-### 0.9.0
-
-- 重要变更： 一些函数合并、所在模块迁移，请确认版本
-- 新增功能： 支持读取含多离子步计算结果的h5/json文件中的磁矩信息
-- BUG修复： get_band_data 函数指定efermi不生效
-
-### 0.8.9
-
-- BUG修复： d_band 脚本运行错误
-
-### 0.8.8
-
-- 新增功能： 支持读取正在进行中的NEB信息，生成movie轨迹文件（可用DS打开观察）
-- 新增功能： 支持NEB转XYZ轨迹文件（可用OVITO打开观察）
-- 新增功能： plot_aimd 支持读取多个h5文件画在同一张图中
-- BUG修复： 电荷差分处理json文件报错
-- BUG修复： 极化曲线标记的数值错误
-- BUG修复： neb_movie_*.json 中反应坐标重复累加错误
-
-### 0.8.7
-
-- 代码重构，大幅修改数据结构，加速处理过程
-- 支持读取h5格式的输出文件
-- 新增AIMD, NEB等部分常用功能
-
-### 0.3.0
-
-- 对应2021A版本DS-PAW，辅助处理一些常见数据文件
+![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
+![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
+![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
+
+# Introduction （简介）
+
+dspawpy is a post-processing tool mainly for DFT package [DS-PAW](https://cloud.hzwtech.com/web/product-service?id=10), providing some functions of data capture, conversion, structure conversion, and drawing. （dspawpy 主要是 [DS-PAW](https://cloud.hzwtech.com/web/product-service?id=10) 软件的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能）
+
+## Installation （安装）
+
+Either by pip: （通过pip安装）
+
+```bash
+pip install dspawpy -U --user
+```
+
+Or by conda: （通过conda安装）
+
+```bash
+conda install -c conda-forge dspawpy
+```
+
+## CHANGELOG （版本更新简述）
+
+### 1.2.0
+
+- 体验优化： 将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
+- 体验优化： cli增加模糊匹配功能
+- 体验优化： optical绘图默认绘制全部数据以便查看
+- 体验优化： neb备份时如果目标文件夹已存在，将原先的改名成附加时间戳的文件夹
+- BUG修复： dos非线性自旋时无法读取h5/json数据
+
+
+### 1.1.9
+
+- BUG修复： 修复cli的一些已知bug
+
+### 1.1.8
+
+- 功能强化： 体数据（volumetric data）支持自定义网格插值（调用scipy的RegularGridInterpolator插值器）；增加 txt 格式支持，每行包含格点的 xyz 坐标和具体数值
+
+### 1.1.7
+
+- BUG修复： 修复conda install dspawpy后cli没有同步安装导致无法唤起的故障
+- BUG修复： 移除 plot_dos 函数中 xlim、ylim两个参数类型提示，以避免python<3.9的运行错误
+- BUG修复： 老版本python, pymatgen, monty等第三方库的兼容性问题
+
+### 1.1.6
+
+- 重要变更： cli 环境部署模块改成dspawpy更新模块，因为现在cli内置于dspawpy中，在hzw机器上唤起cli必定已经source环境了，不再需要原先的1.1功能；仅保留原先的1.2功能，即升级dspawpy
+- BUG修复： 移除 plot_dos 函数中 xlim、ylim两个参数类型提示时使用的 | 符号（需要python3.10支持），以避免python<3.10的运行错误
+
+### 1.1.5
+
+- 功能强化： 从pmg中提取plot_dos函数，增加raw参数用于输出投影态密度绘图坐标点数据到dos_raw.csv，使用案例请参考辅助工具使用教程——dos部分
+
+### 1.1.4
+
+- BUG修复： cli 5-6 d带中心参数传递错误
+- BUG修复： cli 7-1 内部传参错误
+- BUG修复： structure结构写成文件时应采用元素符号而不是带电荷的species
+- BUG修复： __init__.py 中版本号未及时更新(影响1.1.2和1.1.3两个版本)
+
+### 1.1.3
+
+- BUG修复： 增加cli所需两个依赖，移除python3.12的语法警告
+
+### 1.1.2
+
+- 功能强化： cli 默认调用 agg 作为matplotlib的绘图后端，避免在某些linux服务器上由于X11转发未设置导致的QT相关问题
+- 功能强化： cli 优化NEB链功能提示语
+- BUG修复： 兼容python3.12和numpy>1.24
+- BUG修复： 用户脚本兼容新旧pymatgen
+- BUG修复： NEB续算默认备份文件夹改名成backup
+
+### 1.1.1
+
+- 重要变更： cli并入dspapwy，不需要再去官网下载cli了
+- 功能强化： cli多处细节优化，提升交互体验
+- 功能强化： 增加 dump_bs_raw() 和 dump_dos_raw() 函数，功能有限
+
+### 1.1.0
+
+- BUG修复： io.write.write_VESTA() 和 io.write.write_delta_rho_vesta() 增加 inorm 参数，用于控制是否归一化（默认关闭）
+- 功能强化： io.write.write_VESTA() 和 io.write.write_delta_rho_vesta() 增加 compact 参数，可以在不影响VESTA显示效果的前提下，减小写出的文件（如 .cube ）体积（默认关闭）
+- 功能强化： 新增 bdplot() 函数（基于pymatgen的BSDOSPlotter类的get_plot函数优化），用于绘制能带态密度图，详见手册说明
+
+### 1.0.9
+
+- BUG修复： as结构文件中的原子自由度标签可以将 Fix_x Fix_y Fix_z 缩写为 Fix，其他内容不变
+- 重要变更： 使用 diffusion.nebtools.write_json_chain/write_xyz_chain() 生成NEB链时如果step=-1，则优先读取 latestStructureXX.as，失败后尝试 nebXX.h5，最后尝试 nebXX.json；可以使用 ignorels 参数忽略 latestStructureXX.as
+
+### 1.0.8
+
+- BUG修复： 准备弃用的 build_Structures_from_datafile() 未返回结构，read() 不受影响；其他调用 build_Structures_from_datafile() 的函数改为调用 read
+- BUG修复： 修复 io.read.get_band_data() 考虑自旋且设置了zero_to_efermi时，自旋向下能带数据解析错误的问题
+- 功能强化： io.structure模块新增 read() 代替 build_Structures_from_datafile()，write() 代替 io.write.to_file()，convert() 封装 read() 和 write() 函数，便于快速调用
+
+### 1.0.5
+
+- 功能强化： to_file() 写pdb文件时，结构可以不含晶胞信息
+
+### 1.0.4
+
+- BUG修复： build_Structures_from_datafile()选择原子序号时上限设置，h5文件里最后一个离子步信息改成尝试读取
+- 功能强化： build_Structures_from_datafile()支持读取pdb格式
+- 细节修改： AIMD读不到PressureKinetic信息时增加相应警告
+
+### 1.0.3
+
+- BUG修复： 解决浮点数过大时volumetricData相关文件浮点数粘在一起的问题
+- BUG修复： plot_barrier()读取neb.h5/json绘制能垒图时，反应坐标依旧累加
+- BUG修复： plot_bandunfolding()能带反折叠费米能级被默认置零
+- 功能强化： 新增cube格式用于保存volumetricData
+- 功能强化： 全局支持相对路径与绝对路径混写
+- 功能强化： datafile参数以及io.read以及diffusion.nebtools模块中的相应参数，可以是文件位置，也可以是文件所在的文件夹路径
+- 功能强化： build_Structures_from_datafile()增加task参数，用于配合datafile为文件夹路径的情况
+- 重要变更： 移除中文提示语句，精简提示信息
+- 重要变更： volumetricData默认使用cube格式写入
+- 重要变更： 移除thermo_correction()，一个单纯的外包装函数
+- 细节修改： 保存图片或文件时，统一使用 ==> 标记文件绝对路径
+
+### 1.0.2
+
+- BUG修复：  当存在Fix或Mag信息时，structure.as 坐标类型可能解析错误的问题
+- 功能强化： 预览NEB链条函数改名 write_xyz(json)_chain，增加dst参数制定保存路径
+- 功能强化： potential 中数据集不预作限制
+- 功能强化： get_lagtime_msd, get_lagtime_rmsd 自动从数据文件中读取timestep（以前必须手动指定）
+- 细节修改： 优化部分提示语句
+
+### 1.0.1
+
+- BUG修复： to_file绑定filename参数，避免老版本pymatgen的兼容性问题
+- BUG修复： average_along_axis的task参数改成大小写敏感，避免rhoBound任务类型解析错误
+- 功能强化： 将文件存入不存在的目录前，先创建（支持相对路径）
+- 功能强化： write_VESTA和average_along_axis增加subtype参数，指定TotalLocalPotential数据
+
+### 1.0.0
+
+- BUG修复： 文件开头增加utf8编码声明
+- 功能强化： 电荷密度差分支持更多组分（不限二元）
+- 重要变更： io.utils的getZPE、getTSads、getTSgas函数，增加参数用于将计算结果存入文件
+- 重要变更： io.write.write_VESTA() data_type参数可选值从boundcharge改成rhoBound，且大小写敏感，从而保持与DS-PAW输出文件名相同
+
+### 0.9.9
+
+- BUG修复： 修复新版numpy不支持混用array和list生成数组的问题
+- BUG修复： 修复从json文件读能带时zero_to_efermi不生效的问题
+- 新增功能： build_Structures_from_datafile模块支持读取 neb.h5 和 phonon.h5 文件
+- 重要变更： 移除io模块中冗余的 _json.py （相关功能已整合进其他模块中并有所加强）
+- 重要变更： 删除 setup.py 中不需要的 joblib 依赖库
+
+### 0.9.8
+
+- BUG修复： to_file 和 build_Structures_from_datafile 接口统一
+- BUG修复： io.write模块涉及的保存文件操作，当目标路径上层文件夹不存在时将自动创建
+- BUG修复： io.read.get_band_data的zero_to_efermi参数设置为True时，数据的处理逻辑
+- BUG修复： io.read.get_sinfo读取relax.json不再因FixLattice而报错
+- 新增选项： nebtools的summary函数，新增show_converge用于控制是否显示收敛图，outdir用于指定收敛图的路径
+- 新增功能： 写文件涉及的操作，支持传入路径，而不单是文件名
+- 新增功能： nebtools的restart函数支持在Windows机器上操作，不必在旧NEB路径执行，备份路径可随意指定
+- 新增功能： nebtools的get_neb_subfolder函数新增return_abs参数，用于返回子文件夹的绝对路径
+- 重要变更： nebtools的restart函数删除inputin参数，采用压缩较快的zip方法，将生成zip压缩包而不是tar.xz
+- 重要变更： io.read.get_band_data的zero_to_fermi参数改名zero_to_efermi
+
+### 0.9.7
+
+- BUG修复： get_rdf 元素对自己计算RDF时的索引
+- 新增选项：to_file 增加 si 参数，支持读入单个structure以及Structure列表
+
+### 0.9.6
+
+- BUG修复： pymatgen支持的几类结构文件的读取接口
+
+### 0.9.5
+
+- 重要变更： get_band_data 的 shift_efermi 参数改名为 zero_to_fermi
+
+### 0.9.4
+
+- 新增功能： get_band_data 增加 shift_efermi 参数
+- BUG修复： 电荷密度差分函数移除 numpy 多维数组的 shape 参数
+- BUG修复： Fe_1 -> Fe+, Fe_2 -> Fe2+ 用于能带、态密度绘图
+
+### 0.9.3
+
+- 新增功能： 接入pymatgen支持的几类结构文件的读写操作
+- 新增功能： 支持通过 `dspawpy.__version__` 查看版本号
+- 重要变更： write_xyz_traj, write_dump_traj 并入 to_file 函数
+- 细节优化： 大幅提高RDF计算效率
+
+### 0.9.2
+
+- 新增功能： 支持从as文件中解析磁矩和FIX信息
+- 新增功能： 从h5/json文件中读取数据时支持指定读取的离子步（从1开始）
+
+### 0.9.1
+
+- 重要变更： 精简合并多个函数，统一调用方法
+- 新增功能： 支持合并多个xyz和dump文件
+- 细节优化： 读取h5或json文件后若无错误，不再打印空行
+- 细节优化： 耗时的RDF计算显示进度百分比
+
+### 0.9.0
+
+- 重要变更： 一些函数合并、所在模块迁移，请确认版本
+- 新增功能： 支持读取含多离子步计算结果的h5/json文件中的磁矩信息
+- BUG修复： get_band_data 函数指定efermi不生效
+
+### 0.8.9
+
+- BUG修复： d_band 脚本运行错误
+
+### 0.8.8
+
+- 新增功能： 支持读取正在进行中的NEB信息，生成movie轨迹文件（可用DS打开观察）
+- 新增功能： 支持NEB转XYZ轨迹文件（可用OVITO打开观察）
+- 新增功能： plot_aimd 支持读取多个h5文件画在同一张图中
+- BUG修复： 电荷差分处理json文件报错
+- BUG修复： 极化曲线标记的数值错误
+- BUG修复： neb_movie_*.json 中反应坐标重复累加错误
+
+### 0.8.7
+
+- 代码重构，大幅修改数据结构，加速处理过程
+- 支持读取h5格式的输出文件
+- 新增AIMD, NEB等部分常用功能
+
+### 0.3.0
+
+- 对应2021A版本DS-PAW，辅助处理一些常见数据文件
```

### Comparing `dspawpy-1.2.0/dspawpy.egg-info/SOURCES.txt` & `dspawpy-1.2.2/dspawpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/setup.py` & `dspawpy-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     monty_version = "monty<=2021.12.1"  # removed os.path.which
 else:
     pmg_version = "pymatgen >= 2022.2.7"  # removed monty os.path.which
     monty_version = "monty"
 
 setup(
     name="dspawpy",
-    version="1.2.0",
+    version="1.2.2",
     packages=find_packages(),
     url="http://www.hzwtech.com/",
     license="MIT",
     author="Hzwtech",
     author_email="ZhengZhilin@hzwtech.com",
     description="Tools for dspaw",
     install_requires=[
```

