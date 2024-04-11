# Comparing `tmp/qaml-0.0.6.post1.tar.gz` & `tmp/qaml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.6.post1.tar", last modified: Wed Apr 10 17:14:20 2024, max compression
+gzip compressed data, was "qaml-0.0.7.tar", last modified: Thu Apr 11 17:20:48 2024, max compression
```

## Comparing `qaml-0.0.6.post1.tar` & `qaml-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 17:14:20.734454 qaml-0.0.6.post1/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.6.post1/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      723 2024-04-10 17:14:20.734311 qaml-0.0.6.post1/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      172 2024-04-10 16:48:11.000000 qaml-0.0.6.post1/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-10 17:14:00.000000 qaml-0.0.6.post1/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 17:14:20.733372 qaml-0.0.6.post1/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.6.post1/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      852 2024-04-08 20:17:36.000000 qaml-0.0.6.post1/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    10006 2024-04-10 17:13:19.000000 qaml-0.0.6.post1/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-10 17:14:20.734147 qaml-0.0.6.post1/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      723 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-10 17:14:20.000000 qaml-0.0.6.post1/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-10 17:14:20.734495 qaml-0.0.6.post1/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-11 17:20:48.205490 qaml-0.0.7/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-11 17:20:48.205352 qaml-0.0.7/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-11 17:16:45.000000 qaml-0.0.7/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-11 17:20:48.204455 qaml-0.0.7/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-11 17:16:45.000000 qaml-0.0.7/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    10256 2024-04-11 17:19:58.000000 qaml-0.0.7/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-11 17:20:48.205193 qaml-0.0.7/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-11 17:20:48.000000 qaml-0.0.7/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-11 17:20:48.205527 qaml-0.0.7/setup.cfg
```

### Comparing `qaml-0.0.6.post1/LICENSE` & `qaml-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.6.post1/pyproject.toml` & `qaml-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.6-1"
+version = "0.0.7"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.6.post1/qaml/client.py` & `qaml-0.0.7/qaml/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         screenshot = base64.b64encode(buffered.getvalue()).decode("utf-8")
         return screenshot
 
     def execute(self, script):
         screenshot = self.get_screenshot()
         payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.context}
         response = self.req_session.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
-        print(response.text)
+        print(f"Action: {script} - Response: {response.text}")
         actions = response.json()
         available_functions = {
             "tap": self.tap_coordinates,
             "drag": self.drag,
             "swipe": self.swipe,
             "scroll": self.scroll,
             "type_text": self.type_text,
@@ -148,52 +148,56 @@
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.swipe(direction_map[direction])
 
     def type_text(self, text):
         subprocess.run(["adb", "shell", "input", "text", f"'{text}'"])
 
 class IOSClient(BaseClient):
-    def __init__(self, api_key, driver=None, ios_udid=None):
+    def __init__(self, api_key, driver=None, ios_udid=None, use_mjpeg=True):
         super().__init__(api_key)
         self.platform = "iOS"
+        self.use_mjpeg = use_mjpeg
         if driver:
             self.driver = driver
         else:
             # try 3 times to setup the driver
             for _ in range(3):
                 try:
                     self.setup_driver(ios_udid)
                     break
                 except:
                     pass
-            else Exception as e:
-                print(e)
+            else:
                 raise Exception("Failed to setup the driver.")
         self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self, udid):
         options = XCUITestOptions()
         options.udid = udid
-        custom_caps = {"mjpegScreenshotUrl": "http://localhost:9100"}
-        options.load_capabilities(custom_caps)
+        options.new_command_timeout = 60 * 5 # 5 minutes
+        if self.use_mjpeg:
+            custom_caps = {"mjpegScreenshotUrl": "http://localhost:9100"}
+            options.load_capabilities(custom_caps)
 
         def create_driver(options):
             try:
                 return webdriver.Remote('http://localhost:4723', options=options)
             except:
                 return webdriver.Remote('http://localhost:4723/wd/hub', options=options)
         try:
             self.driver = create_driver(options)
         except:
             # Try again without mjpeg-consumer dependency
             options = XCUITestOptions()
             options.udid = udid
             self.driver = create_driver(options)
 
-        self.driver.start_recording_screen(forceRestart=True)
+        if self.use_mjpeg:
+            print("Using MJPEG screenshot.")
+            self.driver.start_recording_screen(forceRestart=True)
         self.driver.update_settings({'waitForIdleTimeout': 0, 'shouldWaitForQuiescence': False, 'maxTypingFrequency': 60})
         # get screenshot to test if the driver is working
         self.driver.get_screenshot_as_base64()
 
     def tap_coordinates(self, x, y):
         self.driver.execute_script("mobile: tap", {"x": x, "y": y})
 
@@ -209,15 +213,15 @@
 
     def type_text(self, text):
         self.driver.find_element(AppiumBy.IOS_PREDICATE, "type == 'XCUIElementTypeApplication'").send_keys(text)
 
     def switch_to_app(self, bundle_id):
         self.driver.activate_app(bundle_id)
 
-def Client(api_key, driver=None):
+def Client(api_key, driver=None, use_mjpeg=True):
     def get_ios_udid():
         system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
         serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
 
         if serial_numbers:
             first_serial_number = serial_numbers[0][1].strip()
             modified_serial_number = first_serial_number[:8] + '-' + first_serial_number[8:]
@@ -245,11 +249,11 @@
 
     android_devices = get_connected_android_devices()
     if android_devices:
         return AndroidClient(api_key)
 
     ios_udid = get_ios_udid()
     if ios_udid:
-        return IOSClient(api_key, ios_udid=ios_udid)
+        return IOSClient(api_key, ios_udid=ios_udid, use_mjpeg=use_mjpeg)
 
     raise Exception("No connected devices found or driver provided.")
```

