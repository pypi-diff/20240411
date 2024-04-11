# Comparing `tmp/labgym-2.4.2.tar.gz` & `tmp/labgym-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgym-2.4.2.tar", last modified: Fri Apr  5 17:39:07 2024, max compression
+gzip compressed data, was "labgym-2.4.3.tar", last modified: Thu Apr 11 06:01:11 2024, max compression
```

## Comparing `labgym-2.4.2.tar` & `labgym-2.4.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0    31919 2024-04-05 17:39:00.952517 labgym-2.4.2/LICENSE.txt
--rw-r--r--   0        0        0      417 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/COPYRIGHT.txt
--rw-r--r--   0        0        0      131 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/NOTICE.txt
--rw-r--r--   0        0        0      882 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/__main__.py
--rw-r--r--   0        0        0    87666 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/analyzebehaviors.py
--rw-r--r--   0        0        0   173802 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/analyzebehaviorsdetector.py
--rw-r--r--   0        0        0    67359 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/categorizers.py
--rw-r--r--   0        0        0    12995 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/detector.py
--rw-r--r--   0        0        0      859 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/detectors/__init__.py
--rw-r--r--   0        0        0      889 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/__init__.py
--rw-r--r--   0        0        0      904 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/analysis/__init__.py
--rw-r--r--   0        0        0     1808 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/analysis/analysis_module.py
--rw-r--r--   0        0        0    67751 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/analysis/analyze_behaviors.py
--rw-r--r--   0        0        0     9322 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/analysis/mine_results.py
--rw-r--r--   0        0        0     4833 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/main_window.py
--rw-r--r--   0        0        0    22593 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/preprocessing.py
--rw-r--r--   0        0        0      904 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/training/__init__.py
--rw-r--r--   0        0        0    51881 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/training/behavior_examples.py
--rw-r--r--   0        0        0    33348 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/training/categorizers.py
--rw-r--r--   0        0        0    22307 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/training/detectors.py
--rw-r--r--   0        0        0     5203 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/training/training_module.py
--rw-r--r--   0        0        0     4473 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/gui/utils.py
--rw-r--r--   0        0        0     8091 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/minedata.py
--rw-r--r--   0        0        0      859 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/models/__init__.py
--rw-r--r--   0        0        0    45139 2024-04-05 17:39:00.956517 labgym-2.4.2/LabGym/tools.py
--rw-r--r--   0        0        0      131 2024-04-05 17:39:00.960517 labgym-2.4.2/NOTICE.txt
--rw-r--r--   0        0        0    13320 2024-04-05 17:39:00.960517 labgym-2.4.2/README.md
--rw-r--r--   0        0        0     2164 2024-04-05 17:39:07.816530 labgym-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      859 2024-04-05 17:39:00.964517 labgym-2.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-05 17:39:00.964517 labgym-2.4.2/tests/test_main.py
--rw-r--r--   0        0        0     1093 2024-04-05 17:39:00.964517 labgym-2.4.2/tests/test_tools.py
--rw-r--r--   0        0        0    14864 1970-01-01 00:00:00.000000 labgym-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    31919 2024-04-11 06:01:06.448275 labgym-2.4.3/LICENSE.txt
+-rw-r--r--   0        0        0      417 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/COPYRIGHT.txt
+-rw-r--r--   0        0        0      131 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/NOTICE.txt
+-rw-r--r--   0        0        0      882 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/__main__.py
+-rw-r--r--   0        0        0    87666 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/analyzebehaviors.py
+-rw-r--r--   0        0        0   173802 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/analyzebehaviorsdetector.py
+-rw-r--r--   0        0        0    68079 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/categorizers.py
+-rw-r--r--   0        0        0    12995 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/detector.py
+-rw-r--r--   0        0        0      859 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/detectors/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/__init__.py
+-rw-r--r--   0        0        0     2115 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/analysis_module.py
+-rw-r--r--   0        0        0    67941 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/analyze_behaviors.py
+-rw-r--r--   0        0        0     7276 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/behavior_plot.py
+-rw-r--r--   0        0        0     9322 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/mine_results.py
+-rw-r--r--   0        0        0     4833 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/main_window.py
+-rw-r--r--   0        0        0    22593 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/preprocessing.py
+-rw-r--r--   0        0        0      904 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/__init__.py
+-rw-r--r--   0        0        0    51881 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/behavior_examples.py
+-rw-r--r--   0        0        0    33348 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/categorizers.py
+-rw-r--r--   0        0        0    22307 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/detectors.py
+-rw-r--r--   0        0        0     5203 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/training_module.py
+-rw-r--r--   0        0        0     4473 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/utils.py
+-rw-r--r--   0        0        0     8091 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/minedata.py
+-rw-r--r--   0        0        0      859 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/models/__init__.py
+-rw-r--r--   0        0        0    49154 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/tools.py
+-rw-r--r--   0        0        0      131 2024-04-11 06:01:06.452275 labgym-2.4.3/NOTICE.txt
+-rw-r--r--   0        0        0    13320 2024-04-11 06:01:06.452275 labgym-2.4.3/README.md
+-rw-r--r--   0        0        0     2164 2024-04-11 06:01:11.084287 labgym-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0      859 2024-04-11 06:01:06.460275 labgym-2.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-11 06:01:06.460275 labgym-2.4.3/tests/test_main.py
+-rw-r--r--   0        0        0     1093 2024-04-11 06:01:06.460275 labgym-2.4.3/tests/test_tools.py
+-rw-r--r--   0        0        0    14864 1970-01-01 00:00:00.000000 labgym-2.4.3/PKG-INFO
```

### Comparing `labgym-2.4.2/LICENSE.txt` & `labgym-2.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/__init__.py` & `labgym-2.4.3/LabGym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-__version__ = "2.4.2"
+__version__ = "2.4.3"
```

### Comparing `labgym-2.4.2/LabGym/__main__.py` & `labgym-2.4.3/LabGym/__main__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/analyzebehaviors.py` & `labgym-2.4.3/LabGym/analyzebehaviors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/analyzebehaviorsdetector.py` & `labgym-2.4.3/LabGym/analyzebehaviorsdetector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/categorizers.py` & `labgym-2.4.3/LabGym/categorizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
                     animations.append(np.array(animation))
 
                 pattern_image = cv2.imread(path_to_pattern_image)
 
                 if code is not None:
                     pattern_image = cv2.flip(pattern_image, code)
 
-                if behavior_mode >= 3:
+                if behavior_mode == 3:
                     if beta is not None:
                         if background_free is True:
                             pattern_image_gray = cv2.cvtColor(pattern_image, cv2.COLOR_BGR2GRAY)
                             thred = cv2.threshold(
                                 pattern_image_gray,
                                 0,
                                 255,
@@ -461,14 +461,15 @@
                                 pattern_image = np.zeros_like(pattern_image)
                             else:
                                 contour = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
                                 pattern_image = extract_blob(pattern_image, contour, channel=3)
                             pattern_image = pattern_image.astype("float")
                             pattern_image[pattern_image > 30] += beta
                         else:
+                            pattern_image = pattern_image.astype("float")
                             pattern_image += beta
                         pattern_image = np.uint8(np.clip(pattern_image, 0, 255))
 
                 if angle is not None:
                     pattern_image = ndimage.rotate(pattern_image, angle, reshape=False, prefilter=False)
 
                 if shear is not None:
@@ -500,15 +501,15 @@
                     pattern_image_black[
                         y : y + pattern_image_scl.shape[0],
                         x : x + pattern_image_scl.shape[1],
                         :,
                     ] = pattern_image_scl
                     pattern_image = pattern_image_black
 
-                if behavior_mode >= 3:
+                if behavior_mode == 3:
                     if channel == 1:
                         pattern_image = cv2.cvtColor(np.uint8(pattern_image), cv2.COLOR_BGR2GRAY)
 
                 pattern_image = cv2.resize(pattern_image, (dim_conv, dim_conv), interpolation=cv2.INTER_AREA)
                 pattern_images.append(img_to_array(pattern_image))
 
                 labels.append(label)
@@ -1684,25 +1685,54 @@
             dim_tconv = int(parameters["dim_tconv"][0])
         if "level_conv" in list(parameters.keys()):
             level_conv = int(parameters["level_conv"][0])
         if "dim_tconv" in list(parameters.keys()):
             level_tconv = int(parameters["level_tconv"][0])
         if "channel" in list(parameters.keys()):
             channel = int(parameters["channel"][0])
-        network = int(parameters["network"][0])
-        if network == 0:
+        if "behavior_kind" in list(parameters.keys()):
+            behavior_mode = int(parameters["behavior_kind"][0])
+        else:
+            behavior_mode = 0
+        if behavior_mode == 0:
+            print("The behavior mode of the Categorizer: Non-interactive.")
+        elif behavior_mode == 1:
+            print("The behavior mode of the Categorizer: Interactive basic.")
+        elif behavior_mode == 2:
             print(
-                "The type of the Categorizer: Pattern Recognizer (Lv "
-                + str(level_conv)
-                + "; Shape "
-                + str(dim_conv)
-                + " X "
-                + str(dim_conv)
-                + " X 3)."
+                "The behavior mode of the Categorizer: Interactive advanced (Social distance "
+                + str(parameters["social_distance"][0])
+                + ")."
             )
+        else:
+            print("The behavior mode of the Categorizer: Static images (non-interactive).")
+        network = int(parameters["network"][0])
+        if network == 0:
+            if behavior_mode==3:
+                print(
+                    "The type of the Categorizer: Pattern Recognizer (Lv "
+                    + str(level_conv)
+                    + "; Shape "
+                    + str(dim_conv)
+                    + " X "
+                    + str(dim_conv)
+                    + " X "
+                    + str(channel)
+                    + ")."
+                )
+            else:
+                print(
+                    "The type of the Categorizer: Pattern Recognizer (Lv "
+                    + str(level_conv)
+                    + "; Shape "
+                    + str(dim_conv)
+                    + " X "
+                    + str(dim_conv)
+                    + " X 3)."
+                )
         if network == 2:
             print(
                 "The type of the Categorizer: Animation Analyzer (Lv "
                 + str(level_tconv)
                 + "; Shape "
                 + str(dim_tconv)
                 + " X "
@@ -1713,30 +1743,15 @@
                 + str(level_conv)
                 + "; Shape "
                 + str(dim_conv)
                 + " X "
                 + str(dim_conv)
                 + " X 3)."
             )
-        if "behavior_kind" in list(parameters.keys()):
-            behavior_mode = int(parameters["behavior_kind"][0])
-        else:
-            behavior_mode = 0
-        if behavior_mode == 0:
-            print("The behavior mode of the Categorizer: Non-interactive.")
-        elif behavior_mode == 1:
-            print("The behavior mode of the Categorizer: Interactive basic.")
-        elif behavior_mode == 2:
-            print(
-                "The behavior mode of the Categorizer: Interactive advanced (Social distance "
-                + str(parameters["social_distance"][0])
-                + ")."
-            )
-        else:
-            print("The behavior mode of the Categorizer: Static images (non-interactive).")
+
         length = int(parameters["time_step"][0])
         print("The length of a behavior example in the Categorizer: " + str(length) + " frames.")
         if int(parameters["inner_code"][0]) == 0:
             print("The Categorizer includes body parts in analysis with STD = " + str(parameters["std"][0]) + ".")
         else:
             print("The Categorizer does not include body parts in analysis.")
         if int(parameters["background_free"][0]) == 0:
@@ -1791,14 +1806,17 @@
                         animations.append(np.array(animation))
 
                     if network != 1:
                         path_to_pattern_image = (
                             os.path.splitext(os.path.join(groundtruth_path, behavior, i))[0] + ".jpg"
                         )
                         pattern_image = cv2.imread(path_to_pattern_image)
+                        if behavior_mode==3:
+                            if channel==1:
+                                pattern_image=cv2.cvtColor(pattern_image,cv2.COLOR_BGR2GRAY)
                         pattern_image = cv2.resize(
                             pattern_image,
                             (dim_conv, dim_conv),
                             interpolation=cv2.INTER_AREA,
                         )
                         pattern_images.append(img_to_array(pattern_image))
```

### Comparing `labgym-2.4.2/LabGym/detector.py` & `labgym-2.4.3/LabGym/detector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/detectors/__init__.py` & `labgym-2.4.3/LabGym/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/__init__.py` & `labgym-2.4.3/LabGym/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/analysis/__init__.py` & `labgym-2.4.3/LabGym/gui/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/analysis/analysis_module.py` & `labgym-2.4.3/LabGym/gui/analysis/analysis_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 USA
 
 Email: bingye@umich.edu
 """
 
 from ..utils import LabGymWindow
 from .analyze_behaviors import AnalyzeBehaviors
+from .behavior_plot import BehaviorPlot
 from .mine_results import MineResults
 
 
 class AnalysisModule(LabGymWindow):
     def __init__(self):
         super().__init__(title="Analysis Module", size=(500, 220))
 
@@ -33,14 +34,23 @@
 
         self.add_submit_button(
             label="Mine Results",
             handler=self.mine_results,
             tool_tip="Automatically mine the analysis results to display the data details that show statistically significant differences among groups of your selection.",
         )
 
+        self.add_submit_button(
+            label="Generate Behavior Plot",
+            handler=self.behavior_plot,
+            tool_tip="Generate a behavior plot given an all_events.xlsx file.",
+        )
+
         self.display_window()
 
     def analyze_behaviors(self, event):
         AnalyzeBehaviors()
 
     def mine_results(self, event):
         MineResults()
+
+    def behavior_plot(self, event):
+        BehaviorPlot()
```

### Comparing `labgym-2.4.2/LabGym/gui/analysis/analyze_behaviors.py` & `labgym-2.4.3/LabGym/gui/analysis/analyze_behaviors.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,29 +25,37 @@
 import wx
 
 from LabGym.analyzebehaviors import AnalyzeAnimal
 from LabGym.analyzebehaviorsdetector import AnalyzeAnimalDetector
 from LabGym.categorizers import CATEGORIZER_FOLDER, get_categorizer_names
 from LabGym.detector import Detector, get_detector_names
 from LabGym.gui.utils import WX_IMAGE_WILDCARD, WX_VIDEO_WILDCARD, LabGymWindow
-from LabGym.tools import plot_evnets
+from LabGym.tools import plot_events
 
 
 class ColorPicker(wx.Dialog):
-    def __init__(self, parent, title, name_and_color):
-        super(ColorPicker, self).__init__(parent=None, title=title, size=(200, 200))
+    """A small window that contains a color picker dialog."""
 
-        self.name_and_color = name_and_color
-        name = self.name_and_color[0]
-        hex_color = self.name_and_color[1][1].lstrip("#")
-        color = tuple(int(hex_color[i : i + 2], 16) for i in (0, 2, 4))
+    def __init__(self, title: str, default_color: str):
+        """Initialize a ColorPicker.
+
+        Args:
+            title:
+                The title of the ColorPicker window.
+            default_color:
+                A string in hex format (e.g. '#ffffff').
+        """
+        super().__init__(parent=None, title=title, size=(200, 200))
 
         boxsizer = wx.BoxSizer(wx.VERTICAL)
 
-        self.color_picker = wx.ColourPickerCtrl(self, colour=color)
+        # Convert hex string to (red, green, blue) tuple
+        raw_hex = default_color.lstrip("#")
+        default_color_rgb = tuple(int(raw_hex[i : i + 2], 16) for i in (0, 2, 4))
+        self.color_picker = wx.ColourPickerCtrl(self, colour=default_color_rgb)
 
         button = wx.Button(self, wx.ID_OK, label="Apply")
 
         boxsizer.Add(0, 10, 0)
         boxsizer.Add(self.color_picker, 0, wx.ALL | wx.CENTER, 10)
         boxsizer.Add(button, 0, wx.ALL | wx.CENTER, 10)
         boxsizer.Add(0, 10, 0)
@@ -959,17 +967,16 @@
                 wx.YES_NO | wx.ICON_QUESTION,
             )
             if dialog.ShowModal() == wx.ID_YES:
                 names_colors = {}
                 n = 0
                 while n < len(self.behavior_to_include):
                     dialog2 = ColorPicker(
-                        self,
                         "Color for " + self.behavior_to_include[n],
-                        [self.behavior_to_include[n], colors[n]],
+                        colors[n][1],
                     )
                     if dialog2.ShowModal() == wx.ID_OK:
                         (r, b, g, _) = dialog2.color_picker.GetColour()
                         new_color = "#%02x%02x%02x" % (r, b, g)
                         self.behaviornames_and_colors[self.behavior_to_include[n]] = [
                             "#ffffff",
                             new_color,
@@ -1289,15 +1296,15 @@
                         time_points = AA.all_time[: min(all_lengths)]
                         all_events_df = pd.DataFrame(event_data, index=time_points)
                         all_events_df.to_excel(
                             os.path.join(self.result_path, "all_events.xlsx"),
                             float_format="%.2f",
                             index_label="time/ID",
                         )
-                        plot_evnets(
+                        plot_events(
                             self.result_path,
                             event_data,
                             time_points,
                             self.behaviornames_and_colors,
                             self.behavior_to_include,
                             width=0,
                             height=0,
@@ -1337,15 +1344,15 @@
                         time_points = AAD.all_time[: min(all_lengths)]
                         all_events_df = pd.DataFrame(event_data, index=time_points)
                         all_events_df.to_excel(
                             os.path.join(self.result_path, "all_events.xlsx"),
                             float_format="%.2f",
                             index_label="time/ID",
                         )
-                        plot_evnets(
+                        plot_events(
                             self.result_path,
                             event_data,
                             time_points,
                             self.behaviornames_and_colors,
                             self.behavior_to_include,
                             width=0,
                             height=0,
```

### Comparing `labgym-2.4.2/LabGym/gui/analysis/mine_results.py` & `labgym-2.4.3/LabGym/gui/analysis/mine_results.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/main_window.py` & `labgym-2.4.3/LabGym/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/preprocessing.py` & `labgym-2.4.3/LabGym/gui/preprocessing.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/training/__init__.py` & `labgym-2.4.3/LabGym/gui/training/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/training/behavior_examples.py` & `labgym-2.4.3/LabGym/gui/training/behavior_examples.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/training/categorizers.py` & `labgym-2.4.3/LabGym/gui/training/categorizers.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/training/detectors.py` & `labgym-2.4.3/LabGym/gui/training/detectors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/training/training_module.py` & `labgym-2.4.3/LabGym/gui/training/training_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/gui/utils.py` & `labgym-2.4.3/LabGym/gui/utils.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/minedata.py` & `labgym-2.4.3/LabGym/minedata.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/models/__init__.py` & `labgym-2.4.3/LabGym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/LabGym/tools.py` & `labgym-2.4.3/LabGym/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import datetime
 import functools
 import gc
 import operator
 import os
 from collections import deque
+from pathlib import Path
 from typing import Sequence, Tuple
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sb
@@ -937,23 +938,52 @@
         pattern_image = cv2.add(inners_image, outlines_image)
     else:
         pattern_image = outlines_image
 
     return pattern_image
 
 
-def plot_evnets(
-    result_path,
-    event_probability,
-    time_points,
-    names_and_colors,
-    behavior_to_include,
-    width=0,
-    height=0,
-):
+def plot_events(
+    result_path: str,
+    event_probability: dict,
+    time_points: list[float],
+    names_and_colors: dict[str, Tuple[str, str]],
+    behavior_to_include: list[str],
+    width: int = 0,
+    height: int = 0,
+) -> None:
+    """Generate time-series behavior plot and colorbars for each behavior.
+
+    Args:
+        result_path:
+            The folder in which to store the behavior plot and colorbars.
+        event_probability:
+            A dictionary with the keys as with the keys as the ID of each
+            animal and the values are lists of lists, where each sub-list
+            has a length of 2 and is in one of the following formats:
+                - ["NA", -1], indicating the animal wasn't detected during
+                  this time point.
+                - [behavior, probability], where behavior is the name of
+                  the behavior and probability is a float between 0 and 1.
+        time_points:
+            A list of floats containing the time points for each behavior
+            for each animal, which is in the leftmost column in the original
+            file.
+        names_and_colors:
+            A dictionary with keys as behavior names and values as lists
+            or tuples containing two strings, where the first string is
+            '#ffffff' and the second string is the hex color code of the
+            color corresponding to the behavior.
+        behavior_to_include:
+            A list of which behaviors to include.
+        width:
+            The width of the behavior plot in inches.
+        height:
+            The height of the behavior plot in inches.
+    """
     print("Exporting the raster plot for this analysis batch...")
     print(datetime.datetime.now())
 
     if width == 0 or height == 0:
         time_length = len(time_points)
         if time_length > 30000:
             width = round(time_length / 3000) + 1
@@ -1217,7 +1247,81 @@
         None
     """
     if n <= 1.0:
         return []
     num_dropped_frames = int(n * (1 - 1 / reduction_factor))
     block_size = n / (n * (1 - 1 / reduction_factor) - 1)
     return [round(block_size * i) for i in range(num_dropped_frames)]
+
+
+def parse_all_events_file(path: Path) -> Tuple[dict, list[float]]:
+    """Parse an all_events.xlsx file.
+
+    Args:
+        path: The path to the all_events.xlsx file.
+
+    Returns:
+        A tuple (events, time_points).
+
+        events is a dictionary with the keys as the ID of each animal and the
+        values are lists of lists, where each sub-list has a length of 2 and
+        is in one of the following formats:
+
+        - ["NA", -1] (The animal wasn't detected during this time point.)
+        - [behavior, probability], where behavior is the name of the behavior
+          and probability is a float between 0 and 1.
+
+        time_points is a list of floats containing the time points for each
+        behavior for each animal, which is in the leftmost column in the
+        original file.
+
+    Raises:
+        ValueError: The all_events.xlsx file is in an invalid format.
+    """
+
+    df = pd.read_excel(path)
+
+    event_probability = {}
+    time_points = []
+    for col_name, col in df.items():
+        try:
+            id = int(col_name)  # type: ignore[reportArgumentType]
+        except ValueError:
+            # Leftmost row, load time points
+            if col_name == "time/ID":
+                try:
+                    time_points = [float(i) for i in col]
+                except ValueError:
+                    raise ValueError("Invalid all_events.xlsx file.")
+            continue
+
+        # The eval() function converts the string representation of the
+        # list into a Python list object.
+        event_probability[id] = []
+        for i in col:
+            event = eval(i)
+            if not _is_valid_event(event):
+                raise ValueError(f"Invalid event {event}.")
+            event_probability[id].append(event)
+
+    return (event_probability, time_points)
+
+
+def _is_valid_event(event: list) -> bool:
+    """Return whether or not the given event is valid."""
+    return (
+        isinstance(event, list)
+        and len(event) == 2
+        and isinstance(event[0], str)
+        and (isinstance(event[1], float) and 0 <= event[1] <= 1 or isinstance(event[1], int) and event[1] == -1)
+    )
+
+
+def get_behaviors_from_all_events(events_behaviors: dict) -> list[str]:
+    """Return a list of the behaviors present in an all_events.xlsx file."""
+    behaviors = []
+    for events in events_behaviors.values():
+        for behavior, _ in events:
+            if behavior not in behaviors and behavior != "NA":
+                behaviors.append(behavior)
+
+    return behaviors
```

### Comparing `labgym-2.4.2/README.md` & `labgym-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/pyproject.toml` & `labgym-2.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = []
-version = "2.4.2"
+version = "2.4.3"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.urls]
 Homepage = "http://github.com/umyelab/LabGym"
 Documentation = "https://labgym.readthedocs.io/en/latest/"
```

### Comparing `labgym-2.4.2/tests/__init__.py` & `labgym-2.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/tests/test_main.py` & `labgym-2.4.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/tests/test_tools.py` & `labgym-2.4.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.2/PKG-INFO` & `labgym-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabGym
-Version: 2.4.2
+Version: 2.4.3
 Summary: Quantify user-defined behaviors.
 Keywords: behavior analysis behavioral analysis user defined behaviors
 Author-Email: Yujia Hu <henryhu@umich.edu>, Rohan Satapathy <rohansat@umich.edu>, M. Victor Struman <strmark@umich.edu>, Kelly Goss <khgoss@umich.edu>, Isabelle Baker <ibaker@umich.edu>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

