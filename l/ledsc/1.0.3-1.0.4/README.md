# Comparing `tmp/ledsc-1.0.3.tar.gz` & `tmp/ledsc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledsc-1.0.3.tar", last modified: Wed Apr 10 21:48:38 2024, max compression
+gzip compressed data, was "ledsc-1.0.4.tar", last modified: Wed Apr 10 22:13:37 2024, max compression
```

## Comparing `ledsc-1.0.3.tar` & `ledsc-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:48:38.757357 ledsc-1.0.3/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:48:38.757357 ledsc-1.0.3/PKG-INFO
--rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.3/README.md
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:48:38.753357 ledsc-1.0.3/ledsc/
--rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-04-10 21:45:20.000000 ledsc-1.0.3/ledsc/__init__.py
--rw-r--r--   0 hell      (1000) hell      (1000)     7487 2024-04-10 21:47:03.000000 ledsc-1.0.3/ledsc/ledsc.py
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:48:38.757357 ledsc-1.0.3/ledsc.egg-info/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/SOURCES.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/dependency_links.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/requires.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/top_level.txt
--rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 21:45:20.000000 ledsc-1.0.3/pyproject.toml
--rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-10 21:48:38.757357 ledsc-1.0.3/setup.cfg
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 22:13:37.608391 ledsc-1.0.4/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 22:13:37.604391 ledsc-1.0.4/PKG-INFO
+-rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.4/README.md
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 22:13:37.604391 ledsc-1.0.4/ledsc/
+-rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-04-10 22:09:45.000000 ledsc-1.0.4/ledsc/__init__.py
+-rw-r--r--   0 hell      (1000) hell      (1000)     7587 2024-04-10 22:11:55.000000 ledsc-1.0.4/ledsc/ledsc.py
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 22:13:37.604391 ledsc-1.0.4/ledsc.egg-info/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 22:13:37.000000 ledsc-1.0.4/ledsc.egg-info/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-10 22:13:37.000000 ledsc-1.0.4/ledsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-10 22:13:37.000000 ledsc-1.0.4/ledsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-10 22:13:37.000000 ledsc-1.0.4/ledsc.egg-info/requires.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-10 22:13:37.000000 ledsc-1.0.4/ledsc.egg-info/top_level.txt
+-rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 22:11:55.000000 ledsc-1.0.4/pyproject.toml
+-rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-10 22:13:37.608391 ledsc-1.0.4/setup.cfg
```

### Comparing `ledsc-1.0.3/PKG-INFO` & `ledsc-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ledsc-1.0.3/README.md` & `ledsc-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ledsc-1.0.3/ledsc/ledsc.py` & `ledsc-1.0.4/ledsc/ledsc.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,17 @@
         :param value: Transition time in seconds
         """
         self.write_register(REG.TRANSITION_PER.value, round(value*1000))
 
     def set_pwm_cycle(self, value: int):
         self.write_register(REG.PWM_CYCLE.value, value)
 
+    def set_px_counter(self, value: int):
+        self.write_register(REG.PX_COUNTER.value, value)
+
     def do_px_trigger(self):
         self.write_register(REG.PX_TRIGGER.value, 1)
 
     def do_reset(self):
         self.write_register(REG.RESET.value, 1)
 
     def get_transition_time(self) -> int:
```

### Comparing `ledsc-1.0.3/ledsc.egg-info/PKG-INFO` & `ledsc-1.0.4/ledsc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

