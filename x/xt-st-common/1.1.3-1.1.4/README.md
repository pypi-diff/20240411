# Comparing `tmp/xt_st_common-1.1.3.tar.gz` & `tmp/xt_st_common-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-1.1.3.tar", max compression
+gzip compressed data, was "xt_st_common-1.1.4.tar", max compression
```

## Comparing `xt_st_common-1.1.3.tar` & `xt_st_common-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      720 2024-04-08 01:46:34.616467 xt_st_common-1.1.3/README.md
--rw-r--r--   0        0        0     3455 2024-04-08 01:46:34.616467 xt_st_common-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     6128 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2024-04-08 01:46:31.124419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2024-04-08 01:46:31.152419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2024-04-08 01:46:31.152419 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2024-04-08 01:46:34.616467 xt_st_common-1.1.3/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     7066 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/xt_st_common/components.py
--rw-r--r--   0        0        0     3162 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3492 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6278 2024-04-08 01:46:31.244421 xt_st_common-1.1.3/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    14981 2024-04-08 01:46:31.248421 xt_st_common-1.1.3/src/xt_st_common/project_actions.py
--rw-r--r--   0        0        0    36448 2024-04-08 01:46:31.248421 xt_st_common-1.1.3/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0    14052 2024-04-08 01:46:31.248421 xt_st_common-1.1.3/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5933 2024-04-08 01:46:31.248421 xt_st_common-1.1.3/src/xt_st_common/session.py
--rw-r--r--   0        0        0     7610 2024-04-08 01:46:31.248421 xt_st_common-1.1.3/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     2114 2024-04-08 01:46:31.248421 xt_st_common-1.1.3/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 xt_st_common-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      720 2024-04-11 05:48:23.206018 xt_st_common-1.1.4/README.md
+-rw-r--r--   0        0        0     3455 2024-04-11 05:48:23.206018 xt_st_common-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6128 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2024-04-11 05:48:18.026050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2024-04-11 05:48:18.050050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2024-04-11 05:48:18.050050 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2024-04-11 05:48:23.206018 xt_st_common-1.1.4/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     7036 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     3162 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3492 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6278 2024-04-11 05:48:18.142049 xt_st_common-1.1.4/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    14981 2024-04-11 05:48:18.146049 xt_st_common-1.1.4/src/xt_st_common/project_actions.py
+-rw-r--r--   0        0        0    36448 2024-04-11 05:48:18.146049 xt_st_common-1.1.4/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0    14052 2024-04-11 05:48:18.146049 xt_st_common-1.1.4/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5933 2024-04-11 05:48:18.146049 xt_st_common-1.1.4/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     7610 2024-04-11 05:48:18.146049 xt_st_common-1.1.4/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     2114 2024-04-11 05:48:18.146049 xt_st_common-1.1.4/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 xt_st_common-1.1.4/PKG-INFO
```

### Comparing `xt_st_common-1.1.3/README.md` & `xt_st_common-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 1.1.3
+# XT-STREAMLIT - 1.1.4
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-1.1.3/pyproject.toml` & `xt_st_common-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "1.1.3"
+version = "1.1.4"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = [
   "Alex Hunt <alex.hunt@csiro.au>",
   "Sam Bradley <sam.bradley@csiro.au>",
   "John Hille <john.hille@csiro.au>",
 ]
 readme = "README.md"
```

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/__init__.py` & `xt_st_common-1.1.4/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-1.1.4/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/components.py` & `xt_st_common-1.1.4/src/xt_st_common/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         <style scoped type="text/css">
             .main .block-container {{
                     padding-top: {header_padding_top};
             }}
             .xt_app_header {{
                 {"border-bottom: 1px solid black;" if header_border else ""}
                 width: 100%;
-                height: 80px;
                 display: flex;
                 justify-content: space-between;
                 align-items: center;
                 flex-wrap: wrap;
                 row-gap: 10px;
             }}
             .app_logo_group{{
```

### Comparing `xt_st_common-1.1.3/src/xt_st_common/config.py` & `xt_st_common-1.1.4/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/database.py` & `xt_st_common-1.1.4/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/fs_upload_page.py` & `xt_st_common-1.1.4/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/project_actions.py` & `xt_st_common-1.1.4/src/xt_st_common/project_actions.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/project_components.py` & `xt_st_common-1.1.4/src/xt_st_common/project_components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/project_models.py` & `xt_st_common-1.1.4/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/session.py` & `xt_st_common-1.1.4/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/storage.py` & `xt_st_common-1.1.4/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/src/xt_st_common/utils.py` & `xt_st_common-1.1.4/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-1.1.3/PKG-INFO` & `xt_st_common-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 1.1.3
+Version: 1.1.4
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -22,15 +22,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.25.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 1.1.3
+# XT-STREAMLIT - 1.1.4
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

