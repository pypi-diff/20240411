# Comparing `tmp/nap-plot-tools-0.0.3a0.tar.gz` & `tmp/nap-plot-tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nap-plot-tools-0.0.3a0.tar", last modified: Tue Nov 28 14:43:00 2023, max compression
+gzip compressed data, was "nap-plot-tools-0.0.4.tar", last modified: Thu Apr 11 11:50:15 2024, max compression
```

## Comparing `nap-plot-tools-0.0.3a0.tar` & `nap-plot-tools-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.311799 nap-plot-tools-0.0.3a0/
--rw-rw-rw-   0        0        0     1526 2023-07-03 07:56:44.000000 nap-plot-tools-0.0.3a0/LICENSE
--rw-rw-rw-   0        0        0     3528 2023-11-28 14:43:00.310799 nap-plot-tools-0.0.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     1866 2023-11-28 14:37:34.000000 nap-plot-tools-0.0.3a0/README.md
--rw-rw-rw-   0        0        0     1670 2023-11-28 14:43:00.317385 nap-plot-tools-0.0.3a0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-10-27 08:08:29.000000 nap-plot-tools-0.0.3a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.220642 nap-plot-tools-0.0.3a0/src/
-drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.262421 nap-plot-tools-0.0.3a0/src/nap_plot_tools/
--rw-rw-rw-   0        0        0      207 2023-11-28 14:40:18.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-11-28 14:40:07.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools/cmap.py
--rw-rw-rw-   0        0        0    12756 2023-11-28 14:40:07.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools/tools.py
-drwxrwxrwx   0        0        0        0 2023-11-28 14:43:00.306799 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/
--rw-rw-rw-   0        0        0     3528 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-11-28 14:42:59.000000 nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.507884 nap-plot-tools-0.0.4/
+-rw-rw-rw-   0        0        0     1526 2023-07-03 07:56:44.000000 nap-plot-tools-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3526 2024-04-11 11:50:15.506885 nap-plot-tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1866 2023-11-28 14:37:34.000000 nap-plot-tools-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1670 2024-04-11 11:50:15.511497 nap-plot-tools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-10-27 08:08:29.000000 nap-plot-tools-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.463002 nap-plot-tools-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.481003 nap-plot-tools-0.0.4/src/nap_plot_tools/
+-rw-rw-rw-   0        0        0      246 2024-04-11 11:44:22.000000 nap-plot-tools-0.0.4/src/nap_plot_tools/__init__.py
+-rw-rw-rw-   0        0        0     7604 2024-04-03 08:59:43.000000 nap-plot-tools-0.0.4/src/nap_plot_tools/cmap.py
+-rw-rw-rw-   0        0        0    15426 2024-04-05 12:15:17.000000 nap-plot-tools-0.0.4/src/nap_plot_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.503883 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/
+-rw-rw-rw-   0        0        0     3526 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/top_level.txt
```

### Comparing `nap-plot-tools-0.0.3a0/LICENSE` & `nap-plot-tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3a0/PKG-INFO` & `nap-plot-tools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nap-plot-tools
-Version: 0.0.3a0
+Version: 0.0.4
 Summary: A NAPari PLOTter TOOLbar and tools for additional functionalities.
 Home-page: https://github.com/zoccoler/nap-plot-tools
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/zoccoler/nap-plot-tools/issues
 Project-URL: Documentation, https://github.com/zoccoler/nap-plot-tools#README.md
```

### Comparing `nap-plot-tools-0.0.3a0/README.md` & `nap-plot-tools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3a0/setup.cfg` & `nap-plot-tools-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.3a0/src/nap_plot_tools/cmap.py` & `nap-plot-tools-0.0.4/src/nap_plot_tools/cmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -313,7 +313,10 @@
         "#9f7e80",
         "#5c4a56",
         "#735647",
         "#bcbcbc",
     ]
 
     return colors_hex
+
+cat10_mod_cmap = make_cat10_mod_cmap()
+cat10_mod_cmap_first_opaque = make_cat10_mod_cmap(first_color_transparent=False)
```

### Comparing `nap-plot-tools-0.0.3a0/src/nap_plot_tools/tools.py` & `nap-plot-tools-0.0.4/src/nap_plot_tools/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from nap_plot_tools.cmap import make_cat10_mod_cmap, get_custom_cat10based_cmap_list
-from qtpy.QtCore import Qt, QSize, QRect
+from qtpy.QtCore import Qt, QSize, QRect, Signal
 from qtpy.QtGui import QColor, QPainter, QPixmap
 from qtpy.QtWidgets import QSpinBox, QToolButton, QToolBar, QVBoxLayout, QWidget, QHBoxLayout, QSizePolicy
 
 import numpy as np
 
 class QtColorBox(QWidget):
     """A widget that shows a square with the current signal class color.
     """
-    
-
     def __init__(self, first_color_transparent=True) -> None:
         super().__init__()
         # TODO: Check why this may be necessary
         # self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
 
         self._height = 24
         self.setFixedWidth(self._height)
@@ -62,15 +60,18 @@
         # Update colorbox
         self.update()
 
 class QtColorSpinBox(QWidget):
     """QtColorSpinBox class.
 
     Custom widget to select a color and a value.
-    """    
+    """
+    # Signal emitted when the spinbox value changes
+    color_spinbox_value_changed_signal = Signal(int)
+
     def __init__(self, parent=None, first_color_transparent=True):
         super().__init__(parent)
         self.layout = QHBoxLayout(self)
         # Colorbox
         self.colorBox = QtColorBox(first_color_transparent=first_color_transparent)
         # Spinbox
         self.spinBox = QSpinBox()
@@ -80,14 +81,17 @@
 
         self.layout.addWidget(self.colorBox)
         self.layout.addWidget(self.spinBox)
 
         # Connect spinbox to color
         self.spinBox.valueChanged.connect(self.colorBox.setValue)
 
+        # Connect spinbox to signal
+        self.spinBox.valueChanged.connect(self.spinboxValueChangedEmitter)
+
     @property
     def value(self):
         return self.spinBox.value()
     
     @value.setter
     def value(self, value):
         """Set the value of the spinbox and colorbox.
@@ -144,14 +148,18 @@
 
     def setMaximum(self, value):
         self.spinBox.setMaximum(value)
 
     def setSingleStep(self, value):
         self.spinBox.setSingleStep(value)
 
+    def spinboxValueChangedEmitter(self):
+        """Emit the color_spinbox_value_changed signal when the spinbox value changes."""
+        self.color_spinbox_value_changed_signal.emit(self.value)
+
 class CustomToolButton(QToolButton):
     """CustomToolButton class.
 
     Custom tool button to add custom icons.
 
     If buttons are checkable, they will display a different icon when checked.
 
@@ -360,8 +368,69 @@
         name : str
             Button name.
         state : bool
             Button checked state.
         """        
         # Set the checked state of the button
         if name in self.buttons and self.buttons[name].isCheckable():
-            self.buttons[name].setChecked(state)
+            self.buttons[name].setChecked(state)
+
+    def disconnect_button_callback(self, name, callback=None):
+        """Disconnect a specific callback for a button, or all callbacks if none is specified.
+
+        Parameters
+        ----------
+        name : str
+            The name of the button whose callback should be disconnected.
+        callback : callable, optional
+            The specific callback function to disconnect. If None, all callbacks are disconnected.
+        """
+        if name in self.buttons:
+            button = self.buttons[name]
+            signal = button.toggled if button.isCheckable() else button.clicked
+            
+            if callback is not None:
+                # Disconnect a specific callback
+                try:
+                    signal.disconnect(callback)
+                except TypeError:
+                    # Callback was not connected
+                    pass
+            else:
+                # Disconnect all callbacks for the signal
+                try:
+                    signal.disconnect()
+                except TypeError:
+                    # No connections to disconnect
+                    pass
+
+    def remove_button(self, name):
+        """Remove a custom button from the toolbar, disconnecting any callbacks.
+
+        Parameters
+        ----------
+        name : str
+            The name of the button to remove.
+        """
+        if name in self.buttons:
+            # Disconnect all callbacks for the button
+            self.disconnect_button_callback(name)
+
+            button = self.buttons[name]
+            # Find the corresponding action and remove it from the toolbar
+            action = self.toolbar.widgetForAction(button.defaultAction())
+            if action:
+                self.toolbar.removeAction(button.defaultAction())
+            
+            # Hide the button as an additional precaution.
+            button.setVisible(False)
+
+            # Delete the button
+            button.deleteLater()
+
+            # Delete the button from the dictionary
+            del self.buttons[name]
+
+            # Adjust toolbar dimensions after removing the button
+            self.update_toolbar_minimum_width()
+            self.update_toolbar_height()
+
```

### Comparing `nap-plot-tools-0.0.3a0/src/nap_plot_tools.egg-info/PKG-INFO` & `nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nap-plot-tools
-Version: 0.0.3a0
+Version: 0.0.4
 Summary: A NAPari PLOTter TOOLbar and tools for additional functionalities.
 Home-page: https://github.com/zoccoler/nap-plot-tools
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/zoccoler/nap-plot-tools/issues
 Project-URL: Documentation, https://github.com/zoccoler/nap-plot-tools#README.md
```

