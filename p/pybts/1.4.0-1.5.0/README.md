# Comparing `tmp/pybts-1.4.0.tar.gz` & `tmp/pybts-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.4.0.tar", max compression
+gzip compressed data, was "pybts-1.5.0.tar", max compression
```

## Comparing `pybts-1.4.0.tar` & `pybts-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0   157658 2024-04-10 19:00:51.503643 pybts-1.4.0/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-10 19:00:51.503643 pybts-1.4.0/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-10 19:00:51.503643 pybts-1.4.0/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-10 19:00:51.507643 pybts-1.4.0/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-10 19:00:51.507643 pybts-1.4.0/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-10 19:00:51.507643 pybts-1.4.0/README.md
--rw-r--r--   0        0        0      393 2024-04-10 19:00:51.507643 pybts-1.4.0/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-10 19:00:51.507643 pybts-1.4.0/pybts/board/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-10 19:00:51.507643 pybts-1.4.0/pybts/board/board.py
--rw-r--r--   0        0        0     9994 2024-04-10 19:00:51.507643 pybts-1.4.0/pybts/board/server.py
--rw-r--r--   0        0        0     7780 2024-04-10 19:00:51.507643 pybts-1.4.0/pybts/builder.py
--rw-r--r--   0        0        0      548 2024-04-10 19:00:51.507643 pybts-1.4.0/pybts/composites/__init__.py
--rw-r--r--   0        0        0     8666 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/composite.py
--rw-r--r--   0        0        0     2175 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5661 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/parallel.py
--rw-r--r--   0        0        0      944 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/selector.py
--rw-r--r--   0        0        0     2541 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/sequence.py
--rw-r--r--   0        0        0      182 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/composites/template.py
--rw-r--r--   0        0        0     3243 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/constants.py
--rw-r--r--   0        0        0     3614 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    19980 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1073 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/main.py
--rw-r--r--   0        0        0    10981 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/node.py
--rw-r--r--   0        0        0      166 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/rl/__init__.py
--rw-r--r--   0        0        0      268 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/rl/builder.py
--rw-r--r--   0        0        0      460 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/rl/common.py
--rw-r--r--   0        0        0     4467 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/rl/nodes.py
--rw-r--r--   0        0        0    14778 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/rl/on_policy.py
--rw-r--r--   0        0        0     1183 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-10 19:00:51.511644 pybts-1.4.0/pybts/templates/index.html
--rw-r--r--   0        0        0  1967920 2024-04-10 19:00:51.523643 pybts-1.4.0/pybts/templates/static/index-BlldS3Jx.js
--rw-r--r--   0        0        0   320362 2024-04-10 19:00:51.523643 pybts-1.4.0/pybts/templates/static/index-DN1S--qx.css
--rw-r--r--   0        0        0     5267 2024-04-10 19:00:51.523643 pybts-1.4.0/pybts/templates/static/info-lb9hZOuB.png
--rw-r--r--   0        0        0     1553 2024-04-10 19:00:51.523643 pybts-1.4.0/pybts/tree.py
--rw-r--r--   0        0        0    10044 2024-04-10 19:00:51.523643 pybts-1.4.0/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-10 19:00:51.523643 pybts-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-11 19:12:46.142182 pybts-1.5.0/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-11 19:12:46.142182 pybts-1.5.0/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-11 19:12:46.146182 pybts-1.5.0/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-11 19:12:46.146182 pybts-1.5.0/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-11 19:12:46.146182 pybts-1.5.0/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-11 19:12:46.146182 pybts-1.5.0/README.md
+-rw-r--r--   0        0        0      393 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/board/board.py
+-rw-r--r--   0        0        0     9994 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/board/server.py
+-rw-r--r--   0        0        0     7780 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/builder.py
+-rw-r--r--   0        0        0      548 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     8666 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2175 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5661 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      944 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2541 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/sequence.py
+-rw-r--r--   0        0        0      182 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/template.py
+-rw-r--r--   0        0        0     3243 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/constants.py
+-rw-r--r--   0        0        0     3618 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    19980 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1073 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/main.py
+-rw-r--r--   0        0        0    10981 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/node.py
+-rw-r--r--   0        0        0       63 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/__init__.py
+-rw-r--r--   0        0        0     9353 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/base_class.py
+-rw-r--r--   0        0        0      268 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/builder.py
+-rw-r--r--   0        0        0      460 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/common.py
+-rw-r--r--   0        0        0    15319 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/nodes.py
+-rw-r--r--   0        0        0     6137 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/off_policy.py
+-rw-r--r--   0        0        0     7295 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0     1183 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/templates/index.html
+-rw-r--r--   0        0        0  1967920 2024-04-11 19:12:46.162182 pybts-1.5.0/pybts/templates/static/index-BlldS3Jx.js
+-rw-r--r--   0        0        0   320362 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/templates/static/index-DN1S--qx.css
+-rw-r--r--   0        0        0     5267 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/templates/static/info-lb9hZOuB.png
+-rw-r--r--   0        0        0     1553 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/tree.py
+-rw-r--r--   0        0        0    10044 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-11 19:12:46.166182 pybts-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.5.0/PKG-INFO
```

### Comparing `pybts-1.4.0/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.5.0/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/README.assets/image-20240329031220580.png` & `pybts-1.5.0/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/README.assets/image-20240329031233459.png` & `pybts-1.5.0/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/README.assets/image-20240401211552611.png` & `pybts-1.5.0/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/README.assets/image-20240401211609525.png` & `pybts-1.5.0/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/README.md` & `pybts-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/board/board.py` & `pybts-1.5.0/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/board/server.py` & `pybts-1.5.0/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/builder.py` & `pybts-1.5.0/pybts/builder.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/__init__.py` & `pybts-1.5.0/pybts/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/composite.py` & `pybts-1.5.0/pybts/composites/composite.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/condition_branch.py` & `pybts-1.5.0/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/parallel.py` & `pybts-1.5.0/pybts/composites/parallel.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/ppa.py` & `pybts-1.5.0/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/selector.py` & `pybts-1.5.0/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/composites/sequence.py` & `pybts-1.5.0/pybts/composites/sequence.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/constants.py` & `pybts-1.5.0/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/converter.py` & `pybts-1.5.0/pybts/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         for key in ctx:
             if callable(ctx[key]):
                 ctx[key] = ctx[key]()
         return eval(value, ctx)
 
     def render(self, value: str, context: dict = None) -> str:
         ctx = { }
+        # if self.node.attrs is not None:
+        #     ctx.update(self.node.attrs)
         if self.node.context is not None:
             ctx.update(self.node.context)
-        if self.node.attrs is not None:
-            ctx.update(self.node.attrs)
         if context is not None:
             ctx.update(context)
         for key in ctx:
             if callable(ctx[key]):
                 ctx[key] = ctx[key]()
         return jinja2.Template(value).render(ctx)
```

### Comparing `pybts-1.4.0/pybts/decorators/nodes.py` & `pybts-1.5.0/pybts/decorators/nodes.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/display.py` & `pybts-1.5.0/pybts/display.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/main.py` & `pybts-1.5.0/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/node.py` & `pybts-1.5.0/pybts/node.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/rl/tree.py` & `pybts-1.5.0/pybts/rl/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/templates/favicon.ico` & `pybts-1.5.0/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/templates/static/index-BlldS3Jx.js` & `pybts-1.5.0/pybts/templates/static/index-BlldS3Jx.js`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/templates/static/index-DN1S--qx.css` & `pybts-1.5.0/pybts/templates/static/index-DN1S--qx.css`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/templates/static/info-lb9hZOuB.png` & `pybts-1.5.0/pybts/templates/static/info-lb9hZOuB.png`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/tree.py` & `pybts-1.5.0/pybts/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pybts/utility.py` & `pybts-1.5.0/pybts/utility.py`

 * *Files identical despite different names*

### Comparing `pybts-1.4.0/pyproject.toml` & `pybts-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.4.0"
+version = "1.5.0"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.4.0/PKG-INFO` & `pybts-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.4.0
+Version: 1.5.0
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

