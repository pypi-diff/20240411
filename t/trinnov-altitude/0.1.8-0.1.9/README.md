# Comparing `tmp/trinnov-altitude-0.1.8.tar.gz` & `tmp/trinnov-altitude-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.8.tar", last modified: Thu Apr 11 00:23:32 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.9.tar", last modified: Thu Apr 11 00:41:18 2024, max compression
```

## Comparing `trinnov-altitude-0.1.8.tar` & `trinnov-altitude-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.029314 trinnov-altitude-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19790 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.8/LICENSE` & `trinnov-altitude-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/PKG-INFO` & `trinnov-altitude-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.8
+Version: 0.1.9
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -174,14 +174,16 @@
 await altitude.mute_toggle()
 ```
 
 ### Page adjust
 
 ```python
 await altitude.page_adjust(delta: int)
+await altitude.page_down()
+await altitude.page_up()
 ```
 
 ### Power
 
 ```python
 altitude.power_on()
 await altitude.power_off()
```

### Comparing `trinnov-altitude-0.1.8/README.md` & `trinnov-altitude-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,16 @@
 await altitude.mute_toggle()
 ```
 
 ### Page adjust
 
 ```python
 await altitude.page_adjust(delta: int)
+await altitude.page_down()
+await altitude.page_up()
 ```
 
 ### Power
 
 ```python
 altitude.power_on()
 await altitude.power_off()
```

### Comparing `trinnov-altitude-0.1.8/setup.cfg` & `trinnov-altitude-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.9/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/trinnov_altitude/const.py` & `trinnov-altitude-0.1.9/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/trinnov_altitude/exceptions.py` & `trinnov-altitude-0.1.9/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/trinnov_altitude/messages.py` & `trinnov-altitude-0.1.9/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.9/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.8/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.9/trinnov_altitude/trinnov_altitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,27 @@
     async def page_adjust(
         self, delta: int, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Changes the menu page currently on the GUI. `delta` indicates the number of
         pages to change, and may be positive or negative.
         """
-        await self._write("bypass 2", timeout)
+        await self._write(f"page_adjust {delta}", timeout)
+
+    async def page_down(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Changes the menu page currently on the GUI down by one page.
+        """
+        await self.page_adjust(-1)
+
+    async def page_up(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Changes the menu page currently on the GUI up by one page.
+        """
+        await self.page_adjust(1)
 
     async def power_off(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """Power off."""
         await self._write("power off SECURED FHZMCH48FE", timeout)
 
     def power_on(self):
         """Power on."""
```

### Comparing `trinnov-altitude-0.1.8/trinnov_altitude.egg-info/PKG-INFO` & `trinnov-altitude-0.1.9/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.8
+Version: 0.1.9
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -174,14 +174,16 @@
 await altitude.mute_toggle()
 ```
 
 ### Page adjust
 
 ```python
 await altitude.page_adjust(delta: int)
+await altitude.page_down()
+await altitude.page_up()
 ```
 
 ### Power
 
 ```python
 altitude.power_on()
 await altitude.power_off()
```

