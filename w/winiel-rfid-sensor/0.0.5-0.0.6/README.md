# Comparing `tmp/winiel-rfid-sensor-0.0.5.tar.gz` & `tmp/winiel-rfid-sensor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winiel-rfid-sensor-0.0.5.tar", last modified: Tue Apr  9 05:13:37 2024, max compression
+gzip compressed data, was "winiel-rfid-sensor-0.0.6.tar", last modified: Thu Apr 11 07:06:41 2024, max compression
```

## Comparing `winiel-rfid-sensor-0.0.5.tar` & `winiel-rfid-sensor-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-09 05:13:37.119896 winiel-rfid-sensor-0.0.5/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-09 05:13:37.119468 winiel-rfid-sensor-0.0.5/PKG-INFO
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       38 2024-04-09 05:13:37.119988 winiel-rfid-sensor-0.0.5/setup.cfg
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      687 2024-04-09 05:11:55.000000 winiel-rfid-sensor-0.0.5/setup.py
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-09 05:13:37.115997 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       22 2024-04-09 05:11:55.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/__init__.py
--rw-r--r--   0 yongjinsohn   (501) staff       (20)     4567 2024-04-09 05:10:17.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/rfid_sensor.py
-drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-09 05:13:37.118984 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/PKG-INFO
--rw-r--r--   0 yongjinsohn   (501) staff       (20)      323 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 04:23:22.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/not-zip-safe
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       15 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/requires.txt
--rw-r--r--   0 yongjinsohn   (501) staff       (20)       19 2024-04-09 05:13:37.000000 winiel-rfid-sensor-0.0.5/winiel_rfid_sensor.egg-info/top_level.txt
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-11 07:06:41.994812 winiel-rfid-sensor-0.0.6/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-11 07:06:41.994373 winiel-rfid-sensor-0.0.6/PKG-INFO
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       38 2024-04-11 07:06:41.994918 winiel-rfid-sensor-0.0.6/setup.cfg
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      760 2024-04-11 07:04:14.000000 winiel-rfid-sensor-0.0.6/setup.py
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-11 07:06:41.990852 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       22 2024-04-11 07:04:14.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/__init__.py
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)     4620 2024-04-11 07:00:38.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/rfid_sensor.py
+drwxr-xr-x   0 yongjinsohn   (501) staff       (20)        0 2024-04-11 07:06:41.993875 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      501 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)      323 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)        1 2024-03-29 04:23:22.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/not-zip-safe
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       15 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/requires.txt
+-rw-r--r--   0 yongjinsohn   (501) staff       (20)       19 2024-04-11 07:06:41.000000 winiel-rfid-sensor-0.0.6/winiel_rfid_sensor.egg-info/top_level.txt
```

### Comparing `winiel-rfid-sensor-0.0.5/setup.py` & `winiel-rfid-sensor-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
 
+import winiel_rfid_sensor
+
 setup(
     name='winiel-rfid-sensor',
-    version='0.0.5',
+    version=winiel_rfid_sensor.__version__,
+    # version='0.0.6',
     description='PYPI tutorial package creation written by winiel',
     author='winiel',
     author_email='winiel@naver.com ',
     url='https://github.com/winiel',
     install_requires=['pyserial', 'pyusb'],
     packages=find_packages(exclude=[]),
     keywords=['winiel', 'rfid', 'sensor'],
```

### Comparing `winiel-rfid-sensor-0.0.5/winiel_rfid_sensor/rfid_sensor.py` & `winiel-rfid-sensor-0.0.6/winiel_rfid_sensor/rfid_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
             if len(data_by_id.items()) > 0:
                 # 거리 추정 결과
                 self.results = self.estimate_distance(data_by_id)
 
                 # 결과 출력
                 # for sensor_id, (occurrence, std_dev, distance) in results.items():
                 #     print(f"Sensor ID: {sensor_id}, Occurrence: {occurrence}, RSSI Std Dev: {std_dev:.2f}, Estimated Distance: {distance:.2f} meters")
+            else :
+                self.results = {}
         except Exception as e:
             print(e)
             self.sensorClose()
 
 
     def estimate_distance(self, data, rssi_at_1m=180, path_loss_exponent=3):
         """
```

