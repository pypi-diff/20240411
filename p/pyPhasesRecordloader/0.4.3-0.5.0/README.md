# Comparing `tmp/pyPhasesRecordloader-0.4.3.tar.gz` & `tmp/pyPhasesRecordloader-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesRecordloader-0.4.3.tar", last modified: Fri Feb 16 07:51:46 2024, max compression
+gzip compressed data, was "pyPhasesRecordloader-0.5.0.tar", last modified: Thu Apr 11 11:39:07 2024, max compression
```

## Comparing `pyPhasesRecordloader-0.4.3.tar` & `pyPhasesRecordloader-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 07:51:46.384187 pyPhasesRecordloader-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1549 2024-02-16 07:51:46.383187 pyPhasesRecordloader-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 07:51:46.380190 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/Event.py
--rw-rw-rw-   0 root         (0) root         (0)    18984 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/EventManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3546 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/NormalizeRecordSignal.py
--rw-rw-rw-   0 root         (0) root         (0)     3288 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/RecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)    10135 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/RecordSignal.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/Signal.py
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 07:51:46.382188 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/
--rw-rw-rw-   0 root         (0) root         (0)     4319 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/Downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1980 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/FolderDownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/ListDownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/NSRRDownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1546 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/S3Downloader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 07:51:46.383187 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/CSVMetaLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     3088 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 07:51:46.383187 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/util/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/util/DynamicModule.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 07:51:46.380190 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1549 2024-02-16 07:51:46.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1298 2024-02-16 07:51:46.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 07:51:46.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-02-16 07:51:46.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-02-16 07:51:46.000000 pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-02-16 07:51:27.000000 pyPhasesRecordloader-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 07:51:46.384187 pyPhasesRecordloader-0.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-02-16 07:51:29.000000 pyPhasesRecordloader-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:07.991166 pyPhasesRecordloader-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1549 2024-04-11 11:39:07.991166 pyPhasesRecordloader-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:07.988166 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/Event.py
+-rw-rw-rw-   0 root         (0) root         (0)    18984 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/EventManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3546 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/NormalizeRecordSignal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6591 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/RecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/RecordSignal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/Signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:07.989166 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/Downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/FolderDownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/ListDownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/NSRRDownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/S3Downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:07.990166 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/CSVMetaLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:07.990166 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/util/DynamicModule.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:07.988166 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1549 2024-04-11 11:39:07.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1342 2024-04-11 11:39:07.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:39:07.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 11:39:07.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 11:39:07.000000 pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-11 11:38:50.000000 pyPhasesRecordloader-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 11:39:07.991166 pyPhasesRecordloader-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-04-11 11:38:51.000000 pyPhasesRecordloader-0.5.0/setup.py
```

### Comparing `pyPhasesRecordloader-0.4.3/LICENSE` & `pyPhasesRecordloader-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/PKG-INFO` & `pyPhasesRecordloader-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloader
-Version: 0.4.3
+Version: 0.5.0
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloader-0.4.3/README.md` & `pyPhasesRecordloader-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/Event.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/Event.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/EventManager.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/EventManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/NormalizeRecordSignal.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/NormalizeRecordSignal.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/Plugin.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/RecordLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/RecordLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,21 +109,24 @@
         dl = self.getDownloader()
         dl.options = self.downloadOptions
         if dl.canReadRemote:
             self.filePath = dl.basePath
         elif not Path(self.filePath).exists():
             dl.downloadTo(self.filePath)
 
+    def getHarmonizedSignal(self, recordName):
+        signal = self.getSignal(recordName)
+        NormalizeRecordSignal().combine(signal, self.combineChannels, self.targetSignals)
+        return signal
+
     def loadRecord(self, recordName, eventTargetFrequency=1) -> Tuple[RecordSignal, Tuple[Event]]:
         # self.downloadOnDemand(recordName)
-        signal = self.getSignal(recordName)
+        signal = self.getHarmonizedSignal(recordName)
         eventList = self.getEventList(recordName, targetFrequency=eventTargetFrequency)
 
-        NormalizeRecordSignal().combine(signal, self.combineChannels, self.targetSignals)
-
         return signal, eventList
 
     def getSignal(self, recordName) -> RecordSignal:
         pass
 
     def loadAnnotation(self, recordName):
         pass
@@ -148,15 +151,15 @@
         packageName = RecordLoader.recordLoaders[RecordLoader.recordLoader.moduleName]
         return RecordLoader.recordLoader.get(packageName)
 
     def getRecordList(self):
         downloader = self.getDownloader()
         return downloader.getRecordList()
 
-    def getMetaData(self, recordId):
+    def getMetaData(self, recordId, withChannels=False):
         self.logError("getMetadata not implemented in used recordloader")
         return {}
 
     def getSignalTypeStrFromDict(self, signalName):
         if self.signalTypeDict == {}:
             self.signalTypeDict = dict(zip(self.targetSignals, self.targetSignalTypes))
         if signalName in self.signalTypeDict:
```

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/RecordSignal.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/RecordSignal.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,23 +100,29 @@
                 raise ChannelsNotPresent([name])
         return self.signalNames.index(name)
 
     def getSignalByName(self, name) -> Signal:
         index = self.getSignalIndexByName(name)
         return self.signals[index]
 
-    def getFirstSignalByName(self, nameList) -> Signal:
+    def getFirstSignalName(self, nameList) -> str:
         try:
             name = next(signalName for signalName in nameList if signalName in self.signalNames)
-        except:
+        except StopIteration:
             if "FLATLINE" in nameList:
-                return self.generateFlatline()
+                return "FLATLINE"
             from .RecordLoader import ChannelsNotPresent
             raise ChannelsNotPresent(nameList, msg="Non of the target signals (%s) is present in the record,: %s you can use FLATLINE as channel name to replace missing channels with a flat line" % (nameList, self.signalNames))
+        return name
+
+    def getFirstSignalByName(self, nameList) -> Signal:
 
+        name = self.getFirstSignalName(nameList)
+        if name == "FLATLINE":
+            return self.generateFlatline()
         index = self.getSignalIndexByName(name)
         return self.signals[index]
 
     def createSignalArray(self, signals, transpose):
         if len(signals) > 1:
             try:
                 a = np.concatenate([s.signal.reshape(1, -1) for s in signals], axis=0)
@@ -177,17 +183,21 @@
     def getAnnotationArray(self, transpose=True):
         "get all annotation signals concatenated into one array"
 
         return self.createSignalArray(self.labelSignals, transpose).astype(self.labelType)
 
     def reduceSignals(self, keepSignalNames):
         newSignals = []
+        newSignalNames = []
         for keep in keepSignalNames:
-            newSignals.append(self.getSignalByName(keep))
-        self.signalNames = keepSignalNames
+            signalName = keep if isinstance(keep, str) else self.getFirstSignalName(keep)
+            signal = self.getSignalByName(signalName)
+            newSignals.append(signal)
+            newSignalNames.append(signal.name)
+        self.signalNames = newSignalNames
         self.signals = newSignals
         self.shape = None
 
     def combine(self, channels, newName="Unknown", mean=True, derive=False):
         count = len(channels)
         mainIndex = self.getSignalIndexByName(channels[0])
         mainSignal = self.signals[mainIndex]
@@ -254,15 +264,15 @@
     def signalCutBySignalBoolSignal(self, boolSignal):
         for s in self.signals + self.labelSignals:
             s.signal = s.signal[boolSignal]
 
     def __getitem__(self, signalNames) -> "RecordSignal":
         """ Returns a new RecordSignal object with the given signalNames.
         """
-        signal = RecordSignal(self.recordId, self.targetFrequency)
+        signal = RecordSignal(targetFrequency=self.targetFrequency, recordId=self.recordId)
         if isinstance(signalNames, str):
             signalNames = [signalNames]
             
         for name in signalNames:
             signal.addSignal(self.getSignalByName(name))
             
         return signal
```

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/Signal.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/Signal.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/Downloader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/Downloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/FolderDownloader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/FolderDownloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/ListDownloader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/ListDownloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/NSRRDownloader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/NSRRDownloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/downloader/S3Downloader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/downloader/S3Downloader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/CSVMetaLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/CSVMetaLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/EDFRecordLoader.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,17 +23,34 @@
         signal.recordId = recordName
         return signal
     
     def getSignalHeaders(self, recordName):
         edfFile = self.getFilePathSignal(recordName)
         return self.loadSignalHeaders(edfFile)
 
-    def getAnnotationTimeByName(self, name):
-        for time, n in zip(self.annotations[0], self.annotations[2]):
-            if n == name:
+    def getAnnotationTimeByName(self, name, lastFirst=False):
+        return self.getAnnotationTimeByNames([name],lastFirst=False)
+    
+    def getFirstAnnotationTimeByName(self, name):
+        return self.getAnnotationTimeByName(name,lastFirst=False)
+
+    def getLastAnnotationTimeByName(self, name):
+        return self.getAnnotationTimeByName(name,lastFirst=False)
+    
+    def getAnnotationTimeByNames(self, names, lastFirst=False):
+        if len(self.annotations) == 0:
+            return None
+        
+        annotationList = zip(self.annotations[0], self.annotations[2])
+
+        if lastFirst:
+            annotationList = reversed(list(annotationList))
+
+        for time, n in annotationList:
+            if n in names:
                 return time
 
         return None
 
     def loadSignal(self, edfFile, annotations=False):
         recordSignal = RecordSignal()
         headers, f = self.loadSignalHeadersAndHandle(edfFile)
@@ -62,60 +79,84 @@
             recordSignal.addSignal(signal, signalName)
             
         return recordSignal
     
     def loadSignalHeaders(self, edfFile, annotations=False):
         return self.loadSignalHeadersAndHandle(edfFile, annotations)[0]
     
-    def loadSignalHeadersAndHandle(self, edfFile, annotations=False):
-        try:
-            self.logDebug("Read EDF Header %s" % edfFile)
-            f = pyedflib.EdfReader(edfFile)
-        except Exception as ex:
-            raise ParseError("Failed to read EDF File %s: %s" % (edfFile, str(ex)))
+    def loadSignalHeadersAndHandle(self, edfFile, annotations=False, checkTargetChannels=True):
+        signalHeaders, f = self.loadEdf(edfFile, self.targetSignals)
 
-        n = f.signals_in_file
-        targetSignals = self.targetSignals if annotations == False else self.annotationSignal
-        if len(targetSignals) == 0:
+        targetSignals = self.targetSignals if annotations is False else self.annotationSignal
+        if checkTargetChannels and len(targetSignals) == 0:
             raise Exception(
                 "The RecordLoader has no target signals to extract, please specificy 'sourceSignals' with the name of the channels"
             )
             
         expectedSignals = len(targetSignals)
         addedSignals = []
         ignoredChannels = []
-        signalHeaders = []
-        for i in range(n):
-            header = f.getSignalHeader(i)
+        targetSignalHeaders = []
+
+        for header in signalHeaders:
             channelLabel = header["label"]
             signalName = self.chanelNameAliasMap[channelLabel] if channelLabel in self.chanelNameAliasMap else channelLabel
-            if signalName in targetSignals:
-                header["signalName"] = signalName
-                header["type"] = self.getSignalTypeStrFromDict(signalName)
-                header["index"] = i
-                self.channelMap[signalName] = i
-                signalHeaders.append(header)
+            if header["signalName"] in targetSignals:
+                targetSignalHeaders.append(header)
                 addedSignals.append(signalName)
             else:
                 ignoredChannels.append(signalName)
 
         self.log("Added %i signals, ignored: %s" % (len(addedSignals), ignoredChannels))
         if len(addedSignals) < expectedSignals:
             missingchannels = set(self.targetSignals) - set(addedSignals) - set(self.optionalSignals)
             if len(missingchannels) > 0:
                 raise ChannelsNotPresent(missingchannels, edfFile)
 
-        return signalHeaders, f
+        return targetSignalHeaders, f
+
+    def loadEdf(self, edfFile, tailorChannels=None):
+        try:
+            self.logDebug("Read EDF Header %s" % edfFile)
+            f = pyedflib.EdfReader(edfFile)
+        except Exception as ex:
+            raise ParseError("Failed to read EDF File %s: %s" % (edfFile, str(ex)))
 
-    def getMetaData(self, recordName):
+        n = f.signals_in_file
+        
+        if f.annotations_in_file > 0:
+            self.annotations = f.readAnnotations()
+            
+        signalHeaders = []
+        for i in range(n):
+            header = f.getSignalHeader(i)
+            channelLabel = header["label"]
+            signalName = self.chanelNameAliasMap[channelLabel] if channelLabel in self.chanelNameAliasMap else channelLabel
+
+            if tailorChannels is None or signalName in tailorChannels:
+                header["signalName"] = signalName
+                header["type"] = self.getSignalTypeStrFromDict(signalName)
+                header["index"] = i
+                self.channelMap[signalName] = i
+                signalHeaders.append(header)
+
+        return signalHeaders, f
+    
+    def getMetaData(self, recordName, withChannels=False):
         edfFile = self.getFilePathSignal(recordName)
-        f = pyedflib.EdfReader(edfFile)
-        return {
+        signalHeaders, f = self.loadEdf(edfFile)
+            
+        metaData = {
             "recordId": recordName,
             "patientName": f.getPatientName(),
             "patientCode": f.getPatientCode(),
             "patientAdd": f.getPatientAdditional(),
             "start": f.getStartdatetime(),
             "technician": f.getTechnician(),
             "dataCount": f.datarecords_in_file,
         }
 
+        if withChannels:
+            metaData["channels"] = signalHeaders
+
+        return metaData
+
```

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/H5RecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/MatRecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/WFDBRecordLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/recordLoaders/XMLAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader/util/DynamicModule.py` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader/util/DynamicModule.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/PKG-INFO` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloader
-Version: 0.4.3
+Version: 0.5.0
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloader-0.4.3/pyPhasesRecordloader.egg-info/SOURCES.txt` & `pyPhasesRecordloader-0.5.0/pyPhasesRecordloader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyPhasesRecordloader/Event.py
 pyPhasesRecordloader/EventManager.py
 pyPhasesRecordloader/NormalizeRecordSignal.py
 pyPhasesRecordloader/Plugin.py
 pyPhasesRecordloader/RecordLoader.py
 pyPhasesRecordloader/RecordSignal.py
 pyPhasesRecordloader/Signal.py
+pyPhasesRecordloader/SignalPreprocessing.py
 pyPhasesRecordloader/__init__.py
 pyPhasesRecordloader.egg-info/PKG-INFO
 pyPhasesRecordloader.egg-info/SOURCES.txt
 pyPhasesRecordloader.egg-info/dependency_links.txt
 pyPhasesRecordloader.egg-info/requires.txt
 pyPhasesRecordloader.egg-info/top_level.txt
 pyPhasesRecordloader/downloader/Downloader.py
```

### Comparing `pyPhasesRecordloader-0.4.3/setup.py` & `pyPhasesRecordloader-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesRecordloader",
-    version="v0.4.3"[1:],
+    version="v0.5.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="Adds a record loaders to the pyPhases package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/",
     packages=setuptools.find_packages(),
```

