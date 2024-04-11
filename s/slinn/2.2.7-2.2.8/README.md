# Comparing `tmp/slinn-2.2.7.tar.gz` & `tmp/slinn-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slinn-2.2.7.tar", last modified: Tue Apr  9 20:20:54 2024, max compression
+gzip compressed data, was "slinn-2.2.8.tar", last modified: Thu Apr 11 17:22:14 2024, max compression
```

## Comparing `slinn-2.2.7.tar` & `slinn-2.2.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.857431 slinn-2.2.7/
--rw-rw-rw-   0        0        0     1059 2024-04-08 14:41:16.000000 slinn-2.2.7/LICENSE
--rw-rw-rw-   0        0        0     6899 2024-04-09 20:20:54.857431 slinn-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     6624 2024-04-09 20:15:11.000000 slinn-2.2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 20:20:54.857431 slinn-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-04-09 20:13:32.000000 slinn-2.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.777821 slinn-2.2.7/slinn/
--rw-rw-rw-   0        0        0      595 2024-04-09 20:13:14.000000 slinn-2.2.7/slinn/__init__.py
--rw-rw-rw-   0        0        0     4488 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/__main__.py
--rw-rw-rw-   0        0        0      360 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/address.py
--rw-rw-rw-   0        0        0       61 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/any_filter.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.807355 slinn-2.2.7/slinn/default/
--rw-rw-rw-   0        0        0       36 2024-02-10 11:37:15.000000 slinn-2.2.7/slinn/default/__init__.py
--rw-rw-rw-   0        0        0    13057 2024-04-08 17:58:05.000000 slinn-2.2.7/slinn/default/manage.py
--rw-rw-rw-   0        0        0      277 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/default/project.json
--rw-rw-rw-   0        0        0      308 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/dispatcher.py
--rw-rw-rw-   0        0        0      161 2024-03-22 21:18:07.000000 slinn-2.2.7/slinn/file.py
--rw-rw-rw-   0        0        0      686 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/filter.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.812356 slinn-2.2.7/slinn/guides/
--rw-rw-rw-   0        0        0       56 2024-02-11 13:06:29.000000 slinn-2.2.7/slinn/guides/__init__.py
--rw-rw-rw-   0        0        0      595 2024-04-09 20:12:59.000000 slinn-2.2.7/slinn/guides/migration1xx2xx.py
--rw-rw-rw-   0        0        0      621 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_api_response.py
--rw-rw-rw-   0        0        0      371 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_json_api_response.py
--rw-rw-rw-   0        0        0      475 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_json_response.py
--rw-rw-rw-   0        0        0      188 2024-02-09 18:54:22.000000 slinn-2.2.7/slinn/http_redirect.py
--rw-rw-rw-   0        0        0      762 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_response.py
--rw-rw-rw-   0        0        0      258 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/link_filter.py
--rw-rw-rw-   0        0        0     3164 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/request.py
--rw-rw-rw-   0        0        0     4989 2024-04-09 20:12:23.000000 slinn-2.2.7/slinn/server.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.813355 slinn-2.2.7/slinn/templates/
--rw-rw-rw-   0        0        0       23 2024-02-09 18:54:22.000000 slinn-2.2.7/slinn/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.828497 slinn-2.2.7/slinn/templates/example/
--rw-rw-rw-   0        0        0      163 2024-02-10 16:27:17.000000 slinn-2.2.7/slinn/templates/example/__init__.py
--rw-rw-rw-   0        0        0      291 2024-02-10 16:22:53.000000 slinn-2.2.7/slinn/templates/example/app.py
--rw-rw-rw-   0        0        0       24 2024-02-10 14:08:22.000000 slinn-2.2.7/slinn/templates/example/config.json
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.832430 slinn-2.2.7/slinn/templates/firstrun/
--rw-rw-rw-   0        0        0      166 2024-02-10 16:27:25.000000 slinn-2.2.7/slinn/templates/firstrun/__init__.py
--rw-rw-rw-   0        0        0      586 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/templates/firstrun/app.py
--rw-rw-rw-   0        0        0       23 2024-02-10 13:32:52.000000 slinn-2.2.7/slinn/templates/firstrun/config.json
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.855463 slinn-2.2.7/slinn/templates/firstrun/data/
--rw-rw-rw-   0        0        0     2241 2024-03-07 15:19:54.000000 slinn-2.2.7/slinn/templates/firstrun/data/slinn.html
--rw-rw-rw-   0        0        0      578 2024-02-09 18:54:22.000000 slinn-2.2.7/slinn/templates/firstrun/data/styles.css
--rw-rw-rw-   0        0        0     1237 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.856429 slinn-2.2.7/slinn.egg-info/
--rw-rw-rw-   0        0        0     6899 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-02-11 13:47:21.000000 slinn-2.2.7/slinn.egg-info/zip-safe
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2024-04-11 12:51:31.000000 slinn-2.2.8/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6649 2024-04-11 17:22:14.387385 slinn-2.2.8/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6385 2024-04-11 15:56:10.000000 slinn-2.2.8/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-11 17:22:14.387385 slinn-2.2.8/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      763 2024-04-11 13:09:34.000000 slinn-2.2.8/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-04-11 12:51:31.000000 slinn-2.2.8/slinn/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/__main__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      349 2024-04-07 20:45:27.000000 slinn-2.2.8/slinn/address.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/any_filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/default/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/default/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12696 2024-04-11 12:51:31.000000 slinn-2.2.8/slinn/default/manage.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      261 2024-04-07 20:24:45.000000 slinn-2.2.8/slinn/default/project.json
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      312 2024-04-11 12:51:31.000000 slinn-2.2.8/slinn/dispatcher.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.8/slinn/file.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/guides/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/guides/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      586 2024-04-11 16:03:48.000000 slinn-2.2.8/slinn/guides/migration1xx2xx.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/http_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/http_json_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/http_json_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/http_redirect.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-04-07 14:32:49.000000 slinn-2.2.8/slinn/http_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/link_filter.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-04-07 14:32:49.000000 slinn-2.2.8/slinn/request.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4785 2024-04-11 15:57:31.000000 slinn-2.2.8/slinn/server.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/templates/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/__init__.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn/templates/example/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/example/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/example/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/example/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn/templates/firstrun/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      549 2024-04-11 16:01:12.000000 slinn-2.2.8/slinn/templates/firstrun/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn/templates/firstrun/data/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/data/slinn.html
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/data/styles.css
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1191 2024-04-07 15:10:25.000000 slinn-2.2.8/slinn/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6649 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      944 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.8/slinn.egg-info/zip-safe
```

### Comparing `slinn-2.2.7/LICENSE` & `slinn-2.2.8/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 00000000: 436f 7079 7269 6768 7420 a920 3230 3234  Copyright . 2024
-00000010: 204d 6172 6b20 5261 6469 6e0d 0a0d 0a50   Mark Radin....P
-00000020: 6572 6d69 7373 696f 6e20 6973 2068 6572  ermission is her
-00000030: 6562 7920 6772 616e 7465 642c 2066 7265  eby granted, fre
-00000040: 6520 6f66 2063 6861 7267 652c 2074 6f20  e of charge, to 
-00000050: 616e 7920 7065 7273 6f6e 206f 6274 6169  any person obtai
-00000060: 6e69 6e67 2061 2063 6f70 7920 6f66 2074  ning a copy of t
-00000070: 6869 7320 736f 6674 7761 7265 2061 6e64  his software and
-00000080: 2061 7373 6f63 6961 7465 6420 646f 6375   associated docu
-00000090: 6d65 6e74 6174 696f 6e20 6669 6c65 7320  mentation files 
-000000a0: 2874 6865 2093 536f 6674 7761 7265 9429  (the .Software.)
-000000b0: 2c20 746f 2064 6561 6c20 696e 2074 6865  , to deal in the
-000000c0: 2053 6f66 7477 6172 6520 7769 7468 6f75   Software withou
-000000d0: 7420 7265 7374 7269 6374 696f 6e2c 2069  t restriction, i
-000000e0: 6e63 6c75 6469 6e67 2077 6974 686f 7574  ncluding without
-000000f0: 206c 696d 6974 6174 696f 6e20 7468 6520   limitation the 
-00000100: 7269 6768 7473 2074 6f20 7573 652c 2063  rights to use, c
-00000110: 6f70 792c 206d 6f64 6966 792c 206d 6572  opy, modify, mer
-00000120: 6765 2c20 7075 626c 6973 682c 2064 6973  ge, publish, dis
-00000130: 7472 6962 7574 652c 2073 7562 6c69 6365  tribute, sublice
-00000140: 6e73 652c 2061 6e64 2f6f 7220 7365 6c6c  nse, and/or sell
-00000150: 2063 6f70 6965 7320 6f66 2074 6865 2053   copies of the S
-00000160: 6f66 7477 6172 652c 2061 6e64 2074 6f20  oftware, and to 
-00000170: 7065 726d 6974 2070 6572 736f 6e73 2074  permit persons t
-00000180: 6f20 7768 6f6d 2074 6865 2053 6f66 7477  o whom the Softw
-00000190: 6172 6520 6973 2066 7572 6e69 7368 6564  are is furnished
-000001a0: 2074 6f20 646f 2073 6f2c 2073 7562 6a65   to do so, subje
-000001b0: 6374 2074 6f20 7468 6520 666f 6c6c 6f77  ct to the follow
-000001c0: 696e 6720 636f 6e64 6974 696f 6e73 3a0d  ing conditions:.
-000001d0: 0a0d 0a54 6865 2061 626f 7665 2063 6f70  ...The above cop
-000001e0: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
-000001f0: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
-00000200: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
-00000210: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
-00000220: 6c20 636f 7069 6573 206f 7220 7375 6273  l copies or subs
-00000230: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
-00000240: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-00000250: 2e0d 0a0d 0a54 4845 2053 4f46 5457 4152  .....THE SOFTWAR
-00000260: 4520 4953 2050 524f 5649 4445 4420 9341  E IS PROVIDED .A
-00000270: 5320 4953 942c 2057 4954 484f 5554 2057  S IS., WITHOUT W
-00000280: 4152 5241 4e54 5920 4f46 2041 4e59 204b  ARRANTY OF ANY K
-00000290: 494e 442c 2045 5850 5245 5353 204f 5220  IND, EXPRESS OR 
-000002a0: 494d 504c 4945 442c 2049 4e43 4c55 4449  IMPLIED, INCLUDI
-000002b0: 4e47 2042 5554 204e 4f54 204c 494d 4954  NG BUT NOT LIMIT
-000002c0: 4544 2054 4f20 5448 4520 5741 5252 414e  ED TO THE WARRAN
-000002d0: 5449 4553 204f 4620 4d45 5243 4841 4e54  TIES OF MERCHANT
-000002e0: 4142 494c 4954 592c 2046 4954 4e45 5353  ABILITY, FITNESS
-000002f0: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
-00000300: 5220 5055 5250 4f53 4520 414e 4420 4e4f  R PURPOSE AND NO
-00000310: 4e49 4e46 5249 4e47 454d 454e 542e 2049  NINFRINGEMENT. I
-00000320: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
-00000330: 2054 4845 2041 5554 484f 5253 204f 5220   THE AUTHORS OR 
-00000340: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
-00000350: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
-00000360: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-00000370: 4553 204f 5220 4f54 4845 5220 4c49 4142  ES OR OTHER LIAB
-00000380: 494c 4954 592c 2057 4845 5448 4552 2049  ILITY, WHETHER I
-00000390: 4e20 414e 2041 4354 494f 4e20 4f46 2043  N AN ACTION OF C
-000003a0: 4f4e 5452 4143 542c 2054 4f52 5420 4f52  ONTRACT, TORT OR
-000003b0: 204f 5448 4552 5749 5345 2c20 4152 4953   OTHERWISE, ARIS
-000003c0: 494e 4720 4652 4f4d 2c20 4f55 5420 4f46  ING FROM, OUT OF
-000003d0: 204f 5220 494e 2043 4f4e 4e45 4354 494f   OR IN CONNECTIO
-000003e0: 4e20 5749 5448 2054 4845 2053 4f46 5457  N WITH THE SOFTW
-000003f0: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
-00000400: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
-00000410: 2049 4e20 5448 4520 534f 4654 5741 5245   IN THE SOFTWARE
-00000420: 2e0d 0a                                  ...
+00000010: 204d 6172 6b20 5261 6469 6e0a 0a50 6572   Mark Radin..Per
+00000020: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
+00000030: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
+00000040: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
+00000050: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
+00000060: 6e67 2061 2063 6f70 7920 6f66 2074 6869  ng a copy of thi
+00000070: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
+00000080: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
+00000090: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
+000000a0: 6865 2093 536f 6674 7761 7265 9429 2c20  he .Software.), 
+000000b0: 746f 2064 6561 6c20 696e 2074 6865 2053  to deal in the S
+000000c0: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
+000000d0: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
+000000e0: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
+000000f0: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
+00000100: 6768 7473 2074 6f20 7573 652c 2063 6f70  ghts to use, cop
+00000110: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
+00000120: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
+00000130: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
+00000140: 652c 2061 6e64 2f6f 7220 7365 6c6c 2063  e, and/or sell c
+00000150: 6f70 6965 7320 6f66 2074 6865 2053 6f66  opies of the Sof
+00000160: 7477 6172 652c 2061 6e64 2074 6f20 7065  tware, and to pe
+00000170: 726d 6974 2070 6572 736f 6e73 2074 6f20  rmit persons to 
+00000180: 7768 6f6d 2074 6865 2053 6f66 7477 6172  whom the Softwar
+00000190: 6520 6973 2066 7572 6e69 7368 6564 2074  e is furnished t
+000001a0: 6f20 646f 2073 6f2c 2073 7562 6a65 6374  o do so, subject
+000001b0: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
+000001c0: 6720 636f 6e64 6974 696f 6e73 3a0a 0a54  g conditions:..T
+000001d0: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+000001e0: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
+000001f0: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
+00000200: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
+00000210: 636c 7564 6564 2069 6e20 616c 6c20 636f  cluded in all co
+00000220: 7069 6573 206f 7220 7375 6273 7461 6e74  pies or substant
+00000230: 6961 6c20 706f 7274 696f 6e73 206f 6620  ial portions of 
+00000240: 7468 6520 536f 6674 7761 7265 2e0a 0a54  the Software...T
+00000250: 4845 2053 4f46 5457 4152 4520 4953 2050  HE SOFTWARE IS P
+00000260: 524f 5649 4445 4420 9341 5320 4953 942c  ROVIDED .AS IS.,
+00000270: 2057 4954 484f 5554 2057 4152 5241 4e54   WITHOUT WARRANT
+00000280: 5920 4f46 2041 4e59 204b 494e 442c 2045  Y OF ANY KIND, E
+00000290: 5850 5245 5353 204f 5220 494d 504c 4945  XPRESS OR IMPLIE
+000002a0: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
+000002b0: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
+000002c0: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
+000002d0: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
+000002e0: 592c 2046 4954 4e45 5353 2046 4f52 2041  Y, FITNESS FOR A
+000002f0: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
+00000300: 4f53 4520 414e 4420 4e4f 4e49 4e46 5249  OSE AND NONINFRI
+00000310: 4e47 454d 454e 542e 2049 4e20 4e4f 2045  NGEMENT. IN NO E
+00000320: 5645 4e54 2053 4841 4c4c 2054 4845 2041  VENT SHALL THE A
+00000330: 5554 484f 5253 204f 5220 434f 5059 5249  UTHORS OR COPYRI
+00000340: 4748 5420 484f 4c44 4552 5320 4245 204c  GHT HOLDERS BE L
+00000350: 4941 424c 4520 464f 5220 414e 5920 434c  IABLE FOR ANY CL
+00000360: 4149 4d2c 2044 414d 4147 4553 204f 5220  AIM, DAMAGES OR 
+00000370: 4f54 4845 5220 4c49 4142 494c 4954 592c  OTHER LIABILITY,
+00000380: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
+00000390: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
+000003a0: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
+000003b0: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
+000003c0: 4f4d 2c20 4f55 5420 4f46 204f 5220 494e  OM, OUT OF OR IN
+000003d0: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
+000003e0: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
+000003f0: 2054 4845 2055 5345 204f 5220 4f54 4845   THE USE OR OTHE
+00000400: 5220 4445 414c 494e 4753 2049 4e20 5448  R DEALINGS IN TH
+00000410: 4520 534f 4654 5741 5245 2e0a            E SOFTWARE..
```

### Comparing `slinn-2.2.7/PKG-INFO` & `slinn-2.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,241 +1,240 @@
-Metadata-Version: 2.1
-Name: slinn
-Version: 2.2.7
-Summary: A HTTPS and HTTP server framework
-Home-page: https://slinn.miotp.ru/
-Author: Mark Radin
-Author-email: mrybs2@gmail.com
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Slinn
-
----
-
-**Slinn is a HTTPS and HTTP server framework**
-
-![License](https://img.shields.io/github/license/mrybs/slinn)
-![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
-
-![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
-![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
-
-![GitHub Repo stars](https://img.shields.io/github/stars/mrybs/slinn)
-![GitHub watchers](https://img.shields.io/github/watchers/mrybs/slinn)
-![GitHub forks](https://img.shields.io/github/forks/mrybs/slinn)
-
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/mrybs/slinn)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mrybs/slinn)
-![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
-
-![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
-
-
-### Simple example
-```python
-from slinn import *
-
-
-dp = Dispatcher('localhost', '127.0.0.1')
-
-
-@dp(LinkFilter('api'))
-def api(request):
-    return HttpJSONAPIResponse(status='ok')
-
-@dp(LinkFilter(''))
-@dp(LinkFilter('index'))
-def index(request):
-    return HttpRedirect('/helloworld')
-
-
-@dp(AnyFilter)
-def helloworld(request):
-     return HttpResponse('Hello world!')
-
-```
-
-### Begin project
-#### Standart
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash
-python3 -m slinn create helloworld
-cd helloworld
-venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
-venv/bin/python manage.py run 
-```
-
-##### Windows:
-```batch
-py -m slinn create helloworld
-cd helloworld
-venv\Scripts\activate
-py manage.py create localhost host=localhost host=127.0.0.1
-py manage.py run 
-```
-
-Insert example into localhost/app.py file
-
-Excepted output
-```
-helloworld $ venv/bin/python manage.py run
-Loading config...
-Apps: firstrun
-Debug mode enabled
-Smart navigation enabled
-
-Starting server...
-HTTP server is available on http://localhost:8080/
-```
-
-To config project you should edit `./project.json`
-
-To config app you should edit `./%app%/config.json`
-
-#### Classic
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash 
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv/bin/activate
-```
-
-##### Windows:
-```batch
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv\Scripts\activate
-```
-
-Insert example into `example.py` and add following code:
-```
-Server(dp).listen(Address(8080))
-```
-then write `python example.py`
-
-Excepted output
-```
-helloworld $ venv/bin/python example.py
-HTTP server is available on http://localhost:8080/
-```
-
-### Functions:
-```python
-from slinn import Server
-
-server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
-server.address(port: int, domain: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
-server.reload(*dispatchers: tuple)  # Reloads server
-server.listen(address: Address)  # Start listening address
-
-Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
-```
-
-```python
-from slinn import Address
-
-address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
-
-Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
-
-# Attributes
-address.port  # port
-address.host  # ip
-address.domain  # non-converted host from constructor
-```
-
-```python
-from slinn import Dispatcher
-
-dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
-
-Dispatcher('localhost', '127.0.0.1', '::1')
-
-# To add handler into dispatcher
-@dispatcher(filter: Filter)
-def handler(request: Request):
-    ...
-
-# handler should return HttpResponse-based object
-```
-
-```python
-from slinn import Filter, LinkFilter, AnyFilter
-
-_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
-_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-
-Filter('/user/.+/profile.*')
-
-# LinkFilter inherits from Filter
-LinkFilter('user/.+/profile')
-
-# AnyFilter as same as Filter('.*')
-```
-
-```python
-from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
-
-http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value: any)  # Sets cookie
-http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
-
-HttpResponse('<h1>Hello world</h1>', content_type='text/html')
-
-# HttpAPIResponse inherits from HttpResponse
-# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
-
-HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
-
-# HttpRedirect inherits from HttpResponse
-HttpRedirect(location: str)
-
-HttpRedirect('slinn.miotp.ru')
-
-# HttpJSONResponse for responding JSON 
-HttpJSONResponse(**payload: dict)
-
-HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
-
-# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
-
-HttpJSONAPIResponse(code=43657, until=1719931149)
-```
-
-```python
-from slinn import Request
-
-request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
-request.parse_http_header(http_header: str)  # Parse HTTP request`s header
-request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
-str(request)  # Convert slinn.Request to info text
-
-# Attributes
-request.ip, request.port  # Client`s IP and port
-request.method  # HTTP method
-request.version  # HTTP version
-request.full_link  # Full link(path and params)
-request.host  # Requested host
-request.user_agent  # Client`s user agent
-request.accept  # maybe supported technologies
-request.encoding  # Supported encodings
-request.language  # Client`s language
-request.link  # Link(only path)
-request.args  # GET args
-request.cookies  # All saved cookies
-request.files # Uploaded files
-```
-
-```python
-from slinn import File
-
-file = File(id: str=None, data: bytes|bytearray=bytearray())
-
-# Attributes
-file.id  # File`s id 
-file.data  # Binary data
-file.headers  # Headers such as Content-Disposition
-```
+Metadata-Version: 2.1
+Name: slinn
+Version: 2.2.8
+Summary: A HTTPS and HTTP server framework
+Home-page: https://slinn.miotp.ru/
+Author: Mark Radin
+Author-email: mrybs2@gmail.com
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Slinn
+
+---
+
+**Slinn is a HTTPS and HTTP server framework**
+
+![License](https://img.shields.io/github/license/mrybs/slinn)
+![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
+
+![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
+![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
+
+![GitHub Repo stars](https://img.shields.io/github/stars/mrybs/slinn)
+![GitHub watchers](https://img.shields.io/github/watchers/mrybs/slinn)
+![GitHub forks](https://img.shields.io/github/forks/mrybs/slinn)
+
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/mrybs/slinn)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mrybs/slinn)
+![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
+
+![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
+
+
+### Simple example
+```python
+from slinn import *
+
+
+dp = Dispatcher()
+
+@dp(LinkFilter('api'))
+def api(request):
+    return HttpJSONAPIResponse(status='ok')
+
+@dp(LinkFilter(''))
+@dp(LinkFilter('index'))
+def index(request):
+    return HttpRedirect('/helloworld')
+
+
+@dp(AnyFilter)
+def helloworld(request):
+     return HttpResponse('Hello world!')
+
+```
+
+### Begin project
+#### Standart
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash
+python3 -m slinn create helloworld
+cd helloworld
+venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
+venv/bin/python manage.py run 
+```
+
+##### Windows:
+```batch
+py -m slinn create helloworld
+cd helloworld
+venv\Scripts\activate
+py manage.py create localhost host=localhost host=127.0.0.1
+py manage.py run 
+```
+
+Insert example into localhost/app.py file
+
+Excepted output
+```
+helloworld $ venv/bin/python manage.py run
+Loading config...
+Apps: firstrun
+Debug mode enabled
+Smart navigation enabled
+
+Starting server...
+HTTP server is available on http://localhost:8080/
+```
+
+To config project you should edit `./project.json`
+
+To config app you should edit `./%app%/config.json`
+
+#### Classic
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash 
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv/bin/activate
+```
+
+##### Windows:
+```batch
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv\Scripts\activate
+```
+
+Insert example into `example.py` and add following code:
+```
+Server(dp).listen(Address(8080))
+```
+then write `python example.py`
+
+Excepted output
+```
+helloworld $ venv/bin/python example.py
+HTTP server is available on http://localhost:8080/
+```
+
+### Functions:
+```python
+from slinn import Server
+
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
+server.address(port: int, domain: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
+server.reload(*dispatchers: tuple)  # Reloads server
+server.listen(address: Address)  # Start listening address
+
+Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
+```
+
+```python
+from slinn import Address
+
+address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
+
+Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
+
+# Attributes
+address.port  # port
+address.host  # ip
+address.domain  # non-converted host from constructor
+```
+
+```python
+from slinn import Dispatcher
+
+dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
+
+Dispatcher('localhost', '127.0.0.1', '::1', '::')
+
+# To add handler into dispatcher
+@dispatcher(filter: Filter)
+def handler(request: Request):
+    ...
+
+# handler should return HttpResponse-based object
+```
+
+```python
+from slinn import Filter, LinkFilter, AnyFilter
+
+_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
+_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
+
+Filter('/user/.+/profile.*')
+
+# LinkFilter inherits from Filter
+LinkFilter('user/.+/profile')
+
+# AnyFilter as same as Filter('.*')
+```
+
+```python
+from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
+
+http_response = HttpResponse(payload: any, data: list[tuple[str, any]]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
+http_response.set_cookie(key: str, value: any)  # Sets cookie
+http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
+
+HttpResponse('<h1>Hello world</h1>', content_type='text/html')
+
+# HttpAPIResponse inherits from HttpResponse
+# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
+
+HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
+
+# HttpRedirect inherits from HttpResponse
+HttpRedirect(location: str)
+
+HttpRedirect('slinn.miotp.ru')
+
+# HttpJSONResponse for responding JSON 
+HttpJSONResponse(**payload: dict)
+
+HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
+
+# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
+
+HttpJSONAPIResponse(code=43657, until=1719931149)
+```
+
+```python
+from slinn import Request
+
+request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
+request.parse_http_header(http_header: str)  # Parse HTTP request`s header
+request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
+str(request)  # Convert slinn.Request to info text
+
+# Attributes
+request.ip, request.port  # Client`s IP and port
+request.method  # HTTP method
+request.version  # HTTP version
+request.full_link  # Full link(path and params)
+request.host  # Requested host
+request.user_agent  # Client`s user agent
+request.accept  # maybe supported technologies
+request.encoding  # Supported encodings
+request.language  # Client`s language
+request.link  # Link(only path)
+request.args  # GET args
+request.cookies  # All saved cookies
+request.files # Uploaded files
+```
+
+```python
+from slinn import File
+
+file = File(id: str=None, data: bytes|bytearray=bytearray())
+
+# Attributes
+file.id  # File`s id 
+file.data  # Binary data
+file.headers  # Headers such as Content-Disposition
+```
```

### Comparing `slinn-2.2.7/README.md` & `slinn-2.2.8/slinn.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,230 +1,240 @@
-# Slinn
-
----
-
-**Slinn is a HTTPS and HTTP server framework**
-
-![License](https://img.shields.io/github/license/mrybs/slinn)
-![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
-
-![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
-![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
-
-![GitHub Repo stars](https://img.shields.io/github/stars/mrybs/slinn)
-![GitHub watchers](https://img.shields.io/github/watchers/mrybs/slinn)
-![GitHub forks](https://img.shields.io/github/forks/mrybs/slinn)
-
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/mrybs/slinn)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mrybs/slinn)
-![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
-
-![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
-
-
-### Simple example
-```python
-from slinn import *
-
-
-dp = Dispatcher('localhost', '127.0.0.1')
-
-
-@dp(LinkFilter('api'))
-def api(request):
-    return HttpJSONAPIResponse(status='ok')
-
-@dp(LinkFilter(''))
-@dp(LinkFilter('index'))
-def index(request):
-    return HttpRedirect('/helloworld')
-
-
-@dp(AnyFilter)
-def helloworld(request):
-     return HttpResponse('Hello world!')
-
-```
-
-### Begin project
-#### Standart
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash
-python3 -m slinn create helloworld
-cd helloworld
-venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
-venv/bin/python manage.py run 
-```
-
-##### Windows:
-```batch
-py -m slinn create helloworld
-cd helloworld
-venv\Scripts\activate
-py manage.py create localhost host=localhost host=127.0.0.1
-py manage.py run 
-```
-
-Insert example into localhost/app.py file
-
-Excepted output
-```
-helloworld $ venv/bin/python manage.py run
-Loading config...
-Apps: firstrun
-Debug mode enabled
-Smart navigation enabled
-
-Starting server...
-HTTP server is available on http://localhost:8080/
-```
-
-To config project you should edit `./project.json`
-
-To config app you should edit `./%app%/config.json`
-
-#### Classic
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash 
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv/bin/activate
-```
-
-##### Windows:
-```batch
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv\Scripts\activate
-```
-
-Insert example into `example.py` and add following code:
-```
-Server(dp).listen(Address(8080))
-```
-then write `python example.py`
-
-Excepted output
-```
-helloworld $ venv/bin/python example.py
-HTTP server is available on http://localhost:8080/
-```
-
-### Functions:
-```python
-from slinn import Server
-
-server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
-server.address(port: int, domain: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
-server.reload(*dispatchers: tuple)  # Reloads server
-server.listen(address: Address)  # Start listening address
-
-Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
-```
-
-```python
-from slinn import Address
-
-address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
-
-Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
-
-# Attributes
-address.port  # port
-address.host  # ip
-address.domain  # non-converted host from constructor
-```
-
-```python
-from slinn import Dispatcher
-
-dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
-
-Dispatcher('localhost', '127.0.0.1', '::1')
-
-# To add handler into dispatcher
-@dispatcher(filter: Filter)
-def handler(request: Request):
-    ...
-
-# handler should return HttpResponse-based object
-```
-
-```python
-from slinn import Filter, LinkFilter, AnyFilter
-
-_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
-_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-
-Filter('/user/.+/profile.*')
-
-# LinkFilter inherits from Filter
-LinkFilter('user/.+/profile')
-
-# AnyFilter as same as Filter('.*')
-```
-
-```python
-from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
-
-http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value: any)  # Sets cookie
-http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
-
-HttpResponse('<h1>Hello world</h1>', content_type='text/html')
-
-# HttpAPIResponse inherits from HttpResponse
-# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
-
-HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
-
-# HttpRedirect inherits from HttpResponse
-HttpRedirect(location: str)
-
-HttpRedirect('slinn.miotp.ru')
-
-# HttpJSONResponse for responding JSON 
-HttpJSONResponse(**payload: dict)
-
-HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
-
-# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
-
-HttpJSONAPIResponse(code=43657, until=1719931149)
-```
-
-```python
-from slinn import Request
-
-request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
-request.parse_http_header(http_header: str)  # Parse HTTP request`s header
-request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
-str(request)  # Convert slinn.Request to info text
-
-# Attributes
-request.ip, request.port  # Client`s IP and port
-request.method  # HTTP method
-request.version  # HTTP version
-request.full_link  # Full link(path and params)
-request.host  # Requested host
-request.user_agent  # Client`s user agent
-request.accept  # maybe supported technologies
-request.encoding  # Supported encodings
-request.language  # Client`s language
-request.link  # Link(only path)
-request.args  # GET args
-request.cookies  # All saved cookies
-request.files # Uploaded files
-```
-
-```python
-from slinn import File
-
-file = File(id: str=None, data: bytes|bytearray=bytearray())
-
-# Attributes
-file.id  # File`s id 
-file.data  # Binary data
-file.headers  # Headers such as Content-Disposition
-```
+Metadata-Version: 2.1
+Name: slinn
+Version: 2.2.8
+Summary: A HTTPS and HTTP server framework
+Home-page: https://slinn.miotp.ru/
+Author: Mark Radin
+Author-email: mrybs2@gmail.com
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Slinn
+
+---
+
+**Slinn is a HTTPS and HTTP server framework**
+
+![License](https://img.shields.io/github/license/mrybs/slinn)
+![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
+
+![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
+![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
+
+![GitHub Repo stars](https://img.shields.io/github/stars/mrybs/slinn)
+![GitHub watchers](https://img.shields.io/github/watchers/mrybs/slinn)
+![GitHub forks](https://img.shields.io/github/forks/mrybs/slinn)
+
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/mrybs/slinn)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mrybs/slinn)
+![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
+
+![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
+
+
+### Simple example
+```python
+from slinn import *
+
+
+dp = Dispatcher()
+
+@dp(LinkFilter('api'))
+def api(request):
+    return HttpJSONAPIResponse(status='ok')
+
+@dp(LinkFilter(''))
+@dp(LinkFilter('index'))
+def index(request):
+    return HttpRedirect('/helloworld')
+
+
+@dp(AnyFilter)
+def helloworld(request):
+     return HttpResponse('Hello world!')
+
+```
+
+### Begin project
+#### Standart
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash
+python3 -m slinn create helloworld
+cd helloworld
+venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
+venv/bin/python manage.py run 
+```
+
+##### Windows:
+```batch
+py -m slinn create helloworld
+cd helloworld
+venv\Scripts\activate
+py manage.py create localhost host=localhost host=127.0.0.1
+py manage.py run 
+```
+
+Insert example into localhost/app.py file
+
+Excepted output
+```
+helloworld $ venv/bin/python manage.py run
+Loading config...
+Apps: firstrun
+Debug mode enabled
+Smart navigation enabled
+
+Starting server...
+HTTP server is available on http://localhost:8080/
+```
+
+To config project you should edit `./project.json`
+
+To config app you should edit `./%app%/config.json`
+
+#### Classic
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash 
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv/bin/activate
+```
+
+##### Windows:
+```batch
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv\Scripts\activate
+```
+
+Insert example into `example.py` and add following code:
+```
+Server(dp).listen(Address(8080))
+```
+then write `python example.py`
+
+Excepted output
+```
+helloworld $ venv/bin/python example.py
+HTTP server is available on http://localhost:8080/
+```
+
+### Functions:
+```python
+from slinn import Server
+
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
+server.address(port: int, domain: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
+server.reload(*dispatchers: tuple)  # Reloads server
+server.listen(address: Address)  # Start listening address
+
+Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
+```
+
+```python
+from slinn import Address
+
+address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
+
+Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
+
+# Attributes
+address.port  # port
+address.host  # ip
+address.domain  # non-converted host from constructor
+```
+
+```python
+from slinn import Dispatcher
+
+dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
+
+Dispatcher('localhost', '127.0.0.1', '::1', '::')
+
+# To add handler into dispatcher
+@dispatcher(filter: Filter)
+def handler(request: Request):
+    ...
+
+# handler should return HttpResponse-based object
+```
+
+```python
+from slinn import Filter, LinkFilter, AnyFilter
+
+_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
+_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
+
+Filter('/user/.+/profile.*')
+
+# LinkFilter inherits from Filter
+LinkFilter('user/.+/profile')
+
+# AnyFilter as same as Filter('.*')
+```
+
+```python
+from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
+
+http_response = HttpResponse(payload: any, data: list[tuple[str, any]]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
+http_response.set_cookie(key: str, value: any)  # Sets cookie
+http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
+
+HttpResponse('<h1>Hello world</h1>', content_type='text/html')
+
+# HttpAPIResponse inherits from HttpResponse
+# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
+
+HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
+
+# HttpRedirect inherits from HttpResponse
+HttpRedirect(location: str)
+
+HttpRedirect('slinn.miotp.ru')
+
+# HttpJSONResponse for responding JSON 
+HttpJSONResponse(**payload: dict)
+
+HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
+
+# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
+
+HttpJSONAPIResponse(code=43657, until=1719931149)
+```
+
+```python
+from slinn import Request
+
+request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
+request.parse_http_header(http_header: str)  # Parse HTTP request`s header
+request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
+str(request)  # Convert slinn.Request to info text
+
+# Attributes
+request.ip, request.port  # Client`s IP and port
+request.method  # HTTP method
+request.version  # HTTP version
+request.full_link  # Full link(path and params)
+request.host  # Requested host
+request.user_agent  # Client`s user agent
+request.accept  # maybe supported technologies
+request.encoding  # Supported encodings
+request.language  # Client`s language
+request.link  # Link(only path)
+request.args  # GET args
+request.cookies  # All saved cookies
+request.files # Uploaded files
+```
+
+```python
+from slinn import File
+
+file = File(id: str=None, data: bytes|bytearray=bytearray())
+
+# Attributes
+file.id  # File`s id 
+file.data  # Binary data
+file.headers  # Headers such as Content-Disposition
+```
```

### Comparing `slinn-2.2.7/setup.py` & `slinn-2.2.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup
-
-def readme():
-    with open('README.md', 'r') as f:
-        return f.read()
-    
-templates = ['firstrun', 'example']
-
-
-setup(name='slinn',
-      version='2.2.7',
-      description='A HTTPS and HTTP server framework',
-      packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
-      package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
-      author='Mark Radin',
-      author_email='mrybs2@gmail.com',
-      url='https://slinn.miotp.ru/',
-      long_description=readme(),
-      long_description_content_type='text/markdown',
-      python_requires='>=3.11',
-      zip_safe=True)
+from setuptools import setup
+
+def readme():
+    with open('README.md', 'r') as f:
+        return f.read()
+    
+templates = ['firstrun', 'example']
+
+
+setup(name='slinn',
+      version='2.2.8',
+      description='A HTTPS and HTTP server framework',
+      packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
+      package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
+      author='Mark Radin',
+      author_email='mrybs2@gmail.com',
+      url='https://slinn.miotp.ru/',
+      long_description=readme(),
+      long_description_content_type='text/markdown',
+      python_requires='>=3.11',
+      zip_safe=True)
```

### Comparing `slinn-2.2.7/slinn/__init__.py` & `slinn-2.2.8/slinn/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from slinn.address import Address
-from slinn.filter import Filter
-from slinn.link_filter import LinkFilter
-from slinn.any_filter import AnyFilter
-from slinn.file import File
-from slinn.request import Request
-from slinn.http_response import HttpResponse
-from slinn.http_redirect import HttpRedirect
-from slinn.http_api_response import HttpAPIResponse
-from slinn.http_json_response import HttpJSONResponse
-from slinn.http_json_api_response import HttpJSONAPIResponse
-from slinn.server import Server
-from slinn.dispatcher import Dispatcher
-
-
-version = 'Slinn Murega v2.2.7 090424A'
+from slinn.address import Address
+from slinn.filter import Filter
+from slinn.link_filter import LinkFilter
+from slinn.any_filter import AnyFilter
+from slinn.file import File
+from slinn.request import Request
+from slinn.http_response import HttpResponse
+from slinn.http_redirect import HttpRedirect
+from slinn.http_api_response import HttpAPIResponse
+from slinn.http_json_response import HttpJSONResponse
+from slinn.http_json_api_response import HttpJSONAPIResponse
+from slinn.server import Server
+from slinn.dispatcher import Dispatcher
+
+
+version = 'Slinn Murega v2.2.8 110424A'
```

### Comparing `slinn-2.2.7/slinn/__main__.py` & `slinn-2.2.8/slinn/__main__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import sys, venv
-from slinn.default import *
-
-
-RED = '\u001b[31m'
-GREEN = '\u001b[32m'
-BLUE = '\u001b[34m'
-RESET = '\u001b[0m'
-BOLD = '\u001b[1m'
-GRAY = '\u001b[38;2;127;127;127m'
-
-
-if __name__ == '__main__':
-	if len(sys.argv) > 1:
-		if sys.argv[1].lower() == 'create':
-			args = get_args(['path'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			import os, slinn, shutil, platform
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			if not os.path.isdir(apppath):
-				os.mkdir(apppath)
-			else:
-				print(f'{BLUE}{apppath} has already existed{RESET}')
-			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
-			shutil.copyfile(modulepath+'default/project.json', f'{apppath}/project.json')
-			venv.create(f'{apppath}/venv')
-			packages_dir = ''
-			if platform.system() == 'Windows':
-				packages_dir = f'{apppath}/venv/Lib/site-packages'
-			else:
-				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
-			try:
-				os.makedirs(packages_dir)
-			except FileExistsError:
-				pass
-			try:
-				shutil.copytree(modulepath, packages_dir+'/slinn')
-			except FileNotFoundError:
-				print(f'{RED}Cannot install slinn to the new virtual environment{RESET}')
-				exit()
-			try:
-				import pip
-				shutil.copytree(os.path.abspath(pip.__file__).replace('__init__.py', ''), packages_dir+'/pip')
-			except FileNotFoundError:
-				print(f'{BLUE}pip was not installed{RESET}')
-			try:
-				import wheel
-				shutil.copytree(os.path.abspath(wheel.__file__).replace('__init__.py', ''), packages_dir+'/wheel')
-			except Exception:
-				print(f'{BLUE}wheel was not installed{RESET}')
-			try:
-				import setuptools
-				shutil.copytree(os.path.abspath(setuptools.__file__).replace('__init__.py', ''), packages_dir+'/setuptools')
-			except Exception:
-				print(f'{BLUE}setuptools was not installed{RESET}')
-			print(f'{GREEN}Project has created{RESET}')
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			try:
-				shutil.copytree(f'{modulepath}templates/firstrun/', f'{apppath}/firstrun')
-				shutil.copytree(f'{modulepath}templates/firstrun/data/', f'{apppath}/templates_data/firstrun')
-				print(f'{GREEN}Template firstrun successfully installed{RESET}') 
-			except FileExistsError:
-				print(f'{BLUE}Template firstrun has already existed installed{RESET}')
-			except FileNotFoundError:
-				print(f'{BLUE}Template firstrun not found{RESET}')
-		elif sys.argv[1].lower() == 'update':
-			args = get_args(['path'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			import os, slinn, shutil, platform
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			if not os.path.isdir(apppath):
-				print(f'{BLUE}`{apppath}` does not exist{RESET}')
-				exit()
-			packages_dir = ''
-			if platform.system() == 'Windows':
-				packages_dir = f'{apppath}/venv/Lib/site-packages'
-			else:
-				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
-			if not os.path.isdir(packages_dir+'/slinn'):
-				print(f'{RED}Virtual environment directory is corrupted. Reinstall the project{RESET}')
-				exit()
-			if not os.path.isfile(apppath+'/manage.py'):
-				print(f'{RED}manage.py file does not exist. Reinstall the project{RESET}')
-				exit()
-			shutil.rmtree(packages_dir+'/slinn')
-			os.remove(apppath+'/manage.py')
-			shutil.copytree(modulepath, packages_dir+'/slinn')
-			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
-			print(f'{GREEN}Project has updated{RESET}')
-		elif sys.argv[1].lower() == 'help':
-			print("""%BOLD%Slinn help page
-
-Commands%RESET%:
-	%cmd% create {project`s name}		%GRAY%# Creates a new project%RESET%
-	%cmd% update {project`s name}		%GRAY%# Updates the project%RESET%
-	%cmd% help                   		%GRAY%# Prints this help%RESET%
-	%cmd% version                		%GRAY%# Prints version of Slinn%RESET%
-""".replace('%cmd%', f'py -m slinn').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
-		elif sys.argv[1].lower() == 'version':
-			print(slinn_version)
-		else:
-			print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
-	else:
-		print(f'{RED}Command was not specified{RESET}')
-
+import sys, venv
+from slinn.default import *
+
+
+RED = '\u001b[31m'
+GREEN = '\u001b[32m'
+BLUE = '\u001b[34m'
+RESET = '\u001b[0m'
+BOLD = '\u001b[1m'
+GRAY = '\u001b[38;2;127;127;127m'
+
+
+if __name__ == '__main__':
+	if len(sys.argv) > 1:
+		if sys.argv[1].lower() == 'create':
+			args = get_args(['path'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			import os, slinn, shutil, platform
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			if not os.path.isdir(apppath):
+				os.mkdir(apppath)
+			else:
+				print(f'{BLUE}{apppath} has already existed{RESET}')
+			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
+			shutil.copyfile(modulepath+'default/project.json', f'{apppath}/project.json')
+			venv.create(f'{apppath}/venv')
+			packages_dir = ''
+			if platform.system() == 'Windows':
+				packages_dir = f'{apppath}/venv/Lib/site-packages'
+			else:
+				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
+			try:
+				os.makedirs(packages_dir)
+			except FileExistsError:
+				pass
+			try:
+				shutil.copytree(modulepath, packages_dir+'/slinn')
+			except FileNotFoundError:
+				print(f'{RED}Cannot install slinn to the new virtual environment{RESET}')
+				exit()
+			try:
+				import pip
+				shutil.copytree(os.path.abspath(pip.__file__).replace('__init__.py', ''), packages_dir+'/pip')
+			except FileNotFoundError:
+				print(f'{BLUE}pip was not installed{RESET}')
+			try:
+				import wheel
+				shutil.copytree(os.path.abspath(wheel.__file__).replace('__init__.py', ''), packages_dir+'/wheel')
+			except Exception:
+				print(f'{BLUE}wheel was not installed{RESET}')
+			try:
+				import setuptools
+				shutil.copytree(os.path.abspath(setuptools.__file__).replace('__init__.py', ''), packages_dir+'/setuptools')
+			except Exception:
+				print(f'{BLUE}setuptools was not installed{RESET}')
+			print(f'{GREEN}Project has created{RESET}')
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			try:
+				shutil.copytree(f'{modulepath}templates/firstrun/', f'{apppath}/firstrun')
+				shutil.copytree(f'{modulepath}templates/firstrun/data/', f'{apppath}/templates_data/firstrun')
+				print(f'{GREEN}Template firstrun successfully installed{RESET}') 
+			except FileExistsError:
+				print(f'{BLUE}Template firstrun has already existed installed{RESET}')
+			except FileNotFoundError:
+				print(f'{BLUE}Template firstrun not found{RESET}')
+		elif sys.argv[1].lower() == 'update':
+			args = get_args(['path'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			import os, slinn, shutil, platform
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			if not os.path.isdir(apppath):
+				print(f'{BLUE}`{apppath}` does not exist{RESET}')
+				exit()
+			packages_dir = ''
+			if platform.system() == 'Windows':
+				packages_dir = f'{apppath}/venv/Lib/site-packages'
+			else:
+				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
+			if not os.path.isdir(packages_dir+'/slinn'):
+				print(f'{RED}Virtual environment directory is corrupted. Reinstall the project{RESET}')
+				exit()
+			if not os.path.isfile(apppath+'/manage.py'):
+				print(f'{RED}manage.py file does not exist. Reinstall the project{RESET}')
+				exit()
+			shutil.rmtree(packages_dir+'/slinn')
+			os.remove(apppath+'/manage.py')
+			shutil.copytree(modulepath, packages_dir+'/slinn')
+			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
+			print(f'{GREEN}Project has updated{RESET}')
+		elif sys.argv[1].lower() == 'help':
+			print("""%BOLD%Slinn help page
+
+Commands%RESET%:
+	%cmd% create {project`s name}		%GRAY%# Creates a new project%RESET%
+	%cmd% update {project`s name}		%GRAY%# Updates the project%RESET%
+	%cmd% help                   		%GRAY%# Prints this help%RESET%
+	%cmd% version                		%GRAY%# Prints version of Slinn%RESET%
+""".replace('%cmd%', f'py -m slinn').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
+		elif sys.argv[1].lower() == 'version':
+			print(slinn_version)
+		else:
+			print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
+	else:
+		print(f'{RED}Command was not specified{RESET}')
+
```

### Comparing `slinn-2.2.7/slinn/default/manage.py` & `slinn-2.2.8/slinn/default/manage.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-import sys, os, shutil, json, base64
-from slinn import version as slinn_version
-import slinn
-
-RED = '\u001b[31m'
-GREEN = '\u001b[32m'
-BLUE = '\u001b[34m'
-RESET = '\u001b[0m'
-BOLD = '\u001b[1m'
-GRAY = '\u001b[38;2;127;127;127m'
-
-
-def arg_parse(arg: str):
-	return base64.urlsafe_b64decode(arg.removeprefix('b64@').encode()+b'==').decode() if arg.startswith('b64@') else arg
-
-def splits(string: str, delimeters: list[str]=[' ', '\n'], quotes: list[str]=[]):
-		result = ['']
-		current_quote = ''
-		for char in str(string):
-			if char in quotes:
-				if current_quote == '':
-					current_quote = char
-					continue
-				elif current_quote == char:
-					current_quote = ''
-					continue
-			if current_quote == '':
-				if char in delimeters:
-					result.append('')
-				else:
-					result[-1] += char
-			else:
-				result[-1] += char
-		return result
-
-def get_args(expecting, text):
-	text = text.strip()
-	if text == '':
-		return {}
-	args = {'not_used': []}
-	Ds = ['\n', ' ']
-	Qs = ['"', "'", '`']
-	spls  = splits(text, Ds, Qs)
-	i = 0
-	while i < len(spls):
-		arg = str(spls[i])
-		try:
-			if arg.strip().endswith('='):
-				W = arg.strip().removesuffix('=').strip()
-				expecting.pop(expecting.index(W))
-				args[W] = arg_parse(str(splits[i + 1]))
-				i += 2
-				continue
-			if len(splits(arg, ['='], Qs)) == 2:
-				spl = splits(arg, ['='])
-				W = str(spl[0])
-				if W not in args.keys():
-					args[W] = arg_parse(str(spl[1]))
-					expecting.pop(expecting.index(W))
-				else:
-					args[W] = [args[W]]
-					args[W].append(arg_parse(str(spl[1])))
-				i += 1
-				continue
-		except ValueError:
-			pass
-
-		if len(expecting) == 0:
-			args['not_used'].append(arg_parse(arg))
-			i += 1
-			continue
-
-		E = expecting.pop(0)
-		args[E] = arg_parse(arg)
-		i += 1
-	return args
-
-def replace_all(text: str, sss: list[str] | str, ss2: str) -> str:
-	for ss1 in sss:
-		text = text.replace(ss1, ss2)
-	return text
-
-def add_quotes_to_list(lst: list[str]):
-		for l in lst:
-			yield f'\'{l}\''
-
-def update():
-	project = open('project.json', 'r')
-	project_json = json.loads(project.read())
-	project.close()
-	if 'apps' not in project_json.keys():
-		return print(f'Updated project.json')
-	apps = []
-	for app in project_json['apps']:
-		if os.path.isdir(app):
-			apps.append(app)
-	project_json['apps'] = apps
-	project = open('project.json', 'w')
-	project.write(json.dumps(project_json, indent=4))
-	project.close()
-	return print(f'Updated project.json')
-
-def main():
-	if len(sys.argv) > 1:
-		if sys.argv[1].lower() == 'run':
-			from slinn import Server, Address
-
-			def config():
-				file = open('project.json')
-				cfg = json.loads(file.read())
-				file.close()
-				return cfg
-			
-			def app_config(app):
-				try:
-					cfg = {"debug": False}
-					file = open(f'{app}/config.json')
-					cfg.update(json.loads(file.read()))
-					file.close()
-					return cfg
-				except FileNotFoundError:
-					print(f'{RED}{app}/config.json file not found{RESET}')
-					exit()
-
-
-			def load_imports(apps, debug=False):
-				imports = []
-				for app in apps:
-					if not app_config(app)['debug'] or debug:
-						imports.append(f'import {app}')
-				return imports
-
-
-			def get_dispatchers(apps, debug=False):
-				dispachers = []
-				for app in apps:
-					if not app_config(app)['debug'] or debug:
-						dispachers.append(f'{app}.dp')
-				return dispachers
-			
-			def app_reload(app):
-				return f'global {app};{app} = importlib.reload({app});'
-			
-			print('Loading config...')
-			cfg = config()
-			debug = cfg["debug"] if "debug" in cfg.keys() else False
-			apps = cfg['apps'] if 'apps' in cfg.keys() else []
-			port = cfg['port'] if 'port' in cfg.keys() else 8080
-			host = cfg['host'] if 'host' in cfg.keys() else ''
-			timeout = float(cfg['timeout']) if 'timeout' in cfg.keys() else 0.03
-			max_bytes_per_recieve = int(cfg['max_bytes_per_recieve']) if 'max_bytes_per_recieve' in cfg.keys() else 4096
-			max_bytes = int(cfg['max_bytes']) if 'max_bytes' in cfg.keys() else 4294967296
-			smart_navigation = cfg['smart_navigation'] if 'smart_navigation' in cfg.keys() else True
-			ssl_fullchain, ssl_key = None, None
-			if 'ssl' in cfg.keys() and 'fullchain' in cfg['ssl'].keys() and 'key' in cfg['ssl'].keys():
-				ssl_fullchain = '"'+cfg['ssl']['fullchain']+'"' if cfg['ssl']['fullchain'] else None    
-				ssl_key = '"'+cfg['ssl']['key']+'"' if cfg['ssl']['key'] else None
-			dps = get_dispatchers(apps, debug)
-			if dps == []:
-				print(f'{RED}Dispatchers not found. Check your apps and ./project.json{RESET}')
-				exit()
-			global get_dir_checksum
-			def get_dir_checksum(dir):
-				import hashlib
-				def get_dir_checksums(dir):
-					def md5(fname):
-						hash_md5 = hashlib.md5()
-						with open(fname, "rb") as f:
-							for chunk in iter(lambda: f.read(4096), b""):
-								hash_md5.update(chunk)
-						return hash_md5.hexdigest()
-					paths = os.listdir(dir)
-					checksums = []
-					for path in paths:
-						if os.path.isdir(path):
-							checksums += get_dir_checksums(dir+'/'+path)
-						elif path.endswith('.py'):
-							checksums.append(path+md5(dir+'/'+path))
-					return checksums
-				return hashlib.md5(''.join([checksum for checksum in get_dir_checksums(dir)]).encode()).hexdigest()
-			global checksum
-			checksum = get_dir_checksum('.')
-
-			reloader = """
-def reloader(server):
-	import importlib, traceback
-	global checksum
-	try:
-		if checksum != get_dir_checksum('.'):
-			checksum = get_dir_checksum('.')
-			"""
-			for app in cfg['apps']:
-				if not app_config(app)['debug'] or debug:
-					reloader += app_reload(app)
-			reloader += """
-			server.reload("""
-			reloader += ",".join(dps)
-			reloader += """)
-	except Exception:
-		print('During handling request, an exception has occured:')
-		traceback.print_exc()
-"""
-
-			apps_info = []
-			for app in cfg['apps']:
-				if not app_config(app)['debug'] or debug:
-					apps_info.append(app)
-				else:
-					apps_info.append('['+app+']')
-			print(f'{GRAY}Apps: ' + ', '.join(apps_info))
-			print('Debug mode ' + 'enabled' if debug else 'disabled')
-			print('Smart navigation ' + ('enabled' if smart_navigation else 'disabled'))
-			print(RESET)
-
-			print('Starting server...')
-			start = ';'.join(load_imports(apps, debug))+reloader+f'server=Server({",".join(dps)}, smart_navigation={smart_navigation}, ssl_fullchain={ssl_fullchain}, ssl_key={ssl_key}, timeout={timeout}, max_bytes_per_recieve={max_bytes_per_recieve}, max_bytes={max_bytes}, _func=reloader);server.listen(Address({port}, "{host}"))'
-			exec(start)
-		elif sys.argv[1].lower() == 'create':
-			args = get_args(['name', 'host'], ' '.join(sys.argv[2:]))
-			if 'name' not in args.keys():
-				return print(f'{RED}The app`s name is not specified{RESET}')
-			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
-			if os.path.isdir(ensure_appname):
-				return print(f'{BLUE}The app named {args["name"]} exists{RESET}')
-			if 'host' not in args.keys():
-				print(f'{BLUE}Hosts were not specified')
-			os.mkdir(ensure_appname)
-			with open(f'{ensure_appname}/__init__.py', 'w') as f:
-				data = """import sys, importlib
-if '%appname%.app' not in sys.modules.keys():
-    from %appname%.app import dp
-else:
-    dp = importlib.reload(sys.modules['%appname%.app']).dp
-""".replace('%appname%', ensure_appname)
-				f.write(data)
-			with open(f'{ensure_appname}/app.py', 'w') as f:
-				data = """from slinn import Dispatcher, Filter, HttpResponse
- 
-dp = Dispatcher(%hosts%)
-
-# Write your code down here                         
-""".replace('%appname%', ensure_appname).replace('%hosts%', '' if 'host' not in args.keys() else ', '.join(add_quotes_to_list(args['host'] if type(args['host']) == list else [args['host']])))
-				f.write(data)
-			with open(f'{ensure_appname}/config.json', 'w') as f:
-				data = """
-{
-	"debug": false
-}
-"""
-				f.write(data)
-			fr = open('project.json', 'r')
-			fj = json.loads(fr.read())
-			fr.close()
-			if 'apps' in fj.keys():
-				fj['apps'].insert(0, ensure_appname)
-			else:
-				fj['apps'] = []
-			fw = open('project.json', 'w')
-			fw.write(json.dumps(fj, indent=4))
-			fw.close()
-			update()
-			print(f'{GREEN}App successfully created{RESET}')
-		elif sys.argv[1].lower() == 'delete':
-			args = get_args(['name'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			if 'name' not in args.keys():
-				return print(f'{RED}The app`s name is not specified{RESET}')
-			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
-			if not os.path.isdir(ensure_appname):
-				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
-			if input(f'{RESET}Are you sure? (y/N) >>> ').lower() not in ['y', 'yes']:
-				return print(f'{RESET}Aborted')
-			shutil.rmtree(ensure_appname)
-			if os.path.isdir(f'{apppath}/templates_data/{ensure_appname}'):
-				shutil.rmtree(f'{apppath}/templates_data/{ensure_appname}')
-			if len(os.listdir(f'{apppath}/templates_data')) == 0:
-				shutil.rmtree(f'{apppath}/templates_data')
-			update()
-			return print(f'{GREEN}App successfully deleted{RESET}')
-		elif sys.argv[1].lower() == 'update':
-			return update()
-		elif sys.argv[1].lower() == 'help':
-			return print("""%BOLD%Slinn manager help page
-
-Commands%RESET%:
-	%cmd% run                                                              %GRAY%# Starts server%RESET%
-	%cmd% create {app`s name} host=(host1) host=(host2)...                 %GRAY%# Creates a new app
-		Example: %cmd% create localhost host=localhost host=127.0.0.1%RESET%
-	%cmd% delete {app`s name} (project`s path)                             %GRAY%# Deletes an app
-		Example: %cmd% delete localhost%RESET%
-	%cmd% template {template`s name} (projects`s path)                     %GRAY%# Installs a template
-		Example: %cmd% template firstrun%RESET%
-	%cmd% update                                                           %GRAY%# Updates project.py%RESET%
-	%cmd% migrate_app {app`s name}                                         %GRAY%# Migrates app(check slinn.guides.migration1xx2xx.migration1xx2xx)%RESET%
-	%cmd% help                                                             %GRAY%# Prints this help%RESET%
-	%cmd% version                                                          %GRAY%# Prints version of Slinn%RESET%
-""".replace('%cmd%', f'py {sys.argv[0]}').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
-		elif sys.argv[1].lower() == 'version':
-			return print(slinn_version)
-		elif sys.argv[1].lower() == 'template':
-			args = get_args(['name', 'path'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			if 'name' not in args.keys():
-				return print(f'{RED}Template name is not specified{RESET}')
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			fr = open('project.json', 'r')
-			fj = json.loads(fr.read())
-			fr.close()
-			if 'apps' in fj.keys():
-				fj['apps'].insert(0, args['name'])
-			else:
-				fj['apps'] = []
-			fw = open('project.json', 'w')
-			fw.write(json.dumps(fj, indent=4))
-			fw.close()
-			update()
-			try:
-				shutil.copytree(f'{modulepath}templates/{args["name"]}/', f'{apppath}/{args["name"]}')
-				try:
-					if not os.isdir(f'{apppath}/templates_data'):
-						os.mkdir(f'{apppath}/templates_data')
-					shutil.copytree(f'{modulepath}templates/{args["name"]}/data/', f'{apppath}/templates_data/{args["name"]}')
-				except  FileExistsError:
-					pass
-				except FileNotFoundError:
-					pass
-				return print(f'{GREEN}Template {args["name"]} successfully installed{RESET}') 
-			except FileExistsError:
-				return print(f'{BLUE}Template {args["name"]} has already installed{RESET}')
-			except FileNotFoundError:
-				return print(f'{BLUE}Template {args["name"]} not found{RESET}')
-		elif sys.argv[1].lower() == 'migrate_app':
-			args = get_args(['name'], ' '.join(sys.argv[2:]))
-			if 'name' not in args.keys():
-				return print(f'{RED}The app`s name is not specified{RESET}')
-			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
-			if not os.path.isdir(ensure_appname):
-				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
-			with open(f'{ensure_appname}/__init__.py', 'w') as f:
-				data = """import sys, importlib
-if '%appname%.app' not in sys.modules.keys():
-    from %appname%.app import dp
-else:
-    dp = importlib.reload(sys.modules['%appname%.app']).dp
-""".replace('%appname%', ensure_appname)
-				f.write(data)
-			with open(f'{ensure_appname}/config.json', 'w') as f:
-				data = """
-{
-	"debug": false
-}
-"""
-				f.write(data)
-			print(f'{GREEN}App successfully migrated{RESET}')
-		else:
-			return print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
-	else:
-		return print(f'{RED}Command was not specified{RESET}')
-
-			
-if __name__ == '__main__':
+import sys, os, shutil, json, base64
+from slinn import version as slinn_version
+import slinn
+
+RED = '\u001b[31m'
+GREEN = '\u001b[32m'
+BLUE = '\u001b[34m'
+RESET = '\u001b[0m'
+BOLD = '\u001b[1m'
+GRAY = '\u001b[38;2;127;127;127m'
+
+
+def arg_parse(arg: str):
+	return base64.urlsafe_b64decode(arg.removeprefix('b64@').encode()+b'==').decode() if arg.startswith('b64@') else arg
+
+def splits(string: str, delimeters: list[str]=[' ', '\n'], quotes: list[str]=[]):
+		result = ['']
+		current_quote = ''
+		for char in str(string):
+			if char in quotes:
+				if current_quote == '':
+					current_quote = char
+					continue
+				elif current_quote == char:
+					current_quote = ''
+					continue
+			if current_quote == '':
+				if char in delimeters:
+					result.append('')
+				else:
+					result[-1] += char
+			else:
+				result[-1] += char
+		return result
+
+def get_args(expecting, text):
+	text = text.strip()
+	if text == '':
+		return {}
+	args = {'not_used': []}
+	Ds = ['\n', ' ']
+	Qs = ['"', "'", '`']
+	spls  = splits(text, Ds, Qs)
+	i = 0
+	while i < len(spls):
+		arg = str(spls[i])
+		try:
+			if arg.strip().endswith('='):
+				W = arg.strip().removesuffix('=').strip()
+				expecting.pop(expecting.index(W))
+				args[W] = arg_parse(str(splits[i + 1]))
+				i += 2
+				continue
+			if len(splits(arg, ['='], Qs)) == 2:
+				spl = splits(arg, ['='])
+				W = str(spl[0])
+				if W not in args.keys():
+					args[W] = arg_parse(str(spl[1]))
+					expecting.pop(expecting.index(W))
+				else:
+					args[W] = [args[W]]
+					args[W].append(arg_parse(str(spl[1])))
+				i += 1
+				continue
+		except ValueError:
+			pass
+
+		if len(expecting) == 0:
+			args['not_used'].append(arg_parse(arg))
+			i += 1
+			continue
+
+		E = expecting.pop(0)
+		args[E] = arg_parse(arg)
+		i += 1
+	return args
+
+def replace_all(text: str, sss: list[str] | str, ss2: str) -> str:
+	for ss1 in sss:
+		text = text.replace(ss1, ss2)
+	return text
+
+def add_quotes_to_list(lst: list[str]):
+		for l in lst:
+			yield f'\'{l}\''
+
+def update():
+	project = open('project.json', 'r')
+	project_json = json.loads(project.read())
+	project.close()
+	if 'apps' not in project_json.keys():
+		return print(f'Updated project.json')
+	apps = []
+	for app in project_json['apps']:
+		if os.path.isdir(app):
+			apps.append(app)
+	project_json['apps'] = apps
+	project = open('project.json', 'w')
+	project.write(json.dumps(project_json, indent=4))
+	project.close()
+	return print(f'Updated project.json')
+
+def main():
+	if len(sys.argv) > 1:
+		if sys.argv[1].lower() == 'run':
+			from slinn import Server, Address
+
+			def config():
+				file = open('project.json')
+				cfg = json.loads(file.read())
+				file.close()
+				return cfg
+			
+			def app_config(app):
+				try:
+					cfg = {"debug": False}
+					file = open(f'{app}/config.json')
+					cfg.update(json.loads(file.read()))
+					file.close()
+					return cfg
+				except FileNotFoundError:
+					print(f'{RED}{app}/config.json file not found{RESET}')
+					exit()
+
+
+			def load_imports(apps, debug=False):
+				imports = []
+				for app in apps:
+					if not app_config(app)['debug'] or debug:
+						imports.append(f'import {app}')
+				return imports
+
+
+			def get_dispatchers(apps, debug=False):
+				dispachers = []
+				for app in apps:
+					if not app_config(app)['debug'] or debug:
+						dispachers.append(f'{app}.dp')
+				return dispachers
+			
+			def app_reload(app):
+				return f'global {app};{app} = importlib.reload({app});'
+			
+			print('Loading config...')
+			cfg = config()
+			debug = cfg["debug"] if "debug" in cfg.keys() else False
+			apps = cfg['apps'] if 'apps' in cfg.keys() else []
+			port = cfg['port'] if 'port' in cfg.keys() else 8080
+			host = cfg['host'] if 'host' in cfg.keys() else ''
+			timeout = float(cfg['timeout']) if 'timeout' in cfg.keys() else 0.03
+			max_bytes_per_recieve = int(cfg['max_bytes_per_recieve']) if 'max_bytes_per_recieve' in cfg.keys() else 4096
+			max_bytes = int(cfg['max_bytes']) if 'max_bytes' in cfg.keys() else 4294967296
+			smart_navigation = cfg['smart_navigation'] if 'smart_navigation' in cfg.keys() else True
+			ssl_fullchain, ssl_key = None, None
+			if 'ssl' in cfg.keys() and 'fullchain' in cfg['ssl'].keys() and 'key' in cfg['ssl'].keys():
+				ssl_fullchain = '"'+cfg['ssl']['fullchain']+'"' if cfg['ssl']['fullchain'] else None    
+				ssl_key = '"'+cfg['ssl']['key']+'"' if cfg['ssl']['key'] else None
+			dps = get_dispatchers(apps, debug)
+			if dps == []:
+				print(f'{RED}Dispatchers not found. Check your apps and ./project.json{RESET}')
+				exit()
+			global get_dir_checksum
+			def get_dir_checksum(dir):
+				import hashlib
+				def get_dir_checksums(dir):
+					def md5(fname):
+						hash_md5 = hashlib.md5()
+						with open(fname, "rb") as f:
+							for chunk in iter(lambda: f.read(4096), b""):
+								hash_md5.update(chunk)
+						return hash_md5.hexdigest()
+					paths = os.listdir(dir)
+					checksums = []
+					for path in paths:
+						if os.path.isdir(path):
+							checksums += get_dir_checksums(dir+'/'+path)
+						elif path.endswith('.py'):
+							checksums.append(path+md5(dir+'/'+path))
+					return checksums
+				return hashlib.md5(''.join([checksum for checksum in get_dir_checksums(dir)]).encode()).hexdigest()
+			global checksum
+			checksum = get_dir_checksum('.')
+
+			reloader = """
+def reloader(server):
+	import importlib, traceback
+	global checksum
+	try:
+		if checksum != get_dir_checksum('.'):
+			checksum = get_dir_checksum('.')
+			"""
+			for app in cfg['apps']:
+				if not app_config(app)['debug'] or debug:
+					reloader += app_reload(app)
+			reloader += """
+			server.reload("""
+			reloader += ",".join(dps)
+			reloader += """)
+	except Exception:
+		print('During handling request, an exception has occured:')
+		traceback.print_exc()
+"""
+
+			apps_info = []
+			for app in cfg['apps']:
+				if not app_config(app)['debug'] or debug:
+					apps_info.append(app)
+				else:
+					apps_info.append('['+app+']')
+			print(f'{GRAY}Apps: ' + ', '.join(apps_info))
+			print('Debug mode ' + 'enabled' if debug else 'disabled')
+			print('Smart navigation ' + ('enabled' if smart_navigation else 'disabled'))
+			print(RESET)
+
+			print('Starting server...')
+			start = ';'.join(load_imports(apps, debug))+reloader+f'server=Server({",".join(dps)}, smart_navigation={smart_navigation}, ssl_fullchain={ssl_fullchain}, ssl_key={ssl_key}, timeout={timeout}, max_bytes_per_recieve={max_bytes_per_recieve}, max_bytes={max_bytes}, _func=reloader);server.listen(Address({port}, "{host}"))'
+			exec(start)
+		elif sys.argv[1].lower() == 'create':
+			args = get_args(['name', 'host'], ' '.join(sys.argv[2:]))
+			if 'name' not in args.keys():
+				return print(f'{RED}The app`s name is not specified{RESET}')
+			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
+			if os.path.isdir(ensure_appname):
+				return print(f'{BLUE}The app named {args["name"]} exists{RESET}')
+			if 'host' not in args.keys():
+				print(f'{BLUE}Hosts were not specified')
+			os.mkdir(ensure_appname)
+			with open(f'{ensure_appname}/__init__.py', 'w') as f:
+				data = """import sys, importlib
+if '%appname%.app' not in sys.modules.keys():
+    from %appname%.app import dp
+else:
+    dp = importlib.reload(sys.modules['%appname%.app']).dp
+""".replace('%appname%', ensure_appname)
+				f.write(data)
+			with open(f'{ensure_appname}/app.py', 'w') as f:
+				data = """from slinn import Dispatcher, Filter, HttpResponse
+ 
+dp = Dispatcher(%hosts%)
+
+# Write your code down here                         
+""".replace('%appname%', ensure_appname).replace('%hosts%', '' if 'host' not in args.keys() else ', '.join(add_quotes_to_list(args['host'] if type(args['host']) == list else [args['host']])))
+				f.write(data)
+			with open(f'{ensure_appname}/config.json', 'w') as f:
+				data = """
+{
+	"debug": false
+}
+"""
+				f.write(data)
+			fr = open('project.json', 'r')
+			fj = json.loads(fr.read())
+			fr.close()
+			if 'apps' in fj.keys():
+				fj['apps'].insert(0, ensure_appname)
+			else:
+				fj['apps'] = []
+			fw = open('project.json', 'w')
+			fw.write(json.dumps(fj, indent=4))
+			fw.close()
+			update()
+			print(f'{GREEN}App successfully created{RESET}')
+		elif sys.argv[1].lower() == 'delete':
+			args = get_args(['name'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			if 'name' not in args.keys():
+				return print(f'{RED}The app`s name is not specified{RESET}')
+			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
+			if not os.path.isdir(ensure_appname):
+				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
+			if input(f'{RESET}Are you sure? (y/N) >>> ').lower() not in ['y', 'yes']:
+				return print(f'{RESET}Aborted')
+			shutil.rmtree(ensure_appname)
+			if os.path.isdir(f'{apppath}/templates_data/{ensure_appname}'):
+				shutil.rmtree(f'{apppath}/templates_data/{ensure_appname}')
+			if len(os.listdir(f'{apppath}/templates_data')) == 0:
+				shutil.rmtree(f'{apppath}/templates_data')
+			update()
+			return print(f'{GREEN}App successfully deleted{RESET}')
+		elif sys.argv[1].lower() == 'update':
+			return update()
+		elif sys.argv[1].lower() == 'help':
+			return print("""%BOLD%Slinn manager help page
+
+Commands%RESET%:
+	%cmd% run                                                              %GRAY%# Starts server%RESET%
+	%cmd% create {app`s name} host=(host1) host=(host2)...                 %GRAY%# Creates a new app
+		Example: %cmd% create localhost host=localhost host=127.0.0.1%RESET%
+	%cmd% delete {app`s name} (project`s path)                             %GRAY%# Deletes an app
+		Example: %cmd% delete localhost%RESET%
+	%cmd% template {template`s name} (projects`s path)                     %GRAY%# Installs a template
+		Example: %cmd% template firstrun%RESET%
+	%cmd% update                                                           %GRAY%# Updates project.py%RESET%
+	%cmd% migrate_app {app`s name}                                         %GRAY%# Migrates app(check slinn.guides.migration1xx2xx.migration1xx2xx)%RESET%
+	%cmd% help                                                             %GRAY%# Prints this help%RESET%
+	%cmd% version                                                          %GRAY%# Prints version of Slinn%RESET%
+""".replace('%cmd%', f'py {sys.argv[0]}').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
+		elif sys.argv[1].lower() == 'version':
+			return print(slinn_version)
+		elif sys.argv[1].lower() == 'template':
+			args = get_args(['name', 'path'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			if 'name' not in args.keys():
+				return print(f'{RED}Template name is not specified{RESET}')
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			fr = open('project.json', 'r')
+			fj = json.loads(fr.read())
+			fr.close()
+			if 'apps' in fj.keys():
+				fj['apps'].insert(0, args['name'])
+			else:
+				fj['apps'] = []
+			fw = open('project.json', 'w')
+			fw.write(json.dumps(fj, indent=4))
+			fw.close()
+			update()
+			try:
+				shutil.copytree(f'{modulepath}templates/{args["name"]}/', f'{apppath}/{args["name"]}')
+				try:
+					if not os.isdir(f'{apppath}/templates_data'):
+						os.mkdir(f'{apppath}/templates_data')
+					shutil.copytree(f'{modulepath}templates/{args["name"]}/data/', f'{apppath}/templates_data/{args["name"]}')
+				except  FileExistsError:
+					pass
+				except FileNotFoundError:
+					pass
+				return print(f'{GREEN}Template {args["name"]} successfully installed{RESET}') 
+			except FileExistsError:
+				return print(f'{BLUE}Template {args["name"]} has already installed{RESET}')
+			except FileNotFoundError:
+				return print(f'{BLUE}Template {args["name"]} not found{RESET}')
+		elif sys.argv[1].lower() == 'migrate_app':
+			args = get_args(['name'], ' '.join(sys.argv[2:]))
+			if 'name' not in args.keys():
+				return print(f'{RED}The app`s name is not specified{RESET}')
+			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
+			if not os.path.isdir(ensure_appname):
+				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
+			with open(f'{ensure_appname}/__init__.py', 'w') as f:
+				data = """import sys, importlib
+if '%appname%.app' not in sys.modules.keys():
+    from %appname%.app import dp
+else:
+    dp = importlib.reload(sys.modules['%appname%.app']).dp
+""".replace('%appname%', ensure_appname)
+				f.write(data)
+			with open(f'{ensure_appname}/config.json', 'w') as f:
+				data = """
+{
+	"debug": false
+}
+"""
+				f.write(data)
+			print(f'{GREEN}App successfully migrated{RESET}')
+		else:
+			return print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
+	else:
+		return print(f'{RED}Command was not specified{RESET}')
+
+			
+if __name__ == '__main__':
 	main()
```

### Comparing `slinn-2.2.7/slinn/guides/migration1xx2xx.py` & `slinn-2.2.8/slinn/guides/migration1xx2xx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0-2.2.7)
-
-Firstly, change all your @dp_xxx.route(...) to @dp_xxx(...)
-Then, you should change some filters from Filter to AnyFilter or LinkFilter where it is suit
-If you have troubles with Smart Navigation, then specify '{"smart_navigation": false}' in your project.json
-
-If you want support of autoreloading your app, follow these steps:
-- Change dp_xxx = Dispatcher(...) to dp = Dispatcher(...) and @dp_xxx.route(...) to @dp(...) OR dp = dp_xxx in the end of the file
-- Execute `py manage.py migrate_app {app`s name}`
+migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0-2.2.8)
+
+Firstly, change all your @dp_xxx.route(...) to @dp_xxx(...)
+Then, you should change some filters from Filter to AnyFilter or LinkFilter where it is suit
+If you have troubles with Smart Navigation, then specify '{"smart_navigation": false}' in your project.json
+
+If you want support of autoreloading your app, follow these steps:
+- Change dp_xxx = Dispatcher(...) to dp = Dispatcher(...) and @dp_xxx.route(...) to @dp(...) OR dp = dp_xxx in the end of the file
+- Execute `py manage.py migrate_app {app`s name}`
 """
```

### Comparing `slinn-2.2.7/slinn/http_api_response.py` & `slinn-2.2.8/slinn/http_api_response.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from slinn.http_response import HttpResponse
-
-
-class HttpAPIResponse(HttpResponse):
-	def __init__(self, payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
-		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
-		default_data = [('Server', 'Slinn'), ('Content-Type', content_type), ('Access-Control-Allow-Origin', '*')]
-		self.data = default_data + data if data is not None else default_data + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
-		self.status = status
+from slinn.http_response import HttpResponse
+
+
+class HttpAPIResponse(HttpResponse):
+	def __init__(self, payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
+		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
+		default_data = [('Server', 'Slinn'), ('Content-Type', content_type), ('Access-Control-Allow-Origin', '*')]
+		self.data = default_data + data if data is not None else default_data + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
+		self.status = status
```

### Comparing `slinn-2.2.7/slinn/http_response.py` & `slinn-2.2.8/slinn/http_response.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-class HttpResponse:
-	def __init__(self, payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
-		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
-		self.data = data if data is not None else [('Content-Type', content_type), ('Server', 'Slinn')] + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
-		self.status = status
-	
-	def set_cookie(self, key: str, value: any):
-		self.data.append(('Set-Cookie', f'{key}={value}'))
-	
-	def make(self, type: str='HTTP/2.0') -> str:
+class HttpResponse:
+	def __init__(self, payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
+		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
+		self.data = data if data is not None else [('Content-Type', content_type), ('Server', 'Slinn')] + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
+		self.status = status
+	
+	def set_cookie(self, key: str, value: any):
+		self.data.append(('Set-Cookie', f'{key}={value}'))
+	
+	def make(self, type: str='HTTP/2.0') -> str:
 		return (f'{type} {self.status}'+'\r\n'+"\r\n".join([str(dat[0])+": "+str(dat[1]) for dat in self.data])+'\r\n\r\n').encode()+self.payload
```

### Comparing `slinn-2.2.7/slinn/request.py` & `slinn-2.2.8/slinn/request.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import urllib.parse
-from slinn import File
-
-class Request:	
-	RESET = '\u001b[0m'
-	GRAY = '\u001b[38;2;127;127;127m'
-
-	@staticmethod
-	def parse_http_header(http_header: str):
-		result = {}
-		for line in http_header.split('\r\n'):
-			key, value = line.split(':')[0], ':'.join(line.split(':')[1:])
-			result[key.strip()] = value.strip()
-		return result
-	
-	@staticmethod
-	def parse_http_body(http_body: bytes):
-		files = [File()]
-		BGNs = [b'-----------------------------', b'------WebKitFormBoundary']
-		END = b'--'
-		binary = 0
-		for line in http_body.split(b'\r\n'):
-			if binary != 2:
-				if line == b'':
-					binary += 1
-				elif b':' in line:
-					key, value = line.split(b':')[0].decode(), b':'.join(line.split(b':')[1:])
-					files[-1].header[key.strip()] = value.strip()
-				elif files[-1].id is None:
-					if line.startswith(BGNs[0]):
-						files[-1].id = line[len(BGNs[0]):]
-					elif line.startswith(BGNs[1]):
-						files[-1].id = line[len(BGNs[1]):]
-				continue
-			if files[-1].id is not None:
-				if line.startswith(BGNs[0]) and line.endswith(END) and line[len(BGNs[0]):-len(END)] == files[-1].id \
-				   or line.startswith(BGNs[1]) and line.endswith(END) and line[len(BGNs[1]):-len(END)] == files[-1].id:
-					files[-1].data = bytes(files[-1].data[:-2])
-					files.append(File())
-					binary = 0
-					continue
-			files[-1].data += line + b'\r\n'
-		return files[:-1]
-
-	def __init__(self, header: str, body: bytes, client_address: tuple[str, int]):
-		def get_args(text):
-				return {} if text == '' else {pair.split('=')[0]: '='.join(pair.split('=')[1:]) for pair in text.split('&')}
-		
-		self.type = header.split('\r\n')[0].strip().split(' ')
-		self.header = {'method': self.type[0], 'link': ' '.join(self.type[1:-1]), 'ver': self.type[-1], 'data': {'user-agent': '', 'Accept': '', 'Accept-Encoding': '', 'Accept-Language': ''}}
-		header = self.parse_http_header(header)
-		self.files = self.parse_http_body(body)
-		self.header['data'].update(header)
-		self.ip, self.port = client_address[:2]
-		self.method = self.header['method']
-		self.version = self.header["ver"]
-		self.full_link = urllib.parse.unquote_plus(self.header["link"].replace('+', ' '))
-		self.host = self.header["data"]["Host"]
-		self.user_agent = self.header["data"]["User-Agent"] if 'User-Agent' in self.header['data'].keys() else self.header['data']['user-agent']
-		self.accept = self.header["data"]["Accept"].split(',')
-		self.encoding = self.header["data"]["Accept-Encoding"].split(',')
-		self.language = self.header["data"]["Accept-Language"].split(',')
-		self.link = self.full_link[:(self.full_link.index('?') if '?' in self.full_link else None)]
-		self.args = get_args(self.full_link[(self.full_link.index('?')+1 if '?' in self.full_link else len(self.full_link)):])
-		self.cookies = {c.split('=')[0]:c.split('=')[1] for c in self.header["data"]["Cookie"].split(';')} if 'Cookie' in self.header['data'] else []
-
-	def __str__(self):
-		return f'{self.GRAY}[{self.method}]{self.RESET} request {self.full_link} from {"" if "." in self.ip else "["}{self.ip}{"" if "." in self.ip else "]"}:{self.port} on {self.host}'
+import urllib.parse
+from slinn import File
+
+class Request:	
+	RESET = '\u001b[0m'
+	GRAY = '\u001b[38;2;127;127;127m'
+
+	@staticmethod
+	def parse_http_header(http_header: str):
+		result = {}
+		for line in http_header.split('\r\n'):
+			key, value = line.split(':')[0], ':'.join(line.split(':')[1:])
+			result[key.strip()] = value.strip()
+		return result
+	
+	@staticmethod
+	def parse_http_body(http_body: bytes):
+		files = [File()]
+		BGNs = [b'-----------------------------', b'------WebKitFormBoundary']
+		END = b'--'
+		binary = 0
+		for line in http_body.split(b'\r\n'):
+			if binary != 2:
+				if line == b'':
+					binary += 1
+				elif b':' in line:
+					key, value = line.split(b':')[0].decode(), b':'.join(line.split(b':')[1:])
+					files[-1].header[key.strip()] = value.strip()
+				elif files[-1].id is None:
+					if line.startswith(BGNs[0]):
+						files[-1].id = line[len(BGNs[0]):]
+					elif line.startswith(BGNs[1]):
+						files[-1].id = line[len(BGNs[1]):]
+				continue
+			if files[-1].id is not None:
+				if line.startswith(BGNs[0]) and line.endswith(END) and line[len(BGNs[0]):-len(END)] == files[-1].id \
+				   or line.startswith(BGNs[1]) and line.endswith(END) and line[len(BGNs[1]):-len(END)] == files[-1].id:
+					files[-1].data = bytes(files[-1].data[:-2])
+					files.append(File())
+					binary = 0
+					continue
+			files[-1].data += line + b'\r\n'
+		return files[:-1]
+
+	def __init__(self, header: str, body: bytes, client_address: tuple[str, int]):
+		def get_args(text):
+				return {} if text == '' else {pair.split('=')[0]: '='.join(pair.split('=')[1:]) for pair in text.split('&')}
+		
+		self.type = header.split('\r\n')[0].strip().split(' ')
+		self.header = {'method': self.type[0], 'link': ' '.join(self.type[1:-1]), 'ver': self.type[-1], 'data': {'user-agent': '', 'Accept': '', 'Accept-Encoding': '', 'Accept-Language': ''}}
+		header = self.parse_http_header(header)
+		self.files = self.parse_http_body(body)
+		self.header['data'].update(header)
+		self.ip, self.port = client_address[:2]
+		self.method = self.header['method']
+		self.version = self.header["ver"]
+		self.full_link = urllib.parse.unquote_plus(self.header["link"].replace('+', ' '))
+		self.host = self.header["data"]["Host"]
+		self.user_agent = self.header["data"]["User-Agent"] if 'User-Agent' in self.header['data'].keys() else self.header['data']['user-agent']
+		self.accept = self.header["data"]["Accept"].split(',')
+		self.encoding = self.header["data"]["Accept-Encoding"].split(',')
+		self.language = self.header["data"]["Accept-Language"].split(',')
+		self.link = self.full_link[:(self.full_link.index('?') if '?' in self.full_link else None)]
+		self.args = get_args(self.full_link[(self.full_link.index('?')+1 if '?' in self.full_link else len(self.full_link)):])
+		self.cookies = {c.split('=')[0]:c.split('=')[1] for c in self.header["data"]["Cookie"].split(';')} if 'Cookie' in self.header['data'] else []
+
+	def __str__(self):
+		return f'{self.GRAY}[{self.method}]{self.RESET} request {self.full_link} from {"" if "." in self.ip else "["}{self.ip}{"" if "." in self.ip else "]"}:{self.port} on {self.host}'
```

### Comparing `slinn-2.2.7/slinn/server.py` & `slinn-2.2.8/slinn/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from slinn import Request, Address, Filter, utils
-import socket, ssl, time, os, traceback
-
-
-RED = '\u001b[31m'
-RESET = '\u001b[0m'
-
-class Server:
-	class Handle:
-		def __init__(self, filter: Filter, function):
-			self.filter = filter
-			self.function = function
-	
-	def __init__(self, *dispatchers: tuple, smart_navigation: bool=True, ssl_fullchain: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296, _func=lambda server: None):
-		self.dispatchers = dispatchers
-		self.smart_navigation = smart_navigation
-		self.server_socket = None
-		self.ssl = ssl_fullchain is not None and ssl_key is not None
-		self.ssl_cert, self.ssl_key = ssl_fullchain, ssl_key
-		self.ssl_context = None
-		self.thread = None
-		self.timeout = timeout
-		self.max_bytes_per_recieve = max_bytes_per_recieve
-		self.max_bytes = max_bytes
-		self._func = _func
-
-	def reload(self, *dispatchers: tuple):
-		if self.thread is not None:
-			self.thread.stop()
-			try:
-				self.thread.join()
-			except RuntimeError:
-				pass
-		self.dispatchers = dispatchers
-			
-
-	def address(self, port: int, domain: str):
-		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"[" if ":" in domain else ""}{domain}{"]" if ":" in domain else ""}{(":"+str(port) if port != 443 else "") if self.ssl else (":"+str(port )if port != 80 else "")}/'
-		
-	def listen(self, address: Address):		
-		self.server_socket = None
-		if socket.has_dualstack_ipv6() and '.' not in address.host and ':' not in address.host:
-			self.server_socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM, dualstack_ipv6=True)
-		elif ':' in address.host:
-			self.server_socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
-		else:
-			self.server_socket = socket.socket(socket.AF_INET if '.' in address.host else socket.AF_INET6, socket.SOCK_STREAM)
-		self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-		try:
-			self.server_socket.bind((address.host, address.port))
-		except PermissionError:
-			print(f'{RED}Permission denied{RESET}')
-			exit(13)
-		if self.ssl:
-			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
-			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
-		self.server_socket.settimeout(self.timeout)
-		self.server_socket.listen()
-		print(self.address(address.port, address.domain))
-		try:
-			while True:
-				try:
-					utils.StoppableThread(target=self.handle_request, args=self.server_socket.accept()).start()
-				except socket.timeout:
-					pass
-		except KeyboardInterrupt:
-			print('Got KeyboardInterrupt, halting the application...')
-			if utils.check_socket(self.server_socket):
-				self.server_socket.close()
-			os._exit(0)
-						
-	def handle_request(self, client_socket, client_address):
-		try:
-			self._func(self)
-			if self.ssl:
-				client_socket = self.ssl_context.wrap_socket(client_socket, server_side=True)
-			try:
-				client_socket.settimeout(self.timeout)
-				data = bytearray()
-				while len(data) < self.max_bytes:
-					try:
-						b = client_socket.recv(self.max_bytes_per_recieve)
-						data += b
-					except TimeoutError:
-						break
-					
-				data = data.split(b'\r\n\r\n')
-				header = data[0].decode()
-				content = b'\r\n\r\n'.join(data[1:])
-				
-				if header == '':
-					return
-
-				request = Request(header, content, client_address)
-				print(request)
-			except KeyError:
-				return print('Got KeyError, probably invalid request. Ignore')
-			except UnicodeDecodeError:
-				return print('Got UnocodeDecodeError, probably invalid request. Ignore')
-			except ConnectionResetError:
-				return print('Connection reset by client')
-			except OSError:
-				return print('Connection closed')
-			for dispatcher in self.dispatchers:
-				if True in [utils.restartswith(request.host, host) for host in dispatcher.hosts]:
-					if self.smart_navigation:
-						sizes = [handle.filter.size(request.link, request.method) for handle in dispatcher.handles]
-						if sizes != []:
-							handle = dispatcher.handles[sizes.index(max(sizes))]
-							if handle.filter.check(request.link, request.method):
-								if utils.check_socket(client_socket):
-									client_socket.sendall(handle.function(request).make(request.version))
-									client_socket.close()
-								return
-					else:
-						for handle in dispatcher.handles:
-							if handle.filter.check(request.link, request.method):
-								if utils.check_socket(client_socket):
-									client_socket.sendall(handle.function(request).make(request.version))
-									client_socket.close()
-								return
-		except ssl.SSLError:
-			print('During handling request, an exception has occured:')
-			traceback.print_exc()
-			print('Got ssl.SSLError, reloading...')
-			self.reload(*self.dispatchers)
-		except Exception:
-			print('During handling request, an exception has occured:')
-			traceback.print_exc()
+from slinn import Request, Address, Filter, utils
+import socket, ssl, time, os, traceback
+
+
+RED = '\u001b[31m'
+RESET = '\u001b[0m'
+
+class Server:
+	class Handle:
+		def __init__(self, filter: Filter, function):
+			self.filter = filter
+			self.function = function
+	
+	def __init__(self, *dispatchers: tuple, smart_navigation: bool=True, ssl_fullchain: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296, _func=lambda server: None):
+		self.dispatchers = dispatchers
+		self.smart_navigation = smart_navigation
+		self.server_socket = None
+		self.ssl = ssl_fullchain is not None and ssl_key is not None
+		self.ssl_cert, self.ssl_key = ssl_fullchain, ssl_key
+		self.ssl_context = None
+		self.thread = None
+		self.timeout = timeout
+		self.max_bytes_per_recieve = max_bytes_per_recieve
+		self.max_bytes = max_bytes
+		self._func = _func
+
+	def reload(self, *dispatchers: tuple):
+		if self.thread is not None:
+			self.thread.stop()
+			try:
+				self.thread.join()
+			except RuntimeError:
+				pass
+		self.dispatchers = dispatchers
+			
+
+	def address(self, port: int, domain: str):
+		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"[" if ":" in domain else ""}{domain}{"]" if ":" in domain else ""}{(":"+str(port) if port != 443 else "") if self.ssl else (":"+str(port )if port != 80 else "")}/'
+		
+	def listen(self, address: Address):		
+		self.server_socket = None
+		if ':' in address.host:
+			self.server_socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
+			if socket.has_dualstack_ipv6():
+				self.server_socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
+		else:
+			self.server_socket = socket.socket(socket.AF_INET if '.' in address.host else socket.AF_INET6, socket.SOCK_STREAM)
+		self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+		try:
+			self.server_socket.bind((address.host, address.port))
+		except PermissionError:
+			print(f'{RED}Permission denied{RESET}')
+			exit(13)
+		if self.ssl:
+			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
+			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
+		self.server_socket.settimeout(self.timeout)
+		self.server_socket.listen()
+		print(self.address(address.port, address.domain))
+		try:
+			while True:
+				try:
+					utils.StoppableThread(target=self.handle_request, args=self.server_socket.accept()).start()
+				except socket.timeout:
+					pass
+		except KeyboardInterrupt:
+			print('Got KeyboardInterrupt, halting the application...')
+			if utils.check_socket(self.server_socket):
+				self.server_socket.close()
+			os._exit(0)
+						
+	def handle_request(self, client_socket, client_address):
+		try:
+			self._func(self)
+			if self.ssl:
+				client_socket = self.ssl_context.wrap_socket(client_socket, server_side=True)
+			try:
+				client_socket.settimeout(self.timeout)
+				data = bytearray()
+				while len(data) < self.max_bytes:
+					try:
+						b = client_socket.recv(self.max_bytes_per_recieve)
+						data += b
+					except TimeoutError:
+						break
+					
+				data = data.split(b'\r\n\r\n')
+				header = data[0].decode()
+				content = b'\r\n\r\n'.join(data[1:])
+				
+				if header == '':
+					return
+
+				request = Request(header, content, client_address)
+				print(request)
+			except KeyError:
+				return print('Got KeyError, probably invalid request. Ignore')
+			except UnicodeDecodeError:
+				return print('Got UnicodeDecodeError, probably invalid request. Ignore')
+			except ConnectionResetError:
+				return print('Connection reset by client')
+			except OSError:
+				return print('Connection closed')
+			for dispatcher in self.dispatchers:
+				if True in [utils.restartswith(request.host, host) for host in dispatcher.hosts]:
+					if self.smart_navigation:
+						sizes = [handle.filter.size(request.link, request.method) for handle in dispatcher.handles]
+						if sizes != []:
+							handle = dispatcher.handles[sizes.index(max(sizes))]
+							if handle.filter.check(request.link, request.method):
+								if utils.check_socket(client_socket):
+									client_socket.sendall(handle.function(request).make(request.version))
+									client_socket.close()
+								return
+					else:
+						for handle in dispatcher.handles:
+							if handle.filter.check(request.link, request.method):
+								if utils.check_socket(client_socket):
+									client_socket.sendall(handle.function(request).make(request.version))
+									client_socket.close()
+								return
+		except ssl.SSLError:
+			print('During handling request, an exception has occured:')
+			traceback.print_exc()
+			print('Got ssl.SSLError, reloading...')
+			self.reload(*self.dispatchers)
+		except Exception:
+			print('During handling request, an exception has occured:')
+			traceback.print_exc()
```

### Comparing `slinn-2.2.7/slinn/templates/firstrun/app.py` & `slinn-2.2.8/slinn/templates/firstrun/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from slinn import Dispatcher, Filter, HttpResponse
-import slinn
- 
-dp = Dispatcher()
-
-def read(filename):
-    file = open(filename, 'r', encoding='utf-8')
-    data = file.read()
-    file.close()
-    return data
-
-# Write your code down here  
-@dp(Filter('/styles.css'))
-def colorscss(request):
-    return HttpResponse(read('templates_data/firstrun/styles.css'))
-                       
-@dp(Filter('.*'))
-def index(request):
-    return HttpResponse(read('templates_data/firstrun/slinn.html').replace('{% version %}', slinn.version.split()[2]), content_type='text/html')
+from slinn import Dispatcher, LinkFilter, AnyFilter, HttpResponse
+import slinn
+
+def read(filename):
+    file = open(filename, 'r', encoding='utf-8')
+    data = file.read()
+    file.close()
+    return data
+ 
+dp = Dispatcher()
+
+@dp(LinkFilter('styles.css'))
+def styles(request):
+    return HttpResponse(read('templates_data/firstrun/styles.css'))
+                       
+@dp(AnyFilter)
+def index(request):
+    return HttpResponse(read('templates_data/firstrun/slinn.html').replace('{% version %}', slinn.version.split()[2]), content_type='text/html')
```

### Comparing `slinn-2.2.7/slinn/templates/firstrun/data/slinn.html` & `slinn-2.2.8/slinn/templates/firstrun/data/slinn.html`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-<html>
-<head>
-	<meta charset="utf-8" name="viewport" content="width=device-width, initial-scale=1">
-	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
-	<script src="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.js?content_type=text/javascript"></script>
-	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.css?content_type=text/css">
-	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/colors_min.css?content_type=text/css">
-	<link rel="stylesheet" href="styles.css">
-
-	<title>Slinn</title>
-
-</head>
-<body>
-	<script>
-		header = new UiHeaderContainer('header', document.querySelector('body'))
-		new UiLabel('slinn', header.elem, 'Slinn — Miot Project')
-		new UiHorizontalFlexSpacer('spacer1', header.elem)
-		new UiLinkLabel('pypi', header.elem, 'Slinn on PyPI', 'https://pypi.org/project/slinn/', 'violet')
-		new UiLinkLabel('homepage', header.elem, 'Slinn`s homepage', 'https://slinn.miotp.ru/', 'violet')
-		new UiLinkLabel('homepage', header.elem, 'Miot Project', 'https://miotp.ru/', 'violet')
-		body = new UiCenterContainer('body', document.querySelector('body'))
-		new UiLabel('title', body.elem, 'Your Slinn server started successfully!')
-		new UiLabel('subtitle', body.elem, 'Congratulations! 🎉')
-		text = new UiText('text', body.elem, '')
-		new UiText('text1', text.elem, 'You are seeing this page because')
-		new UiMonoText('debugtruechip', text.elem, '{"debug": true}', 'violet')
-		new UiText('text2', text.elem, 'is in your')
-		new UiMonoText('projectjson', text.elem, 'project.json', 'violet')
-		new UiText('text3', text.elem, 'file')
-		footer = new UiCenterContainer('footer', document.querySelector('body'))
-
-		new UiText('footertext1', footer.elem, 'Your version: {% version %}')
-		fetch('https://slinn.miotp.ru/check')
-			.then(response => response.text())
-			.then((result) => {
-				console.log(result)
-				latest = result.split('\n')[0].split(': ')[1]
-				nightly = result.split('\n')[1].split(': ')[1]
-				new UiText('footertext2', footer.elem, 'Latest stable version: '+latest+', latest nightly version: '+nightly)
-			})
-	</script>
-</body>
+<html>
+<head>
+	<meta charset="utf-8" name="viewport" content="width=device-width, initial-scale=1">
+	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
+	<script src="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.js?content_type=text/javascript"></script>
+	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.css?content_type=text/css">
+	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/colors_min.css?content_type=text/css">
+	<link rel="stylesheet" href="styles.css">
+
+	<title>Slinn</title>
+
+</head>
+<body>
+	<script>
+		header = new UiHeaderContainer('header', document.querySelector('body'))
+		new UiLabel('slinn', header.elem, 'Slinn — Miot Project')
+		new UiHorizontalFlexSpacer('spacer1', header.elem)
+		new UiLinkLabel('pypi', header.elem, 'Slinn on PyPI', 'https://pypi.org/project/slinn/', 'violet')
+		new UiLinkLabel('homepage', header.elem, 'Slinn`s homepage', 'https://slinn.miotp.ru/', 'violet')
+		new UiLinkLabel('homepage', header.elem, 'Miot Project', 'https://miotp.ru/', 'violet')
+		body = new UiCenterContainer('body', document.querySelector('body'))
+		new UiLabel('title', body.elem, 'Your Slinn server started successfully!')
+		new UiLabel('subtitle', body.elem, 'Congratulations! 🎉')
+		text = new UiText('text', body.elem, '')
+		new UiText('text1', text.elem, 'You are seeing this page because')
+		new UiMonoText('debugtruechip', text.elem, '{"debug": true}', 'violet')
+		new UiText('text2', text.elem, 'is in your')
+		new UiMonoText('projectjson', text.elem, 'project.json', 'violet')
+		new UiText('text3', text.elem, 'file')
+		footer = new UiCenterContainer('footer', document.querySelector('body'))
+
+		new UiText('footertext1', footer.elem, 'Your version: {% version %}')
+		fetch('https://slinn.miotp.ru/check')
+			.then(response => response.text())
+			.then((result) => {
+				console.log(result)
+				latest = result.split('\n')[0].split(': ')[1]
+				nightly = result.split('\n')[1].split(': ')[1]
+				new UiText('footertext2', footer.elem, 'Latest stable version: '+latest+', latest nightly version: '+nightly)
+			})
+	</script>
+</body>
 </html>
```

### Comparing `slinn-2.2.7/slinn/templates/firstrun/data/styles.css` & `slinn-2.2.8/slinn/templates/firstrun/data/styles.css`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-*[name='btngen']{
-	display: block;
-}
-
-@media screen and (max-width: 700px) {
-  *[name='slinn'], *[name='pypi'], *[name='miotproject'], *[name='homepage']{
-    min-width: 200px;
-    display: block;
-    text-align: center;
-  }
-
-  *[name='header']{
-    display: block;
-  }
-}
-
-@media screen and (min-width: 500px){
-  *[name='header']{
-    min-width: 450px;
-  }
-}
-
-@media screen and (max-width: 500px){
-  *[name='header']{
-    max-width: 450px;
-  }
-}
-
-*[name='body']{
-  max-width: 450px;
-  display: block;
-}
-
-*[name='footer'] *{
-  display: block;
+*[name='btngen']{
+	display: block;
+}
+
+@media screen and (max-width: 700px) {
+  *[name='slinn'], *[name='pypi'], *[name='miotproject'], *[name='homepage']{
+    min-width: 200px;
+    display: block;
+    text-align: center;
+  }
+
+  *[name='header']{
+    display: block;
+  }
+}
+
+@media screen and (min-width: 500px){
+  *[name='header']{
+    min-width: 450px;
+  }
+}
+
+@media screen and (max-width: 500px){
+  *[name='header']{
+    max-width: 450px;
+  }
+}
+
+*[name='body']{
+  max-width: 450px;
+  display: block;
+}
+
+*[name='footer'] *{
+  display: block;
 }
```

### Comparing `slinn-2.2.7/slinn.egg-info/PKG-INFO` & `slinn-2.2.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,241 +1,229 @@
-Metadata-Version: 2.1
-Name: slinn
-Version: 2.2.7
-Summary: A HTTPS and HTTP server framework
-Home-page: https://slinn.miotp.ru/
-Author: Mark Radin
-Author-email: mrybs2@gmail.com
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Slinn
-
----
-
-**Slinn is a HTTPS and HTTP server framework**
-
-![License](https://img.shields.io/github/license/mrybs/slinn)
-![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
-
-![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
-![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
-
-![GitHub Repo stars](https://img.shields.io/github/stars/mrybs/slinn)
-![GitHub watchers](https://img.shields.io/github/watchers/mrybs/slinn)
-![GitHub forks](https://img.shields.io/github/forks/mrybs/slinn)
-
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/mrybs/slinn)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mrybs/slinn)
-![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
-
-![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
-
-
-### Simple example
-```python
-from slinn import *
-
-
-dp = Dispatcher('localhost', '127.0.0.1')
-
-
-@dp(LinkFilter('api'))
-def api(request):
-    return HttpJSONAPIResponse(status='ok')
-
-@dp(LinkFilter(''))
-@dp(LinkFilter('index'))
-def index(request):
-    return HttpRedirect('/helloworld')
-
-
-@dp(AnyFilter)
-def helloworld(request):
-     return HttpResponse('Hello world!')
-
-```
-
-### Begin project
-#### Standart
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash
-python3 -m slinn create helloworld
-cd helloworld
-venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
-venv/bin/python manage.py run 
-```
-
-##### Windows:
-```batch
-py -m slinn create helloworld
-cd helloworld
-venv\Scripts\activate
-py manage.py create localhost host=localhost host=127.0.0.1
-py manage.py run 
-```
-
-Insert example into localhost/app.py file
-
-Excepted output
-```
-helloworld $ venv/bin/python manage.py run
-Loading config...
-Apps: firstrun
-Debug mode enabled
-Smart navigation enabled
-
-Starting server...
-HTTP server is available on http://localhost:8080/
-```
-
-To config project you should edit `./project.json`
-
-To config app you should edit `./%app%/config.json`
-
-#### Classic
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash 
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv/bin/activate
-```
-
-##### Windows:
-```batch
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv\Scripts\activate
-```
-
-Insert example into `example.py` and add following code:
-```
-Server(dp).listen(Address(8080))
-```
-then write `python example.py`
-
-Excepted output
-```
-helloworld $ venv/bin/python example.py
-HTTP server is available on http://localhost:8080/
-```
-
-### Functions:
-```python
-from slinn import Server
-
-server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
-server.address(port: int, domain: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
-server.reload(*dispatchers: tuple)  # Reloads server
-server.listen(address: Address)  # Start listening address
-
-Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
-```
-
-```python
-from slinn import Address
-
-address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
-
-Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
-
-# Attributes
-address.port  # port
-address.host  # ip
-address.domain  # non-converted host from constructor
-```
-
-```python
-from slinn import Dispatcher
-
-dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
-
-Dispatcher('localhost', '127.0.0.1', '::1')
-
-# To add handler into dispatcher
-@dispatcher(filter: Filter)
-def handler(request: Request):
-    ...
-
-# handler should return HttpResponse-based object
-```
-
-```python
-from slinn import Filter, LinkFilter, AnyFilter
-
-_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
-_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-
-Filter('/user/.+/profile.*')
-
-# LinkFilter inherits from Filter
-LinkFilter('user/.+/profile')
-
-# AnyFilter as same as Filter('.*')
-```
-
-```python
-from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
-
-http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value: any)  # Sets cookie
-http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
-
-HttpResponse('<h1>Hello world</h1>', content_type='text/html')
-
-# HttpAPIResponse inherits from HttpResponse
-# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
-
-HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
-
-# HttpRedirect inherits from HttpResponse
-HttpRedirect(location: str)
-
-HttpRedirect('slinn.miotp.ru')
-
-# HttpJSONResponse for responding JSON 
-HttpJSONResponse(**payload: dict)
-
-HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
-
-# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
-
-HttpJSONAPIResponse(code=43657, until=1719931149)
-```
-
-```python
-from slinn import Request
-
-request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
-request.parse_http_header(http_header: str)  # Parse HTTP request`s header
-request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
-str(request)  # Convert slinn.Request to info text
-
-# Attributes
-request.ip, request.port  # Client`s IP and port
-request.method  # HTTP method
-request.version  # HTTP version
-request.full_link  # Full link(path and params)
-request.host  # Requested host
-request.user_agent  # Client`s user agent
-request.accept  # maybe supported technologies
-request.encoding  # Supported encodings
-request.language  # Client`s language
-request.link  # Link(only path)
-request.args  # GET args
-request.cookies  # All saved cookies
-request.files # Uploaded files
-```
-
-```python
-from slinn import File
-
-file = File(id: str=None, data: bytes|bytearray=bytearray())
-
-# Attributes
-file.id  # File`s id 
-file.data  # Binary data
-file.headers  # Headers such as Content-Disposition
-```
+# Slinn
+
+---
+
+**Slinn is a HTTPS and HTTP server framework**
+
+![License](https://img.shields.io/github/license/mrybs/slinn)
+![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
+
+![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
+![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
+
+![GitHub Repo stars](https://img.shields.io/github/stars/mrybs/slinn)
+![GitHub watchers](https://img.shields.io/github/watchers/mrybs/slinn)
+![GitHub forks](https://img.shields.io/github/forks/mrybs/slinn)
+
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/mrybs/slinn)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mrybs/slinn)
+![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
+
+![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
+
+
+### Simple example
+```python
+from slinn import *
+
+
+dp = Dispatcher()
+
+@dp(LinkFilter('api'))
+def api(request):
+    return HttpJSONAPIResponse(status='ok')
+
+@dp(LinkFilter(''))
+@dp(LinkFilter('index'))
+def index(request):
+    return HttpRedirect('/helloworld')
+
+
+@dp(AnyFilter)
+def helloworld(request):
+     return HttpResponse('Hello world!')
+
+```
+
+### Begin project
+#### Standart
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash
+python3 -m slinn create helloworld
+cd helloworld
+venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
+venv/bin/python manage.py run 
+```
+
+##### Windows:
+```batch
+py -m slinn create helloworld
+cd helloworld
+venv\Scripts\activate
+py manage.py create localhost host=localhost host=127.0.0.1
+py manage.py run 
+```
+
+Insert example into localhost/app.py file
+
+Excepted output
+```
+helloworld $ venv/bin/python manage.py run
+Loading config...
+Apps: firstrun
+Debug mode enabled
+Smart navigation enabled
+
+Starting server...
+HTTP server is available on http://localhost:8080/
+```
+
+To config project you should edit `./project.json`
+
+To config app you should edit `./%app%/config.json`
+
+#### Classic
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash 
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv/bin/activate
+```
+
+##### Windows:
+```batch
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv\Scripts\activate
+```
+
+Insert example into `example.py` and add following code:
+```
+Server(dp).listen(Address(8080))
+```
+then write `python example.py`
+
+Excepted output
+```
+helloworld $ venv/bin/python example.py
+HTTP server is available on http://localhost:8080/
+```
+
+### Functions:
+```python
+from slinn import Server
+
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
+server.address(port: int, domain: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
+server.reload(*dispatchers: tuple)  # Reloads server
+server.listen(address: Address)  # Start listening address
+
+Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
+```
+
+```python
+from slinn import Address
+
+address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
+
+Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
+
+# Attributes
+address.port  # port
+address.host  # ip
+address.domain  # non-converted host from constructor
+```
+
+```python
+from slinn import Dispatcher
+
+dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
+
+Dispatcher('localhost', '127.0.0.1', '::1', '::')
+
+# To add handler into dispatcher
+@dispatcher(filter: Filter)
+def handler(request: Request):
+    ...
+
+# handler should return HttpResponse-based object
+```
+
+```python
+from slinn import Filter, LinkFilter, AnyFilter
+
+_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
+_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
+
+Filter('/user/.+/profile.*')
+
+# LinkFilter inherits from Filter
+LinkFilter('user/.+/profile')
+
+# AnyFilter as same as Filter('.*')
+```
+
+```python
+from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
+
+http_response = HttpResponse(payload: any, data: list[tuple[str, any]]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
+http_response.set_cookie(key: str, value: any)  # Sets cookie
+http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
+
+HttpResponse('<h1>Hello world</h1>', content_type='text/html')
+
+# HttpAPIResponse inherits from HttpResponse
+# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
+
+HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
+
+# HttpRedirect inherits from HttpResponse
+HttpRedirect(location: str)
+
+HttpRedirect('slinn.miotp.ru')
+
+# HttpJSONResponse for responding JSON 
+HttpJSONResponse(**payload: dict)
+
+HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
+
+# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
+
+HttpJSONAPIResponse(code=43657, until=1719931149)
+```
+
+```python
+from slinn import Request
+
+request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
+request.parse_http_header(http_header: str)  # Parse HTTP request`s header
+request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
+str(request)  # Convert slinn.Request to info text
+
+# Attributes
+request.ip, request.port  # Client`s IP and port
+request.method  # HTTP method
+request.version  # HTTP version
+request.full_link  # Full link(path and params)
+request.host  # Requested host
+request.user_agent  # Client`s user agent
+request.accept  # maybe supported technologies
+request.encoding  # Supported encodings
+request.language  # Client`s language
+request.link  # Link(only path)
+request.args  # GET args
+request.cookies  # All saved cookies
+request.files # Uploaded files
+```
+
+```python
+from slinn import File
+
+file = File(id: str=None, data: bytes|bytearray=bytearray())
+
+# Attributes
+file.id  # File`s id 
+file.data  # Binary data
+file.headers  # Headers such as Content-Disposition
+```
```

### Comparing `slinn-2.2.7/slinn.egg-info/SOURCES.txt` & `slinn-2.2.8/slinn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

