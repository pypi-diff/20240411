# Comparing `tmp/posttestresultstopractitest-0.0.5.tar.gz` & `tmp/posttestresultstopractitest-0.0.6.tar.gz`

## Comparing `posttestresultstopractitest-0.0.5.tar` & `posttestresultstopractitest-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/userInputs.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/__init__.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/ClonePTTestSet.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/Constants.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/EnumClass.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetConfigValues.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTInstance.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTProjectId.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTTest.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTTestSetId.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/Orchestrator.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/PT_APIRequest.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/PostTestResults.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/tests/mainEntrance.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/LICENSE
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/README.md
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/userInputs.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/ClonePTTestSet.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/Constants.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/CreatePTInstance.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/CreatePTTestSet.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/EnumClass.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetConfigValues.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetPTInstance.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetPTProjectId.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetPTTest.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetPTTestSetId.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/Orchestrator.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/PT_APIRequest.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/PostTestResults.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/tests/mainEntrance.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 posttestresultstopractitest-0.0.6/PKG-INFO
```

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/ClonePTTestSet.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/ClonePTTestSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
         data = responseData['data']
    
         newTestSetId = data['id']
         print ("TestSetName:", GetConfigValues.PTTestsetName_New, "-->New test set id: " + newTestSetId)
         return newTestSetId
     else:
-        raise Exception ("Call to clone test set was unsucessful with status code", res.status_code)
+        raise Exception ("Call to clone test set was unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetConfigValues.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetConfigValues.py`

 * *Files identical despite different names*

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTInstance.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/CreatePTInstance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import json
 from src.PostTestResultsToPractiTest import PT_APIRequest
 from src.PostTestResultsToPractiTest import GetConfigValues
 from src.PostTestResultsToPractiTest import GetPTProjectId
 from src.PostTestResultsToPractiTest import Constants
+from src.PostTestResultsToPractiTest import GetPTInstance
 
-def RetrieveInstanceId(filterByTestSetId, filterByTestId):
+def CreatePTInstance(testSetId: int, testId: int) -> int:
+    """Create PractiTest instance given a test set id and test id.
+
+    :param testSetId: PractiTest id for target test set.
+    :param testId: PractiTest id for test to create instance from.
+    :return: PractiTest id for created instance.
+    """
     GetConfigValues.GetConfigValues()
     projectId = GetPTProjectId.RetrieveProjectId()
+
+    if instanceId := GetPTInstance.RetrieveInstanceId(testSetId, testId):
+        return instanceId
     
-    res = PT_APIRequest.getRequest(Constants.PT_API_BASEURL+ "/projects/" + projectId + "/instances.json?set-ids=" + filterByTestSetId)
+    jsonData = json.dumps({"data":{"type":"instances","attributes":{"test-id":testId, "set-id": testSetId}}})
+    
+    res = PT_APIRequest.sendRequest(Constants.PT_API_BASEURL + "/projects/" + projectId +"/instances.json", "post", jsonData)
 
     if res.status_code == 200:
-        allInstances = json.loads(res.content)
-        allInstancesData = allInstances['data']
-        myInstanceData = list(filter(lambda myData:myData['attributes']['test-id']==int(filterByTestId), allInstancesData))   
-        #print ("testData:", myInstanceData)
-               
-        if len(myInstanceData) != 0:
-            myInstanceId = myInstanceData[0]['id']
-            print ("Instance id:", myInstanceId)
-            return myInstanceId
-        else:
-            raise Exception ("No associated instance is found in PT that has the key of 'test-id'= " + filterByTestId)
+        responseData = json.loads(res.content)
+
+        data = responseData['data']
+   
+        newInstanceId = data['id']
+        return newInstanceId
     else:
-        raise Exception ("Call to get a list of instances is unsucessful with status code", res.status_code)
+        raise Exception ("Call to create instance was unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTProjectId.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetPTProjectId.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
         
         if len(myProjectData) != 0:
             myProjectId = myProjectData[0]['id']
             return myProjectId
         else:   
             raise Exception("No matching project id of " + GetConfigValues.PTProjectName + " is found")          
     else:
-        raise Exception("Call to get project id was unsucessful with status code", res.status_code)
+        raise Exception("Call to get project id was unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTTest.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/GetPTTest.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,10 +18,30 @@
         if len(myTestData) != 0:
             myTestId = myTestData[0]['id']
             print ("Test id:", myTestId)
             return myTestId
         else:
             raise Exception ("No associated test is found in PT that has the key of 'Automation Name = '" + filterByAutomationName)
     else:
-        raise Exception ("Call to get a list of tests is unsucessful with status code", res.status_code)
+        raise Exception ("Call to get a list of tests is unsuccessful with status code", res.status_code)
 
-#retrieveProjectId()
+def RetrieveTestIdByName(testName: str) -> int:
+    """Retrieve PractiTest test id provided the test name.
+
+    :param testName: Name of test.
+    :return: PractiTest test id.
+    """
+    projectId = GetPTProjectId.RetrieveProjectId()
+    res = PT_APIRequest.getRequest(Constants.PT_API_BASEURL + "/projects/" + projectId + "/tests.json?name_exact=" + testName)
+
+    if res.status_code == 200:
+        allTests = json.loads(res.content)
+        testsData = allTests["data"]
+        desiredTestData = list(filter(lambda desiredData:desiredData['attributes']['name']==testName, testsData))
+
+        if len(desiredTestData) != 0:
+            testId = desiredTestData[0]['id']
+            return testId
+        else:
+            raise Exception ("No associated test is found in PT that has the key of 'Test Name = '" + testName)
+    else:
+        raise Exception ("Call to get a list of tests is unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/GetPTTestSetId.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/CreatePTTestSet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import json
 from src.PostTestResultsToPractiTest import PT_APIRequest
 from src.PostTestResultsToPractiTest import GetConfigValues
 from src.PostTestResultsToPractiTest import GetPTProjectId
 from src.PostTestResultsToPractiTest import Constants
 
-def RetrieveTestSetId(testSetName):
+def CreatePTTestSet(featureFileName: str, releaseVersion: str = None, customFields: dict = None) -> int:
+    """Create a PractiTest test set provided a feature file name.
+
+    :param featureFileName: Name of feature file.
+    :param releaseVersion: Release version for test set run.
+    :param customFields: Dict of any desired custom fields for test set.
+    :return: PractiTest id for created test set.
+    """
     GetConfigValues.GetConfigValues()
     projectId = GetPTProjectId.RetrieveProjectId()
     
-    res = PT_APIRequest.getRequest(Constants.PT_API_BASEURL + "/projects/" + projectId + "/sets.json?name_exact=" + testSetName)
+    testSetDict = {"data":{"type":"sets","attributes":{"name":featureFileName, "version": releaseVersion}}}
+    testSetDict["data"]["attributes"]["custom-fields"] = customFields
+    jsonData = json.dumps(testSetDict)
+    
+    res = PT_APIRequest.sendRequest(Constants.PT_API_BASEURL + "/projects/" + projectId +"/sets.json", "post", jsonData)
 
     if res.status_code == 200:
-        testSets = json.loads(res.content)
-        testSet = testSets['data']
+        responseData = json.loads(res.content)
 
-        myTestSetData = list(filter(lambda myData:myData['attributes']['name']==testSetName, testSet)) 
-        
-        if len(myTestSetData) != 0:
-            myTestSetId = myTestSetData[0]['id']
-            print (testSetName, "--> Test set id:", myTestSetId)
-            return myTestSetId
-        else:
-            print ("No matching test set of " + testSetName + " is found")
-            return None
+        data = responseData['data']
+   
+        newTestSetId = data['id']
+        return newTestSetId
     else:
-        raise Exception ("Call to get test set was unsucessful with status code", res.status_code)
+        raise Exception ("Call to create test set was unsuccessful with status code", res.status_code)
```

### Comparing `posttestresultstopractitest-0.0.5/src/PostTestResultsToPractiTest/PT_APIRequest.py` & `posttestresultstopractitest-0.0.6/src/PostTestResultsToPractiTest/PT_APIRequest.py`

 * *Files identical despite different names*

### Comparing `posttestresultstopractitest-0.0.5/LICENSE` & `posttestresultstopractitest-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `posttestresultstopractitest-0.0.5/PKG-INFO` & `posttestresultstopractitest-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: PostTestResultsToPractiTest
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create test set and post test results to PractiTest
-Author-email: Tuyen Luan <tuyen.luan@ncr.com>
+Author-email: Tuyen Luan <tuyen.luan@ncr.com>, Truc Mai <tm185237@ncr.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
@@ -22,15 +22,15 @@
         PractiTestTestSetName_New=<NewTestSetNameToBeCreated>
         PT_Token=<yourPractiTestToken>
         ```
 
 
 ## This package makes use of PractiTest's APIs to do the following:
 
-### 1. Use this package to create test_set (to be used in step 2)
+### 1. Use this package to clone test_set (test set needs to be created along with its instances before usage)
 
     Example of how to use it (in Python):
     ```
         from src.PostTestResultsToPractiTest import Orchestrator
         Orchestrator.CreateTestSetProcess()
     ```
 
@@ -38,8 +38,23 @@
 
     Example of how to use it (in Python):
     ```
         from src.PostTestResultsToPractiTest import Orchestrator
         from src.PostTestResultsToPractiTest.EnumClass import TestResultStatus
         Orchestrator.PostToPractiTest("NameOfYourFeatureFileInBDD-including-extension-.feature", TestResultStatus.UNSTABLE, "Output message if any")
     ```
-    Note that TestResultStatus is an enum class, available values are TestResultStatus.PASS, estResultStatus.FAIL, and TestResultStatus.UNSTABLE
+    Note that TestResultStatus is an enum class, available values are TestResultStatus.PASS, estResultStatus.FAIL, and TestResultStatus.UNSTABLE
+
+### 3. Use this package to create test set, fill with instances, and post results all within an automation run.
+
+    Example of how to use it (in Python):
+    ```
+        from src.PostTestResultsToPractiTest import Orchestrator
+        customFields = {'---f-112372': 'Example'}
+        testSetId = Orchestrator.CreateTestSetFromFeature(featureFileName, releaseVersion, customFields)
+        testId = Orchestrator.RetrieveTestId(testName)
+        instanceId = Orchestrator.CreateInstance(testSetId, testId)
+        Orchestrator.PostToPractiTestWithFile(instanceId, passFailStatus, fileDir, fileName)
+    ```
+    Note that passFailStatus is just a boolean value on whether the test passed or failed.
+    The variables fileDir and fileName are the directory and file name respectively for the file that you would like to attach
+    with your test results (logs, reports, etc.).
```

