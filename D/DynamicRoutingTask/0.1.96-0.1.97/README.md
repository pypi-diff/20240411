# Comparing `tmp/DynamicRoutingTask-0.1.96.tar.gz` & `tmp/DynamicRoutingTask-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DynamicRoutingTask-0.1.96.tar", last modified: Wed Apr 10 02:07:36 2024, max compression
+gzip compressed data, was "DynamicRoutingTask-0.1.97.tar", last modified: Thu Apr 11 19:01:52 2024, max compression
```

## Comparing `DynamicRoutingTask-0.1.96.tar` & `DynamicRoutingTask-0.1.97.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.463995 DynamicRoutingTask-0.1.96/Analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    34706 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/DynamicRoutingAnalysisUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    64516 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodelHPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodelSlurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/RLmodel_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/behaviorClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/dr_analysis_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)   110109 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/dr_behav_figs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/dr_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/glm_hmm_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/ncb_meeting_01272023.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/npc_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/presentation_June2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/regressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sac_may2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sessionSummaryFigs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sound_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/sound_sync_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/Analysis/variableBlockDur.py
--rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/DynamicRouting1.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/DynamicRouting1_postSessionAnalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 02:07:36.000000 DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.463995 DynamicRoutingTask-0.1.96/OptoGui/
--rw-r--r--   0 runner    (1001) docker     (127)    34068 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/OptoGui/OptoGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/OptoTagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/RFMapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:07:36.463995 DynamicRoutingTask-0.1.96/SamStimGui/
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/SamStimGui/SamStimGui.py
--rw-r--r--   0 runner    (1001) docker     (127)    62349 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/TaskControl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/TaskUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/camstimControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-10 02:07:33.000000 DynamicRoutingTask-0.1.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/runTask.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:07:36.467995 DynamicRoutingTask-0.1.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-10 02:07:08.000000 DynamicRoutingTask-0.1.96/startTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/Analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    34706 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/DynamicRoutingAnalysisUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64516 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/RLmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/RLmodelHPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/RLmodelSlurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/RLmodel_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/behaviorClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/dr_analysis_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110109 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/dr_behav_figs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/dr_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/glm_hmm_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/ncb_meeting_01272023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/npc_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/presentation_June2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/regressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/sac_may2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/sessionSummaryFigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/sound_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/sound_sync_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/Analysis/variableBlockDur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/DynamicRouting1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/DynamicRouting1_postSessionAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 19:01:52.000000 DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-11 19:01:52.000000 DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:01:52.000000 DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 19:01:52.000000 DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 19:01:52.000000 DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/OptoGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    34068 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/OptoGui/OptoGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/OptoTagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/RFMapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/SamStimGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/SamStimGui/SamStimGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62349 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/TaskControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/TaskUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/camstimControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 19:01:49.000000 DynamicRoutingTask-0.1.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/runTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:01:52.063226 DynamicRoutingTask-0.1.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-11 19:01:28.000000 DynamicRoutingTask-0.1.97/startTask.py
```

### Comparing `DynamicRoutingTask-0.1.96/Analysis/DynamicRoutingAnalysisUtils.py` & `DynamicRoutingTask-0.1.97/Analysis/DynamicRoutingAnalysisUtils.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/RLmodel.py` & `DynamicRoutingTask-0.1.97/Analysis/RLmodel.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/RLmodelHPC.py` & `DynamicRoutingTask-0.1.97/Analysis/RLmodelHPC.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/RLmodelSlurm.py` & `DynamicRoutingTask-0.1.97/Analysis/RLmodelSlurm.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/RLmodel_old.py` & `DynamicRoutingTask-0.1.97/Analysis/RLmodel_old.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/behaviorClustering.py` & `DynamicRoutingTask-0.1.97/Analysis/behaviorClustering.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/dr_analysis_sam.py` & `DynamicRoutingTask-0.1.97/Analysis/dr_analysis_sam.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/dr_behav_figs.py` & `DynamicRoutingTask-0.1.97/Analysis/dr_behav_figs.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/dr_ephys_analysis.py` & `DynamicRoutingTask-0.1.97/Analysis/dr_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/glm_hmm_sam.py` & `DynamicRoutingTask-0.1.97/Analysis/glm_hmm_sam.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/ncb_meeting_01272023.py` & `DynamicRoutingTask-0.1.97/Analysis/ncb_meeting_01272023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/npc_analysis.py` & `DynamicRoutingTask-0.1.97/Analysis/npc_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/presentation_June2023.py` & `DynamicRoutingTask-0.1.97/Analysis/presentation_June2023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/regressionModel.py` & `DynamicRoutingTask-0.1.97/Analysis/regressionModel.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/sac_may2023.py` & `DynamicRoutingTask-0.1.97/Analysis/sac_may2023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/sessionSummaryFigs.py` & `DynamicRoutingTask-0.1.97/Analysis/sessionSummaryFigs.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/sound_ephys_analysis.py` & `DynamicRoutingTask-0.1.97/Analysis/sound_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/sound_sync_test.py` & `DynamicRoutingTask-0.1.97/Analysis/sound_sync_test.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/Analysis/variableBlockDur.py` & `DynamicRoutingTask-0.1.97/Analysis/variableBlockDur.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/DynamicRouting1.py` & `DynamicRoutingTask-0.1.97/DynamicRouting1.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/DynamicRouting1_postSessionAnalysis.py` & `DynamicRoutingTask-0.1.97/DynamicRouting1_postSessionAnalysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/DynamicRoutingTask.egg-info/SOURCES.txt` & `DynamicRoutingTask-0.1.97/DynamicRoutingTask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/OptoGui/OptoGui.py` & `DynamicRoutingTask-0.1.97/OptoGui/OptoGui.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/OptoTagging.py` & `DynamicRoutingTask-0.1.97/OptoTagging.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/RFMapping.py` & `DynamicRoutingTask-0.1.97/RFMapping.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/SamStimGui/SamStimGui.py` & `DynamicRoutingTask-0.1.97/SamStimGui/SamStimGui.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/TaskControl.py` & `DynamicRoutingTask-0.1.97/TaskControl.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/TaskUtils.py` & `DynamicRoutingTask-0.1.97/TaskUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     p = np.polyfit(d['input (V)'],d['power (mW)'],2)
     d['poly coefficients'] = p
     d['offsetV'] = min(np.roots(p))
     return d
 
 
 def powerToVolts(calibrationData,power):
-    return min((np.poly1d(calibrationData['poly coefficients']) - power).roots) if power > 0 else 0
+    return min((np.poly1d(calibrationData['poly coefficients']) - power).roots) if power > 0 else 0.001
 
 
 def voltsToPower(calibrationData,volts):
     return np.polyval(calibrationData['poly coefficients'],volts)
 
 
 def getOptoPulseWaveform(sampleRate,amp,dur=0,delay=0,freq=0,onRamp=0,offRamp=0,offset=0,lastVal=0):
```

### Comparing `DynamicRoutingTask-0.1.96/camstimControl.py` & `DynamicRoutingTask-0.1.97/camstimControl.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/pyproject.toml` & `DynamicRoutingTask-0.1.97/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DynamicRoutingTask"
-version = "0.1.96"
+version = "0.1.97"
 dependencies = [
     "h5py",
     "numpy",
     "pandas",
     "scipy",
     "matplotlib",
 ]
```

### Comparing `DynamicRoutingTask-0.1.96/runTask.py` & `DynamicRoutingTask-0.1.97/runTask.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.96/startTask.py` & `DynamicRoutingTask-0.1.97/startTask.py`

 * *Files identical despite different names*

