# Comparing `tmp/comfy_script-0.4.4.tar.gz` & `tmp/comfy_script-0.4.5.tar.gz`

## Comparing `comfy_script-0.4.4.tar` & `comfy_script-0.4.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.4/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.4/requirements.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.4/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/astutil.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    42450 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.4/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 comfy_script-0.4.4/README.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 comfy_script-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    15864 2020-02-02 00:00:00.000000 comfy_script-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.5/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.5/requirements.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.5/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Latent/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Models/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    42547 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.5/LICENSE.txt
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 comfy_script-0.4.5/README.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 comfy_script-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 comfy_script-0.4.5/PKG-INFO
```

### Comparing `comfy_script-0.4.4/__init__.py` & `comfy_script-0.4.5/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/README.md` & `comfy_script-0.4.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/Runtime.md` & `comfy_script-0.4.5/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/Image/README.md` & `comfy_script-0.4.5/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/Latent/README.md` & `comfy_script-0.4.5/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/Nodes/README.md` & `comfy_script-0.4.5/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/auto-queue.png` & `comfy_script-0.4.5/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/diff.png` & `comfy_script-0.4.5/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/plot.png` & `comfy_script-0.4.5/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/select.png` & `comfy_script-0.4.5/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/type-stubs.png` & `comfy_script-0.4.5/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/type-stubs2.png` & `comfy_script-0.4.5/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/workflow.png` & `comfy_script-0.4.5/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/README/workflow2.png` & `comfy_script-0.4.5/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/docs/images/Runtime/load-api-format.png` & `comfy_script-0.4.5/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/astutil.py` & `comfy_script-0.4.5/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/client/__init__.py` & `comfy_script-0.4.5/src/comfy_script/client/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/nodes/__init__.py` & `comfy_script-0.4.5/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/__init__.py` & `comfy_script-0.4.5/src/comfy_script/runtime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,17 @@
         
         # if main_locals is not None:
         #     for name in 'loop', 'server', 'q', 'extra_model_paths_config_path':
         #         setattr(main, name, main_locals[name])
         
         import comfy.nodes.common
         nodes = types.ModuleType('nodes')
-        exported_nodes = comfy.cmd.server.nodes
+        exported_nodes = getattr(server, 'nodes', None)
+        if exported_nodes is None:
+            exported_nodes = comfy.cmd.server.nodes
         setattr(nodes, 'NODE_CLASS_MAPPINGS', exported_nodes.NODE_CLASS_MAPPINGS)
         setattr(nodes, 'NODE_DISPLAY_NAME_MAPPINGS', exported_nodes.NODE_DISPLAY_NAME_MAPPINGS)
         setattr(nodes, 'EXTENSION_WEB_DIRS', exported_nodes.EXTENSION_WEB_DIRS)
         setattr(nodes, 'MAX_RESOLUTION', comfy.nodes.common.MAX_RESOLUTION)
         # TODO: load_custom_node, load_custom_nodes
         sys.modules['nodes'] = nodes
         # globals()['nodes'] = nodes
```

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/factory.py` & `comfy_script-0.4.5/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/nodes.py` & `comfy_script-0.4.5/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.4.5/src/comfy_script/runtime/data/Images.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.4.5/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.4.5/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.4.5/src/comfy_script/runtime/real/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/transpile/__init__.py` & `comfy_script-0.4.5/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/transpile/prompt.py` & `comfy_script-0.4.5/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.4.5/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.4.5/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/tests/test_astutil.py` & `comfy_script-0.4.5/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/tests/transpile/bypass.json` & `comfy_script-0.4.5/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/tests/transpile/default.json` & `comfy_script-0.4.5/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/tests/transpile/test_transpiler.py` & `comfy_script-0.4.5/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/.gitignore` & `comfy_script-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/LICENSE.txt` & `comfy_script-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.4/README.md` & `comfy_script-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,20 @@
   ```
 
 Install/update ComfyScript:
 ```sh
 python -m pip install -U "comfy-script[default]"
 ```
 
-(`[default]` is necessary to install common dependencies. See [`pyproject.toml`](pyproject.toml) for other options. If no option is specified, `comfy-script` will be installed without any dependencies.)
+`[default]` is necessary to install common dependencies. See [`pyproject.toml`](pyproject.toml) for other options. If no option is specified, `comfy-script` will be installed without any dependencies.
+
+If there are problems with the latest ComfyUI package, one can use the last tested version:
+```
+python -m pip install --no-build-isolation git+https://github.com/hiddenswitch/ComfyUI.git@e49c662c7f026f05a5e082d48b629e2b977c0441
+```
 
 ### Other ways
 ComfyScript can also be used without installed ComfyUI. See [only ComfyScript package](docs/README.md#only-comfyscript-package) for details. And see [uninstallation](docs/README.md#uninstallation) for how to uninstall.
 
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
```

### Comparing `comfy_script-0.4.4/pyproject.toml` & `comfy_script-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.4.4"
+version = "0.4.5"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
```

### Comparing `comfy_script-0.4.4/PKG-INFO` & `comfy_script-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
@@ -115,15 +115,20 @@
   ```
 
 Install/update ComfyScript:
 ```sh
 python -m pip install -U "comfy-script[default]"
 ```
 
-(`[default]` is necessary to install common dependencies. See [`pyproject.toml`](pyproject.toml) for other options. If no option is specified, `comfy-script` will be installed without any dependencies.)
+`[default]` is necessary to install common dependencies. See [`pyproject.toml`](pyproject.toml) for other options. If no option is specified, `comfy-script` will be installed without any dependencies.
+
+If there are problems with the latest ComfyUI package, one can use the last tested version:
+```
+python -m pip install --no-build-isolation git+https://github.com/hiddenswitch/ComfyUI.git@e49c662c7f026f05a5e082d48b629e2b977c0441
+```
 
 ### Other ways
 ComfyScript can also be used without installed ComfyUI. See [only ComfyScript package](docs/README.md#only-comfyscript-package) for details. And see [uninstallation](docs/README.md#uninstallation) for how to uninstall.
 
 ## Transpiler
 The transpiler can translate ComfyUI's workflows to ComfyScript.
```

