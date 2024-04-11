# Comparing `tmp/alliance_platform_frontend-0.0.2.tar.gz` & `tmp/alliance_platform_frontend-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_frontend-0.0.2.tar", last modified: Wed Apr 10 00:56:57 2024, max compression
+gzip compressed data, was "alliance_platform_frontend-0.0.3.tar", last modified: Thu Apr 11 03:08:09 2024, max compression
```

## Comparing `alliance_platform_frontend-0.0.2.tar` & `alliance_platform_frontend-0.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2946 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/README.md
--rw-r--r--   0        0        0       22 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/__init__.py
--rw-r--r--   0        0        0      784 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/button.py
--rw-r--r--   0        0        0     1839 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/date_picker.py
--rw-r--r--   0        0        0     2524 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/icon.py
--rw-r--r--   0        0        0     1421 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/inline_alert.py
--rw-r--r--   0        0        0     1464 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/menubar.py
--rw-r--r--   0        0        0     2075 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/misc.py
--rw-r--r--   0        0        0     1622 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/pagination.py
--rw-r--r--   0        0        0     2270 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/table.py
--rw-r--r--   0        0        0     1127 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/time_input.py
--rw-r--r--   0        0        0     1243 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/utils.py
--rw-r--r--   0        0        0      358 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/apps.py
--rw-r--r--   0        0        0      512 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/__init__.py
--rw-r--r--   0        0        0     3310 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/asset_registry.py
--rw-r--r--   0        0        0    15999 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/base.py
--rw-r--r--   0        0        0    17174 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/context.py
--rw-r--r--   0        0        0     2507 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/middleware.py
--rw-r--r--   0        0        0    13537 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/ssr.py
--rw-r--r--   0        0        0     7051 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vanilla_extract.py
--rw-r--r--   0        0        0    33406 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vite.py
--rw-r--r--   0        0        0      175 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vitePreload.ts
--rw-r--r--   0        0        0    11144 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/dom_possible_standard_names.py
--rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/forms/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/forms/renderers.py
--rw-r--r--   0        0        0     5266 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/management/commands/extract_frontend_assets.py
--rw-r--r--   0        0        0    10434 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/prop_handlers.py
--rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/py.typed
--rw-r--r--   0        0        0     3867 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/settings.py
--rw-r--r--   0        0        0     2684 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templates/bundler_dev_check.html
--rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/__init__.py
--rw-r--r--   0        0        0     5451 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/alliance_ui.py
--rw-r--r--   0        0        0    12851 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/bundler.py
--rw-r--r--   0        0        0     9664 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/form.py
--rw-r--r--   0        0        0    56265 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/react.py
--rw-r--r--   0        0        0     4316 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/vanilla_extract.py
--rw-r--r--   0        0        0     3283 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/alliance_platform/frontend/util.py
--rw-r--r--   0        0        0     2120 2024-04-10 00:56:57.919972 alliance_platform_frontend-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/tests/fixtures/build_test/manifest.json
--rw-r--r--   0        0        0       39 2024-04-10 00:56:33.292116 alliance_platform_frontend-0.0.2/tests/fixtures/development-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0       30 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/fixtures/production-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0      648 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/fixtures/server_build_test/manifest.json
--rw-r--r--   0        0        0     7955 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_alliance_ui_templatetags.py
--rw-r--r--   0        0        0    11119 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_bundler.py
--rw-r--r--   0        0        0    33736 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_bundler_templatetags.py
--rw-r--r--   0        0        0     5837 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_context.py
--rw-r--r--   0        0        0      721 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-10 00:56:33.296115 alliance_platform_frontend-0.0.2/tests/test_utils/bundler.py
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/button.py
+-rw-r--r--   0        0        0     1839 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/date_picker.py
+-rw-r--r--   0        0        0     2524 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/icon.py
+-rw-r--r--   0        0        0     1421 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/inline_alert.py
+-rw-r--r--   0        0        0     1464 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/menubar.py
+-rw-r--r--   0        0        0     2075 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/misc.py
+-rw-r--r--   0        0        0     1622 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/pagination.py
+-rw-r--r--   0        0        0     2270 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/table.py
+-rw-r--r--   0        0        0     1127 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/time_input.py
+-rw-r--r--   0        0        0     1243 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/utils.py
+-rw-r--r--   0        0        0      358 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/apps.py
+-rw-r--r--   0        0        0      633 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/__init__.py
+-rw-r--r--   0        0        0     2402 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/asset_registry.py
+-rw-r--r--   0        0        0    15999 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/base.py
+-rw-r--r--   0        0        0    17116 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/context.py
+-rw-r--r--   0        0        0     2507 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/middleware.py
+-rw-r--r--   0        0        0    13537 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/ssr.py
+-rw-r--r--   0        0        0     7051 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vanilla_extract.py
+-rw-r--r--   0        0        0    33786 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vite.py
+-rw-r--r--   0        0        0      175 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vitePreload.ts
+-rw-r--r--   0        0        0    11144 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/dom_possible_standard_names.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/forms/__init__.py
+-rw-r--r--   0        0        0     1620 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/forms/renderers.py
+-rw-r--r--   0        0        0     5370 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/management/commands/extract_frontend_assets.py
+-rw-r--r--   0        0        0    10434 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/prop_handlers.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/py.typed
+-rw-r--r--   0        0        0     7344 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/settings.py
+-rw-r--r--   0        0        0     2684 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templates/bundler_dev_check.html
+-rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/__init__.py
+-rw-r--r--   0        0        0     5451 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/alliance_ui.py
+-rw-r--r--   0        0        0    12922 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/bundler.py
+-rw-r--r--   0        0        0     9664 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/form.py
+-rw-r--r--   0        0        0    56265 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/react.py
+-rw-r--r--   0        0        0     4316 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/vanilla_extract.py
+-rw-r--r--   0        0        0     3283 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/util.py
+-rw-r--r--   0        0        0     2120 2024-04-11 03:08:09.277969 alliance_platform_frontend-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2503 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/build_test/manifest.json
+-rw-r--r--   0        0        0       39 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/development-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0       30 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/production-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0      648 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/server_build_test/manifest.json
+-rw-r--r--   0        0        0     7955 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_alliance_ui_templatetags.py
+-rw-r--r--   0        0        0    11119 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_bundler.py
+-rw-r--r--   0        0        0    33736 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_bundler_templatetags.py
+-rw-r--r--   0        0        0     5837 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_context.py
+-rw-r--r--   0        0        0      721 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_utils/bundler.py
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.3/PKG-INFO
```

### Comparing `alliance_platform_frontend-0.0.2/README.md` & `alliance_platform_frontend-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/button.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/button.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/date_picker.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/date_picker.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/icon.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/icon.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/inline_alert.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/inline_alert.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/menubar.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/menubar.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/misc.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/misc.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/pagination.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/pagination.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/table.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/table.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/time_input.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/time_input.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/alliance_ui/utils.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/utils.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/base.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/base.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/context.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from django.http import HttpRequest
 from django.template import Origin
 from django.utils.module_loading import import_string
 
 from ..settings import ap_frontend_settings
 from . import get_bundler
 from .asset_registry import FrontendAssetRegistry
-from .asset_registry import frontend_asset_registry as default_frontend_asset_registry
 from .base import AssetFileEmbed
 from .base import BaseBundler
 from .base import HtmlGenerationTarget
 from .base import html_target_browser
 from .ssr import SSRItem
 
 GLOBAL_BUNDLER_ASSET_CONTEXT = threading.local()
@@ -27,21 +26,21 @@
 class NoActiveBundlerAssetContext(Exception):
     """Thrown if :meth:`~alliance_platform.frontend.bundler.context.BundlerAssetContext.get_current` is called when no context is active"""
 
     pass
 
 
 class UndiscoverableAssetsError(Exception):
-    """Thrown if assets are used, but cannot be discovered automatically and aren't registered with ``frontend_asset_registry``"""
+    """Thrown if assets are used, but cannot be discovered automatically and aren't registered with the asset registry"""
 
     def __init__(self, paths: set[Path]):
         paths_str = "\n".join(map(str, paths))
         super().__init__(
             f"The following paths were used but cannot be auto-discovered by `extract_frontend_assets`:\n{paths_str}\n\n"
-            f"To resolve add these paths to `frontend_asset_registry.add_asset(...paths...)`."
+            f"To resolve add these paths to the asset registry, e.g. `frontend_asset_registry.add_asset(...paths...)`."
         )
         self.undiscoverable_assets = paths
 
 
 class BundlerAsset:
     """
     A class representing an asset (e.g. script, stylesheet) that needs to be bundled.
@@ -170,15 +169,15 @@
 
     #: Will be set if used within ``BundlerAssetContextMiddleware``. In other contexts may be unavailable
     request: HttpRequest | None
 
     def __init__(
         self,
         *,
-        frontend_asset_registry: FrontendAssetRegistry = default_frontend_asset_registry,
+        frontend_asset_registry: FrontendAssetRegistry = ap_frontend_settings.FRONTEND_ASSET_REGISTRY,
         html_target=html_target_browser,
         skip_checks=False,
         request: HttpRequest | None = None,
     ):
         self.request = request
         self.skip_checks = skip_checks
         self.html_target = html_target
```

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/middleware.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/middleware.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/ssr.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/ssr.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vanilla_extract.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/bundler/vite.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vite.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,31 @@
             path = path.relative_to(self.root_dir)
         if path not in self.entries:
             raise ViteManifestAssetMissingError(self.manifest_file, path)
         return self.entries[path]
 
 
 class ViteBundler(BaseBundler):
+    """Bundler implementation for `Vite <https://vitejs.dev/>`_.
+
+    Args:
+        root_dir: The root path everything sits under; all other paths are resolved relative to this
+        path_resolvers: A list of :class:`~alliance_platform.frontend.bundler.base.PathResolver` instances used to resolve paths
+        server_build_dir: The directory SSR files are outputted to (see ``yarn build:ssr``)
+        build_dir: The directory client side files are outputted to (see ``yarn build:client``)
+        server_host: The hostname used for the dev server (e.g. ``127.0.0.1``)
+        server_port: The port used for the dev server (e.g. ``5173``)
+        server_protocol: The protocol used for the dev server (``http`` or ``https``)
+        mode: The mode the bundler is running in; one of ``development``, ``production`` or ``preview``
+        wait_for_server: Function that can be passed that will be called before requesting assets for server. This function
+            should handle waiting until the dev server is ready before returning (e.g. by polling the server status)
+        production_ssr_url: URL for SSR (only used in production mode)
+
+    """
+
     #: Directory server side rendering (SSR) files are compiled to
     server_build_dir: Path
     #: Directory client side files are compiled to
     build_dir: Path
     #: Manifest for SSR (only available when in production mode)
     server_build_manifest: ViteManifest
     #: Manifest for client build (only available when in production mode)
@@ -288,26 +305,14 @@
         server_host: str,
         server_port: str,
         server_protocol: str,
         mode: str,
         production_ssr_url: str | None = None,
         wait_for_server: Callable[[], None] | None = None,
     ):
-        """Bundler implementation for `Vite <https://vitejs.dev/>`_.
-
-        Args:
-            root_dir: The root path everything sits under; all other paths are resolved relative to this
-            path_resolvers: A list of :class:`~alliance_platform.frontend.bundler.base.PathResolver` instances used to resolve paths
-            server_build_dir: The directory SSR files are outputted to (see ``yarn build:ssr``)
-            build_dir: The directory client side files are outputted to (see ``yarn build:client``)
-            server_host: The hostname used for the dev server (e.g. ``127.0.0.1``)
-            server_port: The port used for the dev server (e.g. ``5173``)
-            server_protocol: The protocol used for the dev server (``http`` or ``https``)
-            mode: The mode the bundler is running in; one of ``development``, ``production`` or ``preview``
-        """
         self.wait_for_server = wait_for_server
         valid_modes = ["development", "production", "preview"]
         if mode not in valid_modes:
             raise ValueError(f"'mode' must be one of {', '.join(valid_modes)}, received: '{mode}'")
         super().__init__(root_dir, path_resolvers)
         self.mode = mode
         self.server_build_dir = server_build_dir
@@ -466,27 +471,27 @@
         if self.is_development():
             return path
         return self.server_build_dir / self.server_build_manifest.get_asset(path).file
 
     def get_development_ssr_url(self):
         """Returns the URL for SSR rendering used in dev
 
-        See ``dev-server.ts`` for where this is handled.
+        This assumes the Vite dev server has a 'ssr/' endpoint to handle requests.
         """
         return urljoin(self.dev_server_url_base, "ssr")
 
     def get_ssr_url(self):
         """Returns the URL for SSR rendering
 
-        For development see ``dev-server.ts`` for where this is handled.
+        In dev, this uses :meth:`~alliance_platform.frontend.bundler.vite.ViteBundler.get_development_ssr_url`.
 
-        For production see ``production-ssr-server.ts``
+        In production :data:`~alliance_platform.frontend.bundler.vite.ViteBundler.production_ssr_url` is used.
         """
         if self.is_development():
-            return urljoin(self.dev_server_url_base, "ssr")
+            return self.get_development_ssr_url()
         if self.mode == "preview":
             return urljoin(self.preview_url, "ssr")
         if self.production_ssr_url:
             return urljoin(self.production_ssr_url, "ssr")
         return None
 
     def get_ssr_headers(self):
```

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/dom_possible_standard_names.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/dom_possible_standard_names.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/forms/renderers.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/management/commands/extract_frontend_assets.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/management/commands/extract_frontend_assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 from django.core.management.base import OutputWrapper
 from django.template import TemplateSyntaxError
 from django.template import engines
 from django.template.loader import get_template
 from django.template.utils import get_app_template_dirs
 
 from ...bundler import get_bundler
-from ...bundler.asset_registry import frontend_asset_registry
 from ...bundler.context import BundlerAssetContext
 from ...settings import ap_frontend_settings
 
 
 @lru_cache
 def get_all_templates_files() -> list[Path]:
     """Scans all template dirs for template files
 
-    Will exclude any templates the match an entry in :setting:`EXTRACT_ASSETS_EXCLUDE_DIRS`.
+    Will exclude any templates the match an entry in :data:`~alliance_platform.frontend.settings.AlliancePlatformFrontendSettingsType.EXTRACT_ASSETS_EXCLUDE_DIRS`
     """
     dirs = get_app_template_dirs("templates")
     for engine in engines.all():
         dirs += tuple(engine.template_dirs)
     files: list[Path] = []
     for dir in dirs:
         should_exclude = False
@@ -50,15 +49,15 @@
 
 def extract_asset_filenames() -> tuple[list[Any], dict[str, Collection[str]], list[str], list[str]]:
     """Scans all template files for assets that need to be bundled
 
     Returns a 4-tuple: list of filenames, breakdown dict, errors and warnings
     """
 
-    all_files = {str(f) for f in frontend_asset_registry.get_asset_paths()}
+    all_files = {str(f) for f in ap_frontend_settings.FRONTEND_ASSET_REGISTRY.get_asset_paths()}
     breakdown_templates: dict[str, list[str]] = {}
     breakdown = {
         "registry": list(sorted(all_files)),
         "templates": breakdown_templates,
     }
     errors: list[str] = []
     warnings: list[str] = []
@@ -92,15 +91,16 @@
 
 class Command(BaseCommand):
     """
     Extracts used frontend assets from templates used
 
     This works with any template nodes that extend :class:`~alliance_platform.frontend.bundler.context.BundlerAsset`. All templates
     in the system are loaded to gather all used assets. You can exclude specific directories by setting
-    :setting:`EXTRACT_ASSETS_EXCLUDE_DIRS` to either a :class:`pathlib.Path` or ``re.Pattern``.
+    :data:`~alliance_platform.frontend.settings.AlliancePlatformFrontendSettingsType.EXTRACT_ASSETS_EXCLUDE_DIRS`
+    to either a :class:`pathlib.Path` or ``re.Pattern``.
 
     Outputs a valid JSON dump as an array of string paths to files.
 
     Usage::
 
         # Will write data to output.json
         ./manage.py extract_frontend_assets --output output.json
```

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/prop_handlers.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/prop_handlers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templates/bundler_dev_check.html` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templates/bundler_dev_check.html`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/alliance_ui.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/alliance_ui.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/bundler.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/bundler.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
 @register.simple_tag()
 def bundler_dev_checks():
     """Performs dev specific checks and may render some HTML to communicate messages to user
 
     Currently check if the dev server is running for this project, and if not displays an error.
 
     Error will be logged to Django dev console. In addition, an error icon and toggleable modal message will be shown
-    in the HTML unless :setting:`BUNDLER_DISABLE_DEV_CHECK_HTML` is set.
+    in the HTML unless :data:`~alliance_platform.frontend.settings.AlliancePlatformFrontendSettingsType.BUNDLER_DISABLE_DEV_CHECK_HTML` is set.
     """
     bundler = get_bundler()
     if not bundler.is_development():
         return ""
     check = bundler.check_dev_server()
     if not check.is_ok():
         if not check.is_running:
```

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/form.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/react.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/react.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/templatetags/vanilla_extract.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/alliance_platform/frontend/util.py` & `alliance_platform_frontend-0.0.3/alliance_platform/frontend/util.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/pyproject.toml` & `alliance_platform_frontend-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 include = [
     "alliance_platform/frontend/py.typed",
 ]
-version = "0.0.2"
+version = "0.0.3"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [project.urls]
 issues = "https://github.com/AllianceSoftware/alliance-platform-py/issues"
 homepage = "https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend"
```

### Comparing `alliance_platform_frontend-0.0.2/tests/fixtures/build_test/manifest.json` & `alliance_platform_frontend-0.0.3/tests/fixtures/build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/fixtures/server_build_test/manifest.json` & `alliance_platform_frontend-0.0.3/tests/fixtures/server_build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/test_alliance_ui_templatetags.py` & `alliance_platform_frontend-0.0.3/tests/test_alliance_ui_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/test_bundler.py` & `alliance_platform_frontend-0.0.3/tests/test_bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/test_bundler_templatetags.py` & `alliance_platform_frontend-0.0.3/tests/test_bundler_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/test_context.py` & `alliance_platform_frontend-0.0.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/test_utils/__init__.py` & `alliance_platform_frontend-0.0.3/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/tests/test_utils/bundler.py` & `alliance_platform_frontend-0.0.3/tests/test_utils/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.2/PKG-INFO` & `alliance_platform_frontend-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alliance-platform-frontend
-Version: 0.0.2
+Version: 0.0.3
 Summary: Django integration for Frontend Bundlers & React
 Keywords: django alliance alliancesoftware
 Home-page: https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend
 Author-Email: Alliance Software <support@alliancesoftware.com.au>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

