# Comparing `tmp/pyfineflow-1.1.0.tar.gz` & `tmp/pyfineflow-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfineflow-1.1.0.tar", last modified: Wed Apr 10 12:25:57 2024, max compression
+gzip compressed data, was "pyfineflow-1.1.1.tar", last modified: Thu Apr 11 14:46:27 2024, max compression
```

## Comparing `pyfineflow-1.1.0.tar` & `pyfineflow-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:25:56.996308 pyfineflow-1.1.0/
--rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1277 2024-04-10 12:25:56.995309 pyfineflow-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 12:25:56.981309 pyfineflow-1.1.0/pyfineflow/
--rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.1.0/pyfineflow/__init__.py
--rw-rw-rw-   0        0        0     1586 2024-04-10 11:38:17.000000 pyfineflow-1.1.0/pyfineflow/__main__.py
--rw-rw-rw-   0        0        0    16492 2024-04-10 12:25:53.000000 pyfineflow-1.1.0/pyfineflow/core.py
--rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.1.0/pyfineflow/log_conf.py
--rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.1.0/pyfineflow/schemas.py
--rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.1.0/pyfineflow/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:25:56.993308 pyfineflow-1.1.0/pyfineflow.egg-info/
--rw-rw-rw-   0        0        0     1277 2024-04-10 12:25:56.000000 pyfineflow-1.1.0/pyfineflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-10 12:25:56.000000 pyfineflow-1.1.0/pyfineflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:25:56.000000 pyfineflow-1.1.0/pyfineflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-10 12:25:56.000000 pyfineflow-1.1.0/pyfineflow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-10 12:25:56.000000 pyfineflow-1.1.0/pyfineflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 12:25:56.000000 pyfineflow-1.1.0/pyfineflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 12:25:56.997310 pyfineflow-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      676 2024-04-10 12:20:33.000000 pyfineflow-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:46:27.611732 pyfineflow-1.1.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1277 2024-04-11 14:46:27.610732 pyfineflow-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 14:46:27.596926 pyfineflow-1.1.1/pyfineflow/
+-rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.1.1/pyfineflow/__init__.py
+-rw-rw-rw-   0        0        0     2110 2024-04-11 14:44:44.000000 pyfineflow-1.1.1/pyfineflow/__main__.py
+-rw-rw-rw-   0        0        0    17560 2024-04-11 14:24:51.000000 pyfineflow-1.1.1/pyfineflow/core.py
+-rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.1.1/pyfineflow/log_conf.py
+-rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.1.1/pyfineflow/schemas.py
+-rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.1.1/pyfineflow/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:46:27.608664 pyfineflow-1.1.1/pyfineflow.egg-info/
+-rw-rw-rw-   0        0        0     1277 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:46:27.611732 pyfineflow-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      676 2024-04-11 14:46:22.000000 pyfineflow-1.1.1/setup.py
```

### Comparing `pyfineflow-1.1.0/LICENSE` & `pyfineflow-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.0/PKG-INFO` & `pyfineflow-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.1.0
+Version: 1.1.1
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
```

### Comparing `pyfineflow-1.1.0/pyfineflow/core.py` & `pyfineflow-1.1.1/pyfineflow/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,17 +176,27 @@
 
         class FuncReq(BaseModel):
             code: str
             params: dict
 
         @router.post('/func')
         def func(req: FuncReq):
-            vars = {'params': req.params}
-            exec(f"{req.code}\nres=func(params)", vars)
-            return vars['res']
+            try:
+                vars = {'params': req.params}
+                exec(f"{req.code}\nres=func(params)", vars)
+                return vars['res']
+            except Exception as e:
+                error_traceback = traceback.format_exc()
+                # 将错误信息按行分割成列表
+                traceback_lines = error_traceback.splitlines()
+                # 获取最后五行的错误信息
+                last_five_lines = traceback_lines[-5:]
+                error_str = "\n".join(last_five_lines)
+                print(error_str)
+                return {'state': 0, 'msg': f'{error_str}', 'data': None}
 
         @router.post('/run_node')
         def run_node(req: RunNodeReq):
             work_id = req.workId
             if work_id not in self.work_map:
                 self.work_map[work_id] = WorkManager(work_id)
             node_key = req.key
@@ -294,17 +304,27 @@
 
         class FuncReq(BaseModel):
             code: str
             params: dict
 
         @router.post('/func')
         def func(req: FuncReq):
-            vars = {'params': req.params}
-            exec(f"{req.code}\nres=func(params)", vars)
-            return vars['res']
+            try:
+                vars = {'params': req.params}
+                exec(f"{req.code}\nres=func(params)", vars)
+                return {'state': 1, 'msg': f'', 'data': vars['res']}
+            except Exception as e:
+                error_traceback = traceback.format_exc()
+                # 将错误信息按行分割成列表
+                traceback_lines = error_traceback.splitlines()
+                # 获取最后五行的错误信息
+                last_five_lines = traceback_lines[-5:]
+                error_str = "\n".join(last_five_lines)
+                print(error_str)
+                return {'state': 0, 'msg': f'{error_str}', 'data': None}
 
         @router.post('/run_node')
         def run_node(req: RunNodeReq):
             work_id = req.workId
             if work_id not in self.work_map:
                 self.work_map[work_id] = WorkManager(work_id)
             node_key = req.key
```

### Comparing `pyfineflow-1.1.0/pyfineflow/log_conf.py` & `pyfineflow-1.1.1/pyfineflow/log_conf.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.0/pyfineflow/schemas.py` & `pyfineflow-1.1.1/pyfineflow/schemas.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.0/pyfineflow/utils.py` & `pyfineflow-1.1.1/pyfineflow/utils.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.0/pyfineflow.egg-info/PKG-INFO` & `pyfineflow-1.1.1/pyfineflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.1.0
+Version: 1.1.1
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
```

### Comparing `pyfineflow-1.1.0/setup.py` & `pyfineflow-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # --skip-existing 覆盖
 # python setup.py sdist bdist_wheel
 # twine upload dist/* --skip-existing
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyfineflow',
-    version='1.1.0',
+    version='1.1.1',
     packages=find_packages(exclude=['__pycache__']),
     description='python nodes server for fineflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'fastapi[all]~=0.110.1',
     ],
```

