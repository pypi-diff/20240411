# Comparing `tmp/cdk-events-notify-2.2.92.tar.gz` & `tmp/cdk-events-notify-2.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-events-notify-2.2.92.tar", last modified: Tue Apr  9 00:13:09 2024, max compression
+gzip compressed data, was "cdk-events-notify-2.2.93.tar", last modified: Wed Apr 10 00:11:34 2024, max compression
```

## Comparing `cdk-events-notify-2.2.92.tar` & `cdk-events-notify-2.2.93.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.727883 cdk-events-notify-2.2.92/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.727883 cdk-events-notify-2.2.92/src/cdk_events_notify/
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.731883 cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.92.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:12:49.000000 cdk-events-notify-2.2.92/src/cdk_events_notify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.727883 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 00:13:09.000000 cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:11:34.624983 cdk-events-notify-2.2.93/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-10 00:11:34.624983 cdk-events-notify-2.2.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:11:34.624983 cdk-events-notify-2.2.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:11:34.620983 cdk-events-notify-2.2.93/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:11:34.624983 cdk-events-notify-2.2.93/src/cdk_events_notify/
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/src/cdk_events_notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:11:34.624983 cdk-events-notify-2.2.93/src/cdk_events_notify/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/src/cdk_events_notify/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.93.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:11:23.000000 cdk-events-notify-2.2.93/src/cdk_events_notify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:11:34.624983 cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-10 00:11:34.000000 cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-10 00:11:34.000000 cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:11:34.000000 cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 00:11:34.000000 cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 00:11:34.000000 cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/top_level.txt
```

### Comparing `cdk-events-notify-2.2.92/LICENSE` & `cdk-events-notify-2.2.93/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.92/PKG-INFO` & `cdk-events-notify-2.2.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.92
+Version: 2.2.93
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-events-notify-2.2.92/README.md` & `cdk-events-notify-2.2.93/README.md`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.92/setup.py` & `cdk-events-notify-2.2.93/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-events-notify",
-    "version": "2.2.92",
+    "version": "2.2.93",
     "description": "The Events Notify AWS Construct lib for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-events-notify.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_events_notify",
         "cdk_events_notify._jsii"
     ],
     "package_data": {
         "cdk_events_notify._jsii": [
-            "cdk-events-notify@2.2.92.jsii.tgz"
+            "cdk-events-notify@2.2.93.jsii.tgz"
         ],
         "cdk_events_notify": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-events-notify-2.2.92/src/cdk_events_notify/__init__.py` & `cdk-events-notify-2.2.93/src/cdk_events_notify/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.92/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.92.jsii.tgz` & `cdk-events-notify-2.2.93/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.93.jsii.tgz`

 * *Files 3% similar despite different names*

#### Comparing `cdk-events-notify@2.2.92.jsii.tgz-content` & `cdk-events-notify@2.2.93.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'7uJCddpno4t5W2FbSxOaiXYzPxfT9nn8bZrcy6k5tUc='", "'version'": "'2.2.93'"}*

```diff
@@ -3657,15 +3657,15 @@
             }
         }
     },
     "description": "The Events Notify AWS Construct lib for AWS CDK",
     "docs": {
         "stability": "experimental"
     },
-    "fingerprint": "7wKoNc2KuZG6rIE5Rt989eZ2UDmrb57O56p80rM7wF4=",
+    "fingerprint": "7uJCddpno4t5W2FbSxOaiXYzPxfT9nn8bZrcy6k5tUc=",
     "homepage": "https://github.com/neilkuan/cdk-events-notify.git",
     "jsiiVersion": "5.3.34 (build f4c2317)",
     "keywords": [
         "aws",
         "cdk",
         "events",
         "notify"
@@ -3844,9 +3844,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/index:ISlackEventNotify"
         }
     },
-    "version": "2.2.92"
+    "version": "2.2.93"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -44,10 +44,10 @@
         });
     }
 }
 exports.EventNotify = EventNotify;
 _a = JSII_RTTI_SYMBOL_1;
 EventNotify[_a] = {
     fqn: "cdk-events-notify.EventNotify",
-    version: "2.2.92"
+    version: "2.2.93"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSw2QkFBNkI7QUFDN0IsbUNBQW1DO0FBQ25DLGlEQUFpRDtBQUNqRCx5REFBeUQ7QUFDekQsaURBQWlEO0FBQ2pELDZDQUE2QztBQUM3QywyQ0FBdUM7QUFtQ3ZDOztHQUVHO0FBQ0gsTUFBYSxXQUFZLFNBQVEsc0JBQVM7SUFDeEMsWUFBWSxLQUFnQixFQUFFLEVBQVUsRUFBRSxLQUF3QjtRQUNoRSxLQUFLLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBRWpCLElBQUksQ0FBQyxLQUFLLEVBQUUsZUFBZSxJQUFJLENBQUMsS0FBSyxFQUFFLEtBQUssRUFBRSxDQUFDO1lBQzdDLE1BQU0sSUFBSSxLQUFLLENBQUMsK0NBQStDLENBQUMsQ0FBQztRQUNuRSxDQUFDO1FBRUQsTUFBTSxTQUFTLEdBQUcsSUFBSSxNQUFNLENBQUMsUUFBUSxDQUFDLElBQUksRUFBRSxZQUFZLEVBQUU7WUFDeEQsT0FBTyxFQUFFLDJCQUEyQjtZQUNwQyxJQUFJLEVBQUUsTUFBTSxDQUFDLElBQUksQ0FBQyxTQUFTLENBQUMsSUFBSSxDQUFDLElBQUksQ0FBQyxTQUFTLEVBQUUsYUFBYSxDQUFDLENBQUU7WUFDakUsT0FBTyxFQUFFLE1BQU0sQ0FBQyxPQUFPLENBQUMsV0FBVztZQUNuQyxPQUFPLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxPQUFPLENBQUMsQ0FBQyxDQUFDO1lBQ2hDLFlBQVksRUFBRSxJQUFJLENBQUMsYUFBYSxDQUFDLFVBQVU7WUFDM0MsV0FBVyxFQUFFO2dCQUNYLGlCQUFpQixFQUFFLEtBQUssRUFBRSxlQUFlLENBQUMsQ0FBQyxDQUFDLEtBQUssRUFBRSxlQUFlLENBQUMsQ0FBQyxDQUFDLE1BQU07Z0JBQzNFLGlCQUFpQixFQUFFLEtBQUssRUFBRSxLQUFLLEVBQUUsZUFBZSxDQUFDLENBQUMsQ0FBQyxLQUFLLEVBQUUsS0FBSyxFQUFFLGVBQWUsQ0FBQyxDQUFDLENBQUMsTUFBTTtnQkFDekYsa0JBQWtCLEVBQUUsS0FBSyxFQUFFLEtBQUssRUFBRSxnQkFBZ0IsQ0FBQyxDQUFDLENBQUMsS0FBSyxFQUFFLEtBQUssRUFBRSxnQkFBZ0IsQ0FBQyxDQUFDLENBQUMsTUFBTTthQUM3RjtTQUNGLENBQUMsQ0FBQztRQUVILE1BQU0saUJBQWlCLEdBQUcsSUFBSSxNQUFNLENBQUMsY0FBYyxDQUFDLFNBQVMsQ0FBQyxDQUFDO1FBQy9ELElBQUksTUFBTSxDQUFDLElBQUksQ0FBQyxJQUFJLEVBQUUsMkJBQTJCLEVBQUU7WUFDakQsUUFBUSxFQUFFLDJCQUEyQjtZQUNyQyxXQUFXLEVBQUUsa0NBQWtDO1lBQy9DLE9BQU8sRUFBRSxDQUFDLGlCQUFpQixDQUFDO1lBQzVCLFlBQVksRUFBRTtnQkFDWixVQUFVLEVBQUUsQ0FBQyxvQ0FBb0MsQ0FBQzthQUNuRDtTQUNGLENBQUMsQ0FBQztJQUNMLENBQUM7O0FBOUJILGtDQStCQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCAqIGFzIHBhdGggZnJvbSAncGF0aCc7XG5pbXBvcnQgKiBhcyBjZGsgZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0ICogYXMgZXZlbnRzIGZyb20gJ2F3cy1jZGstbGliL2F3cy1ldmVudHMnO1xuaW1wb3J0ICogYXMgdGFyZ2V0IGZyb20gJ2F3cy1jZGstbGliL2F3cy1ldmVudHMtdGFyZ2V0cyc7XG5pbXBvcnQgKiBhcyBsYW1iZGEgZnJvbSAnYXdzLWNkay1saWIvYXdzLWxhbWJkYSc7XG5pbXBvcnQgKiBhcyBsb2dzIGZyb20gJ2F3cy1jZGstbGliL2F3cy1sb2dzJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuLyoqXG4gKiBzbGFjayBldmVudCBub3RpZnkgaW50ZXJmYWNlLlxuICovXG5leHBvcnQgaW50ZXJmYWNlIElTbGFja0V2ZW50Tm90aWZ5IHtcbiAgLyoqXG4gICAqIHNsYWNrIFdlYmhvb2sgVXJsIGZvciBMYW1iZGEgc2VuZCBtZXNzYWdlIHRvIHNsYWNrLlxuICAgKi9cbiAgcmVhZG9ubHkgc2xhY2tXZWJob29rVXJsOiBzdHJpbmc7XG4gIC8qKlxuICAgKiBzbGFjayBDaGFubmVsIE5hbWUgZm9yIExhbWJkYSBzZW5kIG1lc3NhZ2UgdG8gc2xhY2suXG4gICAqL1xuICByZWFkb25seSBzbGFja0NoYW5uZWxOYW1lOiBzdHJpbmc7XG5cbn1cblxuLyoqXG4gKiBldmVudCBub3RpZnkgaW50ZXJmYWNlLlxuICovXG5leHBvcnQgaW50ZXJmYWNlIEV2ZW50Tm90aWZ5UHJvcHMge1xuICAvKipcbiAgICogTGluZSBOb3RpZnkgVG9rZW4gZm9yIExhbWJkYSBzZW5kIG5vdGlmeSBwZXJtaXNzaW9uLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIG5vbmVcbiAgICovXG4gIHJlYWRvbmx5IGxpbmVOb3RpZnlUb2tlbj86IHN0cmluZyB8IHVuZGVmaW5lZDtcblxuICAvKipcbiAgICogTm90aWZ5IHRhcmdldCB0byBTbGFjayBjaGFubmVsLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIG5vbmVcbiAgICovXG4gIHJlYWRvbmx5IHNsYWNrPzogSVNsYWNrRXZlbnROb3RpZnk7XG59XG5cbi8qKlxuICogRXZlbnQgTm90Zml5IENvbnN0cnVjdCBDbGFzcy5cbiAqL1xuZXhwb3J0IGNsYXNzIEV2ZW50Tm90aWZ5IGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM/OiBFdmVudE5vdGlmeVByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkKTtcblxuICAgIGlmICghcHJvcHM/LmxpbmVOb3RpZnlUb2tlbiAmJiAhcHJvcHM/LnNsYWNrKSB7XG4gICAgICB0aHJvdyBuZXcgRXJyb3IoJ1BsZWFzZSBpbnB1dCBsaW5lTm90aWZ5VG9rZW4gb3Igc2xhY2sgb3B0aW9ucycpO1xuICAgIH1cblxuICAgIGNvbnN0IGxhbWJkYUZ1biA9IG5ldyBsYW1iZGEuRnVuY3Rpb24odGhpcywgJ2xhbWJkYV9mdW4nLCB7XG4gICAgICBoYW5kbGVyOiAnbGluZW5vdGlmeS5sYW1iZGFfaGFuZGxlcicsXG4gICAgICBjb2RlOiBsYW1iZGEuQ29kZS5mcm9tQXNzZXQocGF0aC5qb2luKF9fZGlybmFtZSwgJy4uL2Z1bmN0aW9uJykgKSxcbiAgICAgIHJ1bnRpbWU6IGxhbWJkYS5SdW50aW1lLlBZVEhPTl8zXzEyLFxuICAgICAgdGltZW91dDogY2RrLkR1cmF0aW9uLm1pbnV0ZXMoMyksXG4gICAgICBsb2dSZXRlbnRpb246IGxvZ3MuUmV0ZW50aW9uRGF5cy5USFJFRV9EQVlTLFxuICAgICAgZW52aXJvbm1lbnQ6IHtcbiAgICAgICAgTElORV9OT1RJRllfVE9LRU46IHByb3BzPy5saW5lTm90aWZ5VG9rZW4gPyBwcm9wcz8ubGluZU5vdGlmeVRva2VuIDogJ25vbmUnLFxuICAgICAgICBTTEFDS19XRUJIT09LX1VSTDogcHJvcHM/LnNsYWNrPy5zbGFja1dlYmhvb2tVcmwgPyBwcm9wcz8uc2xhY2s/LnNsYWNrV2ViaG9va1VybCA6ICdub25lJyxcbiAgICAgICAgU0xBQ0tfQ0hBTk5FTF9OQU1FOiBwcm9wcz8uc2xhY2s/LnNsYWNrQ2hhbm5lbE5hbWUgPyBwcm9wcz8uc2xhY2s/LnNsYWNrQ2hhbm5lbE5hbWUgOiAnbm9uZScsXG4gICAgICB9LFxuICAgIH0pO1xuXG4gICAgY29uc3QgZXZlbnROb3RpZnlUYXJnZXQgPSBuZXcgdGFyZ2V0LkxhbWJkYUZ1bmN0aW9uKGxhbWJkYUZ1bik7XG4gICAgbmV3IGV2ZW50cy5SdWxlKHRoaXMsICdFdmVudEJ1c0NvbnNvbGVMb2dpbkV2ZW50Jywge1xuICAgICAgcnVsZU5hbWU6ICdFdmVudEJ1c0NvbnNvbGVMb2dpbkV2ZW50JyxcbiAgICAgIGRlc2NyaXB0aW9uOiAnQ29uc29sZSBsb2dpbiBpbiBzcGVjaWZpYyByZWdpb24nLFxuICAgICAgdGFyZ2V0czogW2V2ZW50Tm90aWZ5VGFyZ2V0XSxcbiAgICAgIGV2ZW50UGF0dGVybjoge1xuICAgICAgICBkZXRhaWxUeXBlOiBbJ0FXUyBDb25zb2xlIFNpZ24gSW4gdmlhIENsb3VkVHJhaWwnXSxcbiAgICAgIH0sXG4gICAgfSk7XG4gIH1cbn0iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'2.2.93'"}*

```diff
@@ -129,9 +129,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "2.2.92"
+    "version": "2.2.93"
 }
```

### Comparing `cdk-events-notify-2.2.92/src/cdk_events_notify.egg-info/PKG-INFO` & `cdk-events-notify-2.2.93/src/cdk_events_notify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.92
+Version: 2.2.93
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

