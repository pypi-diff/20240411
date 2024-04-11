# Comparing `tmp/cubestat-0.2.6.tar.gz` & `tmp/cubestat-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.2.6.tar", last modified: Fri Apr  5 15:22:24 2024, max compression
+gzip compressed data, was "cubestat-0.2.7.tar", last modified: Thu Apr 11 19:26:00 2024, max compression
```

## Comparing `cubestat-0.2.6.tar` & `cubestat-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.697566 cubestat-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 15:22:18.000000 cubestat-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 15:22:24.693566 cubestat-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-05 15:22:18.000000 cubestat-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.693566 cubestat-0.2.6/cubestat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15607 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.693566 cubestat-0.2.6/cubestat/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/free_swap_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/linux_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/macos_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/mem_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/nv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/swapusage_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.693566 cubestat-0.2.6/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:22:24.697566 cubestat-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 15:22:18.000000 cubestat-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:26:00.820533 cubestat-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 19:25:53.000000 cubestat-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 19:26:00.816532 cubestat-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-11 19:25:53.000000 cubestat-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:26:00.816532 cubestat-0.2.7/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17333 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:26:00.816532 cubestat-0.2.7/cubestat/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/free_swap_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/linux_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/macos_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/mem_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/nv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-11 19:25:53.000000 cubestat-0.2.7/cubestat/readers/swapusage_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:26:00.816532 cubestat-0.2.7/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 19:26:00.000000 cubestat-0.2.7/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-11 19:26:00.000000 cubestat-0.2.7/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:26:00.000000 cubestat-0.2.7/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 19:26:00.000000 cubestat-0.2.7/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 19:26:00.000000 cubestat-0.2.7/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 19:26:00.000000 cubestat-0.2.7/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:26:00.820533 cubestat-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 19:25:53.000000 cubestat-0.2.7/setup.py
```

### Comparing `cubestat-0.2.6/LICENSE` & `cubestat-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.6/README.md` & `cubestat-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.6/cubestat/cubestat.py` & `cubestat-0.2.7/cubestat/cubestat.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse
 import collections
 import curses
 import itertools
 import os
 import sys
+import math
 
 from enum import Enum
 from math import floor
 from threading import Thread, Lock
 
 from cubestat.readers.linux_reader import LinuxReader
 from cubestat.readers.macos_reader import AppleReader
@@ -19,45 +20,56 @@
         values = list(self.__class__)
         return values[(values.index(self) + 1) % len(values)]
     
 class EnumStr(Enum):
     def __str__(self):
         return self.value
 
-class Percentages(EnumLoop, EnumStr):
-    hidden = 'hidden'
+class Legend(EnumLoop, EnumStr):
+    hidden = 'off'
     last = 'last'
     
 class CPUMode(EnumLoop, EnumStr):
     all = 'all'
     by_cluster = 'by_cluster'
     by_core = 'by_core'
 
+class PowerMode(EnumLoop, EnumStr):
+    combined = 'combined'
+    all = 'all'
+    off = 'off'
+
 class GPUMode(EnumLoop, EnumStr):
     collapsed = 'collapsed'
     load_only = 'load_only'
     load_and_vram = 'load_and_vram'
     
 class Color(EnumStr):
     red = 'red'
     green = 'green'
     blue = 'blue'
     pink = 'pink'
+    olive = 'olive'
+    navy = 'navy'
+    blue_dark = 'blue_dark'
+    purple = 'purple'
     mixed = 'mixed'
+    dark = 'dark'
 
 def auto_cpu_mode():
      return CPUMode.all if os.cpu_count() < 40 else CPUMode.by_cluster
 
 parser = argparse.ArgumentParser("cubestat")
 parser.add_argument('--refresh_ms', '-i', type=int, default=1000, help='Update frequency, milliseconds')
 parser.add_argument('--buffer_size', type=int, default=500, help='How many datapoints to store. Having it larger than screen width is a good idea as terminal window can be resized')
 parser.add_argument('--cpu', type=CPUMode, default=auto_cpu_mode(), choices=list(CPUMode), help='CPU mode - showing all cores, only cumulative by cluster or both. Can be toggled by pressing c.')
 parser.add_argument('--gpu', type=GPUMode, default=GPUMode.load_only, choices=list(GPUMode), help='GPU mode - hidden, showing all GPUs load, or showing load and vram usage. Can be toggled by pressing g.')
+parser.add_argument('--power', type=PowerMode, default=PowerMode.combined, choices=list(PowerMode), help='Power mode - off, showing breakdown CPU/GPU/ANE load, or showing combined usage. Can be toggled by pressing p.')
 parser.add_argument('--color', type=Color, default=Color.mixed, choices=list(Color))
-parser.add_argument('--percentages', type=Percentages, default=Percentages.last, choices=list(Percentages), help='Show/hide numeric utilization percentage. Can be toggled by pressing p.')
+parser.add_argument('--legend', type=Legend, default=Legend.last, choices=list(Legend), help='Show/hide numeric utilization percentage. Can be toggled by pressing l.')
 parser.add_argument('--disk', action="store_true", default=True, help="Show disk read/write. Can be toggled by pressing d.")
 parser.add_argument('--swap', action="store_true", default=True, help="Show swap . Can be toggled by pressing s.")
 parser.add_argument('--network', action="store_true", default=True, help="Show network io. Can be toggled by pressing n.")
 parser.add_argument('--no-disk', action="store_false", dest="disk", help="Hide disk read/write. Can be toggled by pressing d.")
 parser.add_argument('--no-swap', action="store_false", default=True, help="Hide swap. Can be toggled by pressing s.")
 parser.add_argument('--no-network', action="store_false", dest="network", help="Hide network io. Can be toggled by pressing n.")
 
@@ -75,44 +87,67 @@
         self.filling = '.'
 
         self.cells = self.prepare_cells()
         self.stdscr = stdscr
 
         # all of the fields below are mutable and can be accessed from 2 threads
         self.lock = Lock()
-        self.data = {k: collections.defaultdict(lambda: collections.deque(maxlen=args.buffer_size)) for k in ['cpu', 'ram', 'swap', 'gpu', 'ane', 'disk', 'network']}
-        self.colormap = {
-            'cpu': Color.green if args.color == Color.mixed else args.color,
-            'ram': Color.pink if args.color == Color.mixed else args.color,
-            'gpu': Color.red if args.color == Color.mixed else args.color,
-            'ane': Color.red if args.color == Color.mixed else args.color,
-            'disk': Color.blue if args.color == Color.mixed else args.color,
-            'network': Color.blue if args.color == Color.mixed else args.color,
-            'swap': Color.pink if args.color == Color.mixed else args.color,
+        self.data = {k: collections.defaultdict(lambda: collections.deque(maxlen=args.buffer_size)) for k in ['cpu', 'ram', 'swap', 'gpu', 'ane', 'disk', 'network', 'power']}
+        dark_colormap = {
+            'cpu': Color.purple,
+            'ram': Color.navy,
+            'gpu': Color.blue_dark,
+            'ane': Color.blue_dark,
+            'disk': Color.olive,
+            'network': Color.olive,
+            'swap': Color.navy,
+            'power': Color.blue_dark,
         }
+        light_colormap = {
+            'cpu': Color.green,
+            'ram': Color.pink,
+            'gpu': Color.red,
+            'ane': Color.red,
+            'disk': Color.blue,
+            'network': Color.blue,
+            'swap': Color.pink,
+            'power': Color.red,
+        }
+
+        if args.color == Color.mixed:
+            self.colormap = light_colormap
+        elif args.color == Color.dark:
+            self.colormap = dark_colormap
+        else:
+            self.colormap = {k: args.color for k, _ in light_colormap.items()}
         self.snapshots_observed = 0
         self.snapshots_rendered = 0
-        self.percentage_mode = args.percentages
+        self.legend_mode = args.legend
         self.cpumode = args.cpu
         self.show_disk = args.disk
         self.show_swap = args.swap
         self.show_network = args.network
+        self.power_mode = args.power
         self.gpumode = args.gpu
         self.settings_changed = False
         self.reader = reader
         self.vertical_shift = 0
         self.horizontal_shift = 0
 
     def prepare_cells(self):
         chrs = [' ', '▁', '▂', '▃', '▄', '▅', '▆', '▇', '█']
         colorschemes = {
             Color.green: [-1, 150, 107, 22],
             Color.red: [-1, 224, 181, 138],
             Color.blue: [-1, 189, 146, 103],
             Color.pink: [-1, 223, 180, 137],
+            Color.olive: [-1, 58, 101, 144],
+            Color.navy: [-1, 18, 61, 105],
+            Color.blue_dark: [-1, 23, 66, 109],
+            Color.purple: [-1, 53, 96, 138]
         }
         cells = {}
         colorpair = 1
         for name, colors in colorschemes.items():
             cells[name] = []
             for fg, bg in zip(colors[1:], colors[:-1]):
                 curses.init_pair(colorpair, fg, bg)
@@ -150,15 +185,15 @@
             self.stdscr.addch(row, col, chr, color)
         except:
             # TODO: log something
             pass
 
     # buckets is a list of factor/label, e.g. [(1024*1024, 'Mb'), (1024, 'Kb'), (1, 'b')]
     def format_measurement(self, spacing, curr, mx, buckets):
-        if self.percentage_mode != Percentages.last:
+        if self.legend_mode != Legend.last:
             return f'{spacing}╗'
         for lim, unit in buckets[:-1]:
             if mx > lim:
                 return f'last:{curr / lim :3.0f}|{int(mx / lim)}{unit}{spacing}╗'
         return f'last:{curr :3.0f}|{int(mx)}{buckets[-1][1]}{spacing}╗'
 
     def render(self):
@@ -201,14 +236,22 @@
                     if group_name == 'gpu':
                         if is_multigpu and self.gpumode == GPUMode.collapsed and "Total GPU" not in title:
                             continue
                         if self.gpumode == GPUMode.load_only and "vram" in title:
                             continue
                         if is_multigpu and "Total GPU" not in title:
                             indent = '  '
+
+                    if group_name == 'power':
+                        if self.power_mode == PowerMode.off:
+                            continue
+                        if self.power_mode == PowerMode.combined and 'total' not in title:
+                            continue
+                        if 'total' not in title:
+                            indent = '  '
                     
                     if skip > 0:
                         skip -= 1
                         continue
 
                     # render title and left border, for example
                     #
@@ -224,25 +267,30 @@
                     # chart area width
                     width = self.cols - 2 * self.spacing_width - 2 - len(indent)
                     index = max(0, length - width)
                     data_slice = list(itertools.islice(series, index, min(index + width, length)))
 
                     # for percentage-like measurements
                     B = 100.0
-                    strvalue = f'last:{data_slice[-1]:3.0f}%{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
+                    strvalue = f'last:{data_slice[-1]:3.0f}%{spacing}╗' if self.legend_mode == Legend.last else f'{spacing}╗'
                     
                     if group_name == 'disk' or group_name == 'network':
                         B = max(data_slice)
                         B = float(1 if B == 0 else 2 ** (int((B - 1)).bit_length()))
-                        strvalue = self.format_measurement(spacing, data_slice[-1], B, [(1024 * 1024, 'Mb/s'), (1024, 'Kb/s'), (1, 'bytes/s')])
+                        strvalue = self.format_measurement(spacing, data_slice[-1], B, [(1024 * 1024, 'MB/s'), (1024, 'KB/s'), (1, 'Bytes/s')])
 
                     if group_name == 'swap':
                         B = max(data_slice)
                         B = float(1 if B == 0 else 2 ** (int((B - 1)).bit_length()))
-                        strvalue = self.format_measurement(spacing, data_slice[-1], B, [(1024 * 1024, 'Mb'), (1024, 'Kb'), (1, 'bytes')])
+                        strvalue = self.format_measurement(spacing, data_slice[-1], B, [(1024 * 1024, 'MB'), (1024, 'KB'), (1, 'Bytes')])
+
+                    if group_name == 'power':
+                        B = max(data_slice)
+                        B = float(1 if B <= 0 else 10 ** math.ceil(math.log10(B)))
+                        strvalue = self.format_measurement(spacing, data_slice[-1], B, [(1000 * 1000, 'kW'), (1000, 'W'), (1, 'mW')])
 
                     # render the rest of title row
                     #
                     # ╔ GPU util %........................................................................last:  4% ╗
                     # ╚
                     title_filling = self.filling * (self.cols - len(strvalue) - len(titlestr))
                     self.write_string(i * 2, len(titlestr), title_filling)
@@ -280,22 +328,26 @@
     def render_loop(self):
         self.stdscr.keypad(True)
         while True:
             self.render()
             key = self.stdscr.getch()
             if key == ord('q') or key == ord('Q'):
                 exit(0)
-            if key == ord('p'):
+            if key == ord('l'):
                 with self.lock:
-                    self.percentage_mode = self.percentage_mode.next()
+                    self.legend_mode = self.legend_mode.next()
                     self.settings_changed = True
             if key == ord('c'):
                 with self.lock:
                     self.cpumode = self.cpumode.next()
                     self.settings_changed = True
+            if key == ord('p'):
+                with self.lock:
+                    self.power_mode = self.power_mode.next()
+                    self.settings_changed = True
             if key == ord('g'):
                 with self.lock:
                     self.gpumode = self.gpumode.next()
                     self.settings_changed = True
             if key == ord('s'):
                 with self.lock:
                     self.show_swap = not self.show_swap
```

### Comparing `cubestat-0.2.6/cubestat/readers/free_swap_reader.py` & `cubestat-0.2.7/cubestat/readers/free_swap_reader.py`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.6/cubestat/readers/linux_reader.py` & `cubestat-0.2.7/cubestat/readers/linux_reader.py`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.6/cubestat/readers/macos_reader.py` & `cubestat-0.2.7/cubestat/readers/macos_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     ane_power_scalers = {
         "M1": 13000.0,
         "M2": 15500.0,
         "M3": 15500.0,
     }
 
     def __init__(self, interval_ms) -> None:
-        # identity the model to get ANE power scaler
+        # identity the model to get ANE scaler
         brand_str = subprocess.check_output(['sysctl', '-n', 'machdep.cpu.brand_string'], text=True)
         self.ane_scaler = 15500 # default to M2
         for k, v in self.ane_power_scalers.items():
             if k in brand_str:
                 self.ane_scaler = v
-                if 'Ultra' in brand_str:
+                if 'ultra' in brand_str.lower():
                     self.ane_scaler *= 2
                 break
         
         cmd = ['sudo', 'powermetrics', '-f', 'plist', '-i', str(interval_ms), '-s', 'cpu_power,gpu_power,ane_power,network,disk']
         self.powermetrics = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         # we are getting first line here to allow user to enter sudo credentials before 
         # curses initialization.
@@ -52,15 +52,20 @@
                 res['cpu'][title] = 100.0 - 100.0 * cpu['idle_ratio']
                 idle_cluster += cpu['idle_ratio']
                 total_cluster += 1.0
             res['cpu'][cluster_title] = 100.0 - 100.0 * idle_cluster / total_cluster
 
         res['gpu']['GPU util %'] = 100.0 - 100.0 * snapshot['gpu']['idle_ratio']
         
-        res['ane']['ANE util %'] = 100.0 * snapshot['processor']['ane_energy'] / self.ane_scaler
+        res['ane']['ANE util %'] = 100.0 * snapshot['processor']['ane_power'] / self.ane_scaler
+
+        res['power']['total power'] = snapshot['processor']['combined_power']
+        res['power']['ANE power'] = snapshot['processor']['ane_power']
+        res['power']['CPU power'] = snapshot['processor']['cpu_power']
+        res['power']['GPU power'] = snapshot['processor']['gpu_power']
 
         res['disk']['disk read'] = snapshot['disk']['rbytes_per_s']
         res['disk']['disk write'] = snapshot['disk']['wbytes_per_s']
         res['network']['network rx'] = snapshot['network']['ibyte_rate']
         res['network']['network tx'] = snapshot['network']['obyte_rate']
         return res.items(), cpu_clusters
```

### Comparing `cubestat-0.2.6/cubestat/readers/nv_reader.py` & `cubestat-0.2.7/cubestat/readers/nv_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,14 @@
         if self.has_nvidia:
             n_gpus = 0
             for i, v in enumerate(self.nvsmi.DeviceQuery('utilization.gpu,memory.total,memory.used')['gpu']):
                 res[f'GPU {i} util %'] = v['utilization']['gpu_util']
                 total += v['utilization']['gpu_util']
                 res[f'GPU {i} vram used %'] = 100.0 * v['fb_memory_usage']['used'] / v['fb_memory_usage']['total']
                 n_gpus += 1
-        if n_gpus > 1:
-            combined = {}
-            combined[f'[{n_gpus}] Total GPU util %'] = total / n_gpus
-            for k, v in res.items():
-                combined[k] = v
-            return combined
+            if n_gpus > 1:
+                combined = {}
+                combined[f'[{n_gpus}] Total GPU util %'] = total / n_gpus
+                for k, v in res.items():
+                    combined[k] = v
+                return combined
         return res
```

### Comparing `cubestat-0.2.6/cubestat/readers/swapusage_reader.py` & `cubestat-0.2.7/cubestat/readers/swapusage_reader.py`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.6/setup.py` & `cubestat-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.2.6',
+    version='0.2.7',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for system monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE/RAM/swap/IO monitoring for Apple M1/M2/M3, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
```

