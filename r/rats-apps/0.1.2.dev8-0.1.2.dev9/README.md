# Comparing `tmp/rats_apps-0.1.2.dev8-py3-none-any.whl.zip` & `tmp/rats_apps-0.1.2.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -4,12 +4,12 @@
 -rw-r--r--  2.0 unx      553 b- defN 80-Jan-01 00:00 rats/apps/_composite_container.py
 -rw-r--r--  2.0 unx     3131 b- defN 80-Jan-01 00:00 rats/apps/_container.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 rats/apps/_ids.py
 -rw-r--r--  2.0 unx      188 b- defN 80-Jan-01 00:00 rats/apps/_namespaces.py
 -rw-r--r--  2.0 unx      853 b- defN 80-Jan-01 00:00 rats/apps/_plugin_container.py
 -rw-r--r--  2.0 unx     1304 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/apps/py.typed
--rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/RECORD
+-rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/RECORD
 13 files, 14402 bytes uncompressed, 4944 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: rats/apps/_scoping.py
 Comment: 
 
 Filename: rats/apps/py.typed
 Comment: 
 
-Filename: rats_apps-0.1.2.dev8.dist-info/METADATA
+Filename: rats_apps-0.1.2.dev9.dist-info/METADATA
 Comment: 
 
-Filename: rats_apps-0.1.2.dev8.dist-info/WHEEL
+Filename: rats_apps-0.1.2.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: rats_apps-0.1.2.dev8.dist-info/entry_points.txt
+Filename: rats_apps-0.1.2.dev9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_apps-0.1.2.dev8.dist-info/RECORD
+Filename: rats_apps-0.1.2.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rats_apps-0.1.2.dev8.dist-info/METADATA` & `rats_apps-0.1.2.dev9.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-apps
-Version: 0.1.2.dev8
+Version: 0.1.2.dev9
 Summary: research analysis tools for building applications
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_apps-0.1.2.dev8.dist-info/RECORD` & `rats_apps-0.1.2.dev9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 rats/apps/_composite_container.py,sha256=wSWVQWPin2xxIlEoSgk_D1rlc3N2gpTxQ2y9UFdqXy0,553
 rats/apps/_container.py,sha256=JSmO4x0JcnM9gQP0ki9JcGzYqbjmgAj79lZw5YfBrqI,3131
 rats/apps/_ids.py,sha256=dxWCPMpMA_vpaTDJEKNByIBJaX97Db203XqWLhaOezo,457
 rats/apps/_namespaces.py,sha256=THUV_Xj5PtweC23Ob-zsSpk8exC4fT-qRwjpQ6IDm0U,188
 rats/apps/_plugin_container.py,sha256=W_xQD2btc0N2dEb3c5tXM-ZZ4A4diMpkCjbOZdlXYuI,853
 rats/apps/_scoping.py,sha256=-5hl0RoOdQGkxWLIn42hthMUyX8_84sV8H3u40y-gIU,1304
 rats/apps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_apps-0.1.2.dev8.dist-info/METADATA,sha256=498TKmvfbSS_0mgTQ_vDntHzvo1uL1g7jcJIVQGwflA,716
-rats_apps-0.1.2.dev8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_apps-0.1.2.dev8.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
-rats_apps-0.1.2.dev8.dist-info/RECORD,,
+rats_apps-0.1.2.dev9.dist-info/METADATA,sha256=-WiawuBlYmLlPdFLoWa8DvkM1-9Dcn57jNmoJRZIX_4,716
+rats_apps-0.1.2.dev9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_apps-0.1.2.dev9.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
+rats_apps-0.1.2.dev9.dist-info/RECORD,,
```

