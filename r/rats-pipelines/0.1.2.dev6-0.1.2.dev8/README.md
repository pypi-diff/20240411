# Comparing `tmp/rats_pipelines-0.1.2.dev6-py3-none-any.whl.zip` & `tmp/rats_pipelines-0.1.2.dev8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -72,12 +72,12 @@
 -rw-r--r--  2.0 unx     2350 b- defN 80-Jan-01 00:00 rats/services/_scopes.py
 -rw-r--r--  2.0 unx     3798 b- defN 80-Jan-01 00:00 rats/services/_service_container.py
 -rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 rats/services/_service_factory.py
 -rw-r--r--  2.0 unx     3289 b- defN 80-Jan-01 00:00 rats/services/_service_managers.py
 -rw-r--r--  2.0 unx      598 b- defN 80-Jan-01 00:00 rats/services/_services.py
 -rw-r--r--  2.0 unx     1409 b- defN 80-Jan-01 00:00 rats/services/_typed_containers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/services/py.typed
--rw-r--r--  2.0 unx      774 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.2.dev6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.2.dev6.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.2.dev6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6861 b- defN 16-Jan-01 00:00 rats_pipelines-0.1.2.dev6.dist-info/RECORD
+-rw-r--r--  2.0 unx      774 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.2.dev8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.2.dev8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.2.dev8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6861 b- defN 16-Jan-01 00:00 rats_pipelines-0.1.2.dev8.dist-info/RECORD
 81 files, 124827 bytes uncompressed, 37831 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -225,20 +225,20 @@
 
 Filename: rats/services/_typed_containers.py
 Comment: 
 
 Filename: rats/services/py.typed
 Comment: 
 
-Filename: rats_pipelines-0.1.2.dev6.dist-info/METADATA
+Filename: rats_pipelines-0.1.2.dev8.dist-info/METADATA
 Comment: 
 
-Filename: rats_pipelines-0.1.2.dev6.dist-info/WHEEL
+Filename: rats_pipelines-0.1.2.dev8.dist-info/WHEEL
 Comment: 
 
-Filename: rats_pipelines-0.1.2.dev6.dist-info/entry_points.txt
+Filename: rats_pipelines-0.1.2.dev8.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_pipelines-0.1.2.dev6.dist-info/RECORD
+Filename: rats_pipelines-0.1.2.dev8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rats_pipelines-0.1.2.dev6.dist-info/METADATA` & `rats_pipelines-0.1.2.dev8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-pipelines
-Version: 0.1.2.dev6
+Version: 0.1.2.dev8
 Summary: Rats Pipelines
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_pipelines-0.1.2.dev6.dist-info/RECORD` & `rats_pipelines-0.1.2.dev8.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -71,11 +71,11 @@
 rats/services/_scopes.py,sha256=UJKK6XZsuQN0ukTKmpFNjoXsGKNS2eaZ6SUu09HLdOU,2350
 rats/services/_service_container.py,sha256=WeaXkbWRn7rbJTUeI8asTJr57oR-f_WJxitLxgZzZyY,3798
 rats/services/_service_factory.py,sha256=T2-Egvl1WLVrLpH9qxWesFV0uzQj242MPZCGq9u4Ynk,2587
 rats/services/_service_managers.py,sha256=EvyTyX6_OwN9eBoeb9FD7JHOyHHIe0il-bbx8d_l_6U,3289
 rats/services/_services.py,sha256=jQctaj9nqes1_S42PcnJzRRcNhigoyqpTmO_mquq1Uc,598
 rats/services/_typed_containers.py,sha256=xRBlJ5vgeeoJGa1wiYDj3uUdxVmal_3cNzYMcIyrpOA,1409
 rats/services/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_pipelines-0.1.2.dev6.dist-info/METADATA,sha256=py3ncoV5UNqIAsX0WXc4hZJxmjS_y_RUXh8eC3DLj58,774
-rats_pipelines-0.1.2.dev6.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_pipelines-0.1.2.dev6.dist-info/entry_points.txt,sha256=NY28IUb7dnNl0HFwzCGV2o9Uivyh278m0NpQRVDIgRQ,85
-rats_pipelines-0.1.2.dev6.dist-info/RECORD,,
+rats_pipelines-0.1.2.dev8.dist-info/METADATA,sha256=0YcVBda7D_wz7h2J1NOShYwAMUsGepKGh7PRgbJ9AIk,774
+rats_pipelines-0.1.2.dev8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_pipelines-0.1.2.dev8.dist-info/entry_points.txt,sha256=NY28IUb7dnNl0HFwzCGV2o9Uivyh278m0NpQRVDIgRQ,85
+rats_pipelines-0.1.2.dev8.dist-info/RECORD,,
```
