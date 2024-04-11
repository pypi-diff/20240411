# Comparing `tmp/libsrg-4.0.4-py3-none-any.whl.zip` & `tmp/libsrg-4.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 50232 bytes, number of entries: 41
+Zip file size: 53520 bytes, number of entries: 45
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
--rw-r--r--  2.0 unx     8952 b- defN 24-Apr-10 14:34 libsrg/Config.py
+-rw-r--r--  2.0 unx     9651 b- defN 24-Apr-11 01:01 libsrg/Config.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
 -rw-r--r--  2.0 unx     6553 b- defN 24-Apr-09 15:09 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6098 b- defN 24-Apr-09 15:09 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5875 b- defN 24-Apr-02 15:44 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
@@ -16,28 +16,32 @@
 -rw-r--r--  2.0 unx     7024 b- defN 23-Oct-05 17:56 libsrg/Stage0.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 16:52 libsrg/__init__.py
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:35 libsrg/template.py
 -rw-r--r--  2.0 unx    26598 b- defN 24-Apr-09 15:09 libsrg/ztool.py
 -rw-r--r--  2.0 unx     2000 b- defN 24-Apr-08 17:02 libsrg/Statistics/AnalogStatsBase.py
 -rw-r--r--  2.0 unx     1436 b- defN 24-Apr-08 17:02 libsrg/Statistics/AnalogStatsCumulative.py
 -rw-r--r--  2.0 unx     2300 b- defN 24-Apr-08 17:02 libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--  2.0 unx      950 b- defN 24-Apr-11 00:13 libsrg/Statistics/AnalogStatsSlidingWindow.py
 -rw-r--r--  2.0 unx     1175 b- defN 24-Apr-08 17:02 libsrg/Statistics/DiscreteStatsBase.py
 -rw-r--r--  2.0 unx      774 b- defN 24-Apr-08 17:02 libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--  2.0 unx      964 b- defN 24-Apr-11 00:41 libsrg/Statistics/DiscreteStatsSlidingWindow.py
 -rw-r--r--  2.0 unx     3644 b- defN 24-Apr-07 19:48 libsrg/Statistics/RunStatsBase.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/__init__.py
 -rw-r--r--  2.0 unx     2525 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
 -rw-r--r--  2.0 unx     2314 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
 -rw-r--r--  2.0 unx     3884 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--  2.0 unx     2894 b- defN 24-Apr-11 00:21 libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
 -rw-r--r--  2.0 unx     1605 b- defN 24-Apr-09 15:09 libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--  2.0 unx     2607 b- defN 24-Apr-11 00:45 libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
 -rw-r--r--  2.0 unx     1391 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/RunStatsBase_test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/UnitTests/__init__.py
 -rw-r--r--  2.0 unx     2222 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      448 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3424 b- defN 24-Apr-09 15:09 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10694 b- defN 24-Apr-09 15:09 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-10 14:38 libsrg-4.0.4.dist-info/RECORD
-41 files, 148070 bytes uncompressed, 44706 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-11 01:04 libsrg-4.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-11 01:04 libsrg-4.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 01:04 libsrg-4.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-11 01:04 libsrg-4.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3900 b- defN 24-Apr-11 01:04 libsrg-4.0.5.dist-info/RECORD
+45 files, 156624 bytes uncompressed, 47262 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -57,20 +57,26 @@
 
 Filename: libsrg/Statistics/AnalogStatsCumulative.py
 Comment: 
 
 Filename: libsrg/Statistics/AnalogStatsFading.py
 Comment: 
 
+Filename: libsrg/Statistics/AnalogStatsSlidingWindow.py
+Comment: 
+
 Filename: libsrg/Statistics/DiscreteStatsBase.py
 Comment: 
 
 Filename: libsrg/Statistics/DiscreteStatsCumulative.py
 Comment: 
 
+Filename: libsrg/Statistics/DiscreteStatsSlidingWindow.py
+Comment: 
+
 Filename: libsrg/Statistics/RunStatsBase.py
 Comment: 
 
 Filename: libsrg/Statistics/__init__.py
 Comment: 
 
 Filename: libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
@@ -78,17 +84,23 @@
 
 Filename: libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
 Comment: 
 
 Filename: libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
 Comment: 
 
+Filename: libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
+Comment: 
+
 Filename: libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
 Comment: 
 
+Filename: libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
+Comment: 
+
 Filename: libsrg/Statistics/UnitTests/RunStatsBase_test.py
 Comment: 
 
 Filename: libsrg/Statistics/UnitTests/__init__.py
 Comment: 
 
 Filename: libsrg/TKGUI/GuiBase.py
@@ -102,23 +114,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-4.0.4.dist-info/LICENSE.txt
+Filename: libsrg-4.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-4.0.4.dist-info/METADATA
+Filename: libsrg-4.0.5.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-4.0.4.dist-info/WHEEL
+Filename: libsrg-4.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-4.0.4.dist-info/top_level.txt
+Filename: libsrg-4.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-4.0.4.dist-info/RECORD
+Filename: libsrg-4.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/Config.py

```diff
@@ -211,8 +211,28 @@
         """Looks for item in maps
         :param item: item name
         :return: (depth, value) if found tuple with depth and value, else (None,None)
         """
         for depth, dct in enumerate(self.maps):
             if item in dct:
                 return depth, dct[item]
-        return (None, None)
+        return (None, None)
+
+    def to_list(self)-> list[tuple[str, Any, int]]:
+        """Finds and alphabetizes all config items in config
+        :return: Ordered list of tuples (name, value, depth)
+        """
+        return self.config_to_list(self)
+
+    @staticmethod
+    def config_to_list(config: Self)-> list[tuple[str, Any, int]]:
+        """Finds and alphabetizes all config items in config
+        :param config: Config instance
+        :return: Ordered list of tuples (name, value, depth)
+        """
+        names = list(config.keys())
+        names.sort()
+        lst=[]
+        for name in names:
+            depth,val = config.find_item_depth(name)
+            lst.append((name,val,depth))
+        return lst
```

## Comparing `libsrg-4.0.4.dist-info/LICENSE.txt` & `libsrg-4.0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-4.0.4.dist-info/METADATA` & `libsrg-4.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 4.0.4
+Version: 4.0.5
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-4.0.4.dist-info/RECORD` & `libsrg-4.0.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 libsrg/AppTemplate.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
-libsrg/Config.py,sha256=-S5rmb6sWSEwkebX9WGy60ShBktEIFtMLYzK1M79zjQ,8952
+libsrg/Config.py,sha256=pl1amYXWkrkrH__mxU0nbwmeHd1dD7kWGJrZvjFlFtM,9651
 libsrg/ElapsedTime.py,sha256=m-DxzdpfbElWAPpC0aZXWfrAOODUDb0I-x4w8FWlrZw,1878
 libsrg/Info.py,sha256=EQcale4UIw0Zp6IID42SjIAAfDGnOd7S37PVQxOEcFA,6553
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=84ffFwRkvqGKERvDT5GCDTyGEXPA9VfUF7N7lNN9XgA,6098
 libsrg/LoggingCounter.py,sha256=42YlyNOvebDk9c1kXhSzklPD-nlzxDz6DkwfApw8p80,5875
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
@@ -15,27 +15,31 @@
 libsrg/Stage0.py,sha256=xK8a5mCAlwXzpOgSvnj0elD65cT3RYYb3ubCkAGp8nw,7024
 libsrg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/template.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
 libsrg/ztool.py,sha256=aB-w0TRTjtM84leVfJuxYyIfniX_z6Qnsy5fVocvRPs,26598
 libsrg/Statistics/AnalogStatsBase.py,sha256=kM3CuTU-BMQh6iBGJmPho_IrekHLC1Mo8ccIqS6SbDQ,2000
 libsrg/Statistics/AnalogStatsCumulative.py,sha256=mHSUNKwBZo6OWLHNg3Xyt3w7Oq6XBF5n-lf_Hbn32Ag,1436
 libsrg/Statistics/AnalogStatsFading.py,sha256=mXy9YxIX1jfUuc-76UlSsLnPYitB-8V9TBn0QgUzwe8,2300
+libsrg/Statistics/AnalogStatsSlidingWindow.py,sha256=toAhv10J-ERyULtnyP2ZQPyapSEFyEhhRCfIR1h_q70,950
 libsrg/Statistics/DiscreteStatsBase.py,sha256=-9M0p7V-8GcZ0a6pHCrH6FmE62TECIq28fvbW2i46l4,1175
 libsrg/Statistics/DiscreteStatsCumulative.py,sha256=jU2nrV1CGY6F8nNJ6nAsA219zQ1XkIqPaccGb_QNpQ0,774
+libsrg/Statistics/DiscreteStatsSlidingWindow.py,sha256=PP4MMMh1VDQOoY8u59m5QN8yTkgrvDHClitNpPmAcjQ,964
 libsrg/Statistics/RunStatsBase.py,sha256=RyHDcbtzPRwMdNZfOa-GOAFmuIqpBafR9zVqiT467yw,3644
 libsrg/Statistics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/Statistics/UnitTests/AnalogStatsBase_test.py,sha256=OuKqBAwq1Q_U3l1xGAt0TcofljZTHca1YDHcRFsq3c0,2525
 libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py,sha256=ZwLiZSb3FB1MOMwzyZ65vHtPmNI4vhMZJicwkYBi848,2314
 libsrg/Statistics/UnitTests/AnalogStatsFading_test.py,sha256=C-pKVwKocnX7_IjZYnEmqUykMDYFDjiut49Ac2YSN58,3884
+libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py,sha256=sVPjZRFlbmujrQAJVJWDZadl2BJp6JI6Gx_JKU9feWk,2894
 libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py,sha256=kqbPk28ukAKLpiQMXeccFzHx764s8y6vRugRci9twR8,1605
+libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py,sha256=2idi1NA9X2wnLBD_Qle7NOJIB2Vlv5XEKf1oSArSNEw,2607
 libsrg/Statistics/UnitTests/RunStatsBase_test.py,sha256=p08NLMKYH2TG6Bea250uJWcRMGSKS4Qv7hTU7tj9F8s,1391
 libsrg/Statistics/UnitTests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/TKGUI/GuiBase.py,sha256=D6Jnzh5BZigjJ9XV9n9q4JcfcmX0qYwVfL2jf5TWQ6I,2222
 libsrg/TKGUI/GuiRequest.py,sha256=376qIPvpgg8l4crgPnjqwRnzdTND-mjicNC5VtkY5Hg,448
 libsrg/TKGUI/GuiRequestQueue.py,sha256=WVvdNXLtIaxkdRNbtsUCM7O4BOP-qLdYWVUVju3-xmc,3424
 libsrg/TKGUI/LoggerGUI.py,sha256=jXK77Zw2ettkItf9t5-FEKmQv65honqD27L_X8zOS0I,10694
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-4.0.4.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-4.0.4.dist-info/METADATA,sha256=upDK_efi95qTusRrmcxM5eMQr_6vJPJUdEn4v9mPwZU,3357
-libsrg-4.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libsrg-4.0.4.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-4.0.4.dist-info/RECORD,,
+libsrg-4.0.5.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-4.0.5.dist-info/METADATA,sha256=_j00HrlqMGvGfYwXzUGporj4Tnbk2BdOnBi3UuStFnI,3357
+libsrg-4.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-4.0.5.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-4.0.5.dist-info/RECORD,,
```

