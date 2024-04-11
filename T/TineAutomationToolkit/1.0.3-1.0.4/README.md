# Comparing `tmp/TineAutomationToolkit-1.0.3.tar.gz` & `tmp/TineAutomationToolkit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.0.3.tar", last modified: Wed Apr 10 09:28:43 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.0.4.tar", last modified: Thu Apr 11 01:14:28 2024, max compression
```

## Comparing `TineAutomationToolkit-1.0.3.tar` & `TineAutomationToolkit-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/
--rw-rw-rw-   0        0        0     2280 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      356 2024-03-19 04:35:22.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/detect/
--rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/detect/detectelement.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      587 2024-03-19 04:35:08.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     3404 2024-04-09 05:36:45.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0    11638 2024-04-10 08:38:10.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     5899 2024-03-19 02:59:09.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 09:28:43.000000 TineAutomationToolkit-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-10 09:24:58.000000 TineAutomationToolkit-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/
+-rw-rw-rw-   0        0        0     2280 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      356 2024-03-19 04:35:22.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/
+-rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/detectelement.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      587 2024-03-19 04:35:08.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     3913 2024-04-11 01:12:35.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    11638 2024-04-10 08:38:10.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     5899 2024-03-19 02:59:09.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-11 01:06:41.000000 TineAutomationToolkit-1.0.4/setup.py
```

### Comparing `TineAutomationToolkit-1.0.3/PKG-INFO` & `TineAutomationToolkit-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.3/README.md` & `TineAutomationToolkit-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/detect/detectelement.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/detectelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,14 +65,32 @@
 
         อาร์กิวเมนต์:  
 
         app_id - BundleId สำหรับ iOS, ชื่อแพ็คเกจสำหรับ Android.
         ใหม่ใน AppiumLibrary เวอร์ชัน 2
         """
         return self._current_application().terminate_app(app_id)
+    
+    def commond_install_app(self, app_path, app_package):
+        """ Install App via Appium
+        
+        Android .
+
+        - app_path - path to app (.apk)
+        - app_package - package of install app to verify
+
+        Ios .
+
+        - app_path - path to app (.app | .ipa)
+        - bundleId - package of install app to verify
+        """
+        driver = self._current_application()
+        driver.install_app(app_path)
+        return driver.is_app_installed(app_package)
+    
     #PRIVATE_FUNCTION
         
     def _current_application(self):
         """Return the instance of the current application
         From AppiumFlutterLibrary
 
         =========================================================
```

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/controlelement.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/controlelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.3/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.3/setup.py` & `TineAutomationToolkit-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.0.3",
+    version="1.0.4",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```

