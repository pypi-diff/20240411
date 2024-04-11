# Comparing `tmp/mly_pipeline-1.0.2.tar.gz` & `tmp/mly_pipeline-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-1.0.2.tar", last modified: Wed Feb 21 14:22:12 2024, max compression
+gzip compressed data, was "mly_pipeline-1.0.3.tar", last modified: Thu Apr 11 09:10:05 2024, max compression
```

## Comparing `mly_pipeline-1.0.2.tar` & `mly_pipeline-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-02-21 14:22:12.194237 mly_pipeline-1.0.2/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      151 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2190 2024-02-15 14:45:05.000000 mly_pipeline-1.0.2/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-07-24 14:34:35.000000 mly_pipeline-1.0.2/LICENSE
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1307 2024-02-21 14:22:12.193237 mly_pipeline-1.0.2/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      800 2024-01-16 16:04:52.000000 mly_pipeline-1.0.2/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-02-21 14:22:12.114236 mly_pipeline-1.0.2/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-02-21 14:22:12.128236 mly_pipeline-1.0.2/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5972 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2356 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2102 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2737 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/runningasearchoffline.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13544 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/runningasearchonline.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14888 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-02-21 14:22:12.178237 mly_pipeline-1.0.2/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-1.0.2/mly_pipeline/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      411 2024-02-21 14:22:11.000000 mly_pipeline-1.0.2/mly_pipeline/_version.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28615 2024-02-15 14:47:33.000000 mly_pipeline-1.0.2/mly_pipeline/continuous_FAR.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-1.0.2/mly_pipeline/continuous_FAR_test.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9042 2024-02-21 14:16:51.000000 mly_pipeline-1.0.2/mly_pipeline/create_status_page.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    43507 2024-02-20 15:51:57.000000 mly_pipeline-1.0.2/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13912 2023-09-22 09:55:30.000000 mly_pipeline-1.0.2/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28169 2024-02-21 14:16:51.000000 mly_pipeline-1.0.2/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7304 2024-01-10 15:17:08.000000 mly_pipeline-1.0.2/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20565 2024-02-20 15:51:57.000000 mly_pipeline-1.0.2/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    15221 2024-02-21 14:16:51.000000 mly_pipeline-1.0.2/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49631 2024-02-15 14:47:33.000000 mly_pipeline-1.0.2/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-02-21 14:22:12.189237 mly_pipeline-1.0.2/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-1.0.2/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-24 14:34:35.000000 mly_pipeline-1.0.2/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-02-21 14:22:12.191237 mly_pipeline-1.0.2/mly_pipeline.egg-info/
--rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1307 2024-02-21 14:22:12.000000 mly_pipeline-1.0.2/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      952 2024-02-21 14:22:12.000000 mly_pipeline-1.0.2/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2024-02-21 14:22:12.000000 mly_pipeline-1.0.2/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      326 2024-02-21 14:22:12.000000 mly_pipeline-1.0.2/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       63 2024-02-21 14:22:12.000000 mly_pipeline-1.0.2/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2024-02-21 14:22:12.000000 mly_pipeline-1.0.2/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1495 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      467 2024-01-19 15:08:50.000000 mly_pipeline-1.0.2/requirements.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2024-02-21 14:22:12.194237 mly_pipeline-1.0.2/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:10:05.359153 mly_pipeline-1.0.3/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      151 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2190 2024-02-15 14:45:05.000000 mly_pipeline-1.0.3/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-07-24 14:34:35.000000 mly_pipeline-1.0.3/LICENSE
+-rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1307 2024-04-11 09:10:05.348153 mly_pipeline-1.0.3/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      800 2024-01-16 16:04:52.000000 mly_pipeline-1.0.3/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:10:05.249152 mly_pipeline-1.0.3/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:10:05.274152 mly_pipeline-1.0.3/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5972 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      924 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2356 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2102 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2737 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/runningasearchoffline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13544 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/runningasearchonline.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14888 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:10:05.312152 mly_pipeline-1.0.3/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-1.0.3/mly_pipeline/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      411 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline/_version.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28615 2024-04-09 10:49:26.000000 mly_pipeline-1.0.3/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-1.0.3/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10174 2024-04-11 08:54:04.000000 mly_pipeline-1.0.3/mly_pipeline/create_status_page.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    44628 2024-04-09 16:16:56.000000 mly_pipeline-1.0.3/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13912 2023-09-22 09:55:30.000000 mly_pipeline-1.0.3/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    30627 2024-04-09 14:57:09.000000 mly_pipeline-1.0.3/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9904 2024-04-11 08:51:59.000000 mly_pipeline-1.0.3/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20565 2024-04-09 10:49:26.000000 mly_pipeline-1.0.3/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16138 2024-04-09 13:52:15.000000 mly_pipeline-1.0.3/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    53802 2024-04-09 11:18:37.000000 mly_pipeline-1.0.3/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:10:05.336153 mly_pipeline-1.0.3/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-1.0.3/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-24 14:34:35.000000 mly_pipeline-1.0.3/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2024-04-11 09:10:05.345153 mly_pipeline-1.0.3/mly_pipeline.egg-info/
+-rw-r--r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1307 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      952 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      326 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       63 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2024-04-11 09:10:05.000000 mly_pipeline-1.0.3/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1495 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      467 2024-01-19 15:08:50.000000 mly_pipeline-1.0.3/requirements.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2024-04-11 09:10:05.359153 mly_pipeline-1.0.3/setup.cfg
```

### Comparing `mly_pipeline-1.0.2/.gitlab-ci.yml` & `mly_pipeline-1.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/LICENSE` & `mly_pipeline-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/PKG-INFO` & `mly_pipeline-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 1.0.2
+Version: 1.0.3
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-1.0.2/README.md` & `mly_pipeline-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/Makefile` & `mly_pipeline-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/conf.py` & `mly_pipeline-1.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/index.rst` & `mly_pipeline-1.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/installation.rst` & `mly_pipeline-1.0.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/runningasearch.rst` & `mly_pipeline-1.0.3/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/runningasearchoffline.rst` & `mly_pipeline-1.0.3/docs/source/runningasearchoffline.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/runningasearchonline.rst` & `mly_pipeline-1.0.3/docs/source/runningasearchonline.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/docs/source/settingupasearch.rst` & `mly_pipeline-1.0.3/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/__init__.py` & `mly_pipeline-1.0.3/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/continuous_FAR.py` & `mly_pipeline-1.0.3/mly_pipeline/continuous_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/continuous_FAR_test.py` & `mly_pipeline-1.0.3/mly_pipeline/continuous_FAR_test.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/create_status_page.py` & `mly_pipeline-1.0.3/mly_pipeline/create_status_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,61 +28,85 @@
     return directory+'/'+jsonfile
 
 def make_clickable(url, name):
     return '<a href="{}" rel="noopener noreferrer" target="_blank">{}</a>'.format(url,name)
 
 def create_event_table(search_path,format='html',):
 
+    with open('config.json') as json_file:
+        config = json.load(json_file)
+
+    if config['trigger_destination'] in ['test','playground']:
+        url = "https://gracedb-"+config['trigger_destination']+".ligo.org"
+        print("Current trigger_destination url is :"+url)
+            
+        config['trigger_destination'] = url
+
+    elif config['trigger_destination'] == 'online':
+        url = "https://gracedb-test.ligo.org"
+        print("Current trigger_destination url is :"+url)
+
+    else:
+        url = ''
+        print("No real url to be used")
+
     pd_table = None
 
     triggers_directory = f"{search_path}/trigger_directory"
 
     events = os.listdir(triggers_directory)
     if len(events)!=0:
         for event_dir in events:
             
             event_name = event_dir.split('-')[0]
             json_file_path = find_json_file(triggers_directory+'/'+event_dir)
 
             with open(json_file_path) as json_file:
                 event_info = json.load(json_file)
 
-
             event_info['datetime'] = str(from_gps(event_info['central_time'] ))
 
             del event_info['scores']
             del event_info['gpstime']
             del event_info['channels']
-
+            del event_info['instance_start_time']
+            del event_info['start_time']
+            del event_info['end_time']
+            del event_info['start_frequency']
+            del event_info['end_frequency']
+            
             file_prefix = json_file_path.split('/')[-1][:-5]
 
             event_info['ifos'] = ''.join(event_info['ifos'])
             event_info['far'] = f"{event_info['far']:.4e}"
             event_info['SNR'] = f"{event_info['SNR']:.2f}"
             event_info['central_time'] = f"{event_info['central_time']:.3f}"
             event_info['central_freq'] = f"{event_info['central_freq']:.1f} Hz"
             event_info['duration'] = f"{event_info['duration']:.5f} sec"
             event_info['bandwidth'] = f"{event_info['bandwidth']:.1f} Hz"
 
 
             event_info['GraceDB_ID'] = event_name
-            event_info['GraceDB_ID_url'] = f"https://gracedb-test.ligo.org/events/{event_name}/view/"
+            event_info['GraceDB_ID_url'] = f"{url}/events/{event_name}/view/"
 
+            event_info['summary_url'] = f"trigger_directory/{event_dir}/{file_prefix}_summary.png"
             event_info['strain_plot_url'] = f"trigger_directory/{event_dir}/{file_prefix}_strain.png"
             event_info['tf_map_url'] = f"trigger_directory/{event_dir}/{file_prefix}_tfmap.png"
             event_info['correlation_plot_url'] = f"trigger_directory/{event_dir}/{file_prefix}_correlation.png"
             event_info['skymap_url'] = f"trigger_directory/{event_dir}/{file_prefix}_skymap.png"
 
+            event_info['Summary'] = "link"
             event_info['Timeseries'] = "link"
             event_info['TFmap'] = "link"
             event_info['Correlation'] = "link"
             event_info['Skymap'] = "link"
 
             columns = list(event_info.keys())
             columns.insert(0, columns.pop(columns.index('datetime')))
+            columns.insert(0, columns.pop(columns.index('ifos')))
             columns.insert(0, columns.pop(columns.index('GraceDB_ID')))
 
 
 
             if pd_table is None:
 
                 pd_table = pd.DataFrame(event_info,index=[0])
@@ -92,25 +116,28 @@
                 pd_table = pd.concat([pd_table,event_info],ignore_index=True)
                 
 
         pd_table= pd_table[columns]
         pd_table= pd_table.sort_values(by='central_time',ignore_index=True,ascending=False)
 
         pd_table['GraceDB_ID'] = pd_table.apply(lambda x: make_clickable(x['GraceDB_ID_url'], x['GraceDB_ID']), axis=1)
+        pd_table['Summary'] = pd_table.apply(lambda x: make_clickable(x['summary_url'], x['Summary']), axis=1)
         pd_table['Timeseries'] = pd_table.apply(lambda x: make_clickable(x['strain_plot_url'], x['Timeseries']), axis=1)
         pd_table['Correlation'] = pd_table.apply(lambda x: make_clickable(x['correlation_plot_url'], x['Correlation']), axis=1)
         pd_table['TFmap'] = pd_table.apply(lambda x: make_clickable(x['tf_map_url'], x['TFmap']), axis=1)
         pd_table['Skymap'] = pd_table.apply(lambda x: make_clickable(x['skymap_url'], x['Skymap']), axis=1)
 
 
         del pd_table['GraceDB_ID_url']
+        del pd_table['summary_url']
         del pd_table['strain_plot_url']
         del pd_table['correlation_plot_url']
         del pd_table['tf_map_url']
         del pd_table['skymap_url']
+        
 
         pd_table= pd_table.set_index('GraceDB_ID')
 
         if format=='html':
             pd_table = pd_table.style.to_html(index=False,classes='center')
 
     else:
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline/initialization.py` & `mly_pipeline-1.0.3/mly_pipeline/initialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
             
             # Collection of the process ids of the scripts
             f.write("    processID=()"+ "\n")
             # Used to sinchronise the independent scripts of the search
             f.write("    unixtime=$(date +%s)" + "\n")
             # The number of paralel schripts to run 
             # !Note: If you change this from the config, you will have to 
-            #        edit in the runall.sh script by hand.
-            f.write("    STEP="+str(kwargs['parallel_scripts'])+ "\n\n")
+            #        edit in the runall.sh script by hand.CD ..
+            f.write("    STEP="+"$(jq -r '.parallel_scripts' config.json)"+ "\n\n")
             
             # Lopp to run the scripts for the search
             f.write("    for INITIAL in `seq 0 $(($STEP-1))`" + "\n")
             f.write("    do" + "\n\n")
             f.write("        nohup python -m mly_pipeline.search"
                              +" --splitter [$STEP,$INITIAL]"
                              +" --time_reference $unixtime" 
@@ -517,15 +517,17 @@
                           DEFAULT_ONLINE = {}
 
                         , DEFAULT_OFFLINE = {}
 
                         , O4_ONLINE = {"H":"H1:GDS-CALIB_STATE_VECTOR"
                                       ,"L":"L1:GDS-CALIB_STATE_VECTOR"
                                       ,"V":"V1:DQ_ANALYSIS_STATE_VECTOR"}
-                        , O3MDC_ONLINE = {}
+                        , O3MDC_ONLINE = {"H":"H1:GDS-CALIB_STATE_VECTOR"
+                                      ,"L":"L1:GDS-CALIB_STATE_VECTOR"
+                                      ,"V":"V1:DQ_ANALYSIS_STATE_VECTOR"}
                         , O3REPLAY_ONLINE = {}
                         )
 
     active_flags_dict = dict( 
                           DEFAULT_ONLINE = {"H":"" ,"L":"" ,"V":""}
 
                         , DEFAULT_OFFLINE = {"H": "H1:DMT-ANALYSIS_READY:1"
@@ -550,18 +552,42 @@
                                 
 
     if kwargs['search_mode'] == "BENCHMARK_MDC_OFFLINE":
         segment_list_default = "/home/vasileios.skliris/public_html/benchmark_segments.txt"
     else:
         segment_list_default = []
 
-    if len(kwargs['detectors'])==3:
-        skymap_config = dict(alpha = 2.2, beta = 1.0, sigma = 161.1 ,nside =64)
-    elif len(kwargs['detectors'])==2:
-        skymap_config = dict(alpha = 1.3, beta = 1.0, sigma = 35.9 ,nside =64)
+    if len(kwargs['detectors'])==3: # Needs to be reevaluated
+        skymap_config = dict(alpha = 2.2
+                           , beta = 1.0
+                           , sigma = 161.1 
+                           , nside =64
+                           , ramp_duration = 1/16
+                           , ramp_center = 0
+                           , duration_limit = 1/32)
+                           
+    elif len(kwargs['detectors'])==2: 
+        if 'O3' in kwargs['search_mode']:
+            skymap_config = dict(alpha = 2.0
+                            , beta = 1.0
+                            , sigma = 25.0 
+                            , nside =64
+                            , ramp_duration = 1/16
+                            , ramp_center = 0
+                            , duration_limit = 1/32)
+
+        else:
+            skymap_config = dict(alpha = 3.7
+                                , beta = 1.0
+                                , sigma = 20.5 
+                                , nside =64
+                                , ramp_duration = 1/16
+                                , ramp_center = 0
+                                , duration_limit = 1/32)
+
 
     # # # # # # # CONFIG FILE # # # # # # #
 
     configuration = dict(
         
 
     # Mode that creates some presets if used
@@ -628,18 +654,18 @@
     # Number of seconds to wait between each read attempt.
     wait=0.5,
         
     # Number of seconds required for PSD calculation.
     required_buffer=16,  
         
     # Number of seconds before current GPS time to begin search.
-    start_lag=92,
+    start_lag=64,
         
     # If search time is left behind by that amount of seconds it skips ahead.
-    gps_reset_time=32,
+    gps_reset_time=128,
         
     # FAR file that is used to calculate FAR. It is used only at
     # the beggining of the search, until there is enough background estimation.
     
     farfile= ("/home/vasileios.skliris/mly-hermes/outputs/FARfile" if ('ONLINE' in kwargs['search_mode']) else kwargs["falseAlarmRates"]+"/FARfile" ),
     
     # # # Models
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-1.0.3/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/manager.py` & `mly_pipeline-1.0.3/mly_pipeline/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import random
 
 from mly.tools import dirlist
 from mly.datatools import *
 from .search_functions import *
 from dqsegdb2.query import query_segments
 from gwpy.segments import Segment, SegmentList, DataQualityFlag
-from gwpy.time import from_gps, to_gps
+from gwpy.time import from_gps, to_gps, tconvert
 from datetime import datetime
 
 
 # # # Managing arguments
 # 
 # List of arguments to pass:
 arguments = [
@@ -74,289 +74,236 @@
 ch.setFormatter(formatter)
 
 # add ch to logger
 logger.addHandler(ch)
 
 
 
+def manage_output_directory(config=None):
 
+    output_directory = config['output_directory']
+    maxDataFrameSize = config['maxDataFrameSize']
 
-def main(config):
+    frame_size_check=0
+    fileList = dirlist(output_directory)
+    dFramesList  = []
+    jsonList = []
+    # Listing the files in the directory
+    # Separating the json from pkl
+    for file in fileList:
+
+        if ".json" in file:
+            jsonList.append(file)
+        elif ".pkl" in file:
+            dFramesList.append(file)
+
+    # if there are no new outputs we skip that step
+    if len(jsonList)!=0: 
+
+        # We expect that every time the manager runs, there is a temp_frame
+        # file that might have events but it is not of the size we group
+        # them (maxDataFrameSize). 
+        try:
 
-    config = checkOutputDirectoryArguments(config)
+            with open(output_directory+'tempFrame.pkl','rb') as obj:
+                temp_frame = pickle.load(obj)
+        # The first time manager is running this file is created instead.
+        except FileNotFoundError:
+            temp_frame = pd.DataFrame(columns = ['gpstime','far','ifos'
+                                                ,'coincidence','coherency'
+                                                ,'combined','trigger'])
+
+            temp_frame["trigger"]=temp_frame["trigger"].astype(bool)
+
+            logger.info(f"Creating tempfile for the first time.")
+
+        # The size of the frame
+        initial_temp_frame_size=len(temp_frame)
+        json_list_size = len(jsonList)
 
-    # The size in which we group the outputs
-    if config['maxDataFrameSize']==None: 
-        config['maxDataFrameSize']=3600
+        #logger.info(f"Check that all files used, initial temp frame file {initial_temp_frame_size}")
+        #logger.info(f"Check that all files used, json list size {json_list_size}")
 
-    maxDataFrameSize = int(config['maxDataFrameSize'])
+        # A check value to make sure we add all the json files.
+        frame_size_check = json_list_size + initial_temp_frame_size
 
+        # Adding all the events in json format to the temp_frame
+        for file in jsonList:
 
-    # This is the time scale to use for the plots
-    timeUnitDict={1:'s', 60:'m', 3600:'h', 24*3600:'days',30*24*3600:'months', 365*24*3600:'years'}
+            try:
+                with open(output_directory+file,"r") as jf:
+                    p=json.load(jf)
+                    jf.close()
+            # Need to explain why this try point
+            except Exception as e:
+                frame_size_check = -1
+                logger.warning(f"Exception in loading json file {file}, {e}")
+                continue
 
-    if config['timeUnit']==None: 
-        config['timeUnit']=3600
-    else:
-        config['timeUnit']=int(config['timeUnit'])
-        
+            # Reformating the score parameters to the desired format.
+            for k in list(p['scores'].keys()):
+                p[k]=p['scores'][k]
+            # Making a string of ifos list to avoid line breaking into two
+            p['ifos'] = [str(p['ifos'])]
+
+            if file[0]=='N':
+                p['trigger']=False
+            elif file[0]=='T':
+                p['trigger']=True
+            else:
+                p['trigger']=False
 
-    sys.stdout.flush()
 
+            del(p['scores'])  
+            del(p['channels'])  
 
-    lastdatetimehour = -1 # Hour index so that some processes run every hour only
+            p = pd.DataFrame(p)
+            p["trigger"]=p["trigger"].astype(bool) # Avoiding a future warning
 
-    while (1):
-        logger.debug(f"PROCESSES before output management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+            temp_frame=pd.concat([temp_frame,p],ignore_index=True)
 
-        loopT0=time.time()
-        
-        output_directory = config['output_directory']
-        
-        frameSizeCheck=0
-        fileList = dirlist(output_directory)
-        dFramesList  = []
-        jsonList = []
-        # Listing the files in the directory
-        # Separating the json from pkl
-        for file in fileList:
-
-            if ".json" in file:
-                jsonList.append(file)
-            elif ".pkl" in file:
-                dFramesList.append(file)
-
-        # if there are no new outputs we skip that step
-        if len(jsonList)!=0: 
-
-            # We expect that every time the manager runs, there is a tempFrame
-            # file that might have events but it is not of the size we group
-            # them (maxDataFrameSize). 
-            try:
+        # Reseting index and sorting by GPS time
+        temp_frame=temp_frame.sort_values(by="gpstime").reset_index(drop=True)
+        # Rearanging the columns
+        temp_frame = temp_frame[['gpstime','far','ifos','coincidence','coherency'
+                            ,'combined','trigger']]
+        # Chopping the temp_frame to chuncs of maxDataFrameSize outputs
+        # IMPORTANT: We don't separate them by hour, we just collect 
+        # maxDataFrameSize of them together
 
-                with open(output_directory+'tempFrame.pkl','rb') as obj:
-                    tempFrame = pickle.load(obj)
-            # The first time manager is running this file is created instead.
-            except Exception as e:
-                tempFrame = pd.DataFrame(columns = ['gpstime','far','ifos'
-                                                    ,'coincidence','coherency'
-                                                    ,'combined','trigger'])
-                logger.info(f"Creating tempfile for the first time.")
+        while len(temp_frame) > maxDataFrameSize:
 
-            # The size of the frame
-            initialTempFrameSize=len(tempFrame)
+            # Creating a newframe to include the maxDataFrameSize instances
+            newFrame=temp_frame[:maxDataFrameSize]
+            with open(output_directory+str(newFrame['gpstime'][0])+"-"
+                    +str(newFrame['gpstime'][maxDataFrameSize-1])
+                    +"_"+str(maxDataFrameSize)+'.pkl', 'wb') as output:
+                pickle.dump(newFrame, output, 4)
 
-            # A check value to make sure we add all the json files.
-            frameSizeCheck = len(jsonList) + initialTempFrameSize
+            # Removing the newframe from temp_frame
+            temp_frame=temp_frame[maxDataFrameSize:].reset_index(drop=True)
 
-            # Adding all the events in json format to the tempFrame
-            for file in jsonList:
-                try:
-                    with open(output_directory+file,"r") as jf:
-                        p=json.load(jf)
-                        jf.close()
-                except Exception as e:
-                    logger.warning(f"Exception in loading json file {file}, {e}")
-                    continue
+            frame_size_check=-maxDataFrameSize
 
+        # What is left in temp_frame, overights the temp_frame.pkl
+        with open(output_directory+'tempFrame.pkl', 'wb') as output:
+            pickle.dump(temp_frame, output, 4)
+            logger.info(f"Saving the incomplete group of outputs: {output_directory}tempFrame.pkl")
 
+        frame_size_check-=len(temp_frame)
+        # We remove all json files already included in a dataFrame
+        for file in jsonList:
+            os.remove( output_directory + file )
+        
+        logger.info(f"Check that all files used, must be zero {frame_size_check}")
 
-            # Reformating the score parameters to the desired format.
-                for k in list(p['scores'].keys()):
-                    p[k]=p['scores'][k]
-                # Making a list of ifos to avoid line breaking into two
-                #p['ifos'] = [p['ifos']]
-
-                if file[0]=='N':
-                    p['trigger']=False
-                elif file[0]=='T':
-                    p['trigger']=True
-                else:
-                    p['trigger']=False
-
-
-                del(p['scores'])  
-                tempFrame=pd.concat([tempFrame, pd.DataFrame.from_dict(p)]
-                                    ,ignore_index=True)
-
-            # Reseting index and sorting by GPS time
-            tempFrame=tempFrame.sort_values(by="gpstime").reset_index(drop=True)
-            # Rearanging the columns
-            tempFrame = tempFrame[['gpstime','far','ifos','coincidence','coherency'
-                                ,'combined','trigger']]
-            # Chopping the tempFrame to chuncs of maxDataFrameSize outputs
-            # IMPORTANT: We don't separate them by hour, we just collect 
-            # maxDataFrameSize of them together
-
-            _frame = tempFrame[:10]
-
-
-            while len(tempFrame) > maxDataFrameSize:
-
-                # Creating a newframe to include the maxDataFrameSize instances
-                newFrame=tempFrame[:maxDataFrameSize]
-                with open(output_directory+str(newFrame['gpstime'][0])+"-"
-                        +str(newFrame['gpstime'][maxDataFrameSize-1])
-                        +"_"+str(maxDataFrameSize)+'.pkl', 'wb') as output:
-                    pickle.dump(newFrame, output, 4)
-
-                # logger.info("Saving group of outputs: ", output_directory+str(newFrame['gpstime'][0])+"-"
-                #     +str(newFrame['gpstime'][maxDataFrameSize-1])
-                #     +"-"+str(maxDataFrameSize)+'.pkl')
-
-                # Removing the newframe from tempFrame
-                tempFrame=tempFrame[maxDataFrameSize:].reset_index(drop=True)
-
-                frameSizeCheck-=maxDataFrameSize
-
-            # What is left in tempFrame, overights the tempFrame.pkl
-            with open(output_directory+'tempFrame.pkl', 'wb') as output:
-                pickle.dump(tempFrame, output, 4)
-                logger.info(f"Saving the incomplete group of outputs: {output_directory}tempFrame.pkl")
 
-            
-            # We remove all json files already included in a dataFrame
-            for file in jsonList:
-                os.remove( output_directory + file )
 
 
-            
-        logger.debug(f"PROCESSES before FAR management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+def manage_master_directory(config=None):
 
-        # # # FileSystem for FAR management
-        #
-        # Listing all files saved in the temp file (files to be managed)
-        detectors= list( det for det in config['detectors'])
-        
-        t0=time.time()
 
-        numberOfFiles={}
-        fileNumbers={}
-        dataSetDict={}
-        
-        # For each detector we count how many files have been saved in all
-        # detectors and we sort them.
-        for det in detectors:
-            numberOfFiles[det] = len(dirlist(config['masterDirectory']+'/temp/'+det))
-            fileNumbers[det] = sorted(list(file.split('_')[0] for file in dirlist(
-                config['masterDirectory']+'/temp/'+det)))
-            dataSetDict[det] = []
-
-        # If there are no files we skip this step
-        if len(fileNumbers[detectors[0]])==0:
-            logger.info(f"Empty temp directory")
-            #time.sleep(60)
-            
-        # If the files included in temp are less than maxDataFrameSize, we skip
-        # this step.
-        elif (int(float(fileNumbers[detectors[0]][-1]))
-            -int(float(fileNumbers[detectors[0]][0]))) < maxDataFrameSize:
-            logger.info(f"Not enough data \
-                        {maxDataFrameSize - (int(float(fileNumbers[detectors[0]][-1])) -  int(float(fileNumbers[detectors[0]][0])))}\
-                        to run the FAR test yet")
-            
-        # If the files included in temp are enough we group them
-        elif (int(float(fileNumbers[detectors[0]][-1]))
-            -int(float(fileNumbers[detectors[0]][0]))) >= maxDataFrameSize:
-            
-            c=0
-            
-            # We keep track of the files used to delete them later
-            filesToDelete=[]
-            
-            # Checking that all detectors have the same number of files
-            logger.debug(f"Number of files for each detector: {list(len(fileNumbers[det]) for det in detectors)}")
-            
-            lastFileNumber=None
-            # print("group size check: ",len(fileNumbers[detectors[0]][:int(maxDataFrameSize)]))
-            
-            for filenumber in fileNumbers[detectors[0]][:int(maxDataFrameSize)]:
+    maxDataFrameSize = config['maxDataFrameSize']
+    # Listing all files saved in the temp file (files to be managed)
+    detectors= list( det for det in config['detectors'])
+    
 
-                # For each file we in first detector we check that it exists in the
-                # other detectors too. 
-                if all( list( os.path.isfile(config['masterDirectory']
-                                            +'/temp/'+det+'/'+fileNumbers[detectors[0]][c]
-                                            +'_1.pkl') for det in detectors)):
-                    _temp_dataSetDict = {}
+    number_of_files={}
+    file_numbers={}
+    dataSet_dict={}
+    
+    # For each detector we count how many files have been saved in all
+    # detectors and we sort them.
+    for det in detectors:
+        number_of_files[det] = len(dirlist(config['masterDirectory']+'/temp/'+det))
+        file_numbers[det] = sorted(list(file.split('_')[0] for file in dirlist(
+            config['masterDirectory']+'/temp/'+det)))
+        dataSet_dict[det] = []
+
+    # If there are no files we skip this step
+    if len(file_numbers[detectors[0]])==0:
+        logger.info(f"Empty temp directory")
+        
+    # If the files included in temp are less than maxDataFrameSize, we skip
+    # this step.
+    elif (int(float(file_numbers[detectors[0]][-1]))
+        -int(float(file_numbers[detectors[0]][0]))) < maxDataFrameSize:
+        logger.info(f"Not enough data \
+                    {maxDataFrameSize - (int(float(file_numbers[detectors[0]][-1])) -  int(float(file_numbers[detectors[0]][0])))}\
+                    to run the FAR test yet")
+        
+    # If the files included in temp are enough we group them
+    elif (int(float(file_numbers[detectors[0]][-1]))
+        -int(float(file_numbers[detectors[0]][0]))) >= maxDataFrameSize:
+        
+        c=0
+        
+        # We keep track of the files used to delete them later
+        file_to_delete=[]
+        
+        # Checking that all detectors have the same number of files
+        logger.debug(f"Number of files for each detector: {list(len(file_numbers[det]) for det in detectors)}")
+        
+        last_file_number=None
+        
+        for filenumber in file_numbers[detectors[0]][:int(maxDataFrameSize)]:
+
+            # For each file we in first detector we check that it exists in the
+            # other detectors too. 
+            if all( list( os.path.isfile(config['masterDirectory']
+                                        +'/temp/'+det+'/'+file_numbers[detectors[0]][c]
+                                        +'_1.pkl') for det in detectors)):
+                _temp_dataSet_dict = {}
 
-                    try:
-                        for det in detectors:
-                                _temp_dataSetDict[det] = DataPod.load(config['masterDirectory']
-                                                        +'/temp/'+det+'/'+str(filenumber)+'_1.pkl')
-                        for det in detectors:
+                try:
+                    for det in detectors:
+                            _temp_dataSet_dict[det] = DataPod.load(config['masterDirectory']
+                                                    +'/temp/'+det+'/'+str(filenumber)+'_1.pkl')
+                    for det in detectors:
 
-                            dataSetDict[det].append(_temp_dataSetDict[det])
+                        dataSet_dict[det].append(_temp_dataSet_dict[det])
 
-                    except Exception as e:
+                except Exception as e:
 
-                        logger.warning("Empty file detected: "+config['masterDirectory']
-                                            +'/temp/'+det+'/'+str(filenumber)+'_1.pkl')
+                    logger.warning(f"Exception {type(e)}:{e} was raised at fille {config['masterDirectory']}/temp/{det}/{filenumber}_1.pkl")
 
-                            
                         
-                    lastFileNumber=int(float(filenumber))
-                    filesToDelete.append(str(filenumber)+'_1.pkl')
                     
-                    
-                
-                # Othewise we delete it and it can't be used
-                else:
-                    filesToDelete.append(str(filenumber)+'_1.pkl')
+                last_file_number=int(float(filenumber))
+                file_to_delete.append(str(filenumber)+'_1.pkl')
                 
-                c+=1
-
-            # We use those two for name creation
-            first = str(int(float(fileNumbers[detectors[0]][0])))
-            last = str(lastFileNumber)
-            # print('first,last: ',first,last)
+            # Othewise we delete it and it can't be used
+            else:
+                file_to_delete.append(str(filenumber)+'_1.pkl')
             
-            # Saving the instances in dataSets
-            for det in detectors:
-                _set = DataSet(dataSetDict[det])
-                name = first+'-'+last+'_'+str(len(_set))
-                _set.save(config['masterDirectory']+'/' + det + '/' + name)
-
-                # # Deleting files that already passed.
-                for file in filesToDelete:
-                    try:
-                        os.remove(config['masterDirectory']+'/temp/'+det+'/'+file)
-                    except Exception as e:
-                        pass
-
-        logger.debug(f"PROCESSES before efficiency and buffers management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
-
-        # # # Efficiency test buffer management
-        #
-
-        if os.path.isdir(config['efficiencies']):
-            manage_efficiency_test(config)
+            c+=1
 
-        # # # FAR test management 
-        #
-
-        manage_FAR_inefernce_files(config)
-        
-        # Updates latest segment plot
-        if datetime.now().hour != lastdatetimehour:
-            print('start segments plot')
-            segments_plot()
-            print('end segments plot')
-
-        # Update FAR plot
-        far_plot()
-        # # # Update status page
-        manage_status_page()  
-
-        # Timing
-        logger.info(f"Manager loop time:{time.time()-loopT0}, waiting 5 minutes ... ")
-        sys.stdout.flush()
-
-        time.sleep(5*60)
+        # We use those two for name creation
+        first = str(int(float(file_numbers[detectors[0]][0])))
+        last = str(last_file_number)
+        # print('first,last: ',first,last)
         
+        # Saving the instances in dataSets
+        for det in detectors:
+            _set = DataSet(dataSet_dict[det])
+            name = first+'-'+last+'_'+str(len(_set))
+            _set.save(config['masterDirectory']+'/' + det + '/' + name)
 
+            # # Deleting files that already passed.
+            for file in file_to_delete:
+                try:
+                    os.remove(config['masterDirectory']+'/temp/'+det+'/'+file)
+                except FileNotFoundError as e:
+                    logger.warning(f"Exception {type(e)}:{e} was raised at while trying to delete file {config['masterDirectory']}/temp/{det}/{file}")
+                    pass
+                except Exception as e:
+                    logger.warning(f"Exception {type(e)}:{e} was raised at while trying to delete file {config['masterDirectory']}/temp/{det}/{file}")
+                    raise(e)
+    
+    return None
 
 
 
 
 def manage_efficiency_test(config = None):
 
     if config is None:
@@ -398,15 +345,15 @@
         for each_pod in pod_list:    
             os.remove(config['bufferDirectory']+"/temp/"+each_pod)
         
         issue_efficiency_test()
         logger.info(f"Efficiency test initiated")
 
 def issue_efficiency_test():
-    os.system("nohup python -m mly_pipeline.make_eff_estimation --mode condor > efficiencyTest.out &")
+    os.system("nohup python -m mly_pipeline.make_eff_estimation --mode condor &> efficiencyTest.out &")
 
 def manage_FAR_inefernce_files(config = None):
 
     if config is None:
         with open('config.json') as json_file:
             config = json.load(json_file)
     # # # FAR test management 
@@ -600,15 +547,15 @@
             logger.info(f"New FARfile interpolations saced")
 
             if (farfile_to_delete is not None 
                     and farfile_to_delete!="FARfile_"+str(farfile_size)+".pkl"):
                 os.remove(config['falseAlarmRates']+"/FARfile/"+farfile_to_delete)
             
         # Overwriting config farfile when enough files
-        if len(hourly_files)!=0 and (farfile_size) >= 10*365*24*3600 and (config['farfile'] != config['falseAlarmRates']+"/FARfile"):
+        if len(hourly_files)!=0 and (farfile_size) >=4*365*24*3600 and (config['farfile'] != config['falseAlarmRates']+"/FARfile"):
 
             with open('config.json') as json_file:
                 _config = json.load(json_file)
                 _config['farfile'] = config['falseAlarmRates']+"/FARfile"
             with open("config.json", "w") as config_json:
                 json.dump(_config, config_json,indent=4)
                 config_json.close()
@@ -683,69 +630,199 @@
 def segments_plot():
 
 
     detectors = config['detectors']
 
     if 'ONLINE' in config['search_mode']:
 
-        end = int(to_gps(datetime.now().date()))-3600
+        end = float(tconvert(gpsordate = 'now'))
         start = end-3600*24*3+3600
 
     elif 'OFFLINE' in config['search_mode'] and isinstance(config['segment_list'],(list,tuple)):
 
         start = config['segment_list'][0]
         end = config['segment_list'][-1]
 
     else:
 
         print('NO VALID SEGMENT INPUT WAS PROVIDED')
 
     detector_active_flag =  config['active_flags']
     detector_segments =[]
 
-    time0 = time.time()
     for det in detectors:
         individual_detector_segment = query_segments(detector_active_flag[det], start, end)['active']
         detector_segments.append(individual_detector_segment)
 
-    time1 = time.time()-time0
-
     coincident_segments = SegmentList(detector_segments[0])
     for segment in detector_segments[1:]:
         coincident_segments = coincident_segments & segment
 
-    time2 = time.time()-time1
+    slist = get_segments_out_of_outputs(gps_start = start
+                                        , gps_end = None
+                                        , target_directory = config['output_directory'])
 
+    flag = DataQualityFlag(name=' '
+                    , active=slist
+                    , known=coincident_segments)
 
-    files = sorted(os.listdir(config['masterDirectory']+'/'+detectors[0]))
-    slist = SegmentList([])
+    plot = flag.plot(color='gwpy:ligo-hanford',alpha =0.6)
+    #plt.title('Processed Segments the last 3 days')
+    plot.savefig('segment_plot.png')
 
-    for file in files:
-        try:
 
-            start_gps = int(file.split('-')[0])
-            duration = int(file.split('_')[1].split('.')[0])
-            slist.append(Segment(start_gps,start_gps+duration + 1 ))
-        except Exception as e:
+def get_segments_out_of_outputs(gps_start
+                                ,gps_end=None
+                                ,target_directory='output_directory/'
+                                ,include_tempFile=False
+                                ,similarity_radius = 1):
+
+    if gps_end is None:
+        include_tempFile = True
+        gps_end = float(tconvert(gpsordate = 'now'))
 
-            print(file,':', e)
 
-    slist = slist.coalesce() 
 
-    slist = slist & SegmentList([Segment(start, end)])
-    time3 = time.time()-time2
+    files = list(file for file in sorted(os.listdir(target_directory)) 
+                if (file[-4:]=='.pkl' and 'tempFrame' not in file 
+                and float(file.split('-')[1].split('_')[0]) > gps_start 
+                and float(file.split('-')[0]) < gps_end)
+                )
+    # Initial value to check 
+    df = None
+
+    # Loading all output files
+    for i, file in enumerate(files):
+
+        if i == 0: 
+            with open(f"{target_directory}/{file}",'rb') as out:
+                df = pickle.load(out)
+        else:
+            with open(f"{target_directory}/{file}",'rb') as out:
+                df_ = pickle.load(out)
+
+            df = pd.concat([df,df_],ignore_index = True)
+
+    # Including tempFile if requested
+    if include_tempFile and df is not None:
+        with open(f"{target_directory}/tempFrame.pkl",'rb') as out:
+            df_ = pickle.load(out)
+
+        df = pd.concat([df,df_],ignore_index = True)
+
+    if len(files)==0:
+        print('empty')
+        return []
 
-    flag = DataQualityFlag(name=' '
-                    , active=slist
-                    , known=coincident_segments)
+    # Sort the DataFrame based on gpstime column
+    df_sorted = df.sort_values(by='gpstime')
+    
+    df_sorted = df_sorted[(df_sorted['gpstime']>=gps_start) & (gps_end>df_sorted['gpstime'])]
+    # Initialize variables for segment creation
+    start_time = None
+    end_time = None
+    segments = []
+
+    # Iterate through sorted DataFrame to identify continuous segments
+    for idx, row in df_sorted.iterrows():
+        if start_time is None:
+            start_time = int(row['gpstime'])
+            end_time = int(row['gpstime'])+1
+        elif int(row['gpstime']) - end_time > similarity_radius:  # If the difference is more than 2 seconds
+            # Create a segment and start a new one
+            segments.append(Segment(start_time, end_time))
+            start_time = int(row['gpstime'])
+            end_time = int(row['gpstime'])+1
+        else:
+            # Extend the segment
+            end_time = int(row['gpstime'])+1
+
+    # Create a segment for the last continuous segment
+    if start_time is not None:
+        segments.append(Segment(start_time, end_time))
 
-    plot = flag.plot(color='gwpy:ligo-hanford',alpha =0.6)
-    #plt.title('Processed Segments the last 3 days')
-    plot.savefig('segment_plot.png')
+    # Return a segment list
+    return segments
+
+
+def main(config):
+
+    config = checkOutputDirectoryArguments(config)
+
+    # The size in which we group the outputs
+    if config['maxDataFrameSize']==None: 
+        config['maxDataFrameSize']=3600
+
+    maxDataFrameSize = int(config['maxDataFrameSize'])
+
+
+    # This is the time scale to use for the plots
+    timeUnitDict={1:'s', 60:'m', 3600:'h', 24*3600:'days',30*24*3600:'months', 365*24*3600:'years'}
+
+    if config['timeUnit']==None: 
+        config['timeUnit']=3600
+    else:
+        config['timeUnit']=int(config['timeUnit'])
+        
+
+    sys.stdout.flush()
+
+
+    lastdatetimehour = -1 # Hour index so that some processes run every hour only
 
+    while (1):
+
+        loopT0=time.time()
+
+        # # # Managing the output directory files
+        #
+        #        
+        logger.debug(f"PROCESSES before output management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+        
+        manage_output_directory(config)
+
+        # # # FileSystem for FAR management
+        #
+        logger.debug(f"PROCESSES before FAR management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
+        manage_master_directory(config)
+
+        # # # Efficiency test buffer management
+        #
+        logger.debug(f"PROCESSES before efficiency and buffers management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+        if os.path.isdir(config['efficiencies']):
+            manage_efficiency_test(config)
+
+        # # # FAR test management 
+        #
+        manage_FAR_inefernce_files(config)
+        
+        # # # Updating page plots
+        # 
+        
+        if datetime.now().hour != lastdatetimehour:
+
+            segments_plot()
+        
+        lastdatetimehour = datetime.now().hour
+
+        far_plot()
+
+        # # # Update status page
+        #
+        manage_status_page()  
+        logger.info(f"Status page updated")
+
+        # Timing
+        logger.info(f"Manager loop time:{(time.time()-loopT0)/60} minutes, waiting 5 minutes ... ")
+        sys.stdout.flush()
+
+        time.sleep(5*60)
+        
+        
 if __name__ == "__main__":
         
     main(config)
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline/mly_to_grace.py` & `mly_pipeline-1.0.3/mly_pipeline/mly_to_grace.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,16 +34,67 @@
 for argument in arguments:
     kwargs[argument] = getattr(args, argument)
 
 # Config file is inherited by the search script updated
 with open('config.json') as json_file:
     config = json.load(json_file)
 
-# config = ast.literal_eval(kwargs['config'])  
-    
+def summary_plot(mly_pod,config,save_path = None):
+    from mly.skymap_utils import skymap_plot_function, mask_window_tf
+    from mly.plugins import plotcorrerlaion
+    from mly_pipeline.search_functions import tf_map_masked_plot_function
+
+    duration = config['duration']
+    fs = config['fs']
+    detectors = config['detectors']
+
+    # Recreating the mask as it is not retrievable
+    mask = mask_window_tf(duration, fs,mly_pod.PE['start_time']
+                                      ,mly_pod.PE['end_time'] 
+                                      ,config['skymap']['ramp_duration'] 
+                                      ,config['skymap']['ramp_center']
+                                      ,config['skymap']['duration_limit']).numpy()
+ 
+    plt.figure(figsize=(18, 9))
+
+    # Correlation plot
+    ax1 = plt.subplot(2,4,5)
+    ax1 = plotcorrerlaion(mly_pod.strain,detectors,fs,data=mly_pod.correlation,ax=ax1)
+
+    # Masked tf-map plot
+    ax2 = plt.subplot(2,4,6)
+    ax2 = tf_map_masked_plot_function( mly_pod.strain,tf_map = mly_pod.tf_map ,data = mly_pod.tf_map_masked, ax = ax2)
+
+    # Skymap
+    ax3 = plt.subplot(2,2,4,projection='astro hours mollweide')
+    ax3 = skymap_plot_function(mly_pod.strain,data=mly_pod.sky_map,ax = ax3)
+
+    # The filtered time-series plot
+    ax4 = plt.subplot(2,1,1)
+    ax4.set_title("Whitened Time-series")
+    ax4.plot(np.arange(0,duration,1/fs),mly_pod.sky_map[-1][0]*mask  ,label='H1 Filtered',color='#ee0000')
+    ax4.plot(np.arange(0,duration,1/fs),mly_pod.sky_map[-1][1]*mask  +5 ,label='L1 Filtered',color='#4ba6ff')
+
+    ax4.plot(np.arange(0,duration,1/fs),mly_pod.strain[0] ,label='H1',color='#ee0000',alpha = 0.5)
+    ax4.plot(np.arange(0,duration,1/fs),mly_pod.strain[1] +5 ,label='L1',color='#4ba6ff',alpha = 0.5)
+
+    ax4.plot(np.arange(0,duration,1/fs),mask ,color='k',label = 'Mask')
+    ax4.plot(np.arange(0,duration,1/fs),mask +5 ,color='k')
+
+    ax4.legend()
+    plt.tight_layout()
+
+    if save_path is not None:
+        plt.savefig(save_path)
+
+
+
+
+
+
     
 """This function issues a GraceDB event provided with a json file.
 
 Parameters
 ----------
 
 
@@ -171,15 +222,19 @@
         thepod.uwstrain = thepod.uwstrain[:2]
 
     # Create skymap plugin:
     thepod.addPlugIn(skymap_plugin(alpha = config['skymap']['alpha']
                                   ,beta = config['skymap']['beta']
                                   ,sigma =config['skymap']['sigma']
                                   ,nside = config['skymap']['nside']
-                                  ,window_parameter = (thepod.PE['start_time'], thepod.PE['end_time'], 1/16)))
+                                  ,window_parameter = (thepod.PE['start_time'], thepod.PE['end_time']
+                                                     ,config['skymap']['ramp_duration'] 
+                                                     ,config['skymap']['ramp_center']
+                                                     ,config['skymap']['duration_limit']
+                                                     ,thepod.PE['start_frequency'], thepod.PE['end_frequency'])))
 
     skymap_path = f"{config['trigger_directory']}/{eventDirectory}/mly.multiorder.fits"
     
     skymap_prob = thepod.sky_map[0]
 
     order = int(math.log2(config['skymap']['nside']))
     npix = ah.nside_to_npix(config['skymap']['nside'])
@@ -192,30 +247,33 @@
 
     with open(skymap_path, "w") as f:
         fits.write_sky_map( skymap_path, moc_data)
     
     # Upload skymap to grace db:
     if kwargs['trigger_destination'] != 'None':
 
-        client.write_log(graceEventDict['graceid'], 'Sky Localization',  filename=skymap_path, tg_name='sky_loc')
+        client.write_log(graceEventDict['graceid'], 'Sky Localization',  filename=skymap_path, tag_name='sky_loc')
         client.write_label(graceEventDict['graceid'], 'SKYMAP_READY')
     
     print("Latency after skymap log: ",time.time()-timeafterclient)
 
     thepod.plot('sky_map')
     plt.savefig(f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_skymap.png")
+    
+    summary_plot(thepod,config,save_path= f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}_summary.png")
 
     if kwargs['trigger_destination'] != 'None':
 
         plot_string = f"{config['trigger_directory']}/{eventDirectory}/T_{gpsstring}_{detectors}"
 
-        client.write_log(graceEventDict['graceid'], 'TimeSeries Plot',  filename=f"{plot_string}_strain.png", tg_name='strain')
-        client.write_log(graceEventDict['graceid'], 'Correlation Plot',  filename=f"{plot_string}_correlation.png", tg_name='strain')
-        client.write_log(graceEventDict['graceid'], 'Time-Frequency Map',  filename=f"{plot_string}_tfmap.png", tg_name='tfplots')
-        client.write_log(graceEventDict['graceid'], 'Skymap Probability',  filename=f"{plot_string}_skymap.png", tg_name='sky_loc')
+        #client.write_log(graceEventDict['graceid'], 'TimeSeries Plot',  filename=f"{plot_string}_strain.png", tag_name='strain')
+        #client.write_log(graceEventDict['graceid'], 'Correlation Plot',  filename=f"{plot_string}_correlation.png", tag_name='strain')
+        client.write_log(graceEventDict['graceid'], 'Time-Frequency Map',  filename=f"{plot_string}_tfmap.png", tag_name='tfplots')
+        client.write_log(graceEventDict['graceid'], 'Skymap Probability',  filename=f"{plot_string}_skymap.png", tag_name='sky_loc')
+        client.write_log(graceEventDict['graceid'], 'Summary Plot',  filename=f"{plot_string}_summary.png", tag_name='em_follow')
 
 
 raise SystemExit()
 
 # if __name__ == "__main__":
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline/offline_search.py` & `mly_pipeline-1.0.3/mly_pipeline/offline_search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/search.py` & `mly_pipeline-1.0.3/mly_pipeline/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,20 +81,20 @@
     # Check arguments and set values in config dict:
     config = checkArguments(config)
     
     np.random.seed( config['seed'] + int(config['script_index']))
 
     log_level = logging.getLevelName(config["log_level"])
 
-    logger = logging.getLogger("logger_for_search")
+    logger = logging.getLogger(f"logger_for_search_{config['script_index']}")
     logger.setLevel(logging.DEBUG)
 
 
     # create console handler and set level to debug
-    ch = handlers.TimedRotatingFileHandler('log/search.log', when='H',interval=12, backupCount=1,)
+    ch = handlers.TimedRotatingFileHandler(f"log/search{config['script_index']}.log", when='H',interval=24, backupCount=7,)
     ch.setLevel(log_level)
 
     # create formatter
     formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s")
 
     # add formatter to ch
     ch.setFormatter(formatter)
@@ -147,32 +147,32 @@
     
     logger.debug(f"PROCESSES before main loop: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
     # # # Main Loop
     while (1):  
         
         # Get GPS time for this script to search
-        gps_time, gps_index = calculateRequiredGPSTime(config, gps_index, initial_gps_time)
+        gps_time, gps_index = calculateRequiredGPSTime(config, gps_index, initial_gps_time,logger=logger)
         logger.info(f"S{config['script_index']} - Requested / Difference from current GPS time: {gps_time} / {gpstime.gps_time_now() - gps_time}")
 
         
         loopt0 = time.time()  #Get time at iteration start.
         
         # # Data Aquisition 
-        buffers = aquireData(config, gps_time)
+        buffers = aquireData(config, gps_time, logger=logger)
         
         getdatatime=time.time()
         
+        logger.info(f"S{config['script_index']} - Reading data aquisition time: {getdatatime - loopt0}") 
+
         # If data aquisition fails, reset loop:
         if (buffers is None):
             sys.stdout.flush()
             continue
-            
-        logger.info(f"S{config['script_index']} - Detector data aquisition time: {getdatatime - loopt0}") 
-        
+                    
         gpsBeforeInference = gpstime.gps_time_now()
         timeBeforeInference = time.time()
                 
         # # Data processing and inference
         
         # Putting data inside datapod format 
         buffer_pod = DataPod(
@@ -209,44 +209,50 @@
         ifos = ",".join([f"{detector}1" for detector in config["detectors"]])
         
         # Create mly_output dictionary, GraceDB event file basis
         
         interpolated_FAR_t0=time.time()
         interpolated_FAR_trials = 0
         
-
         while interpolated_FAR_trials < 3:
             try:
-                interpolated_FAR = far(config['farfile']+"/"+"FARfile_interpolation.pkl"
+                interpolated_FAR_ = far(config['farfile']+"/"+"FARfile_interpolation.pkl"
                                     ,result["total"][0], inverse = False)
+                interpolated_FAR = interpolated_FAR_ # Updating with the most current one
+
                 break
             except:
                 try:
-                    interpolated_FAR = far(config['farfile']+"/"+"FARfile_interpolation_reserve.pkl"
+                    interpolated_FAR_ = far(config['farfile']+"/"+"FARfile_interpolation_reserve.pkl"
                                         ,result["total"][0], inverse = False)
+                    interpolated_FAR = interpolated_FAR_ # Updating with the most current one
+
                     break
                 except Exception as e:
                     interpolated_FAR_trials+=1
                     if interpolated_FAR_trials >= 3:
-                        raise e
-        logger.info(f"S{config['script_index']} - Loading interpolated_FAR time: ,{time.time()-interpolated_FAR_t0}, {interpolated_FAR_trials}")
+                        logger.warning(f"S{config['script_index']} - Loading interpolated_FAR attempts exceded 3. Using the most previous one. Exception: {type(e)},{e}")
+        
+        
+        logger.info(f"S{config['script_index']} - Loading interpolated_FAR time: ,{time.time()-interpolated_FAR_t0},trials: {interpolated_FAR_trials}")
         logger.debug(f"PROCESSES after interpolation loading: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
         instance_start_time = result["GPSH"][0]
         mly_output = {
             "gpstime": instance_start_time,
             "far": interpolated_FAR,
             "ifos": ifos,
             "channels": list(config['channels'][det] for det in config['detectors']),
             "scores": {
                 "coincidence": result["scores1"][0],
                 "coherency": result["scores2"][0],
                 "combined": result["total"][0]
-            }
-
+            },
+            "instance_start_time": instance_start_time
+            
         }
         
         
         # Internal latency, from GPS selection to scores.
         logger.debug(f"S{config['script_index']} - internal_latency {gpsBeforeInference - gps_time}")
 
         # # # Follow up
@@ -257,36 +263,42 @@
         # Create string of joined detector names
         detectors = "".join(config["detectors"])
 
         threshold_t0=time.time()
         threshold_trials = 0
         while threshold_trials < 3:
             try:
-                threshold = far(config['farfile']+"/"+"FARfile_interpolation_inverse.pkl"
+                threshold_ = far(config['farfile']+"/"+"FARfile_interpolation_inverse.pkl"
                                     ,config['far_config']['threshold'], inverse = True)
+                threshold =  threshold_ # Updating with the most current one
+
                 break
             except:
                 try:
-                    threshold = far(config['farfile']+"/"+"FARfile_interpolation_inverse_reserve.pkl"
+                    threshold_ = far(config['farfile']+"/"+"FARfile_interpolation_inverse_reserve.pkl"
                                         ,config['far_config']['threshold'], inverse = True)
+                    threshold =  threshold_ # Updating with the most current one
                     break
                 except Exception as e:
                     threshold_trials+=1
                     if threshold_trials >= 3:
                         raise e
-        logger.debug(f"S{config['script_index']} - Loading threshold interpolation time: {time.time()-threshold_t0,threshold_trials}")
+                        
+        logger.info(f"S{config['script_index']} - Loading threshold interpolation time: {time.time()-threshold_t0},trials: {threshold_trials}, threshold:{threshold}")
 
         # Perform time- and frequency-domain parameter estimation.
         # It adds parameter estimation to events.
         pe_t0 = time.time()
         mly_output = runTimeFrequencyParameterEstimation(thepod,  mly_output)
-        logger.info(f"PE time {time.time()- pe_t0}s")
+        logger.info(f"S{config['script_index']} - PE time {time.time()- pe_t0}s")
         # If result us above threshold, do all even relate actions 
-                
-        logger.debug(f"PROCESSES after runTimeFrequencyParameterEstimation : {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+        logger.debug(f"S{config['script_index']} - PROCESSES after runTimeFrequencyParameterEstimation : {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+        
+        logger.info(f"S{config['script_index']} - Requested / Difference from current GPS time after PE: {gps_time} / {gpstime.gps_time_now() - gps_time}")
 
         if mly_output["scores"]["combined"] >= threshold:
 
             eventDirectory = 'tempEventDirectory_'+str(mly_output['gpstime'])
             os.mkdir(f"{config['trigger_directory']}/{eventDirectory}")
 
             # Saving trigger into the trigger_directory
@@ -347,15 +359,15 @@
         # Timing the loop to see if we need more splits in splitter.
         print(f"Processing loop duration: {str(time.time()-timeBeforeInference)}")  
         
         gps_time += config["num_scripts"]
         
         sys.stdout.flush()
 
-        if time.time() - start_time > 24*3600:
+        if time.time() - start_time > 3600:
 
             os.system(f"> search_step_{config['script_index']}.out")      
         
 
 
 if __name__ == "__main__":
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline/search_functions.py` & `mly_pipeline-1.0.3/mly_pipeline/search_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -608,15 +608,15 @@
         config['prefix'] = prefix_name_list[0]
         return config
     else:
         raise ValueError("Prefix names are not consistent in frames")
 
 
     
-def readFrameFile(frames, channel, state_vector_channel , start_gps = None, end_gps = None, wait = 0.5, timeout = 5, count=0):
+def readFrameFile(frames, channel, state_vector_channel , start_gps = None, end_gps = None, wait = 0.5, timeout = 5, count=0, logger = None):
     
     """A wrapper function for TimeSeries.read from gwpy. It reads the channels
     from the frames provided. If the reading fails for any reason it 
     waits <wait> time and tries again, up to <timeout> times.
     
     Parameters
     ----------
@@ -646,116 +646,136 @@
     timeseries data: gwpy.timeseries.TimeSeries 
         If data are fetched sucessfully it returns a gwpy TimeSeries
         
     None: 
         If data are not fetched after <timeout> attemts
 
     """
-
+    
     if state_vector_channel is not None:
         channels = [channel, state_vector_channel]
     else:
         channels = [channel]
     
     try:
         
         try:
             data = TimeSeriesDict.read(frames, channels, start = start_gps, end = end_gps)
-            
+
         except Exception as ex:
+            if logger is not None and type(ex)!=RuntimeError:
+                 logger.debug(f"Exception ({type(ex)} at TimeSeriesDict.read: {ex}") 
             raise(ex)
         
         if state_vector_channel is not None:
 
-            state_vector_status = StateVector(data[state_vector_channel]).boolean[:,0:2].value.all()
+            state_vector_status = ( StateVector(data[state_vector_channel]).boolean[:,0:2].value.all()  # Observing 
+                                  & StateVector(data[state_vector_channel]).boolean[:,5:9].value.all() )# Clear of injections
 
             if state_vector_status:
+                if logger is not None:
+                     logger.debug(f"Attempt to access the data {count+1}") 
+                     logger.info(f"State vector [0,1,5,6,7,8] indeces are {state_vector_status}") 
+
                 return data[channel]
 
             else:
-                    
-                raise Exception(f"State vector is {state_vector_status}")
+                raise Exception(f"State vector [0,1,5,6,7,8] indeces are {state_vector_status}")
         else:
-
+            if logger is not None: logger.info(f"Attempt to access the data {count+1}") 
             return data[channel]
             
     except Exception as e:
 
         time.sleep(wait)
         count += 1
         if count < timeout:
             return readFrameFile(frames, channel, state_vector_channel, start_gps, end_gps 
-                                    , wait = wait, timeout=timeout, count = count)
+                                    , wait = wait, timeout=timeout, count = count,logger=logger)
             
         else:
-            print(e)
-            print("Could not find frames.")
-            
+            if logger is not None:
+                logger.info(f"Could not find frames, Exception: {e}") 
+
+
         return None
     
-def far_interpolation(testfile, testNumber, inverse = False):
 
-    """Creates an interpolation function based on the FARfile
-    provided. 
-       
-    Parameters
-    ----------
-    
-    testfile: str (path)
-        The pickle file or the path to that file, 
-        that has the false alarm test values to be used 
-        for the interpolation.
-        
-    testNumber: int 
-        The file provided might only have the loudest 
-        results from a bigger test dustribution. By defining
-        testNumber the total number of thests is used.
-        
-    inverse: bool
-        If false it will give an interpolation of FAR to scores.
-        Or if true it will give an interpolation of scores to given FAR.
-    
-    Returns
-    -------
 
-    interpolation function: scipy.interpolate
+def logarithmic_indices(length, n_points):
     """
+    Generate indices of points to sample in logarithmic order.
+
+    Args:
+    - length: int, length of the array
+    - n_points: int, number of points to sample
+
+    Returns:
+    - indices: list of int, indices of points to sample
+    """
+    # Generate logarithmically spaced indices that are unique
+    log_indices = np.unique(np.append( np.logspace(0, np.log10(length - 1), num=n_points-1, base=10, dtype=int), length-1) )
+    # Convert to list
+    indices = list(log_indices)
+    return indices    
+
+    
+def far_interpolation(testfile, testNumber, min_tail_points=24, inverse = False):
+
     if isinstance(testfile,str):
         with open(testfile,'rb') as obj:
             dataR = pickle.load(obj)
     else:
         dataR = testfile
                 
     # dataR= dataR[dataR['score'] > 0.0001]
 
     try:
         scoreR=np.sort(np.array(dataR['score'])).tolist()[::-1]
     except Exception as e:
         scoreR=np.sort(np.array(dataR['scores1'])*np.array(dataR['scores2'])).tolist()[::-1]
     scoreFrequency=(np.arange(len(scoreR))+1)/testNumber
+
     
+    # The number of points in the tail that belong 
+    # to less than once per month FAR.
+    month_tail = testNumber//(30*24*3600) 
+
+    if month_tail >= min_tail_points:
+
+        new_indeces = np.append(np.arange(month_tail)                               # The indeces of the significant events (all indeces)
+                               ,logarithmic_indices(len(scoreR) - month_tail ,100)) # The indeces of all the rest (logarithmic)
+
+        # Applying the indeces
+        scoreR         = np.array(scoreR)[[new_indeces]][0]
+        scoreFrequency = np.array(scoreFrequency)[[new_indeces]][0]
+
+        print(scoreR[0],scoreR[-1])
+
+        print(scoreFrequency[0],scoreFrequency[-1])
+
     if inverse==False:
-        
+    
         farInterpolation=interp1d(
             scoreR,
             scoreFrequency,
             bounds_error=False,
             fill_value=(scoreFrequency[-1],scoreFrequency[0])
         )
-        return farInterpolation
         
     elif inverse==True:
         
         farInterpolation=interp1d(
             scoreFrequency,
             scoreR,
             bounds_error=False,
-            fill_value=(scoreR[-1],scoreR[0])
-            )
-        return farInterpolation
+            fill_value=(scoreR[0],scoreR[-1])
+        )
+
+    return farInterpolation
     
 
 
 def far(far_interp, input , inverse=False):
     
     """Uses the interpolation function provided
     to provide the FAR of the input score provided (inverse=False)
@@ -944,15 +964,15 @@
         config['segment_list'] = coincident_segments
 
         segmentlist = list([seg[0],seg[1]] for seg in coincident_segments)
         np.savetxt('used_segments.txt', segmentlist, delimiter=',')
 
     return config
 
-def calculateRequiredGPSTime(config, gps_index, initial_gps_time):
+def calculateRequiredGPSTime(config, gps_index, initial_gps_time,logger=None):
     
     """Injests command line arguments dictionary and outputs runtime config
         dictionary. Includes error checking.
        
        Parameters
        ----------
            
@@ -979,28 +999,34 @@
     num_scripts = config["num_scripts"]
     script_index = config["script_index"]
     gps_reset_time = config["gps_reset_time"]
     required_buffer = config["required_buffer"]
     
     #Find gps time for script
     gps_time = initial_gps_time + num_scripts*gps_index + script_index
-    
+
+
     # If gps_time falls to far behind current time, reset gps time by  
     # making the index go appropriatly forward.
-    if (gpstime.gps_time_now() - gps_time) > gps_reset_time:            
+    if (gpstime.gps_time_now() - gps_time) > gps_reset_time:
+        logger.info(f"S{config['script_index']} Before gps push - Requested / Difference from current GPS time: {gps_time} / {gpstime.gps_time_now() - gps_time}")
+
+        if logger is not None:
+            logger.info(f"Reseting GPS target time by skipping {num_scripts * int(gpstime.gps_time_now()-gps_time)//num_scripts + script_index } seconds")     
+                    
         gps_index += int(gpstime.gps_time_now()-gps_time)//num_scripts  
         gps_time = initial_gps_time + num_scripts*gps_index + script_index
-        print("RESETING GPS TIME INDEX")
+
     else:
         # Iterate gps index
         gps_index += 1
 
     return gps_time, gps_index
 
-def aquireData(config, gps_time):
+def aquireData(config, gps_time,logger=None):
     
     """Aquires required data at inputted gps time.
        
        Parameters
        ----------
            
        config: dict
@@ -1028,15 +1054,16 @@
         state_vector = config["state_vectors"][detector_initial] if (config["state_vectors"] != {}) else None
         #Search for frame files, return None if not found
         strain = readFrameFile(
             frames, 
             config["channels"][detector_initial],
             state_vector,
             wait = config["wait"],
-            timeout = int((config["num_scripts"]*1.5)/config["wait"]) # Using up to 1.5 times the time available in one loop of time. 
+            timeout = int((config["num_scripts"]*1.5)/config["wait"]), # Using up to 1.5 times the time available in one loop of time. 
+            logger = logger
         )
 
         if strain is not None:
             #Resample all strain data:
             strain = strain.resample(config["fs"]).value[int(config["fs"]*0.5):-int(config["fs"]*0.5)]
         else:
             #If no frame file is found return None
@@ -1072,24 +1099,31 @@
        -------
     
        mly_output: dictionary
            Dictionary containing mly output values.
     """
     
     thepod.addPlugIn(tf_map_plugin)
+    thepod.addPlugIn(tf_map_masked_plugin)
     thepod.addPlugIn(pe_plugin)
 
     if mly_output is not None:
         mly_output["SNR"] = thepod.PE['SNR']
         mly_output["central_time"] = mly_output['gpstime']+thepod.PE['peakTime']
         mly_output['gpstime'] = mly_output["central_time"]
         mly_output["duration"] = thepod.PE['duration']
         mly_output["central_freq"] = thepod.PE['peakFreq']
         mly_output["bandwidth"] = thepod.PE['bandwidth']
 
+        mly_output["start_time"] = thepod.PE['start_time']
+        mly_output["end_time"] = thepod.PE['end_time']
+        mly_output["start_frequency"] = thepod.PE['start_frequency']
+        mly_output["end_frequency"] = thepod.PE['end_frequency']
+
+
         return mly_output
 
    
 def podToFileSystem(pod, masterDirectory):
     
     """This function takes a dataPod and splits it into seperate ones
     depending on the detectors included. It saves individual DataPods
@@ -1121,16 +1155,14 @@
         _pod = DataPod(pod.strain[pod.detectors.index(det)]
                        ,detectors = [det]
                        ,fs = pod.fs
                        ,gps = [_gps])
         
         _pod.save(masterDirectory+'temp/'+det+'/'+str(_gps)+'_1')
     
-
-
 def create_tf_map(data,fs, Tfft = 1/16, wind=None, verbose = True):
 
     # % --------------------------------------------------------------------------
     # %    Create the time-frequency map of the data.
     # % --------------------------------------------------------------------------
 
     # % ---- THE PE FUNCTION WILL START HERE.
@@ -1193,29 +1225,33 @@
             print('  Power out = ' + str(powerOut))
             
         # % ---- FFT and retain non-negative frequencies only ([0,...,Nyquist]).
         sdata= np.fft.fft(sdata,axis=0)
         #print(tf_map.shape, sdata[np.arange(0,Nfft//2+1),:].shape)
         #tf_map = tf_map + abs(sdata)[np.arange(0,Nfft//2+1),:]**2
         tf_map = tf_map + abs(sdata[np.arange(0,Nfft//2+1),:])**2
+
     if verbose:
         plt.figure()
         plt.imshow(tf_map)
 
     return(tf_map)
-    
 
 def masked_tf_map(tf_map
                 , bpp = 0.05   # %-- fraction of loudest pixels in the map to keep for PE
                 , verbose = True
                 , searchRadius = 2):  # %-- radius in pixels to search for neighbors
     # % --------------------------------------------------------------------------
     # %    Threshold and cluster the time-frequency map.
     # % --------------------------------------------------------------------------
 
+    # Keep everything except the two first and two last rows that are corupted
+    tf_map[:2, :] = 0
+    tf_map[-2:, :] = 0
+    
     # % ---- Number of pixels retained.
     Nbp = int(bpp*tf_map.size) #matlab would have ceil for index being +1
     
     # N = int(T*fs)          # %-- timeseries length
     # Nfft = int(Tfft*fs)    # %-- FFT length
     # # % ---- Number of columns in the segmented overlapping data.
     # Ncol = 2*N//Nfft-1
@@ -1379,54 +1415,120 @@
 
         ax.set_title("Masked map")
     
     pe_dict = dict( peakTime = peakTime
                    ,duration = duration
                    ,bandwidth = bandwidth
                    ,peakFreq = peakFreq
+                   ,start_frequency = startFreq
+                   ,end_frequency = endFreq
                    ,start_time = startTime
                    ,end_time = endTime
                    ,SNR = SNR)
 
 
     return pe_dict
 
 
-def tf_map_gen_function(strain,fs):
+# PLUGIN FUNCTIONS (tf_map)
 
+def tf_map_gen_function(strain,fs,detectors,gps):
+
+
+    # Making a specific exception when search is run in two detectors.
+    if 'V' in detectors and gps[detectors.index('V')]==0.0:
+
+        detectors_ = detectors.copy()
+        detectors_.remove('V')
+
+        if all( list( gps[detectors_.index(det)] != 0.0 for det in detectors_)):
+            strain = np.delete(strain, detectors.index('V'),axis=0)
 
     tf_map = create_tf_map(data = np.transpose(strain),fs = fs, Tfft = 1/16, verbose = False)
 
     return tf_map
 
-def tf_map_plot_function( strain,data = None):
+def tf_map_plot_function( strain,data = None, ax = None):
 
     T0 = (1/16)/2  # Tfft/2 %-- central time of first bin
     dT = (1/16)/2  # Tfft/2 %-- hard-coded for 50% overlap
     # % ---- Convert all frequencues from bins to Hz.
     F0 = 0       # %-- central freq of first bin
     dF = 1/(1/16) # 1/Tfft%-- spacing of frequency bins
 
     Nrow , Ncol = data.shape
     
-    fig, ax = plt.subplots()
-    ax.imshow(data, origin='lower',extent=[T0,Nrow*dT,F0,Ncol*dF],aspect = 1/(Ncol*dF))
+    if ax is None:
+        fig, ax = plt.subplots()
+    im = ax.imshow(data, origin='lower',extent=[T0,Nrow*dT,F0,Ncol*dF],aspect = 1/(Ncol*dF))
+    ax.set_xlabel("Time (s)")
+    ax.set_ylabel("Frequency (Hz)")
     ax.set_title("Time-Frequency map")
+    ax.figure.colorbar(im)
 
     return ax
 
-def pe_gen_function(fs, tf_map):
+# PLUGIN FUNCTIONS (tf_map_masked)
+
+def tf_map_masked_gen_function(strain,fs,tf_map):
 
     mask , masked_map , map_median = masked_tf_map(tf_map = tf_map , bpp = 0.05, verbose = False)
+
+    return [mask , masked_map , map_median]
+
+def tf_map_masked_plot_function( strain,tf_map,data = None, ax = None):
+
+    T0 = (1/16)/2  # Tfft/2 %-- central time of first bin
+    dT = (1/16)/2  # Tfft/2 %-- hard-coded for 50% overlap
+    # % ---- Convert all frequencues from bins to Hz.
+    F0 = 0       # %-- central freq of first bin
+    dF = 1/(1/16) # 1/Tfft%-- spacing of frequency bins
+
+    mask , masked_map , map_median = data
+
+    Nrow , Ncol = tf_map.shape
+
+    if ax is None:    
+        fig, ax = plt.subplots()
+    im = ax.imshow(tf_map, origin='lower',extent=[T0,Nrow*dT,F0,Ncol*dF],aspect = 1/(Ncol*dF))
+    ax.set_xlabel("Time (s)")
+    ax.set_ylabel("Frequency (Hz)")
+    ax.set_title("Time-Frequency map")
+    ax.figure.colorbar(im,shrink = 0.5)
+
+    # Masking plot
+    f = lambda x,y: mask[int(y),int(x) ]
+    g = np.vectorize(f)
+    
+    x = np.linspace(0,mask.shape[1], mask.shape[1]*100)
+    y = np.linspace(0,mask.shape[0], mask.shape[0]*100)
+    X, Y= np.meshgrid(x[:-1],y[:-1])
+    Z = g(X[:-1],Y[:-1])
+
+    ax.contour(Z, [0.5], colors='r', linewidths=1
+                ,extent=[T0,Nrow*dT,F0,Ncol*dF])
+
+    return ax
+
+
+# PLUGIN FUNCTIONS (PE)
+
+def pe_gen_function(fs, tf_map_masked):
+
+    mask, masked_map, map_median = tf_map_masked
+
     return compute_PE(mask, masked_map, map_median, fs , verbose = False)
 
 
 
+tf_map_plugin = PlugIn('tf_map',genFunction=tf_map_gen_function,attributes=['strain','fs','detectors','gps']
+                               ,plotFunction=tf_map_plot_function, plotAttributes=['strain'])
 
+tf_map_masked_plugin = PlugIn('tf_map_masked',genFunction=tf_map_masked_gen_function,attributes=['strain','fs','tf_map']
+                                             ,plotFunction=tf_map_masked_plot_function, plotAttributes=['strain','tf_map'])
 
-tf_map_plugin = PlugIn('tf_map',genFunction=tf_map_gen_function,attributes=['strain','fs'],plotFunction=tf_map_plot_function, plotAttributes=['strain'])
 
-pe_plugin = PlugIn('PE', genFunction = pe_gen_function,attributes=['fs','tf_map'])
+pe_plugin = PlugIn('PE', genFunction = pe_gen_function,attributes=['fs','tf_map_masked'])
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline/tests/__init__.py` & `mly_pipeline-1.0.3/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-1.0.3/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-1.0.3/mly_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 1.0.2
+Version: 1.0.3
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-1.0.2/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-1.0.3/mly_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-1.0.2/pyproject.toml` & `mly_pipeline-1.0.3/pyproject.toml`

 * *Files identical despite different names*

