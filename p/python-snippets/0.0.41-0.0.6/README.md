# Comparing `tmp/python-snippets-0.0.41.tar.gz` & `tmp/python-snippets-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-snippets-0.0.41.tar", last modified: Thu Apr 11 06:12:08 2024, max compression
+gzip compressed data, was "python-snippets-0.0.6.tar", last modified: Tue Nov  1 06:44:17 2022, max compression
```

## Comparing `python-snippets-0.0.41.tar` & `python-snippets-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-11 06:12:08.259786 python-snippets-0.0.41/
--rw-r--r--   0 chenhao    (501) staff       (20)      248 2024-04-11 06:12:08.259601 python-snippets-0.0.41/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)       98 2022-05-31 09:28:56.000000 python-snippets-0.0.41/README.md
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-11 06:12:08.259336 python-snippets-0.0.41/python_snippets.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      248 2024-04-11 06:12:08.000000 python-snippets-0.0.41/python_snippets.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)      395 2024-04-11 06:12:08.000000 python-snippets-0.0.41/python_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-11 06:12:08.000000 python-snippets-0.0.41/python_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)       43 2024-04-11 06:12:08.000000 python-snippets-0.0.41/python_snippets.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        9 2024-04-11 06:12:08.000000 python-snippets-0.0.41/python_snippets.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-11 06:12:08.000000 python-snippets-0.0.41/python_snippets.egg-info/zip-safe
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-11 06:12:08.259847 python-snippets-0.0.41/setup.cfg
--rwxr-xr-x   0 chenhao    (501) staff       (20)     1407 2024-02-04 07:32:57.000000 python-snippets-0.0.41/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-11 06:12:08.256619 python-snippets-0.0.41/snippets/
--rw-r--r--   0 chenhao    (501) staff       (20)      562 2024-03-07 03:20:54.000000 python-snippets-0.0.41/snippets/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5645 2024-03-07 05:46:39.000000 python-snippets-0.0.41/snippets/decorators.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2936 2024-02-04 07:37:02.000000 python-snippets-0.0.41/snippets/evaluate.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3400 2024-04-11 03:18:14.000000 python-snippets-0.0.41/snippets/logs.py
--rw-r--r--   0 chenhao    (501) staff       (20)      560 2023-10-19 10:20:06.000000 python-snippets-0.0.41/snippets/mixin.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1875 2024-03-07 02:56:24.000000 python-snippets-0.0.41/snippets/perf.py
--rw-r--r--   0 chenhao    (501) staff       (20)    12280 2024-03-19 07:59:22.000000 python-snippets-0.0.41/snippets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 06:44:17.188819 python-snippets-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-01 06:44:01.000000 python-snippets-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/python_snippets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 06:44:16.000000 python-snippets-0.0.6/python_snippets.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 06:44:17.188819 python-snippets-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      849 2022-11-01 06:44:01.000000 python-snippets-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7856 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/utils.py
```

### Comparing `python-snippets-0.0.41/snippets/utils.py` & `python-snippets-0.0.6/snippets/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,47 +5,47 @@
    File Name：     utils.py
    Author :       chenhao
    time：          2021/10/14 17:41
    Description :
 -------------------------------------------------
 """
 import collections
-import copy
-import json
 import os
+import json
 import pickle
-import re
 import subprocess
 import time
-from datetime import datetime
-import pandas as pd
-from typing import Any, Dict, Iterable, List, Sequence, Tuple, _GenericAlias, Union
-
+import logging
 import numpy as np
 from pydantic import BaseModel
+from datetime import datetime
+
+from typing import Any, List, Sequence, Tuple, Iterable, Dict, _GenericAlias
+
 from tqdm import tqdm
-from loguru import logger
+
+logger = logging.getLogger(__name__)
 
 
 # 创建一个目录
 def create_dir_path(path: str):
-    dir_path = os.path.abspath(os.path.dirname(path))
+    dir_path = os.path.dirname(path)
     if not os.path.exists(dir_path):
         os.makedirs(dir_path)
 
 
 # 将一个object encode成json string的方法
 class PythonObjectEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, bytes):
             return str(obj)
         if isinstance(obj, set):
             return list(obj)
         if isinstance(obj, BaseModel):
-            return obj.model_dump(exclude_none=True, exclude_defaults=True)
+            return obj.dict(exclude_none=True, exclude_defaults=True)
         if isinstance(obj, datetime):
             return obj.strftime("%Y-%M-%d %H:%m:%S")
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
@@ -82,16 +82,15 @@
 def jdump_lines(obj, fp, mode="w", progbar=False):
     iter_obj = tqdm(obj) if progbar else obj
     if isinstance(fp, str):
         create_dir_path(fp)
         fp = open(fp, mode=mode, encoding="utf8")
     with fp:
         for item in iter_obj:
-            line = json.dumps(item, ensure_ascii=False,
-                              cls=PythonObjectEncoder) + "\n"
+            line = json.dumps(item, ensure_ascii=False, cls=PythonObjectEncoder) + "\n"
             fp.write(line)
 
 
 # 将json string load成python object
 def as_python_object(dct):
     if '_python_object' in dct:
         python_value = dct['_python_object']
@@ -122,128 +121,46 @@
     Args:
         fp: 文件路径或者open之后的对象
         max_data_num: 最大load的数据条目数
         return_generator: 是否返回generator
     Returns: json object的generator
     """
 
-    def get_gen(f):
-        if isinstance(f, str):
-            f = open(f, mode='r', encoding="utf8")
+    def get_gen(fp):
+        if isinstance(fp, str):
+            fp = open(fp, mode='r', encoding="utf8")
         idx = 0
-        with f as f:
-            for line in f:
-                line = line.strip()
-                if not line:
+        with fp as fp:
+            for line in fp:
+                if not line.strip():
                     continue
-                yield jloads(line)
+                yield jloads(line.strip())
                 idx += 1
                 if max_data_num and idx >= max_data_num:
                     break
 
     gen = get_gen(fp)
     if return_generator:
-        return gen
+        gen
     return list(gen)
 
-# table类的文件转化为list of dict
-
-
-def table2json(path, **kwargs):
-    if path.endswith("csv"):
-        df = pd.read_csv(path, **kwargs)
-    if path.endswith("xlsx"):
-        df = pd.read_excel(path, **kwargs)
-    df.replace(np.nan, None, inplace=True)
-    cols = df.columns.tolist()
-    cols = [e for e in cols if not e.startswith("Unnamed")]
-    df = df[cols]
-    records = df.to_dict(orient="records")
-    return records
-
-
-# 将list数据存储成table格式
-def dump2table(data, path:str):
-    if isinstance(data, list):
-        data = pd.DataFrame.from_records(data)
-    assert isinstance(data, pd.DataFrame)
-    df = data
-    if path.endswith(".csv"):
-        df.to_csv(path, index=False)
-    elif path.endswith(".xlsx"):
-        df.to_excel(path, index=False)
-    else:
-        raise Exception(f"Unknown file format: {path}")
-
 
 # 一行一行地读取文件内容
 def load_lines(fp, return_generator=False):
     if isinstance(fp, str):
+        create_dir_path(fp)
         fp = open(fp, mode="r", encoding="utf8")
     with fp:
         lines = fp.readlines()
         if return_generator:
             return (e.strip() for e in lines if e)
         return [e.strip() for e in lines if e]
 
-# 根据后缀名读取list数据
-
-
-def read2list(file_path: Union[str, List], **kwargs) -> List[Union[str, dict]]:
-
-    def _read2list(file_path, **kwargs):
-        suffix = os.path.splitext(file_path)[-1].lower()
-        if suffix == ".json":
-            return jload(file_path, **kwargs)
-        if suffix == ".jsonl":
-            return jload_lines(file_path, **kwargs)
-        if suffix in [".xlsx", ".csv"]:
-            return table2json(file_path, **kwargs)
-        if suffix in [".txt"]:
-            return load_lines(file_path, **kwargs)
-        else:
-            logger.warning(f"unknown suffix:{suffix}, read as txt")
-            return load_lines(file_path, **kwargs)
-
-    if isinstance(file_path, list):
-        rs = []
-        for f in file_path:
-            logger.info(f"reading file_path={f}")
-            rs.extend(_read2list(f, **kwargs))
-        return rs
-    else:
-        return _read2list(file_path=file_path, **kwargs)
-
-
-# 将list数据按照后缀名格式dump到文件
-def dump2list(data: List, file_path: str, **kwargs):
-    create_dir_path(file_path)
-    suffix = os.path.splitext(file_path)[-1].lower()
-    if suffix == ".json":
-        return jdump(data, file_path, **kwargs)
-    if suffix == ".jsonl":
-        return jdump_lines(data, file_path, **kwargs)
-    if suffix in [".xlsx", ".csv"]:
-        return dump2table(data, file_path)
-    if suffix in [".txt"]:
-        return dump_lines(data, file_path, **kwargs)
-    else:
-        logger.warning(f"unknown suffix:{suffix}, dump as txt")
-        return dump_lines(data, file_path, **kwargs)
-
-
-dump_list = dump2list
-load2list = read2list
-
-dump = dump2list
-load = read2list
 
 # 递归将obj中的float做精度截断
-
-
 def pretty_floats(obj, r=4):
     if isinstance(obj, float):
         return round(obj, r)
     elif isinstance(obj, dict):
         return dict((k, pretty_floats(v)) for k, v in obj.items())
     elif isinstance(obj, (list, tuple)):
         return map(pretty_floats, obj)
@@ -258,19 +175,15 @@
         if len(batch) == batch_size:
             yield batch
             batch = []
     if batch:
         yield batch
 
 
-batchify = get_batched_data
-
 # 将$seq序列转化成下标到元素以及元素到下标的dict
-
-
 def seq2dict(seq: Sequence) -> Tuple[dict, dict]:
     item2id = {item: idx for idx, item in enumerate(seq)}
     id2item = {idx: item for idx, item in enumerate(seq)}
     return item2id, id2item
 
 
 # 得到$fmt格式化之后的当前时间字符串表示
@@ -293,29 +206,28 @@
         return [e for item in seq for e in item]
     else:
         return (e for item in seq for e in item)
 
 
 # 将$seq序列聚合成dict。 key表示字典key生成的函数。 map_func表示字典value值的映射函数。
 # 返回的字典会根据value序列长度倒序排序
-def groupby(seq: Sequence, key=lambda x: x, map_func=lambda x: x, reduce_func=None,
+def groupby(seq: Sequence, key=lambda x: x, map_func=lambda x: x,
             sort_type="v_len", reverse=True) -> Dict[Any, List]:
     rs_dict = collections.defaultdict(list)
     for i in seq:
         rs_dict[key(i)].append(map_func(i))
 
     def sort_func(x):
         if sort_type == "v_len":
             return len(x[1])
         if sort_type == "k":
             return x[0]
         return 0
+
     items = sorted(rs_dict.items(), key=sort_func, reverse=reverse)
-    if reduce_func:
-        items = [(k, reduce_func(v)) for k, v in items]
     return collections.OrderedDict(items)
 
 
 def star_surround_info(info: str, fix_length=128) -> str:
     star_num = max(fix_length - len(info), 2)
     left_star_num = star_num // 2
     right_star_num = star_num - left_star_num
@@ -327,77 +239,20 @@
 def print_info(info, target_logger=None, fix_length=128):
     star_info = star_surround_info(info, fix_length)
     if target_logger:
         target_logger.info(star_info)
     else:
         print(star_info)
 
-# 把一个dict转化到一个Union类型
+
+def get_cur_dir():
+    return os.path.abspath(os.path.dirname(__file__))
+
+
 def union_parse_obj(union: _GenericAlias, d: dict):
     for cls in union.__args__:
         try:
             obj = cls(**d)
             return obj
         except:
             pass
     raise Exception(f"fail to convert {d} to union {union}")
-
-# 获取一个包的最新version
-def get_latest_version(package_name: str) -> str:
-    cmd = f"pip install {package_name}=="
-    status, output = execute_cmd(cmd)
-    pattern = "\(from versions:(.*?)\)"
-
-    for item in re.findall(pattern, output):
-        if item is None:
-            return "0.0.1"
-
-        # item
-        versions = [tuple(int(i) for i in e.strip().split("."))
-                    for e in item.split(",")]
-        # versions
-        latest_version = max(versions)
-        latest_version = ".".join(str(i) for i in latest_version)
-        return latest_version
-
-# 获取一个version的下一个版本
-def get_next_version(version: str, level=0) -> str:
-    pieces = version.split(".")
-    idx = len(pieces) - level - 1
-    val = pieces[idx]
-    if val.startswith("v"):
-        pieces[idx] = "v" + str(int(val[1])+1)
-    else:
-        pieces[idx] = str(int(val)+1)
-    return ".".join(pieces)
-
-
-
-def deep_update(origin:dict, new_data:dict, inplace=True)->dict:
-    """递归跟新dict
-
-    Args:
-        origin (dict): 原始dict
-        new_data (dict): 需要更新的数据
-        inplace (bool, optional): 是否在原dict上直接修改. Defaults to True.
-
-    Returns:
-        dict: 更新后的dict
-    """
-    to_update = origin if inplace else copy.deepcopy(origin)
-    
-    def _deep_update_inplace(tu:dict, nd:dict)->dict:
-        for k,v in nd.items():
-            if k not in to_update:
-                tu[k] = v
-            else:
-                if isinstance(v, dict) and isinstance(to_update[k], dict):
-                    _deep_update_inplace(to_update[k], v)
-                else:
-                    tu[k] =v
-        return tu            
-    return _deep_update_inplace(to_update, new_data)
-    
-        
-            
-    
-
```

