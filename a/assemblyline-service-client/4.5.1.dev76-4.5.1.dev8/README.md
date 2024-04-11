# Comparing `tmp/assemblyline_service_client-4.5.1.dev76-py3-none-any.whl.zip` & `tmp/assemblyline_service_client-4.5.1.dev8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9594 bytes, number of entries: 8
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-11 13:59 assemblyline_service_client/VERSION
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 13:59 assemblyline_service_client/__init__.py
--rw-r--r--  2.0 unx    22546 b- defN 24-Apr-11 13:59 assemblyline_service_client/task_handler.py
--rw-r--r--  2.0 unx     1396 b- defN 24-Apr-11 13:59 assemblyline_service_client-4.5.1.dev76.dist-info/LICENCE.md
--rw-r--r--  2.0 unx     1577 b- defN 24-Apr-11 13:59 assemblyline_service_client-4.5.1.dev76.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 13:59 assemblyline_service_client-4.5.1.dev76.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-11 13:59 assemblyline_service_client-4.5.1.dev76.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      803 b- defN 24-Apr-11 13:59 assemblyline_service_client-4.5.1.dev76.dist-info/RECORD
-8 files, 26454 bytes uncompressed, 8146 bytes compressed:  69.2%
+Zip file size: 9587 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       11 b- defN 24-Feb-22 20:16 assemblyline_service_client/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-22 20:16 assemblyline_service_client/__init__.py
+-rw-r--r--  2.0 unx    22606 b- defN 24-Feb-22 20:16 assemblyline_service_client/task_handler.py
+-rw-r--r--  2.0 unx     1396 b- defN 24-Feb-22 20:16 assemblyline_service_client-4.5.1.dev8.dist-info/LICENCE.md
+-rw-r--r--  2.0 unx     1576 b- defN 24-Feb-22 20:16 assemblyline_service_client-4.5.1.dev8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-22 20:16 assemblyline_service_client-4.5.1.dev8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-Feb-22 20:16 assemblyline_service_client-4.5.1.dev8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      798 b- defN 24-Feb-22 20:16 assemblyline_service_client-4.5.1.dev8.dist-info/RECORD
+8 files, 26507 bytes uncompressed, 8149 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: assemblyline_service_client/__init__.py
 Comment: 
 
 Filename: assemblyline_service_client/task_handler.py
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev76.dist-info/LICENCE.md
+Filename: assemblyline_service_client-4.5.1.dev8.dist-info/LICENCE.md
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev76.dist-info/METADATA
+Filename: assemblyline_service_client-4.5.1.dev8.dist-info/METADATA
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev76.dist-info/WHEEL
+Filename: assemblyline_service_client-4.5.1.dev8.dist-info/WHEEL
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev76.dist-info/top_level.txt
+Filename: assemblyline_service_client-4.5.1.dev8.dist-info/top_level.txt
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev76.dist-info/RECORD
+Filename: assemblyline_service_client-4.5.1.dev8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## assemblyline_service_client/VERSION

```diff
@@ -1 +1 @@
-4.5.1.dev76
+4.5.1.dev8
```

## assemblyline_service_client/task_handler.py

```diff
@@ -163,15 +163,16 @@
             with open(self.service_manifest_yml, 'w') as yml_fh:
                 yaml.safe_dump(self.service_manifest_data, yml_fh)
 
     # noinspection PyBroadException
     def cleanup_working_directory(self, folder_path):
         for file in os.listdir(folder_path):
             file_path = os.path.join(folder_path, file)
-            if file_path not in [self.task_fifo_path, self.done_fifo_path, self.service_manifest_yml]:
+            # if file_path not in [self.task_fifo_path, self.done_fifo_path]:
+            if file_path != self.task_fifo_path or file_path != self.done_fifo_path:
                 try:
                     if os.path.isfile(file_path):
                         os.unlink(file_path)
                     elif os.path.isdir(file_path):
                         shutil.rmtree(file_path)
                 except Exception:
                     pass
```

## Comparing `assemblyline_service_client-4.5.1.dev76.dist-info/LICENCE.md` & `assemblyline_service_client-4.5.1.dev8.dist-info/LICENCE.md`

 * *Files identical despite different names*

## Comparing `assemblyline_service_client-4.5.1.dev76.dist-info/METADATA` & `assemblyline_service_client-4.5.1.dev8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-service-client
-Version: 4.5.1.dev76
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Service client
 Home-page: https://github.com/CybercentreCanada/assemblyline-service-client/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `assemblyline_service_client-4.5.1.dev76.dist-info/RECORD` & `assemblyline_service_client-4.5.1.dev8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-assemblyline_service_client/VERSION,sha256=iqWsiCUB4qG6Ft4zqwxt5BpBP0Cew2wVsHSog45Go9Y,12
+assemblyline_service_client/VERSION,sha256=vOZcm5VwouAZxLcIFar44guiJDMF80lns5xK0hj2a3Q,11
 assemblyline_service_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-assemblyline_service_client/task_handler.py,sha256=uiAOFBy-8Cylv2hwK2d3I58nPGKe1nmvtVOc0C0x1l8,22546
-assemblyline_service_client-4.5.1.dev76.dist-info/LICENCE.md,sha256=NSkYo9EH8h5oOkzg4VhjAHF4339MqPP2cQ8msTPgl-c,1396
-assemblyline_service_client-4.5.1.dev76.dist-info/METADATA,sha256=KSfdH0c1t2Y2TGcpwdOvXiq8Hb4y2P-1pC_4NsTTm7Y,1577
-assemblyline_service_client-4.5.1.dev76.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-assemblyline_service_client-4.5.1.dev76.dist-info/top_level.txt,sha256=clNWHvn8nw0kR15l5TASxWxIQvKGKe5Pso3kVPMiJv0,28
-assemblyline_service_client-4.5.1.dev76.dist-info/RECORD,,
+assemblyline_service_client/task_handler.py,sha256=Ej7VVUbzz3L_08Pag9zHmHXa1x2olbRaEH9pxSOdvzI,22606
+assemblyline_service_client-4.5.1.dev8.dist-info/LICENCE.md,sha256=NSkYo9EH8h5oOkzg4VhjAHF4339MqPP2cQ8msTPgl-c,1396
+assemblyline_service_client-4.5.1.dev8.dist-info/METADATA,sha256=odv8ciDLHLFQc7hmQjMsjaFEm4bH3j07bIL70lLFE1s,1576
+assemblyline_service_client-4.5.1.dev8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+assemblyline_service_client-4.5.1.dev8.dist-info/top_level.txt,sha256=clNWHvn8nw0kR15l5TASxWxIQvKGKe5Pso3kVPMiJv0,28
+assemblyline_service_client-4.5.1.dev8.dist-info/RECORD,,
```

