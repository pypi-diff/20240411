# Comparing `tmp/rapid_videocr-2.2.7-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18591 bytes, number of entries: 12
--rw-r--r--  2.0 unx      201 b- defN 23-Aug-07 01:20 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx      811 b- defN 23-Aug-07 01:20 rapid_videocr/logger.py
--rw-r--r--  2.0 unx    10398 b- defN 23-Aug-07 01:20 rapid_videocr/main.py
--rw-r--r--  2.0 unx    13484 b- defN 23-Aug-07 01:20 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     4526 b- defN 23-Aug-07 01:20 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Aug-07 01:20 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     8163 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/RECORD
-12 files, 53115 bytes uncompressed, 16879 bytes compressed:  68.2%
+Zip file size: 16456 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      201 b- defN 23-Oct-08 10:55 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Oct-08 10:55 rapid_videocr/logger.py
+-rw-r--r--  2.0 unx    10398 b- defN 23-Oct-08 10:55 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    13512 b- defN 23-Oct-08 10:55 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     4526 b- defN 23-Oct-08 10:55 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Oct-08 10:55 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Oct-08 10:55 rapid_videocr-2.2.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      841 b- defN 23-Oct-08 10:55 rapid_videocr-2.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Oct-08 10:55 rapid_videocr-2.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Oct-08 10:55 rapid_videocr-2.2.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Oct-08 10:55 rapid_videocr-2.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1013 b- defN 23-Oct-08 10:55 rapid_videocr-2.2.8.dist-info/RECORD
+12 files, 45820 bytes uncompressed, 14744 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.7.dist-info/LICENSE
+Filename: rapid_videocr-2.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.7.dist-info/METADATA
+Filename: rapid_videocr-2.2.8.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.7.dist-info/WHEEL
+Filename: rapid_videocr-2.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.7.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.7.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.7.dist-info/RECORD
+Filename: rapid_videocr-2.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/rapid_videocr.py

```diff
@@ -23,24 +23,25 @@
 class RapidVideOCR:
     def __init__(
         self,
         is_concat_rec: bool = False,
         concat_batch: int = 10,
         out_format: str = "all",
         is_print_console: bool = False,
+        **kwargs,
     ) -> None:
         """Init
 
         Args:
             is_concat_rec (bool, optional): Whether to single recognition. Defaults to False.
             concat_batch (int, optional): The batch of concating image nums in concat recognition mode. Defaults to 10.
             out_format (str, optional): Output format of subtitle(srt, txt, all). Defaults to 'all'.
             is_print_console (bool, optional): Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.
         """
-        self.rapid_ocr = RapidOCR(width_height_ratio=-1)
+        self.rapid_ocr = RapidOCR(width_height_ratio=-1, **kwargs)
         self.cropper = CropByProject()
 
         self.batch_size = concat_batch
         self.is_concat_rec = is_concat_rec
         self.out_format = out_format
         self.is_print_console = is_print_console
```

## Comparing `rapid_videocr-2.2.7.dist-info/LICENSE` & `rapid_videocr-2.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.2.7.dist-info/RECORD` & `rapid_videocr-2.2.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 rapid_videocr/__init__.py,sha256=92pzSLPek0VGNZYO9DDOkXi6JNWCh_pb5ud9KoiMeJs,201
 rapid_videocr/logger.py,sha256=N3EqcXUElZo_Ta5fyueHRodIKe64PfDnFbqtz2IjfeU,811
 rapid_videocr/main.py,sha256=Hl44yFsdl7KFrrEpOtr-_T7f3UGlsESBp6UqLLUx-QA,10398
-rapid_videocr/rapid_videocr.py,sha256=GTxPnDI5H6Bb6FxTUKGstKD_ZeKiQIvqfTkiY52R9GA,13484
+rapid_videocr/rapid_videocr.py,sha256=5wgixsUJ-cd2xbbjaKMDZ6tQTOOJakPgv1ymYC6x0aQ,13512
 rapid_videocr/utils.py,sha256=aXQTl9EP1iKpifVUfMMOyCLsQ0nmfbEU-3rprPayYi4,4526
 rapid_videocr/video_sub_finder.py,sha256=FilAtJl0a2e81ZGDpPiL8n-JvYe3vRQrbw2rxLJyjIE,2996
-rapid_videocr-2.2.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapid_videocr-2.2.7.dist-info/METADATA,sha256=kmsRsCWjBZJmxWE1O3AQxsb7yNuny_b8mPUm1Wvlm0c,8163
-rapid_videocr-2.2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-rapid_videocr-2.2.7.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
-rapid_videocr-2.2.7.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
-rapid_videocr-2.2.7.dist-info/RECORD,,
+rapid_videocr-2.2.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapid_videocr-2.2.8.dist-info/METADATA,sha256=wdKlEtA3ohGkfWLLpkYQfpVgGtD-rxWzkTELQuQqxfY,841
+rapid_videocr-2.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rapid_videocr-2.2.8.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
+rapid_videocr-2.2.8.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
+rapid_videocr-2.2.8.dist-info/RECORD,,
```

