# Comparing `tmp/beepy_web-0.9.0.tar.gz` & `tmp/beepy_web-0.9.2.tar.gz`

## Comparing `beepy_web-0.9.0.tar` & `beepy_web-0.9.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.env.template
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.python-version
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.0/requirements.txt
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/__init__.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/attrs.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/children.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/components.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/context.py
--rw-r--r--   0        0        0    21167 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/framework.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/listeners.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/router.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/style.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/tags.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/trackable.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/types.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/__init__.py
--rwxr-xr-x   0        0        0     5051 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/__main__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/actions.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/plot.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/table.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/dev.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/internal.py
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/js_py.py
--rw-r--r--   0        0        0   179389 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/package-lock.json
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/webpack.prod.js
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.0/LICENSE
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.0/README.md
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 beepy_web-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.2/.env.template
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.2/.python-version
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.2/requirements.txt
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/__init__.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/attrs.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/children.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/components.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/context.py
+-rw-r--r--   0        0        0    21167 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/framework.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/listeners.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/router.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/style.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/tags.py
+-rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/trackable.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/types.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/dev/__init__.py
+-rwxr-xr-x   0        0        0     5051 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/table.py
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.2/beepy/utils/js_py.py
+-rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/package-lock.json
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/webpack.prod.js
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.2/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.2/README.md
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 beepy_web-0.9.2/PKG-INFO
```

### Comparing `beepy_web-0.9.0/.pre-commit-config.yaml` & `beepy_web-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/__init__.py` & `beepy_web-0.9.2/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/attrs.py` & `beepy_web-0.9.2/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/children.py` & `beepy_web-0.9.2/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/components.py` & `beepy_web-0.9.2/beepy/components.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/context.py` & `beepy_web-0.9.2/beepy/context.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/framework.py` & `beepy_web-0.9.2/beepy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from beepy.context import _SPECIAL_CHILD_STRINGS, CONTENT, OVERWRITE, SUPER
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __CONFIG__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 
-__version__ = '0.9.0'  # For internal development set to 0.0a0
+__version__ = '0.9.2'  # For internal development set to 0.0a0
 __CONFIG__['version'] = __version__
 
 
 _TAG_INITIALIZED = False
 
 
 class _MetaTag(_MetaComponent):
```

### Comparing `beepy_web-0.9.0/beepy/listeners.py` & `beepy_web-0.9.2/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/router.py` & `beepy_web-0.9.2/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/style.py` & `beepy_web-0.9.2/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/tags.py` & `beepy_web-0.9.2/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/trackable.py` & `beepy_web-0.9.2/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/types.py` & `beepy_web-0.9.2/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/dev/__main__.py` & `beepy_web-0.9.2/beepy/dev/__main__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/modules/context_menu.py` & `beepy_web-0.9.2/beepy/modules/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/modules/local_storage.py` & `beepy_web-0.9.2/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/modules/modal.py` & `beepy_web-0.9.2/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/modules/table.py` & `beepy_web-0.9.2/beepy/modules/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/modules/tabs.py` & `beepy_web-0.9.2/beepy/modules/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/api.py` & `beepy_web-0.9.2/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/asyncio.py` & `beepy_web-0.9.2/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/common.py` & `beepy_web-0.9.2/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/dev.py` & `beepy_web-0.9.2/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/import_hooks.py` & `beepy_web-0.9.2/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/internal.py` & `beepy_web-0.9.2/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/js.py` & `beepy_web-0.9.2/beepy/utils/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/beepy/utils/js_py.py` & `beepy_web-0.9.2/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/web/package-lock.json` & `beepy_web-0.9.2/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.9.2'}}", "'version'": "'0.9.2'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.8.10"
+            "version": "0.9.2"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.8.10"
+    "version": "0.9.2"
 }
```

### Comparing `beepy_web-0.9.0/web/package.json` & `beepy_web-0.9.2/web/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.9.2'"}*

```diff
@@ -32,9 +32,9 @@
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "publish-2": "cp ../README.md . && npm publish --access=public && rm README.md",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.8.10"
+    "version": "0.9.2"
 }
```

### Comparing `beepy_web-0.9.0/web/webpack.prod.js` & `beepy_web-0.9.2/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/web/src/beepy.js` & `beepy_web-0.9.2/web/src/beepy.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.0'
+    __version__ = '0.9.2'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
```

### Comparing `beepy_web-0.9.0/web/src/dev-server.js` & `beepy_web-0.9.2/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/web/src/files.js` & `beepy_web-0.9.2/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/web/src/main.css` & `beepy_web-0.9.2/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/web/src/python.js` & `beepy_web-0.9.2/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/web/src/utils.js` & `beepy_web-0.9.2/web/src/utils.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/.gitignore` & `beepy_web-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/LICENSE` & `beepy_web-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/README.md` & `beepy_web-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/pyproject.toml` & `beepy_web-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.0/PKG-INFO` & `beepy_web-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.0
+Version: 0.9.2
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://kor0p.github.io/BeePy/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

