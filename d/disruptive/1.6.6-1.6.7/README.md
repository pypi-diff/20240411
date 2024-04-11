# Comparing `tmp/disruptive-1.6.6.tar.gz` & `tmp/disruptive-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disruptive-1.6.6.tar", last modified: Thu Feb 22 08:34:13 2024, max compression
+gzip compressed data, was "disruptive-1.6.7.tar", last modified: Thu Apr 11 09:03:13 2024, max compression
```

## Comparing `disruptive-1.6.6.tar` & `disruptive-1.6.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:13.158991 disruptive-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-22 08:34:02.000000 disruptive-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-02-22 08:34:13.158991 disruptive-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-22 08:34:02.000000 disruptive-1.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:13.154991 disruptive-1.6.6/disruptive/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:13.158991 disruptive-1.6.6/disruptive/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67942 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/events/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:13.158991 disruptive-1.6.6/disruptive/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/eventhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17641 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/resources/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-22 08:34:02.000000 disruptive-1.6.6/disruptive/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 08:34:13.158991 disruptive-1.6.6/disruptive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-02-22 08:34:13.000000 disruptive-1.6.6/disruptive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-22 08:34:13.000000 disruptive-1.6.6/disruptive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 08:34:13.000000 disruptive-1.6.6/disruptive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-22 08:34:13.000000 disruptive-1.6.6/disruptive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 08:34:13.000000 disruptive-1.6.6/disruptive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 08:34:02.000000 disruptive-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-22 08:34:13.158991 disruptive-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-22 08:34:02.000000 disruptive-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-11 09:03:02.000000 disruptive-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-11 09:03:13.544314 disruptive-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-11 09:03:02.000000 disruptive-1.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.540314 disruptive-1.6.7/disruptive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/disruptive/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68441 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/disruptive/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/eventhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17641 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/resources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-11 09:03:02.000000 disruptive-1.6.7/disruptive/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:13.544314 disruptive-1.6.7/disruptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 09:03:13.000000 disruptive-1.6.7/disruptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 09:03:02.000000 disruptive-1.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-11 09:03:13.544314 disruptive-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 09:03:02.000000 disruptive-1.6.7/setup.py
```

### Comparing `disruptive-1.6.6/LICENSE` & `disruptive-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/PKG-INFO` & `disruptive-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.6.6
+Version: 1.6.7
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
```

### Comparing `disruptive-1.6.6/README.md` & `disruptive-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/__init__.py` & `disruptive-1.6.7/disruptive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Metadata
-__version__ = '1.6.6'
+__version__ = '1.6.7'
 
 # If set, logs of chosen level and higher are printed to console.
 # Default value None results in no logs at any level.
 log_level = None
 
 # REST API base URLs of which all endpoints are an expansion.
 base_url = 'https://api.disruptive-technologies.com/v2'
```

### Comparing `disruptive-1.6.6/disruptive/authentication.py` & `disruptive-1.6.7/disruptive/authentication.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/errors.py` & `disruptive-1.6.7/disruptive/errors.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/events/__init__.py` & `disruptive-1.6.7/disruptive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/events/events.py` & `disruptive-1.6.7/disruptive/events/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,60 +231,68 @@
     ----------
     celsius : float
         Temperature value in Celsius.
     fahrenheit : float
         Temperature value in Fahrenheit.
     samples : list[TemperatureSample]
         Temperature values sampled over a single heartbeat.
+    is_backfilled : bool
+        Indicates if the temperature event is backfilled.
     timestamp : datetime
         Timestamp of when the event was received by a Cloud Connector.
 
     """
 
     def __init__(self,
                  celsius: float,
                  samples: Optional[list] = None,
+                 is_backfilled: Optional[bool] = None,
                  timestamp: Optional[datetime | str] = None,
                  ) -> None:
         """
         Constructs the Temperature object. The `fahrenheit` attribute is
         calculated from the provided `celsius` parameter.
 
         Parameters
         ----------
         celsius : float
             Temperature value in Celsius.
         samples : list[TemperatureSample]
             Temperature values sampled over a single heartbeat.
+        is_backfilled : bool
+            Indicates if the temperature event is backfilled.
         timestamp : datetime, str, optional
             Timestamp in either datetime or string iso8601 format
             (i.e. yyyy-MM-ddTHH:mm:ssZ).
 
         """
 
         # Set parameter attributes.
         self.celsius: float = celsius
         self.samples: Optional[list] = samples
         self.fahrenheit: float = dttrans._celsius_to_fahrenheit(celsius)
+        self.is_backfilled: Optional[bool] = is_backfilled
         self.timestamp: Optional[datetime | str] = timestamp
 
         # Inherit parent _EventData class init with repacked data dictionary.
         _EventData.__init__(self, self.__repack(), 'temperature')
 
     def __repr__(self) -> str:
         string = '{}.{}('\
             'celsius={}, '\
             'samples={}, '\
+            'is_backfilled={}, '\
             'timestamp={}'\
             ')'
         return string.format(
             self.__class__.__module__,
             self.__class__.__name__,
             self.celsius,
             self.samples,
+            self.is_backfilled,
             repr(dttrans.to_iso8601(self.timestamp)),
         )
 
     @classmethod
     def _from_raw(cls, data: dict) -> Temperature:
         """
         Constructs a Temperature object from API response data.
@@ -309,28 +317,31 @@
                 timestamp=sample['sampleTime'],
             ))
 
         # Construct the object with unpacked parameters.
         obj = cls(
             celsius=data['value'],
             samples=sample_objs,
+            is_backfilled=data['isBackfilled'],
             timestamp=data['updateTime'],
         )
 
         # Re-inherit from parent, but now providing response data.
         _EventData.__init__(obj, data, obj.event_type)
 
         return obj
 
     def __repack(self) -> dict:
         data: dict = dict()
         if self.celsius is not None:
             data['value'] = self.celsius
         if self.samples is not None:
             data['samples'] = [s._raw for s in self.samples]
+        if self.is_backfilled is not None:
+            data['isBackfilled'] = self.is_backfilled
         if self.timestamp is not None:
             data['updateTime'] = self.timestamp
         return data
 
 
 class TemperatureSample(dtoutputs.OutputBase):
     """
```

### Comparing `disruptive-1.6.6/disruptive/logging.py` & `disruptive-1.6.7/disruptive/logging.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/outputs.py` & `disruptive-1.6.7/disruptive/outputs.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/requests.py` & `disruptive-1.6.7/disruptive/requests.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/claim.py` & `disruptive-1.6.7/disruptive/resources/claim.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/data_connector.py` & `disruptive-1.6.7/disruptive/resources/data_connector.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/device.py` & `disruptive-1.6.7/disruptive/resources/device.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/emulator.py` & `disruptive-1.6.7/disruptive/resources/emulator.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/eventhistory.py` & `disruptive-1.6.7/disruptive/resources/eventhistory.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/organization.py` & `disruptive-1.6.7/disruptive/resources/organization.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/project.py` & `disruptive-1.6.7/disruptive/resources/project.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/role.py` & `disruptive-1.6.7/disruptive/resources/role.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/service_account.py` & `disruptive-1.6.7/disruptive/resources/service_account.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/resources/stream.py` & `disruptive-1.6.7/disruptive/resources/stream.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive/transforms.py` & `disruptive-1.6.7/disruptive/transforms.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/disruptive.egg-info/PKG-INFO` & `disruptive-1.6.7/disruptive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.6.6
+Version: 1.6.7
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
```

### Comparing `disruptive-1.6.6/disruptive.egg-info/SOURCES.txt` & `disruptive-1.6.7/disruptive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disruptive-1.6.6/setup.cfg` & `disruptive-1.6.7/setup.cfg`

 * *Files identical despite different names*

