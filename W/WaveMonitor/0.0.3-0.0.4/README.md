# Comparing `tmp/WaveMonitor-0.0.3.tar.gz` & `tmp/wavemonitor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveMonitor-0.0.3.tar", last modified: Wed Apr 10 16:08:11 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `WaveMonitor-0.0.3.tar` & `wavemonitor-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 16:08:11.118450 WaveMonitor-0.0.3/
--rw-rw-rw-   0        0        0     1066 2024-01-29 11:15:32.000000 WaveMonitor-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       12 2024-02-08 08:53:23.000000 WaveMonitor-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2069 2024-04-10 16:08:11.118450 WaveMonitor-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1495 2024-04-10 16:00:48.000000 WaveMonitor-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 16:08:11.102841 WaveMonitor-0.0.3/WaveMonitor.egg-info/
--rw-rw-rw-   0        0        0     2069 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-10 16:08:11.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 16:08:10.000000 WaveMonitor-0.0.3/WaveMonitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 16:08:11.102841 WaveMonitor-0.0.3/assets/
--rw-rw-rw-   0        0        0    11131 2024-02-08 08:53:23.000000 WaveMonitor-0.0.3/assets/icon.png
--rw-rw-rw-   0        0        0    36100 2024-03-12 08:05:54.000000 WaveMonitor-0.0.3/assets/snapshot.png
--rw-rw-rw-   0        0        0    10884 2024-03-12 08:04:40.000000 WaveMonitor-0.0.3/assets/style.qss
--rw-rw-rw-   0        0        0    19261 2024-02-08 09:18:55.000000 WaveMonitor-0.0.3/assets/style2.qss
--rw-rw-rw-   0        0        0      640 2024-04-10 15:48:57.000000 WaveMonitor-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 16:08:11.118450 WaveMonitor-0.0.3/setup.cfg
+-rw-r--r--   0        0        0    36100 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/assets/snapshot.png
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/__init__.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/client.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/gui.py
+-rw-r--r--   0        0        0    22080 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/window.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/assets/icon.png
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/assets/style.qss
+-rw-r--r--   0        0        0    19261 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/src/wave_monitor/assets/style2.qss
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/tests/simple_usage.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/README.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 wavemonitor-0.0.4/PKG-INFO
```

### Comparing `WaveMonitor-0.0.3/LICENSE` & `wavemonitor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.3/PKG-INFO` & `wavemonitor-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,70 @@
-Metadata-Version: 2.1
-Name: WaveMonitor
-Version: 0.0.3
-Summary: A simple GUI for monitoring waveforms.
-Author-email: Qiujv <qiujv@outlook.com>
-Project-URL: Homepage, https://github.com/Qiujv/WaveMonitor
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: msgpack
-Requires-Dist: msgpack_numpy
-Requires-Dist: numpy
-Requires-Dist: pyqtgraph
-Requires-Dist: PySide6
-
-# Wave Monitor
-
-![snapshot](assets/snapshot.png)
-
-A simple GUI for monitoring waveforms. It plots waveforms with PyQtGraph in a separate process. The GUI is built with PySide6.
-
-The `WaveMonitor` class is the main interface. It provides methods for adding and removing waveforms from the plot, clearing the plot, and etc.
-
-In GUI, right click to show the menu. Keyboard shortcuts are also supported.
-
-# Installation
-
-```bash
-pip install WaveMonitor
-```
-
-or install from source.
-
-```bash
-pip install git+https://github.com/Qiujv/WaveMonitor.git
-```
-
-# Usage
-Avoid calling `clear` if you only want to update the plot. It is more efficient to update the plot with `add_wfm`.
-
-```python
-from wave_monitor import WaveMonitor
-import numpy as np
-
-monitor = WaveMonitor()
-monitor.autoscale()
-# monitor.clear()
-
-t = np.linspace(0, 1, 1_000_001)  # 1m pts ~= 1ms for 1GSa/s.
-n = 20
-i_waves = [np.cos(2 * np.pi * f * t) for f in range(1, n + 1)]
-q_waves = [np.sin(2 * np.pi * f * t) for f in range(1, n + 1)]
-
-for i, (i_wave, q_wave) in enumerate(zip(i_waves, q_waves)):
-    monitor.add_wfm(f"wave_{i}", t, [i_wave, q_wave])
-monitor.autoscale()
-
-monitor.add_wfm("wave_1", t, [i_waves[-1], q_waves[-1]])  # Replaces previous wfm.
-
-monitor.remove_wfm("wave_10")
-
-```
-
-# Thanks
-
-This project is derived from [WaveViewer](https://github.com/kahojyun/wave-viewer).
-
-The icon is downloaded from https://www.freepik.com/icons/oscilloscope and made by piksart.
+Metadata-Version: 2.3
+Name: WaveMonitor
+Version: 0.0.4
+Summary: A simple GUI for monitoring waveforms.
+Project-URL: Homepage, https://github.com/Qiujv/WaveMonitor
+Author-email: Qiujv <qiujv@outlook.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Requires-Dist: msgpack
+Requires-Dist: msgpack-numpy
+Requires-Dist: numpy
+Requires-Dist: pyqtgraph
+Requires-Dist: pyside6
+Description-Content-Type: text/markdown
+
+# Wave Monitor
+
+![snapshot](assets/snapshot.png)
+
+A simple GUI for monitoring waveforms. It plots waveforms with PyQtGraph in a separate process. The GUI is built with PySide6.
+
+The `WaveMonitor` class is the main interface. It provides methods for adding and removing waveforms from the plot, clearing the plot, and etc.
+
+In GUI, right click to show the menu. Keyboard shortcuts are also supported.
+
+# Installation
+
+```bash
+pip install WaveMonitor
+```
+
+or install from source.
+
+```bash
+pip install git+https://github.com/Qiujv/WaveMonitor.git
+```
+
+# Usage
+Avoid calling `clear` if you only want to update the plot. It is more efficient to update the plot with `add_wfm`.
+
+```python
+from wave_monitor import WaveMonitor
+import numpy as np
+
+monitor = WaveMonitor()
+monitor.autoscale()
+# monitor.clear()
+
+t = np.linspace(0, 1, 1_000_001)  # 1m pts ~= 1ms for 1GSa/s.
+n = 20
+i_waves = [np.cos(2 * np.pi * f * t) for f in range(1, n + 1)]
+q_waves = [np.sin(2 * np.pi * f * t) for f in range(1, n + 1)]
+
+for i, (i_wave, q_wave) in enumerate(zip(i_waves, q_waves)):
+    monitor.add_wfm(f"wave_{i}", t, [i_wave, q_wave])
+monitor.autoscale()
+
+monitor.add_wfm("wave_1", t, [i_waves[-1], q_waves[-1]])  # Replaces previous wfm.
+
+monitor.remove_wfm("wave_10")
+
+```
+
+# Thanks
+
+This project is derived from [WaveViewer](https://github.com/kahojyun/wave-viewer).
+
+The icon is downloaded from https://www.freepik.com/icons/oscilloscope and made by piksart.
```

### Comparing `WaveMonitor-0.0.3/README.md` & `wavemonitor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.3/assets/icon.png` & `wavemonitor-0.0.4/src/wave_monitor/assets/icon.png`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.3/assets/snapshot.png` & `wavemonitor-0.0.4/assets/snapshot.png`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.3/assets/style.qss` & `wavemonitor-0.0.4/src/wave_monitor/assets/style.qss`

 * *Files identical despite different names*

### Comparing `WaveMonitor-0.0.3/assets/style2.qss` & `wavemonitor-0.0.4/src/wave_monitor/assets/style2.qss`

 * *Files identical despite different names*

