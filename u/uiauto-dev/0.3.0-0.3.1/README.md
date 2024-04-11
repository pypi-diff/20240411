# Comparing `tmp/uiauto_dev-0.3.0.tar.gz` & `tmp/uiauto_dev-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiauto_dev-0.3.0.tar", max compression
+gzip compressed data, was "uiauto_dev-0.3.1.tar", max compression
```

## Comparing `uiauto_dev-0.3.0.tar` & `uiauto_dev-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1068 2024-02-18 02:48:04.400793 uiauto_dev-0.3.0/LICENSE
--rw-r--r--   0        0        0      585 2024-04-01 15:30:41.627882 uiauto_dev-0.3.0/README.md
--rw-r--r--   0        0        0     1081 2024-04-01 15:30:49.785887 uiauto_dev-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      268 2024-04-01 15:30:41.632788 uiauto_dev-0.3.0/uiauto_dev/__init__.py
--rw-r--r--   0        0        0      177 2024-04-01 15:30:41.633441 uiauto_dev-0.3.0/uiauto_dev/__main__.py
--rw-r--r--   0        0        0     2423 2024-04-01 15:30:41.633862 uiauto_dev-0.3.0/uiauto_dev/app.py
--rw-r--r--   0        0        0     1773 2024-04-01 15:30:41.634199 uiauto_dev-0.3.0/uiauto_dev/appium_proxy.py
--rw-r--r--   0        0        0     4493 2024-04-01 15:30:41.634471 uiauto_dev-0.3.0/uiauto_dev/cli.py
--rw-r--r--   0        0        0     2634 2024-04-01 15:30:41.634812 uiauto_dev-0.3.0/uiauto_dev/command_proxy.py
--rw-r--r--   0        0        0     1001 2024-04-01 15:30:41.635028 uiauto_dev-0.3.0/uiauto_dev/command_types.py
--rw-r--r--   0        0        0     5852 2024-04-01 15:30:41.635834 uiauto_dev-0.3.0/uiauto_dev/driver/android.py
--rw-r--r--   0        0        0     5324 2024-04-01 15:30:41.636254 uiauto_dev-0.3.0/uiauto_dev/driver/appium.py
--rw-r--r--   0        0        0     1838 2024-04-01 15:30:41.636533 uiauto_dev-0.3.0/uiauto_dev/driver/base_driver.py
--rw-r--r--   0        0        0     4378 2024-04-01 15:30:41.636842 uiauto_dev-0.3.0/uiauto_dev/driver/ios.py
--rw-r--r--   0        0        0     2454 2024-04-01 15:30:41.637158 uiauto_dev-0.3.0/uiauto_dev/driver/mock.py
--rw-r--r--   0        0        0      335 2024-04-01 15:30:41.637525 uiauto_dev-0.3.0/uiauto_dev/exceptions.py
--rw-r--r--   0        0        0      727 2024-04-01 15:30:41.637725 uiauto_dev-0.3.0/uiauto_dev/model.py
--rw-r--r--   0        0        0     2327 2024-04-01 15:30:41.637953 uiauto_dev-0.3.0/uiauto_dev/provider.py
--rw-r--r--   0        0        0     3876 2024-04-01 15:30:41.638214 uiauto_dev-0.3.0/uiauto_dev/router/device.py
--rw-r--r--   0        0        0      891 2024-04-01 15:30:41.638386 uiauto_dev-0.3.0/uiauto_dev/router/xml.py
--rw-r--r--   0        0        0     1240 2024-04-01 15:30:41.638617 uiauto_dev-0.3.0/uiauto_dev/static/demo.html
--rw-r--r--   0        0        0     4289 2024-04-01 15:30:41.639132 uiauto_dev-0.3.0/uiauto_dev/utils/common.py
--rw-r--r--   0        0        0      638 2024-04-01 15:30:41.639371 uiauto_dev-0.3.0/uiauto_dev/utils/exceptions.py
--rw-r--r--   0        0        0    17387 2024-04-01 15:30:41.639863 uiauto_dev-0.3.0/uiauto_dev/utils/usbmux.py
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 uiauto_dev-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/README.md
+-rw-r--r--   0        0        0     1081 2024-04-11 05:03:11.882846 uiauto_dev-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      268 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/__init__.py
+-rw-r--r--   0        0        0      177 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/__main__.py
+-rw-r--r--   0        0        0     2410 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/app.py
+-rw-r--r--   0        0        0     1773 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/appium_proxy.py
+-rw-r--r--   0        0        0     5200 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/cli.py
+-rw-r--r--   0        0        0     2634 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/command_proxy.py
+-rw-r--r--   0        0        0     1001 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/command_types.py
+-rw-r--r--   0        0        0     5852 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/android.py
+-rw-r--r--   0        0        0     5324 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/appium.py
+-rw-r--r--   0        0        0     1838 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/base_driver.py
+-rw-r--r--   0        0        0     4378 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/ios.py
+-rw-r--r--   0        0        0     2454 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/mock.py
+-rw-r--r--   0        0        0      335 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/exceptions.py
+-rw-r--r--   0        0        0      727 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/model.py
+-rw-r--r--   0        0        0     2327 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/provider.py
+-rw-r--r--   0        0        0     3876 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/router/device.py
+-rw-r--r--   0        0        0      891 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/router/xml.py
+-rw-r--r--   0        0        0     1240 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/static/demo.html
+-rw-r--r--   0        0        0     4289 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/utils/common.py
+-rw-r--r--   0        0        0      638 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/utils/exceptions.py
+-rw-r--r--   0        0        0    17387 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/utils/usbmux.py
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 uiauto_dev-0.3.1/PKG-INFO
```

### Comparing `uiauto_dev-0.3.0/LICENSE` & `uiauto_dev-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/README.md` & `uiauto_dev-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # uiauto-dev
-[![codecov](https://codecov.io/gh/codeskyblue/uiauto-dev/graph/badge.svg?token=aLTg4VOyQH)](https://codecov.io/gh/codeskyblue/uiauto-dev)
+[![codecov](https://codecov.io/gh/codeskyblue/appinspector/graph/badge.svg?token=aLTg4VOyQH)](https://codecov.io/gh/codeskyblue/appinspector)
 [![PyPI version](https://badge.fury.io/py/uiauto-dev.svg)](https://badge.fury.io/py/uiauto-dev)
 
 https://uiauto.dev
 
 UI Inspector for Android and iOS, help inspector element properties, and auto generate XPath, script.
```

### Comparing `uiauto_dev-0.3.0/pyproject.toml` & `uiauto_dev-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uiauto-dev"
-version = "0.3.0"
+version = "0.3.1"
 description = "Mobile UI Automation, include UI hierarchy inspector, script recorder"
 homepage = "https://uiauto.dev"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uiauto_dev-0.3.0/uiauto_dev/app.py` & `uiauto_dev-0.3.1/uiauto_dev/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,8 +85,8 @@
     print(static_dir / "demo.html")
     return FileResponse(static_dir / "demo.html")
 
 
 @app.get("/")
 def index_redirect():
     """ redirect to uiauto_dev.devsleep.com """
-    return RedirectResponse("https://uiauto_dev.devsleep.com")
+    return RedirectResponse("https://uiauto.dev")
```

### Comparing `uiauto_dev-0.3.0/uiauto_dev/appium_proxy.py` & `uiauto_dev-0.3.1/uiauto_dev/appium_proxy.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/cli.py` & `uiauto_dev-0.3.1/uiauto_dev/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from __future__ import annotations
 
 import logging
 import platform
 import sys
 from pprint import pprint
+import threading
+import time
 
 import click
 import httpx
 import pydantic
 import uvicorn
 
 from uiauto_dev import __version__, command_proxy
@@ -34,15 +36,14 @@
         console_handler = logging.StreamHandler()
         console_handler.setLevel(logging.DEBUG)
         
         formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
         console_handler.setFormatter(formatter)
 
         root_logger.addHandler(console_handler)
-
         logger.debug("Verbose mode enabled")
 
 
 def run_driver_command(provider: BaseProvider, command: Command, params: list[str] = None):
     if command == Command.LIST:
         devices = provider.list_devices()
         print("==> Devices <==")
@@ -107,35 +108,54 @@
 
 
 @cli.command()
 @click.option("--port", default=20242, help="port number", show_default=True)
 @click.option("--host", default="127.0.0.1", help="host", show_default=True)
 @click.option("--reload", is_flag=True, default=False, help="auto reload, dev only")
 @click.option("-f", "--force", is_flag=True, default=False, help="shutdown alrealy runningserver")
-def server(port: int, host: str, reload: bool, force: bool):
+@click.option("--no-browser", is_flag=True, default=False, help="do not open browser")
+def server(port: int, host: str, reload: bool, force: bool, no_browser: bool):
     logger.info("version: %s", __version__)
     if force:
         try:
             httpx.get(f"http://{host}:{port}/shutdown", timeout=3)
         except httpx.HTTPError:
             pass
 
     # if args.mock:
     #     os.environ["uiauto_dev_MOCK"] = "1"
     use_color = True
     if platform.system() == 'Windows':
         use_color = False
+    
+    if not no_browser:
+        th = threading.Thread(target=open_browser_when_server_start, args=(f"http://{host}:{port}",))
+        th.daemon = True
+        th.start()
     uvicorn.run("uiauto_dev.app:app", host=host, port=port, reload=reload, use_colors=use_color)
 
 
+def open_browser_when_server_start(server_url: str):
+    deadline = time.time() + 10
+    while time.time() < deadline:
+        try:
+            httpx.get(f"{server_url}/api/info", timeout=1)
+            break
+        except Exception as e:
+            time.sleep(0.5)
+    import webbrowser
+    web_url = "https://uiauto.dev"
+    logger.info("open browser: %s", web_url)
+    webbrowser.open(web_url)
+
 def main():
     # set logger level to INFO
     # logging.basicConfig(level=logging.INFO)
     logger.setLevel(logging.INFO)
     if len(sys.argv) == 1:
-        cli.main(args=["server"], prog_name="uiauto_dev")
+        cli.main(args=["server"], prog_name="uiauto.dev")
     else:
         cli()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `uiauto_dev-0.3.0/uiauto_dev/command_proxy.py` & `uiauto_dev-0.3.1/uiauto_dev/command_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from __future__ import annotations
 
 import typing
 from typing import Callable, Dict, Optional
 
 from pydantic import BaseModel
 
-from uiauto_dev.command_types import Command, CurrentAppResponse, DumpResponse, InstallAppRequest, \
-    InstallAppResponse, TapRequest, WindowSizeResponse
+from uiauto_dev.command_types import Command, CurrentAppResponse, DumpResponse, InstallAppRequest, InstallAppResponse, \
+    TapRequest, WindowSizeResponse
 from uiauto_dev.driver.base_driver import BaseDriver
 
 COMMANDS: Dict[Command, Callable] = {}
 
 
 def register(command: Command):
     def wrapper(func):
```

### Comparing `uiauto_dev-0.3.0/uiauto_dev/command_types.py` & `uiauto_dev-0.3.1/uiauto_dev/command_types.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/driver/android.py` & `uiauto_dev-0.3.1/uiauto_dev/driver/android.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/driver/appium.py` & `uiauto_dev-0.3.1/uiauto_dev/driver/appium.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/driver/base_driver.py` & `uiauto_dev-0.3.1/uiauto_dev/driver/base_driver.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/driver/ios.py` & `uiauto_dev-0.3.1/uiauto_dev/driver/ios.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/driver/mock.py` & `uiauto_dev-0.3.1/uiauto_dev/driver/mock.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/model.py` & `uiauto_dev-0.3.1/uiauto_dev/model.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/provider.py` & `uiauto_dev-0.3.1/uiauto_dev/provider.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/router/device.py` & `uiauto_dev-0.3.1/uiauto_dev/router/device.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/router/xml.py` & `uiauto_dev-0.3.1/uiauto_dev/router/xml.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/static/demo.html` & `uiauto_dev-0.3.1/uiauto_dev/static/demo.html`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/utils/common.py` & `uiauto_dev-0.3.1/uiauto_dev/utils/common.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/utils/exceptions.py` & `uiauto_dev-0.3.1/uiauto_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.0/uiauto_dev/utils/usbmux.py` & `uiauto_dev-0.3.1/uiauto_dev/utils/usbmux.py`

 * *Files identical despite different names*

