# Comparing `tmp/robotframework-testsuitesmanagement-0.7.6.tar.gz` & `tmp/robotframework-testsuitesmanagement-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-testsuitesmanagement-0.7.6.tar", last modified: Tue Apr  9 15:47:54 2024, max compression
+gzip compressed data, was "robotframework-testsuitesmanagement-0.7.7.tar", last modified: Thu Apr 11 15:49:00 2024, max compression
```

## Comparing `robotframework-testsuitesmanagement-0.7.6.tar` & `robotframework-testsuitesmanagement-0.7.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/CConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/configuration_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/CStruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/LibListener.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.651656 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.651656 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/
+-rw-r--r--   0 runner    (1001) docker     (127)    33982 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/CConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/configuration_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/CStruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/LibListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-11 15:49:00.000000 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-11 15:49:00.000000 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:49:00.000000 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 15:49:00.000000 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 15:49:00.000000 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 15:49:00.000000 robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:49:00.655655 robotframework-testsuitesmanagement-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-04-11 15:46:57.000000 robotframework-testsuitesmanagement-0.7.7/setup.py
```

### Comparing `robotframework-testsuitesmanagement-0.7.6/LICENSE` & `robotframework-testsuitesmanagement-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/PKG-INFO` & `robotframework-testsuitesmanagement-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-testsuitesmanagement
-Version: 0.7.6
+Version: 0.7.7
 Summary: Functionality to manage RobotFramework testsuites
 Home-page: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-testsuitesmanagement-0.7.6/README.rst` & `robotframework-testsuitesmanagement-0.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/CConfig.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/CConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,17 +324,17 @@
             ROBFW_AIO_Data.update({key:v})
         oJsonPreprocessor = CJsonPreprocessor(syntax="python", currentCfg=ROBFW_AIO_Data)
         try:
             oJsonCfgData = oJsonPreprocessor.jsonLoad(self.sTestCfgFile)
         except Exception as error:
             CConfig.bLoadedCfg = False
             CConfig.sLoadedCfgError = ''
-            for item in str(error).split(': \''):
-                CConfig.sLoadedCfgError += f"{item}\n                  "
-            logger.error(f"Loading of JSON configuration file failed! Reason: {CConfig.sLoadedCfgError}")
+            for line in str(error).splitlines():
+                logger.error(f"{line}") # outcome: every single line starts with timestamp and log level
+                CConfig.sLoadedCfgError += f"{line}\n                  " # to be compatible with original version
             BuiltIn().unknown('Loading of JSON configuration file failed!')
             raise Exception
 
         self.sLocalConfig = CString.NormalizePath(self.sLocalConfig)
         if self.sLocalConfig != '':
             try:
                 oLocalConfig = oJsonPreprocessor.jsonLoad(self.sLocalConfig)
@@ -530,17 +530,18 @@
         '''
         oJsonPreprocessor = CJsonPreprocessor(syntax="python")
         try:
             oSuiteConfig = oJsonPreprocessor.jsonLoad(CString.NormalizePath(self.sTestSuiteCfg))
         except Exception as error:
             CConfig.bLoadedCfg = False
             CConfig.sLoadedCfgError = ''
-            for item in str(error).split(': \''):
-                CConfig.sLoadedCfgError += f"'{item}', "
-            logger.error(f"Loading of JSON configuration file failed! Reason: {CConfig.sLoadedCfgError}")
+            for line in str(error).splitlines():
+                logger.error(f"{line}") # outcome: every single line starts with timestamp and log level
+                CConfig.sLoadedCfgError += f"{line}\n                  " # to be compatible with original version / but when the error is already logged, for what do we need to store the error message in sLoadedCfgError?
+            logger.error('Loading of JSON configuration file failed!')
             return False
         sListOfVariants = ''
         for item in list(oSuiteConfig.keys()):
             sListOfVariants = sListOfVariants + f"'{item}', "
         if not re.match(r'^[a-zA-Z0-9.\u0080-\U0010FFFF\_\-\:@\$]+$', self.sConfigName):
             CConfig.sLoadedCfgError = f"Testsuite management - Loading configuration level 2 failed! The variant name '{self.sConfigName}' \
 is invalid. Please find the suitable variant in this list: {sListOfVariants}"
```

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/__init__.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/configuration_schema.json` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/configuration_schema.json`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/CSetup.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/CSetup.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/__init__.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/CStruct.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/CStruct.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/Event.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/Event.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/LibListener.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/LibListener.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/__init__.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/__init__.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/version.py` & `robotframework-testsuitesmanagement-0.7.7/RobotFramework_TestsuitesManagement/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of package RobotFramework_TestsuitesManagement
 #
-VERSION      = "0.7.6"
-VERSION_DATE = "01.04.2024"
+VERSION      = "0.7.7"
+VERSION_DATE = "10.04.2024"
```

### Comparing `robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/PKG-INFO` & `robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-testsuitesmanagement
-Version: 0.7.6
+Version: 0.7.7
 Summary: Functionality to manage RobotFramework testsuites
 Home-page: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/SOURCES.txt` & `robotframework-testsuitesmanagement-0.7.7/robotframework_testsuitesmanagement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.6/setup.py` & `robotframework-testsuitesmanagement-0.7.7/setup.py`

 * *Files identical despite different names*

