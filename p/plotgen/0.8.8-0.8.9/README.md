# Comparing `tmp/plotgen-0.8.8-py3-none-any.whl.zip` & `tmp/plotgen-0.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 39903 bytes, number of entries: 6
--rwxrwxr-x  2.0 unx   205251 b- defN 24-Feb-09 09:43 plotgen-0.8.8.data/scripts/plotgen
--rw-rw-r--  2.0 unx     1074 b- defN 24-Feb-09 09:43 plotgen-0.8.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7109 b- defN 24-Feb-09 09:43 plotgen-0.8.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Feb-09 09:43 plotgen-0.8.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-Feb-09 09:43 plotgen-0.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      478 b- defN 24-Feb-09 09:43 plotgen-0.8.8.dist-info/RECORD
-6 files, 214005 bytes uncompressed, 39039 bytes compressed:  81.8%
+Zip file size: 39911 bytes, number of entries: 6
+-rwxrwxr-x  2.0 unx   205238 b- defN 24-Feb-12 20:14 plotgen-0.8.9.data/scripts/plotgen
+-rw-rw-r--  2.0 unx     1074 b- defN 24-Feb-12 20:14 plotgen-0.8.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7109 b- defN 24-Feb-12 20:14 plotgen-0.8.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Feb-12 20:14 plotgen-0.8.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-Feb-12 20:14 plotgen-0.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      478 b- defN 24-Feb-12 20:14 plotgen-0.8.9.dist-info/RECORD
+6 files, 213992 bytes uncompressed, 39047 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: plotgen-0.8.8.data/scripts/plotgen
+Filename: plotgen-0.8.9.data/scripts/plotgen
 Comment: 
 
-Filename: plotgen-0.8.8.dist-info/LICENSE
+Filename: plotgen-0.8.9.dist-info/LICENSE
 Comment: 
 
-Filename: plotgen-0.8.8.dist-info/METADATA
+Filename: plotgen-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: plotgen-0.8.8.dist-info/WHEEL
+Filename: plotgen-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: plotgen-0.8.8.dist-info/top_level.txt
+Filename: plotgen-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: plotgen-0.8.8.dist-info/RECORD
+Filename: plotgen-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `plotgen-0.8.8.data/scripts/plotgen` & `plotgen-0.8.9.data/scripts/plotgen`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # import warnings
 # warnings.filterwarnings('error')
 
 # FUTURE: pyarrow
 # import csv.Sniffer
 
 __prog__ = 'plotgen'
-__version__ = '0.8.8'
+__version__ = '0.8.9'
 __url__ = 'https://github.com/bgottschall/plotgen'
 
 
 # All options that are forwared to the plotting script will be filtered through here
 def escapedStr(val: str):
   return val.translate(str.maketrans({
       "'": r"\'",
@@ -2146,16 +2146,17 @@
         if r in subplotGridDefinition and c in subplotGridDefinition[r]:
             subplot = subplotGridDefinition[r][c]
             if subplot['palette_count'] is None:
                 if subplot['palette_local']:
                     subplot['palette_count'] = subplot['traces'] if args.per_trace_colours else subplot['frames'] if args.per_frame_colours else 1
                 else:
                     subplot['palette_count'] = totalTraceCount if args.per_trace_colours else totalFrameCount if args.per_frame_colours else totalInputCount
-                subplot['palette_count'] = max(0, subplot['palette_count'] - len(subplot['colours']))
-            subplot['colours'].extend([f"rgba({int(255*r)}, {int(255*g)}, {int(255*b)}, {subplot['palette_opacity']})" for (r, g, b) in color_palette(subplot['palette'], subplot['palette_count'])])
+            
+            paletteExtend = max(0, subplot['palette_count'] - len(subplot['colours']))
+            subplot['colours'].extend([f"rgba({int(255*r)}, {int(255*g)}, {int(255*b)}, {subplot['palette_opacity']})" for (r, g, b) in color_palette(subplot['palette'], paletteExtend)])
 
             subplot['cmap'] = None
 
             if subplot['palette_reverse']:
                 subplot['colours'].reverse()
 
             if args.theme == 'palette' and args.colour_debug:
```

## Comparing `plotgen-0.8.8.dist-info/LICENSE` & `plotgen-0.8.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plotgen-0.8.8.dist-info/METADATA` & `plotgen-0.8.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotgen
-Version: 0.8.8
+Version: 0.8.9
 Summary: A plotly plotting script generator and data parser
 Home-page: https://github.com/bgottschall/plotgen
 Author: Björn Gottschall
 Author-email: info@gottschall.no
 License: MIT
 Keywords: tables graph plot parser plotly
 Platform: UNKNOWN
```

