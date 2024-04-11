# Comparing `tmp/libsrg-4.0.3-py3-none-any.whl.zip` & `tmp/libsrg-4.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 50109 bytes, number of entries: 41
+Zip file size: 50232 bytes, number of entries: 41
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
--rw-r--r--  2.0 unx     8570 b- defN 24-Apr-09 14:56 libsrg/Config.py
+-rw-r--r--  2.0 unx     8952 b- defN 24-Apr-10 14:34 libsrg/Config.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
 -rw-r--r--  2.0 unx     6553 b- defN 24-Apr-09 15:09 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6098 b- defN 24-Apr-09 15:09 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5875 b- defN 24-Apr-02 15:44 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
@@ -31,13 +31,13 @@
 -rw-r--r--  2.0 unx     1391 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/RunStatsBase_test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/UnitTests/__init__.py
 -rw-r--r--  2.0 unx     2222 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      448 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3424 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10694 b- defN 24-Apr-09 15:09 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-09 15:09 libsrg-4.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Apr-09 15:09 libsrg-4.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 15:09 libsrg-4.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-09 15:09 libsrg-4.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-09 15:09 libsrg-4.0.3.dist-info/RECORD
-41 files, 147688 bytes uncompressed, 44583 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/RECORD
+41 files, 148070 bytes uncompressed, 44706 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -102,23 +102,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-4.0.3.dist-info/LICENSE.txt
+Filename: libsrg-4.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-4.0.3.dist-info/METADATA
+Filename: libsrg-4.0.4.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-4.0.3.dist-info/WHEEL
+Filename: libsrg-4.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-4.0.3.dist-info/top_level.txt
+Filename: libsrg-4.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-4.0.3.dist-info/RECORD
+Filename: libsrg-4.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/Config.py

```diff
@@ -85,15 +85,15 @@
         return out
 
     @classmethod
     def text_to_dict(cls, text: str) -> dict[str, Any]:
         """
         Converts a string into a dict. Content type is determined using a few heuristics.
         * convert from json if a line starting with "{" is found
-        * convert from yaml if a line starting with "---" is found  TODO
+        * convert from yaml if a line starting with "---" is found  TODO #36
         * convert from ini/configparser if a line starting with "[" is found
           * note first level in dict will be sections, not items
         * convert from env/bash name=value  otherwise
         :param text:
         :return: ict[str, Any]
         """
         text = cls.strip_comments(text)
@@ -202,7 +202,17 @@
         :param key: item name
         :param value: item value
         :param overwrite: Allow overwriting existing item (defaults True)
         :return: None
         """
         if key not in self or overwrite:
             self[key] = value
+
+    def find_item_depth(self, item: str) -> Tuple[Optional[int], Any]:
+        """Looks for item in maps
+        :param item: item name
+        :return: (depth, value) if found tuple with depth and value, else (None,None)
+        """
+        for depth, dct in enumerate(self.maps):
+            if item in dct:
+                return depth, dct[item]
+        return (None, None)
```

## Comparing `libsrg-4.0.3.dist-info/LICENSE.txt` & `libsrg-4.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-4.0.3.dist-info/METADATA` & `libsrg-4.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 4.0.3
+Version: 4.0.4
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-4.0.3.dist-info/RECORD` & `libsrg-4.0.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 libsrg/AppTemplate.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
-libsrg/Config.py,sha256=oJ25mDLa1Ka8vGqeEyxYf5NuFq55961iW_VEkKsKNvc,8570
+libsrg/Config.py,sha256=-S5rmb6sWSEwkebX9WGy60ShBktEIFtMLYzK1M79zjQ,8952
 libsrg/ElapsedTime.py,sha256=m-DxzdpfbElWAPpC0aZXWfrAOODUDb0I-x4w8FWlrZw,1878
 libsrg/Info.py,sha256=EQcale4UIw0Zp6IID42SjIAAfDGnOd7S37PVQxOEcFA,6553
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=84ffFwRkvqGKERvDT5GCDTyGEXPA9VfUF7N7lNN9XgA,6098
 libsrg/LoggingCounter.py,sha256=42YlyNOvebDk9c1kXhSzklPD-nlzxDz6DkwfApw8p80,5875
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
@@ -30,12 +30,12 @@
 libsrg/Statistics/UnitTests/RunStatsBase_test.py,sha256=p08NLMKYH2TG6Bea250uJWcRMGSKS4Qv7hTU7tj9F8s,1391
 libsrg/Statistics/UnitTests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/TKGUI/GuiBase.py,sha256=D6Jnzh5BZigjJ9XV9n9q4JcfcmX0qYwVfL2jf5TWQ6I,2222
 libsrg/TKGUI/GuiRequest.py,sha256=376qIPvpgg8l4crgPnjqwRnzdTND-mjicNC5VtkY5Hg,448
 libsrg/TKGUI/GuiRequestQueue.py,sha256=WVvdNXLtIaxkdRNbtsUCM7O4BOP-qLdYWVUVju3-xmc,3424
 libsrg/TKGUI/LoggerGUI.py,sha256=jXK77Zw2ettkItf9t5-FEKmQv65honqD27L_X8zOS0I,10694
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-4.0.3.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-4.0.3.dist-info/METADATA,sha256=2S2BCSkKKuPJTJGVCWQffud0Nr--D_7BuGOhIyv7I5M,3357
-libsrg-4.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libsrg-4.0.3.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-4.0.3.dist-info/RECORD,,
+libsrg-4.0.4.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-4.0.4.dist-info/METADATA,sha256=upDK_efi95qTusRrmcxM5eMQr_6vJPJUdEn4v9mPwZU,3357
+libsrg-4.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-4.0.4.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-4.0.4.dist-info/RECORD,,
```

