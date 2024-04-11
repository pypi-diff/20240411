# Comparing `tmp/hs_correct-0.0.4.tar.gz` & `tmp/hs_correct-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hs_correct-0.0.4.tar", last modified: Wed Apr 10 03:26:10 2024, max compression
+gzip compressed data, was "hs_correct-0.0.5.tar", last modified: Thu Apr 11 06:16:03 2024, max compression
```

## Comparing `hs_correct-0.0.4.tar` & `hs_correct-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.748284 hs_correct-0.0.4/
--rw-rw-rw-   0        0        0      213 2024-04-10 01:56:17.000000 hs_correct-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      272 2024-04-10 03:26:10.748284 hs_correct-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      100 2024-04-01 06:28:15.000000 hs_correct-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.731677 hs_correct-0.0.4/correct/
--rw-rw-rw-   0        0        0     3868 2024-04-10 01:57:50.000000 hs_correct-0.0.4/correct/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.731677 hs_correct-0.0.4/correct/exception/
--rw-rw-rw-   0        0        0      610 2024-04-02 06:36:33.000000 hs_correct-0.0.4/correct/exception/correct_exception.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.731677 hs_correct-0.0.4/correct/funcs/
--rw-rw-rw-   0        0        0    17656 2024-04-10 01:57:09.000000 hs_correct-0.0.4/correct/funcs/alignment.py
--rw-rw-rw-   0        0        0     2663 2024-04-10 01:56:17.000000 hs_correct-0.0.4/correct/funcs/correction.py
--rw-rw-rw-   0        0        0     7035 2024-04-10 02:06:54.000000 hs_correct-0.0.4/correct/funcs/data_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.731677 hs_correct-0.0.4/correct/logger/
--rw-rw-rw-   0        0        0     1791 2024-03-19 09:58:45.000000 hs_correct-0.0.4/correct/logger/logger.py
--rw-rw-rw-   0        0        0       24 2024-04-01 08:38:32.000000 hs_correct-0.0.4/correct/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.731677 hs_correct-0.0.4/correct/response/
--rw-rw-rw-   0        0        0     1210 2024-04-02 06:36:33.000000 hs_correct-0.0.4/correct/response/response.py
--rw-rw-rw-   0        0        0      186 2024-03-29 02:44:54.000000 hs_correct-0.0.4/correct/response/response_code.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.747352 hs_correct-0.0.4/correct/tools/
--rw-rw-rw-   0        0        0      461 2024-03-29 02:14:14.000000 hs_correct-0.0.4/correct/tools/constants.py
--rw-rw-rw-   0        0        0     1632 2024-04-08 06:46:25.000000 hs_correct-0.0.4/correct/tools/min_edit_distance.py
--rw-rw-rw-   0        0        0     1625 2024-03-27 06:56:01.000000 hs_correct-0.0.4/correct/tools/point_handle.py
--rw-rw-rw-   0        0        0     2655 2024-03-27 06:56:01.000000 hs_correct-0.0.4/correct/tools/rectangle_handle.py
--rw-rw-rw-   0        0        0     5275 2024-04-09 02:47:59.000000 hs_correct-0.0.4/correct/tools/str_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:26:10.748284 hs_correct-0.0.4/hs_correct.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-10 03:26:10.000000 hs_correct-0.0.4/hs_correct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2024-04-10 03:26:10.000000 hs_correct-0.0.4/hs_correct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 03:26:10.000000 hs_correct-0.0.4/hs_correct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-10 03:26:10.000000 hs_correct-0.0.4/hs_correct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 03:26:10.000000 hs_correct-0.0.4/hs_correct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-04-10 01:56:17.000000 hs_correct-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 03:26:10.748284 hs_correct-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-04-10 03:24:26.000000 hs_correct-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.634563 hs_correct-0.0.5/
+-rw-rw-rw-   0        0        0      213 2024-04-10 01:56:17.000000 hs_correct-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      272 2024-04-11 06:16:03.618939 hs_correct-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2024-04-01 06:28:15.000000 hs_correct-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/
+-rw-rw-rw-   0        0        0     2871 2024-04-11 06:14:35.000000 hs_correct-0.0.5/correct/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/exception/
+-rw-rw-rw-   0        0        0      610 2024-04-02 06:36:33.000000 hs_correct-0.0.5/correct/exception/correct_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/funcs/
+-rw-rw-rw-   0        0        0    16537 2024-04-11 06:14:35.000000 hs_correct-0.0.5/correct/funcs/alignment.py
+-rw-rw-rw-   0        0        0     2122 2024-04-11 06:14:35.000000 hs_correct-0.0.5/correct/funcs/correction.py
+-rw-rw-rw-   0        0        0     7035 2024-04-10 02:06:54.000000 hs_correct-0.0.5/correct/funcs/data_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/logger/
+-rw-rw-rw-   0        0        0     1791 2024-03-19 09:58:45.000000 hs_correct-0.0.5/correct/logger/logger.py
+-rw-rw-rw-   0        0        0       24 2024-04-01 08:38:32.000000 hs_correct-0.0.5/correct/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/response/
+-rw-rw-rw-   0        0        0     1210 2024-04-02 06:36:33.000000 hs_correct-0.0.5/correct/response/response.py
+-rw-rw-rw-   0        0        0      186 2024-03-29 02:44:54.000000 hs_correct-0.0.5/correct/response/response_code.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/tools/
+-rw-rw-rw-   0        0        0      461 2024-03-29 02:14:14.000000 hs_correct-0.0.5/correct/tools/constants.py
+-rw-rw-rw-   0        0        0     1632 2024-04-08 06:46:25.000000 hs_correct-0.0.5/correct/tools/min_edit_distance.py
+-rw-rw-rw-   0        0        0     1625 2024-03-27 06:56:01.000000 hs_correct-0.0.5/correct/tools/point_handle.py
+-rw-rw-rw-   0        0        0     2655 2024-03-27 06:56:01.000000 hs_correct-0.0.5/correct/tools/rectangle_handle.py
+-rw-rw-rw-   0        0        0     5281 2024-04-10 09:31:13.000000 hs_correct-0.0.5/correct/tools/str_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/hs_correct.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-04-10 01:56:17.000000 hs_correct-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 06:16:03.634563 hs_correct-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-04-11 06:15:35.000000 hs_correct-0.0.5/setup.py
```

### Comparing `hs_correct-0.0.4/correct/exception/correct_exception.py` & `hs_correct-0.0.5/correct/exception/correct_exception.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/funcs/alignment.py` & `hs_correct-0.0.5/correct/funcs/alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,41 +118,14 @@
                            f"answer:{ele['data']['answer']}、"
                            f"code:{ele['code']}、"
                            f"message:{ele['message']}"
                            )
     return align_res
 
 
-def tmp_call():
-    timestamp1 = time.time()
-    dt1 = datetime.fromtimestamp(timestamp1)
-    formatted_dt1 = dt1.strftime("%Y-%m-%d %H:%M:%S")
-    print("批改对齐部分开始时间：" + formatted_dt1)
-    icount = 20
-    quad1_coords = [(0, 0), (0, 2), (2, 2), (2, 0)]
-    quad2_coords = [(1, 1), (1, 3), (3, 3), (3, 1)]
-    for i in range(icount):
-        iou_c1 = bbox_iou_eval(quad1_coords, quad2_coords)
-        # print('i_' + str(i) + ':' + str(iou_c1))
-        for j in range(icount):
-            iou_c3 = bbox_iou_eval(quad1_coords, quad2_coords)
-            # print('j_' + str(i) + ':' + str(iou_c3))
-            for k in range(icount):
-                iou_c5 = bbox_iou_eval(quad1_coords, quad2_coords)
-                # print('k_' + str(i) + ':' + str(iou_c5))
-
-    timestamp2 = time.time()
-    dt2 = datetime.fromtimestamp(timestamp2)
-    formatted_dt2 = dt2.strftime("%Y-%m-%d %H:%M:%S")
-    print("批改对齐部分结束时间：" + formatted_dt2)
-
-    delta_time = timestamp2 - timestamp1
-    print("批改对齐部分总耗时: {:.2f}分钟".format(delta_time / 60))
-
-
 # 定义一个函数用来判断某个点是否在矩形框内
 def point_match_area(point_co, box_co):
     x1, y1, x2, y2 = find_minmax_xy_of_quadrilateral(box_co)
     px, py = point_co
 
     # 检查点的 x 坐标是否在矩形框的 x 坐标范围内
     if x1 <= px <= x2:
```

### Comparing `hs_correct-0.0.4/correct/funcs/correction.py` & `hs_correct-0.0.5/correct/funcs/correction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 对比笔迹和答案进行批改
 """
-import random
 
 from correct.tools.str_tools import similarity
 from correct.tools.constants import constants
 
 
 def correct(params: dict):
     """
@@ -54,34 +53,17 @@
     return {
         'success': [
             {
                 'mark_location': {
                     "x": ele['point'][0],
                     "y": ele['point'][1]
                 },
-                'ocr_content': ele['ocr_text'],
+                'ocr_text': ele['ocr_text'],
                 'answer': ele['answer'],
                 # 考虑到实际场景，编辑距离操作中的替换操作给的惩罚比插入和编辑大一些
                 'match_rate': similarity(ele['answer'], ele['ocr_text'], constants.NUM_ONE, constants.NUM_ONE,
                                          constants.NUM_ONE),
                 'sub_id': ele['id'],
                 'parent_id': ele['parent_id'],
             } for ele in params
         ]
     }
-
-
-def tmp_res(mark_data: dict):
-    return {
-        "success": [{
-            "mark_location": {
-                "x": ele['point'][0],
-                "y": ele['point'][1]
-            },
-            "ocr_content": str(ele['answer']) + str(random.randint(1, 10)),
-            "answer": ele['answer'],
-            "match_rate": "{:.4f}".format(random.uniform(0.5, 1.0)),
-            "sub_id": ele['id'],
-            "parent_id": ele['parent_id']
-        } for ele in mark_data],
-        "ignored": []
-    }
```

### Comparing `hs_correct-0.0.4/correct/funcs/data_handle.py` & `hs_correct-0.0.5/correct/funcs/data_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/logger/logger.py` & `hs_correct-0.0.5/correct/logger/logger.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/response/response.py` & `hs_correct-0.0.5/correct/response/response.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/tools/min_edit_distance.py` & `hs_correct-0.0.5/correct/tools/min_edit_distance.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/tools/point_handle.py` & `hs_correct-0.0.5/correct/tools/point_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/tools/rectangle_handle.py` & `hs_correct-0.0.5/correct/tools/rectangle_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/correct/tools/str_tools.py` & `hs_correct-0.0.5/correct/tools/str_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         paragraphs.append(current_paragraph)
 
     return paragraphs
 
 
 def split_list(lst):
     """
-    你一个列表，元素类型可能是以下三种情况：纯中文、纯特殊字符、纯英文，把这个列表的每个元素做处理并合成一个新列表，处理过程规则如下：
+    一个列表，任意元素的类型可能是以下三种情况：纯中文、纯特殊字符、纯英文，把这个列表的每个元素做处理并合成一个新列表，处理过程规则如下：
     如果元素是纯中文或纯字符，拆分为单个文字或字符；如果元素是纯英文，保持原样
     :param lst: 例如：['我是谁', '？？', 'niubility', ' ', 'she', ' ', 'is', '! ', '好好好', '！']
     :return: 例如：['我', '是', '谁', '？', '？', 'niubility', ' ', 'she', ' ', 'is', '! ', '好', '好', '好', '！']
     """
     # 定义正则表达式来匹配纯中文、纯特殊字符和纯英文
     pattern_chinese = re.compile(r'^[\u4e00-\u9fff]+$')
     pattern_special = re.compile(r'^[^\w]+$')  # 匹配非字母数字的字符
```

### Comparing `hs_correct-0.0.4/hs_correct.egg-info/SOURCES.txt` & `hs_correct-0.0.5/hs_correct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.4/setup.py` & `hs_correct-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def parse_requirements(filename):
     line_iter = (line.strip() for line in open(filename))
     return [line for line in line_iter if line and not line.startswith("#")]
 
 
 setup(
     name='hs_correct',
-    version='0.0.4',
+    version='0.0.5',
     description='hs-correct-module',
     classifiers=[],
     keywords='hs-correct-module',
     author='zgl',
     author_email='',
     url='',
     license='MIT',
```

