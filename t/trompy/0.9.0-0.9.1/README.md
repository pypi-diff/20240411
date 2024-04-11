# Comparing `tmp/trompy-0.9.0.tar.gz` & `tmp/trompy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\trompy-0.9.0.tar", last modified: Fri Apr 24 10:11:03 2020, max compression
+gzip compressed data, was "dist\trompy-0.9.1.tar", last modified: Sun Apr 26 14:09:01 2020, max compression
```

## Comparing `trompy-0.9.0.tar` & `trompy-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2020-04-24 10:11:03.000000 trompy-0.9.0/
--rw-rw-rw-   0        0        0     1084 2020-04-17 07:33:54.000000 trompy-0.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2020-04-21 09:50:15.000000 trompy-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0      993 2020-04-24 10:11:03.000000 trompy-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       92 2020-04-17 07:10:47.000000 trompy-0.9.0/README.md
--rw-rw-rw-   0        0        0      101 2020-04-21 07:30:47.000000 trompy-0.9.0/README.rst
--rw-rw-rw-   0        0        0       86 2020-04-24 10:11:03.000000 trompy-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2250 2020-04-24 10:09:33.000000 trompy-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy/
--rw-rw-rw-   0        0        0     1347 2020-04-21 13:12:54.000000 trompy-0.9.0/trompy/__init__.py
--rw-rw-rw-   0        0        0    14945 2020-04-21 08:23:51.000000 trompy-0.9.0/trompy/barscatter.py
--rw-rw-rw-   0        0        0     2616 2020-04-17 14:22:20.000000 trompy-0.9.0/trompy/fig_utils.py
--rw-rw-rw-   0        0        0     4520 2020-04-21 08:26:30.000000 trompy-0.9.0/trompy/general_utils.py
--rw-rw-rw-   0        0        0      392 2020-04-20 11:46:57.000000 trompy-0.9.0/trompy/gui_utils.py
--rw-rw-rw-   0        0        0     3048 2020-04-19 12:47:23.000000 trompy-0.9.0/trompy/lick_figs.py
--rw-rw-rw-   0        0        0    21423 2020-04-20 13:56:43.000000 trompy-0.9.0/trompy/lick_gui.py
--rw-rw-rw-   0        0        0     9495 2020-04-18 18:13:36.000000 trompy-0.9.0/trompy/lick_utils.py
--rw-rw-rw-   0        0        0     2405 2020-04-17 09:19:41.000000 trompy-0.9.0/trompy/medfilereader.py
--rw-rw-rw-   0        0        0     2199 2020-04-17 09:18:33.000000 trompy-0.9.0/trompy/metafile_utils.py
--rw-rw-rw-   0        0        0    22701 2020-04-23 22:02:30.000000 trompy-0.9.0/trompy/photo_gui.py
--rw-rw-rw-   0        0        0     4788 2020-04-21 08:33:10.000000 trompy-0.9.0/trompy/roc_utils.py
--rw-rw-rw-   0        0        0    18660 2020-04-23 22:02:17.000000 trompy-0.9.0/trompy/snipper_utils.py
--rw-rw-rw-   0        0        0      717 2020-04-17 14:14:53.000000 trompy-0.9.0/trompy/stats_utils.py
--rw-rw-rw-   0        0        0     9647 2020-04-23 18:19:38.000000 trompy-0.9.0/trompy/testsnipper.py
--rw-rw-rw-   0        0        0     6675 2020-04-23 22:02:21.000000 trompy-0.9.0/trompy/trials_figs.py
-drwxrwxrwx   0        0        0        0 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy.egg-info/
--rw-rw-rw-   0        0        0      993 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2020-04-24 10:11:03.000000 trompy-0.9.0/trompy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-04-26 14:09:01.000000 trompy-0.9.1/
+-rw-rw-rw-   0        0        0     1084 2020-04-17 07:33:54.000000 trompy-0.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2020-04-21 09:50:15.000000 trompy-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      993 2020-04-26 14:09:01.000000 trompy-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2020-04-17 07:10:47.000000 trompy-0.9.1/README.md
+-rw-rw-rw-   0        0        0      101 2020-04-21 07:30:47.000000 trompy-0.9.1/README.rst
+-rw-rw-rw-   0        0        0       86 2020-04-26 14:09:01.000000 trompy-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2250 2020-04-26 14:06:14.000000 trompy-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy/
+-rw-rw-rw-   0        0        0     1347 2020-04-21 13:12:54.000000 trompy-0.9.1/trompy/__init__.py
+-rw-rw-rw-   0        0        0    14945 2020-04-21 08:23:51.000000 trompy-0.9.1/trompy/barscatter.py
+-rw-rw-rw-   0        0        0     2616 2020-04-17 14:22:20.000000 trompy-0.9.1/trompy/fig_utils.py
+-rw-rw-rw-   0        0        0     4520 2020-04-21 08:26:30.000000 trompy-0.9.1/trompy/general_utils.py
+-rw-rw-rw-   0        0        0      392 2020-04-20 11:46:57.000000 trompy-0.9.1/trompy/gui_utils.py
+-rw-rw-rw-   0        0        0     3048 2020-04-19 12:47:23.000000 trompy-0.9.1/trompy/lick_figs.py
+-rw-rw-rw-   0        0        0    21423 2020-04-20 13:56:43.000000 trompy-0.9.1/trompy/lick_gui.py
+-rw-rw-rw-   0        0        0     9495 2020-04-18 18:13:36.000000 trompy-0.9.1/trompy/lick_utils.py
+-rw-rw-rw-   0        0        0     2405 2020-04-17 09:19:41.000000 trompy-0.9.1/trompy/medfilereader.py
+-rw-rw-rw-   0        0        0     2199 2020-04-17 09:18:33.000000 trompy-0.9.1/trompy/metafile_utils.py
+-rw-rw-rw-   0        0        0    23708 2020-04-26 14:03:07.000000 trompy-0.9.1/trompy/photo_gui.py
+-rw-rw-rw-   0        0        0     4788 2020-04-21 08:33:10.000000 trompy-0.9.1/trompy/roc_utils.py
+-rw-rw-rw-   0        0        0    18660 2020-04-23 22:02:17.000000 trompy-0.9.1/trompy/snipper_utils.py
+-rw-rw-rw-   0        0        0      717 2020-04-17 14:14:53.000000 trompy-0.9.1/trompy/stats_utils.py
+-rw-rw-rw-   0        0        0     2037 2020-04-26 13:43:57.000000 trompy-0.9.1/trompy/testsnipper.py
+-rw-rw-rw-   0        0        0     6675 2020-04-23 22:02:21.000000 trompy-0.9.1/trompy/trials_figs.py
+drwxrwxrwx   0        0        0        0 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy.egg-info/
+-rw-rw-rw-   0        0        0      993 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2020-04-26 14:09:01.000000 trompy-0.9.1/trompy.egg-info/top_level.txt
```

### Comparing `trompy-0.9.0/LICENSE.txt` & `trompy-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/PKG-INFO` & `trompy-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: trompy
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of tools for data analysis and plotting that originated in the McCutcheon Lab (UiT, Tromso)
 Home-page: https://github.com/mccutcheonlab
 Author: James E McCutcheon
 Author-email: j.mccutcheon@uit.no
 License: MIT
-Download-URL: https://github.com/mccutcheonlab/trompy/archive/v0.9.0-alpha.tar.gz
+Download-URL: https://github.com/mccutcheonlab/trompy/archive/v0.9.1-alpha.tar.gz
 Description: # trompy
          Collection of tools for plotting and data analysis from McCutcheon Lab in Tromsø
         
 Keywords: neuroscience,behavior
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `trompy-0.9.0/setup.py` & `trompy-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 from distutils.core import setup
 setup(
   name = 'trompy',         # How you named your package folder (MyLib)
   packages = ['trompy'],   # Chose the same as "name"
-  version = '0.9.0',      # Start with a small number and increase it with every change you make
+  version = '0.9.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A collection of tools for data analysis and plotting that originated in the McCutcheon Lab (UiT, Tromso)',   # Give a short description about your library
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'James E McCutcheon',                   # Type in your name
   author_email = 'j.mccutcheon@uit.no',      # Type in your E-Mail
   url = 'https://github.com/mccutcheonlab',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/mccutcheonlab/trompy/archive/v0.9.0-alpha.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/mccutcheonlab/trompy/archive/v0.9.1-alpha.tar.gz',    # I explain this later on
   keywords = ['neuroscience', 'behavior'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'matplotlib',
           'xlrd',
           'scipy',
           'xlsxwriter',
```

### Comparing `trompy-0.9.0/trompy/__init__.py` & `trompy-0.9.1/trompy/__init__.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/barscatter.py` & `trompy-0.9.1/trompy/barscatter.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/fig_utils.py` & `trompy-0.9.1/trompy/fig_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/general_utils.py` & `trompy-0.9.1/trompy/general_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/lick_figs.py` & `trompy-0.9.1/trompy/lick_figs.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/lick_gui.py` & `trompy-0.9.1/trompy/lick_gui.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/lick_utils.py` & `trompy-0.9.1/trompy/lick_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/medfilereader.py` & `trompy-0.9.1/trompy/medfilereader.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/metafile_utils.py` & `trompy-0.9.1/trompy/metafile_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/photo_gui.py` & `trompy-0.9.1/trompy/photo_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,14 @@
         self.loaddataBtn.grid(column=0, row=2,rowspan=2, sticky=(N,S,E,W))
         self.filenameLbl.grid(column=0, row=4, rowspan=2, sticky=(E,W))
         self.timelockLbl.grid(column=0, row=4, rowspan=2, sticky=(E,W))
         
         self.primarysigLbl.grid(column=1, row=0)
         self.autofsigLbl.grid(column=1, row=2)
         
-        self.makelickrunsBtn.grid(column=1, row=7)
-        
         self.baselineLbl.grid(column=0, row=8, sticky=E)
         self.baselineField.grid(column=1, row=8)
         self.lengthLbl.grid(column=0, row=9, sticky=E)
         self.lengthField.grid(column=1, row=9)
         self.fsnipLbl.grid(column=0, row=10, sticky=E)
         self.fsnipField.grid(column=1, row=10)
         self.noisethLbl.grid(column=0, row=11, sticky=E)
@@ -228,20 +226,17 @@
         self.chooseeventMenu = ttk.OptionMenu(self, self.eventsVar, eventOptions[0], *eventOptions)
         self.chooseeventMenu.grid(column=0, row=6)
 
         snipOptions = ['blue', 'uv', 'filt', 'filt_z']
         self.choosesnipMenu = ttk.OptionMenu(self, self.snipsVar, snipOptions[0], *snipOptions)
         self.choosesnipMenu.grid(column=6, row=12)
    
-        onsetOptions = ['onset', 'offset']
+        onsetOptions = ['onset', 'offset', 'runs', 'random', 'notes']
         self.onsetMenu = ttk.OptionMenu(self, self.onsetVar, onsetOptions[0], *onsetOptions)
         self.onsetMenu.grid(column=1, row=6)
-
-        self.chooselicksMenu = ttk.OptionMenu(self, self.lickrunsVar, lickrunOptions[0], *lickrunOptions)
-        self.chooselicksMenu.grid(column=0, row=7)
         
     def loaddata(self):   
         self.progress['value'] = 0
         
         self.progress['value'] = 40
         # load in streams
         self.loadstreams()
@@ -348,20 +343,43 @@
         self.singletrialviewer()
         self.heatmapviewer()
         self.averagesnipsviewer()
         self.sessionviewer()
         
     def setevents(self):
         try:
-            if 'runs' in self.eventsVar.get():
-                key=self.eventsVar.get().split('-')
-                self.events = self.runs[key[1]]
-            else:
-                self.eventepoc = getattr(self.epocs, self.eventsVar.get())
-                self.events = getattr(self.eventepoc, self.onsetVar.get())
+            self.eventepoc = getattr(self.epocs, self.eventsVar.get())
+            if self.onsetVar.get() == 'onset' or self.onsetVar.get() == 'offset':
+                try:
+                   self.events = getattr(self.eventepoc, self.onsetVar.get())
+                except AttributeError:
+                    alert(f'{self.eventsVar.get()} does not have {self.onsetVar.get()}')
+            elif self.onsetVar.get() == 'runs':
+                try:
+                    tmp = getattr(self.eventepoc, 'onset')
+                    self.events = [val for i, val in enumerate(tmp) if (val - tmp[i-1]) > float(self.baseline.get())]
+                except:
+                    alert(f'Cannot calculate runs for {self.eventsVar.get()}')
+            elif self.onsetVar.get() == 'random':
+                try:
+                    nevents = len(getattr(self.eventepoc, 'onset'))
+                    if nevents > 100:
+                        nevents = 100
+                    elif nevents < 10:
+                        nevents = 10
+                except AttributeError:
+                    nevents = 30
+                print(f'Creating {nevents} random events.')
+                self.events = list(np.sort(np.random.randint(low=120, high=int(len(self.data)/self.fs)-120, size=30)))
+            elif self.onsetVar.get() == 'notes':
+                try:
+                    self.events = self.eventepoc.notes.ts
+                except:
+                    alert('Could not find notes.')
+                    
         except:
             alert('Cannot set events')
             
     def setlicks(self):
         try:
             self.lickepoc = getattr(self.epocs, self.lickrunsVar.get())
             self.licks = getattr(self.lickepoc, self.onsetVar.get())
```

### Comparing `trompy-0.9.0/trompy/roc_utils.py` & `trompy-0.9.1/trompy/roc_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/snipper_utils.py` & `trompy-0.9.1/trompy/snipper_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/stats_utils.py` & `trompy-0.9.1/trompy/stats_utils.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy/trials_figs.py` & `trompy-0.9.1/trompy/trials_figs.py`

 * *Files identical despite different names*

### Comparing `trompy-0.9.0/trompy.egg-info/PKG-INFO` & `trompy-0.9.1/trompy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: trompy
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of tools for data analysis and plotting that originated in the McCutcheon Lab (UiT, Tromso)
 Home-page: https://github.com/mccutcheonlab
 Author: James E McCutcheon
 Author-email: j.mccutcheon@uit.no
 License: MIT
-Download-URL: https://github.com/mccutcheonlab/trompy/archive/v0.9.0-alpha.tar.gz
+Download-URL: https://github.com/mccutcheonlab/trompy/archive/v0.9.1-alpha.tar.gz
 Description: # trompy
          Collection of tools for plotting and data analysis from McCutcheon Lab in Tromsø
         
 Keywords: neuroscience,behavior
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `trompy-0.9.0/trompy.egg-info/SOURCES.txt` & `trompy-0.9.1/trompy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

