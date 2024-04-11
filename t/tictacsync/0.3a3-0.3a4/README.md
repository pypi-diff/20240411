# Comparing `tmp/tictacsync-0.3a3.tar.gz` & `tmp/tictacsync-0.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictacsync-0.3a3.tar", last modified: Fri Apr  5 00:11:10 2024, max compression
+gzip compressed data, was "tictacsync-0.3a4.tar", last modified: Thu Apr 11 00:00:48 2024, max compression
```

## Comparing `tictacsync-0.3a3.tar` & `tictacsync-0.3a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-05 00:11:10.957913 tictacsync-0.3a3/
--rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.3a3/LICENSE
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-05 00:11:10.956993 tictacsync-0.3a3/PKG-INFO
--rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.3a3/README.md
--rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-05 00:11:10.958126 tictacsync-0.3a3/setup.cfg
--rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-04-05 00:10:49.000000 tictacsync-0.3a3/setup.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-05 00:11:10.948524 tictacsync-0.3a3/tictacsync/
--rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.3a3/tictacsync/__init__.py
--rw-r--r--   0 lutzray    (501) staff       (20)    27558 2024-04-02 15:17:03.000000 tictacsync-0.3a3/tictacsync/device_scanner.py
--rw-r--r--   0 lutzray    (501) staff       (20)    11385 2024-04-04 23:58:33.000000 tictacsync-0.3a3/tictacsync/entry.py
--rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.3a3/tictacsync/multi2polywav.py
--rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.3a3/tictacsync/remergemix.py
--rw-r--r--   0 lutzray    (501) staff       (20)    45925 2024-04-05 00:10:01.000000 tictacsync-0.3a3/tictacsync/timeline.py
--rw-r--r--   0 lutzray    (501) staff       (20)    76810 2024-04-02 15:13:47.000000 tictacsync-0.3a3/tictacsync/yaltc.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-05 00:11:10.954982 tictacsync-0.3a3/tictacsync.egg-info/
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-05 00:11:10.000000 tictacsync-0.3a3/tictacsync.egg-info/PKG-INFO
--rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-05 00:11:10.000000 tictacsync-0.3a3/tictacsync.egg-info/SOURCES.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-05 00:11:10.000000 tictacsync-0.3a3/tictacsync.egg-info/dependency_links.txt
--rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-05 00:11:10.000000 tictacsync-0.3a3/tictacsync.egg-info/entry_points.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.3a3/tictacsync.egg-info/not-zip-safe
--rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-05 00:11:10.000000 tictacsync-0.3a3/tictacsync.egg-info/requires.txt
--rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-05 00:11:10.000000 tictacsync-0.3a3/tictacsync.egg-info/top_level.txt
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-11 00:00:48.361852 tictacsync-0.3a4/
+-rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.3a4/LICENSE
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-11 00:00:48.361395 tictacsync-0.3a4/PKG-INFO
+-rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.3a4/README.md
+-rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-11 00:00:48.362011 tictacsync-0.3a4/setup.cfg
+-rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-04-11 00:00:22.000000 tictacsync-0.3a4/setup.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-11 00:00:48.354502 tictacsync-0.3a4/tictacsync/
+-rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.3a4/tictacsync/__init__.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    27616 2024-04-10 23:52:37.000000 tictacsync-0.3a4/tictacsync/device_scanner.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    11393 2024-04-10 23:36:02.000000 tictacsync-0.3a4/tictacsync/entry.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.3a4/tictacsync/multi2polywav.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.3a4/tictacsync/remergemix.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    47608 2024-04-06 15:04:38.000000 tictacsync-0.3a4/tictacsync/timeline.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    76810 2024-04-02 15:13:47.000000 tictacsync-0.3a4/tictacsync/yaltc.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-11 00:00:48.360900 tictacsync-0.3a4/tictacsync.egg-info/
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/PKG-INFO
+-rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/entry_points.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.3a4/tictacsync.egg-info/not-zip-safe
+-rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/requires.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/top_level.txt
```

### Comparing `tictacsync-0.3a3/LICENSE` & `tictacsync-0.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a3/PKG-INFO` & `tictacsync-0.3a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.3a3
+Version: 0.3a4
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tictacsync-0.3a3/README.md` & `tictacsync-0.3a4/README.md`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a3/setup.py` & `tictacsync-0.3a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     entry_points = {
         "console_scripts": [
         'tictacsync = tictacsync.entry:main',
         'remergemix = tictacsync.remergemix:main',
         'multi2polywav = tictacsync.multi2polywav:main',
         ]
         },
-    version = '0.3a3',
+    version = '0.3a4',
     description = "command for syncing audio video recordings",
     long_description_content_type='text/markdown',
     long_description = long_descr,
     include_package_data=True,
     zip_safe=False,
     author = "Raymond Lutz",
     author_email = "lutzrayblog@mac.com",
```

### Comparing `tictacsync-0.3a3/tictacsync/device_scanner.py` & `tictacsync-0.3a4/tictacsync/device_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,47 +226,48 @@
         Returns nothing
 
         Populates Scanner.found_media_files, a list of Media objects
 
         Sets Scanner.input_structure = 'loose'|'folder_is_device'
 
         """
-        visible = [f for f in listdir(self.top_directory) if f[0] != '.']
-        logger.debug('visible: %s'%visible)
-        are_dir = all([isdir(join(self.top_directory, f)) for f in visible])
-        are_files = all([isfile(join(self.top_directory, f)) for f in visible])
-        logger.debug('dir: %s'%[isdir(join(self.top_directory, f)) for f
-              in visible])
-        if are_dir:
-            visible = [e for e in visible if e != 'SyncedMedia']
-            print('\nAssuming those are device folders: ',end='')
-            [print('[gold1]%s[/gold1]'%f, end=', ') for f in visible[:-1]]
-            print('[gold1]%s[/gold1].'%visible[-1])
-            self.input_structure = 'folder_is_device'
-        else: # are_files
-            self.input_structure = 'loose'
-            self.top_dir_has_multicam = False
         files = Path(self.top_directory).rglob('*.*')
         paths = [
             p
             for p in files
             if p.suffix[1:] in av_file_extensions
             and 'SyncedMedia' not in p.parts
         ]
+        logger.debug('found media files %s'%paths)
+        parents = [p.parent for p in paths]
+        logger.debug('found parents %s'%parents)
+        def _list_all_the_same(a_list):
+            return a_list.count(a_list[0]) == len(a_list)
+        all_parents_are_the_same = _list_all_the_same(parents)
+        logger.debug('all_parents_are_the_same %s'%all_parents_are_the_same)
+        if all_parents_are_the_same:
+            # all media (video + audio) are in a same folder, so this is loose
+            self.input_structure = 'loose'
+            # for now (TO DO?) 'loose' == no multi-cam
+            self.top_dir_has_multicam = False
+        else:
+            # check later if inside each folder, media have same device,
+            # for now, we'll guess structure is 'folder_is_device'
+            self.input_structure = 'folder_is_device'
         for p in paths:
             new_media = media_at_path(self.input_structure, p) # dev UID set here
             self.found_media_files.append(new_media)
         # files from devices without UID or name
-        def _same(l):
-            return all(e == l[0] for e in l)
+        # def _list_all_the_same(l):
+        #     return all(e == l[0] for e in l)
         def _try_name(medias):
             # return common first strings in filename
             names = [m.path.name for m in medias]
             transposed_names = list(map(list, zip(*names)))
-            same = list(map(_same, transposed_names))
+            same = list(map(_list_all_the_same, transposed_names))
             try:
                 first_diff = same.index(False)
             except:
                 return names[0].split('.')[0]
             return names[0][:first_diff]
         no_device_UID_media = [m for m in self.found_media_files
                     if not m.device.UID]
```

### Comparing `tictacsync-0.3a3/tictacsync/entry.py` & `tictacsync-0.3a4/tictacsync/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,18 @@
                     help='terse output')
     args = parser.parse_args()
     if args.verbose_output:
         logger.add(sys.stderr, level="DEBUG")
     # logger.add(sys.stdout, filter="__main__")
     # logger.add(sys.stdout, filter="device_scanner")
     # logger.add(sys.stdout, filter="yaltc") _extract_sound_to_merge
-    logger.add(sys.stdout, filter=lambda r: r["function"] == "build_audio_and_write_video")
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_audio_devices")
-    logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_mix")
-    logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mix")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "scan_media_and_build_devices_UID")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_multi2mono")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_mix")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mix")
     top_dir = args.directory[0]
     if os.path.isfile(top_dir):
         file = top_dir
         process_single(file, args)
     if not os.path.isdir(top_dir):
         print('%s is not a directory or doesnt exist.'%top_dir)
         sys.exit(1)
```

### Comparing `tictacsync-0.3a3/tictacsync/multi2polywav.py` & `tictacsync-0.3a4/tictacsync/multi2polywav.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a3/tictacsync/remergemix.py` & `tictacsync-0.3a4/tictacsync/remergemix.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a3/tictacsync/timeline.py` & `tictacsync-0.3a4/tictacsync/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,32 +62,31 @@
     status = sox_transform.build(str(source), str(dest))
     logger.debug('sox status %s'%status)
 
 def _sox_keep(audio_file, kept_channels) -> tempfile.NamedTemporaryFile:
     """
     Returns a NamedTemporaryFile containing the selected kept_channels
 
-    Building dict according to pysox.remix format.
-    https://pysox.readthedocs.io/en/latest/api.html#sox.transform.Transformer.remix
-    eg: 4 channels with TicTacCode_channel at #2 
-    returns {1: [1], 2: [3], 3: [4]}
-    ie the number of channels drops by one and chan 2 is missing
-    excluded_channels is a list of Zero Based indexing chan numbers
-
+    if len(kept_channels) == 1 then it's a mono mix on the specified track
+    if len(kept_channels) == 2 then it's a stereo mix on the specified tracks
     """
+
+
+
+
     audio_file = _pathname(audio_file)
     nchan = sox.file_info.channels(audio_file)
     logger.debug('in file of %i chan, have to keep %s'%
         (nchan, kept_channels))
     all_channels = range(1, nchan + 1) # from 1 to nchan included
-    # list of list for pysox API
-    # eg [[1], [3], [4]]
+    # Building dict according to pysox.remix format.
+    # https://pysox.readthedocs.io/en/latest/api.html#sox.transform.Transformer.remix
+    # eg:   {1: [3], 2: [4]} to keep channels 3 & 4    
     kept_channels = [[n] for n in kept_channels]
     sox_remix_dict = dict(zip(all_channels, kept_channels))
-    # {1: [1], 2: [3], 3: [4]} -> from 4 to 3 chan and chan 2 is dropped
     output_fh = tempfile.NamedTemporaryFile(suffix='.wav', delete=DEL_TEMP)
     out_file = _pathname(output_fh)
     logger.debug('sox in and out files: %s %s'%(audio_file, out_file))
     # sox_transform.set_output_format(channels=1)
     sox_transform = sox.Transformer()
     sox_transform.remix(sox_remix_dict)
     logger.debug('sox remix transform: %s'%sox_transform)
@@ -155,14 +154,34 @@
         _pathname(out_file_handle))
     nchan = sox.file_info.channels(
         _pathname(out_file_handle)) 
     logger.debug('merged file duration %f s with %i channels '%
         (merged_duration, nchan))
     return out_file_handle
 
+def _sox_multi2mono(multichan_tmpfl) -> tempfile.NamedTemporaryFile:
+    # return a mono mix down
+    n_chan_input = sox.file_info.channels(_pathname(multichan_tmpfl))
+    logger.debug('n chan input: %s'%n_chan_input)
+    if n_chan_input == 1: # nothing to mix down
+        return multichan_tmpfl
+    mono_tpfl = tempfile.NamedTemporaryFile(suffix='.wav',
+                    delete=DEL_TEMP)
+    tfm = sox.Transformer()
+    tfm.channels(1)
+    status = tfm.build(_pathname(multichan_tmpfl),_pathname(mono_tpfl))
+    logger.debug('n chan ouput: %s'%
+                sox.file_info.channels(_pathname(mono_tpfl)))
+    logger.debug('sox.build status for _sox_multi2mono(): %s'%status)
+    if status != True:
+        print('Error, sox did not normalize file in _sox_multi2mono()')
+        sys.exit(1)
+    return mono_tpfl
+
+
 def _sox_mix(paths:list) -> tempfile.NamedTemporaryFile:
     """
     mix files referred by the list of Path into a new temporary files passed on return
     """
     def _sox_norm(tempf):
         normed_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',
                         delete=DEL_TEMP)
@@ -179,14 +198,16 @@
     N = len(paths)
     if N == 1: # nothing to mix
         logger.debug('one file: nothing to mix')
         return paths[0]
     cbn.set_input_format(file_type=['wav']*N)
     filenames = [_pathname(p) for p in paths]
     logger.debug('%i files to mix %s'%(N, filenames))
+    logger.debug('nchan for each file %s'%[sox.file_info.channels(f) for
+                                    f in filenames])
     mixed_tempf = tempfile.NamedTemporaryFile(suffix='.wav',delete=DEL_TEMP)
     status = cbn.build(filenames,
                 _pathname(mixed_tempf),
                 combine_type='mix',
                 input_volumes=[1/N]*N)
     logger.debug('sox.build status for mix: %s'%status)
     if status != True:
@@ -576,43 +597,70 @@
 
     def _get_mix(self, device, multichan_tmpfl) -> tempfile.NamedTemporaryFile:
         """        
         If device has an associated Tracks description that declares a (mono or
         stereo) mix track, returns a tmpfl containing the corresponding
         tracks. If not, mix all the tracks with sox.
 
+        If no L-R tracks are declared in tracks.txt, a mono mix is returned;
+        If some
+        micL micR or mixL mixR
+
         """
         if device.tracks is None:
             logger.debug('no tracks.txt, mixing all')
-            return _sox_mix(_split_channels(multichan_tmpfl))
+            return _sox_multi2mono(multichan_tmpfl)
         mix_tracks = device.tracks.mix
         if mix_tracks == []:
             logger.debug('tracks.txt present but no mix trx, mixing all')
-            return _sox_mix(_split_channels(multichan_tmpfl))
+            return _sox_multi2mono(multichan_tmpfl)
+        # if here, mix exists
         logger.debug('%s has mix %s'%(device.name, mix_tracks))
         logger.debug('device %s'%device)
         if 'ttc' in device.tracks.rawtrx:
             sox_TTC_chan = device.tracks.rawtrx.index('ttc')
         elif 'tc' in device.tracks.rawtrx:
             sox_TTC_chan = device.tracks.rawtrx.index('tc')
         else:
             print('Error: no tc or ttc tag in track.txt')
             sys.exit(1)
-        sox_TTC_chan += 1 # sox NZBIDX
+        sox_TTC_chan += 1 # sox Not ZBIDX
         logger.debug('TTC chan %i'%sox_TTC_chan)
         # redo indexing since tracks.txt numbers refere to complete
         # files and here audio file had TTC and muted channels
-        # removed.
-        shift = 0
-        if mix_tracks[0] > sox_TTC_chan:
-            shift += 1
-        for unused_tr in device.tracks.unused:
-            if mix_tracks[0] > unused_tr:
+        # removed:
+        if len(mix_tracks) == 2: # two tracks to shift
+            mixL_chan, mixR_chan = mix_tracks
+            # shifting left chan if necessary
+            shift = 0
+            if mixL_chan > sox_TTC_chan:
+                shift += 1
+            for unused_tr in device.tracks.unused:
+                if mixL_chan > unused_tr:
+                    shift += 1
+            mixL_chan -= shift
+            # shifting right chan if necessary
+            shift = 0
+            if mixR_chan > sox_TTC_chan:
+                shift += 1
+            for unused_tr in device.tracks.unused:
+                if mixR_chan > unused_tr:
+                    shift += 1
+            mixR_chan -= shift
+            mix_tracks = [mixL_chan, mixR_chan]
+        else: # mono, one track to shift
+            monomix_chan = mix_tracks[0]
+            shift = 0
+            if monomix_chan > sox_TTC_chan:
                 shift += 1
-        mix_tracks = [t-shift for t in mix_tracks]
+            for unused_tr in device.tracks.unused:
+                if monomix_chan > unused_tr:
+                    shift += 1
+            monomix_chan -= shift
+            mix_tracks = [monomix_chan]
         logger.debug('new mix_tracks: %s'%mix_tracks)
         return _sox_keep(multichan_tmpfl, mix_tracks)
             
 
     def build_audio_and_write_video(self, top_dir, output_dir,
                                     write_multicam_structure,
                                     asked_ISOs):
@@ -689,16 +737,14 @@
         # dev_mixes_mix contains all audio recorders if many
         mixes = [self._get_mix(device, multi_chan_audio)
                 for device, multi_chan_audio
                 in merged_audio_files_by_device]
         logger.debug('there are %i dev mixes'%len(mixes))
         logger.debug('mixes %s'%mixes)
         dev_mixes_mix = _sox_mix(mixes)
-        # dev_mixes_mix = _sox_combine([audio for _, audio
-        #         in merged_audio_files_by_device]) # all devices
         logger.debug('will merge with %s'%(_pathname(dev_mixes_mix)))
         self.ref_recording.synced_audio = dev_mixes_mix
         logger.debug('dev_mixes_mix n chan: %i'%
             sox.file_info.channels(_pathname(dev_mixes_mix)))
         self._merge_audio_and_video()
         # devices_and_monofiles is list of (device, [monofiles])
         # [(dev1, multichan1), (dev2, multichan2)] in
```

### Comparing `tictacsync-0.3a3/tictacsync/yaltc.py` & `tictacsync-0.3a4/tictacsync/yaltc.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a3/tictacsync.egg-info/PKG-INFO` & `tictacsync-0.3a4/tictacsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.3a3
+Version: 0.3a4
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

