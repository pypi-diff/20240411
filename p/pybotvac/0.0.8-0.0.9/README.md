# Comparing `tmp/pybotvac-0.0.8.tar.gz` & `tmp/pybotvac-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybotvac-0.0.8.tar", last modified: Sat Jul 14 16:13:40 2018, max compression
+gzip compressed data, was "dist\pybotvac-0.0.9.tar", last modified: Sun Jul 22 16:47:00 2018, max compression
```

## Comparing `pybotvac-0.0.8.tar` & `pybotvac-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxrwx   0        0        0        0 2018-07-14 16:13:40.000000 pybotvac-0.0.8/
--rw-rw-rw-   0        0        0     1100 2016-05-29 17:29:36.000000 pybotvac-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3852 2018-07-14 16:13:40.000000 pybotvac-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2018-07-14 16:13:40.000000 pybotvac-0.0.8/pybotvac/
--rw-rw-rw-   0        0        0     3863 2018-02-11 10:56:06.000000 pybotvac-0.0.8/pybotvac/account.py
-drwxrwxrwx   0        0        0        0 2018-07-14 16:13:40.000000 pybotvac-0.0.8/pybotvac/cert/
--rw-rw-rw-   0        0        0     1744 2016-05-18 19:58:56.000000 pybotvac-0.0.8/pybotvac/cert/neatocloud.com.crt
--rw-rw-rw-   0        0        0     6187 2018-06-23 13:18:07.000000 pybotvac-0.0.8/pybotvac/robot(Conflicted).py
--rw-rw-rw-   0        0        0     6279 2018-07-14 16:02:18.000000 pybotvac-0.0.8/pybotvac/robot.py
--rw-rw-rw-   0        0        0       81 2018-06-23 18:16:13.000000 pybotvac-0.0.8/pybotvac/__init__(Conflicted).py
--rw-rw-rw-   0        0        0       81 2018-07-14 16:02:18.000000 pybotvac-0.0.8/pybotvac/__init__.py
-drwxrwxrwx   0        0        0        0 2018-07-14 16:13:40.000000 pybotvac-0.0.8/pybotvac.egg-info/
--rw-rw-rw-   0        0        0        1 2018-07-14 16:13:39.000000 pybotvac-0.0.8/pybotvac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3852 2018-07-14 16:13:39.000000 pybotvac-0.0.8/pybotvac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3852 2018-06-23 18:19:13.000000 pybotvac-0.0.8/pybotvac.egg-info/PKG-INFO(Conflicted)
--rw-rw-rw-   0        0        0      288 2018-06-23 18:19:13.000000 pybotvac-0.0.8/pybotvac.egg-info/SOURCES(Conflicted 1).txt
--rw-rw-rw-   0        0        0      351 2018-06-23 18:19:13.000000 pybotvac-0.0.8/pybotvac.egg-info/SOURCES(Conflicted).txt
--rw-rw-rw-   0        0        0      434 2018-07-14 16:13:39.000000 pybotvac-0.0.8/pybotvac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2018-07-14 16:13:39.000000 pybotvac-0.0.8/pybotvac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2799 2018-06-23 18:04:17.000000 pybotvac-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2018-07-14 16:13:40.000000 pybotvac-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      692 2018-06-23 18:04:32.000000 pybotvac-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2018-07-22 16:47:00.000000 pybotvac-0.0.9/
+-rw-rw-rw-   0        0        0     1100 2016-05-29 17:29:36.000000 pybotvac-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3852 2018-07-22 16:47:00.000000 pybotvac-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac/
+-rw-rw-rw-   0        0        0     3929 2018-07-22 16:44:29.000000 pybotvac-0.0.9/pybotvac/account.py
+drwxrwxrwx   0        0        0        0 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac/cert/
+-rw-rw-rw-   0        0        0     1744 2016-05-18 19:58:56.000000 pybotvac-0.0.9/pybotvac/cert/neatocloud.com.crt
+-rw-rw-rw-   0        0        0     6436 2018-07-22 16:44:29.000000 pybotvac-0.0.9/pybotvac/robot.py
+-rw-rw-rw-   0        0        0       81 2018-07-22 16:44:29.000000 pybotvac-0.0.9/pybotvac/__init__.py
+drwxrwxrwx   0        0        0        0 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3852 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3852 2018-06-23 18:19:13.000000 pybotvac-0.0.9/pybotvac.egg-info/PKG-INFO(Conflicted)
+-rw-rw-rw-   0        0        0      288 2018-06-23 18:19:13.000000 pybotvac-0.0.9/pybotvac.egg-info/SOURCES(Conflicted 1).txt
+-rw-rw-rw-   0        0        0      351 2018-07-14 16:06:33.000000 pybotvac-0.0.9/pybotvac.egg-info/SOURCES(Conflicted).txt
+-rw-rw-rw-   0        0        0      371 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2018-07-22 16:47:00.000000 pybotvac-0.0.9/pybotvac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2799 2018-06-23 18:04:17.000000 pybotvac-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2018-07-22 16:47:00.000000 pybotvac-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      692 2018-06-23 18:04:32.000000 pybotvac-0.0.9/setup.py
```

### Comparing `pybotvac-0.0.8/LICENSE` & `pybotvac-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotvac-0.0.8/PKG-INFO` & `pybotvac-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotvac
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for controlling Neato pybotvac Connected vacuum robot
 Home-page: https://github.com/stianaske/pybotvac
 Author: Stian Askeland
 Author-email: stianaske@gmail.com
 License: Licensed under the MIT license. See LICENSE file for details
 Description: # pybotvac
```

### Comparing `pybotvac-0.0.8/pybotvac/account.py` & `pybotvac-0.0.9/pybotvac/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,16 @@
                             headers=self._headers)
         resp.raise_for_status()
 
         for robot in resp.json()['robots']:
             self._robots.add(Robot(name=robot['name'],
                                    serial=robot['serial'],
                                    secret=robot['secret_key'],
-                                   traits=robot['traits']))
+                                   traits=robot['traits'],
+                                   endpoint=robot['nucleo_url']))
 
     @staticmethod
     def get_map_image(url, dest_path=None):
         """
         Return a requested map from a robot.
 
         :return:
```

### Comparing `pybotvac-0.0.8/pybotvac/cert/neatocloud.com.crt` & `pybotvac-0.0.9/pybotvac/cert/neatocloud.com.crt`

 * *Files identical despite different names*

### Comparing `pybotvac-0.0.8/pybotvac/robot(Conflicted).py` & `pybotvac-0.0.9/pybotvac/robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import requests
 import hashlib
 import hmac
 import time
 import os.path
+import re
 
 # Disable warning due to SubjectAltNameWarning in certificate
 requests.packages.urllib3.disable_warnings()
 
 SUPPORTED_SERVICES = ['basic-1', 'minimal-2', 'basic-2', 'basic-3']
 
 
 class UnsupportedDevice(Exception):
     pass
 
 
 class Robot:
     """Data and methods for interacting with a Neato Botvac Connected vacuum robot"""
 
-    def __init__(self, serial, secret, traits, name=''):
+    def __init__(self, serial, secret, traits, name='',
+                 endpoint='https://nucleo.neatocloud.com:4443'):
         """
         Initialize robot
 
         :param serial: Robot serial
         :param secret: Robot secret
         :param name: Name of robot (optional)
         :param traits: Extras the robot supports
         """
         self.name = name
         self.serial = serial
         self.secret = secret
         self.traits = traits
 
-        self._url = 'https://nucleo.neatocloud.com/vendors/neato/robots/{0}/messages'.format(self.serial)
+        self._url = '{endpoint}/vendors/neato/robots/{serial}/messages'.format(
+            endpoint=re.sub(':\d+', '', endpoint),  # Remove port number
+            serial=self.serial)
         self._headers = {'Accept': 'application/vnd.neato.nucleo.v1'}
 
         if self.service_version not in SUPPORTED_SERVICES:
             raise UnsupportedDevice("Version " + self.service_version + " of service houseCleaning is not known")
 
     def __str__(self):
         return "Name: %s, Serial: %s, Secret: %s Traits: %s" % (self.name, self.serial, self.secret, self.traits)
@@ -121,14 +125,17 @@
         return self._message({'reqId': "1", 'cmd': "enableSchedule"})
 
     def disable_schedule(self):
         return self._message({'reqId': "1", 'cmd': "disableSchedule"})
 
     def get_schedule(self):
         return self._message({'reqId': "1", 'cmd': "getSchedule"})
+    
+    def locate(self):
+        return self._message({'reqId': "1", 'cmd': "findMe"})
 
     @property
     def schedule_enabled(self):
         return self.get_robot_state().json()['details']['isScheduleEnabled']
 
     @schedule_enabled.setter
     def schedule_enabled(self, enable):
```

### Comparing `pybotvac-0.0.8/pybotvac.egg-info/PKG-INFO` & `pybotvac-0.0.9/pybotvac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotvac
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for controlling Neato pybotvac Connected vacuum robot
 Home-page: https://github.com/stianaske/pybotvac
 Author: Stian Askeland
 Author-email: stianaske@gmail.com
 License: Licensed under the MIT license. See LICENSE file for details
 Description: # pybotvac
```

### Comparing `pybotvac-0.0.8/pybotvac.egg-info/PKG-INFO(Conflicted)` & `pybotvac-0.0.9/pybotvac.egg-info/PKG-INFO(Conflicted)`

 * *Files identical despite different names*

### Comparing `pybotvac-0.0.8/README.md` & `pybotvac-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pybotvac-0.0.8/setup.py` & `pybotvac-0.0.9/setup.py`

 * *Files identical despite different names*

