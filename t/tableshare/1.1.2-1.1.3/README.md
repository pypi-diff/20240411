# Comparing `tmp/tableshare-1.1.2.tar.gz` & `tmp/tableshare-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableshare-1.1.2.tar", last modified: Sun Apr  7 14:09:26 2024, max compression
+gzip compressed data, was "tableshare-1.1.3.tar", last modified: Thu Apr 11 13:22:50 2024, max compression
```

## Comparing `tableshare-1.1.2.tar` & `tableshare-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 14:09:26.950556 tableshare-1.1.2/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:58:56.000000 tableshare-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      931 2024-04-07 14:09:26.949559 tableshare-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2305 2024-02-28 05:51:28.000000 tableshare-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 14:09:26.950556 tableshare-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1661 2024-04-07 14:09:12.000000 tableshare-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:09:26.948562 tableshare-1.1.2/tableshare.egg-info/
--rw-rw-rw-   0        0        0      931 2024-04-07 14:09:26.000000 tableshare-1.1.2/tableshare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-04-07 14:09:26.000000 tableshare-1.1.2/tableshare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 14:09:26.000000 tableshare-1.1.2/tableshare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-07 14:09:26.000000 tableshare-1.1.2/tableshare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 14:09:26.000000 tableshare-1.1.2/tableshare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 13:22:50.081608 tableshare-1.1.3/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:58:56.000000 tableshare-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      931 2024-04-11 13:22:50.081608 tableshare-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2305 2024-02-28 05:51:28.000000 tableshare-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:22:50.081608 tableshare-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1779 2024-04-11 13:22:30.000000 tableshare-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:22:50.081608 tableshare-1.1.3/tableshare.egg-info/
+-rw-rw-rw-   0        0        0      931 2024-04-11 13:22:49.000000 tableshare-1.1.3/tableshare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-11 13:22:49.000000 tableshare-1.1.3/tableshare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:22:49.000000 tableshare-1.1.3/tableshare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-11 13:22:49.000000 tableshare-1.1.3/tableshare.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-04-11 13:22:49.000000 tableshare-1.1.3/tableshare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:22:49.000000 tableshare-1.1.3/tableshare.egg-info/top_level.txt
```

### Comparing `tableshare-1.1.2/LICENSE` & `tableshare-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tableshare-1.1.2/PKG-INFO` & `tableshare-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableshare
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for scraping and sharing table data from web pages.
 Home-page: https://github.com/baiguanba/tableshare
 Author: Guanba
 Author-email: baiguanba@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baiguanba/tableshare/issues
 Keywords: python,table,webtable,scrawler
```

### Comparing `tableshare-1.1.2/README.md` & `tableshare-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tableshare-1.1.2/setup.py` & `tableshare-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
 00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a56  find_packages..V
-00000030: 4552 5349 4f4e 203d 2027 312e 312e 3227  ERSION = '1.1.2'
+00000030: 4552 5349 4f4e 203d 2027 312e 312e 3327  ERSION = '1.1.3'
 00000040: 0d0a 4445 5343 5249 5054 494f 4e20 3d20  ..DESCRIPTION = 
 00000050: 2741 2050 7974 686f 6e20 6c69 6272 6172  'A Python librar
 00000060: 7920 666f 7220 7363 7261 7069 6e67 2061  y for scraping a
 00000070: 6e64 2073 6861 7269 6e67 2074 6162 6c65  nd sharing table
 00000080: 2064 6174 6120 6672 6f6d 2077 6562 2070   data from web p
 00000090: 6167 6573 2e27 0d0a 0d0a 7365 7475 7028  ages.'....setup(
 000000a0: 0d0a 2020 2020 6e61 6d65 3d27 7461 626c  ..    name='tabl
@@ -20,85 +20,93 @@
 00000130: 80e6 9c89 e58c 850d 0a20 2020 2069 6e73  .........    ins
 00000140: 7461 6c6c 5f72 6571 7569 7265 733d 5b27  tall_requires=['
 00000150: 7265 7175 6573 7473 272c 2027 7061 6e64  requests', 'pand
 00000160: 6173 272c 2027 6273 3427 2c20 2744 7269  as', 'bs4', 'Dri
 00000170: 7373 696f 6e50 6167 6527 5d2c 2320 e5a6  ssionPage'],# ..
 00000180: 82e6 9e9c e69c 89e5 85b6 e4bb 96e4 be9d  ................
 00000190: e8b5 96ef bc8c e8af b7e5 9ca8 e8bf 99e9  ................
-000001a0: 878c e6b7 bbe5 8aa0 0d0a 2020 2020 6b65  ..........    ke
-000001b0: 7977 6f72 6473 3d5b 2770 7974 686f 6e27  ywords=['python'
-000001c0: 2c27 7461 626c 6527 2c27 7765 6274 6162  ,'table','webtab
-000001d0: 6c65 272c 2773 6372 6177 6c65 7227 5d2c  le','scrawler'],
-000001e0: 0d0a 2020 2020 7079 7468 6f6e 5f72 6571  ..    python_req
-000001f0: 7569 7265 733d 273e 3d33 2e36 272c 2020  uires='>=3.6',  
-00000200: 2320 e68c 87e5 ae9a e694 afe6 8c81 e79a  # ..............
-00000210: 8450 7974 686f 6ee7 8988 e69c ac0d 0a20  .Python........ 
-00000220: 2020 2061 7574 686f 723d 2747 7561 6e62     author='Guanb
-00000230: 6127 2c20 2023 20e6 9bbf e68d a2e4 b8ba  a',  # .........
-00000240: e4bd a0e7 9a84 e590 8de5 ad97 0d0a 2020  ..............  
-00000250: 2020 6175 7468 6f72 5f65 6d61 696c 3d27    author_email='
-00000260: 6261 6967 7561 6e62 6140 6f75 746c 6f6f  baiguanba@outloo
-00000270: 6b2e 636f 6d27 2c20 2023 20e6 9bbf e68d  k.com',  # .....
-00000280: a2e4 b8ba e4bd a0e7 9a84 e794 b5e5 ad90  ................
-00000290: e982 aee4 bbb6 e59c b0e5 9d80 0d0a 2020  ..............  
-000002a0: 2020 6465 7363 7269 7074 696f 6e3d 4445    description=DE
-000002b0: 5343 5249 5054 494f 4e2c 2020 2320 e5ba  SCRIPTION,  # ..
-000002c0: 93e7 9a84 e7ae 80e7 9fad e68f 8fe8 bfb0  ................
-000002d0: 0d0a 2020 2020 6c6f 6e67 5f64 6573 6372  ..    long_descr
-000002e0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-000002f0: 7970 653d 2774 6578 742f 6d61 726b 646f  ype='text/markdo
-00000300: 776e 272c 2020 2320 e68c 87e5 ae9a e995  wn',  # ........
-00000310: bfe6 8f8f e8bf b0e7 9a84 e6a0 bce5 bc8f  ................
-00000320: 0d0a 2020 2020 7572 6c3d 2768 7474 7073  ..    url='https
-00000330: 3a2f 2f67 6974 6875 622e 636f 6d2f 6261  ://github.com/ba
-00000340: 6967 7561 6e62 612f 7461 626c 6573 6861  iguanba/tablesha
-00000350: 7265 272c 2020 2320 e5ba 93e7 9a84 e4b8  re',  # ........
-00000360: bbe9 a1b5 e688 96e6 ba90 e4bb a3e7 a081  ................
-00000370: e4bb 93e5 ba93 e993 bee6 8ea5 0d0a 2020  ..............  
-00000380: 2020 636c 6173 7369 6669 6572 733d 5b20    classifiers=[ 
-00000390: 2023 20e9 8089 e68b a9e9 8082 e5bd 93e7   # .............
-000003a0: 9a84 e588 86e7 b1bb e599 a80d 0a20 2020  .............   
-000003b0: 2020 2020 2027 4465 7665 6c6f 706d 656e       'Developmen
-000003c0: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
-000003d0: 416c 7068 6127 2c0d 0a20 2020 2020 2020  Alpha',..       
-000003e0: 2027 496e 7465 6e64 6564 2041 7564 6965   'Intended Audie
-000003f0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-00000400: 7327 2c0d 0a20 2020 2020 2020 2027 546f  s',..        'To
-00000410: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000420: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000430: 6962 7261 7269 6573 203a 3a20 5079 7468  ibraries :: Pyth
-00000440: 6f6e 204d 6f64 756c 6573 272c 0d0a 2020  on Modules',..  
-00000450: 2020 2020 2020 274c 6963 656e 7365 203a        'License :
-00000460: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000470: 3a20 4d49 5420 4c69 6365 6e73 6527 2c0d  : MIT License',.
-00000480: 0a20 2020 2020 2020 2027 5072 6f67 7261  .        'Progra
-00000490: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000004a0: 3a20 5079 7468 6f6e 203a 3a20 332e 3627  : Python :: 3.6'
-000004b0: 2c0d 0a20 2020 2020 2020 2027 5072 6f67  ,..        'Prog
-000004c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000004d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000004e0: 3727 2c0d 0a20 2020 2020 2020 2027 5072  7',..        'Pr
-000004f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000500: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000510: 332e 3827 2c0d 0a20 2020 2020 2020 2027  3.8',..        '
-00000520: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000530: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000540: 3a20 332e 3927 2c0d 0a20 2020 2020 2020  : 3.9',..       
-00000550: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
-00000560: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000570: 203a 3a20 332e 3130 272c 0d0a 2020 2020   :: 3.10',..    
-00000580: 5d2c 0d0a 2020 2020 6c69 6365 6e73 653d  ],..    license=
-00000590: 274d 4954 272c 2020 2320 e4bd a0e7 9a84  'MIT',  # ......
-000005a0: e5ba 93e4 bdbf e794 a8e7 9a84 e8ae b8e5  ................
-000005b0: 8faf e8af 810d 0a20 2020 2070 726f 6a65  .......    proje
-000005c0: 6374 5f75 726c 733d 7b20 2023 20e9 a1b9  ct_urls={  # ...
-000005d0: e79b aee9 93be e68e a50d 0a20 2020 2020  ...........     
-000005e0: 2020 2022 4275 6720 5472 6163 6b65 7222     "Bug Tracker"
-000005f0: 3a20 2268 7474 7073 3a2f 2f67 6974 6875  : "https://githu
-00000600: 622e 636f 6d2f 6261 6967 7561 6e62 612f  b.com/baiguanba/
-00000610: 7461 626c 6573 6861 7265 2f69 7373 7565  tableshare/issue
-00000620: 7322 0d0a 2020 2020 7d2c 0d0a 2020 2020  s"..    },..    
-00000630: 7363 7269 7074 733d 5b5d 2c20 2023 20e5  scripts=[],  # .
-00000640: a682 e69e 9ce4 bda0 e79a 84e5 ba93 e58c  ................
-00000650: 85e5 90ab e58f afe6 89a7 e8a1 8ce6 9687  ................
-00000660: e4bb b6ef bc8c e8af b7e5 9ca8 e8bf 99e9  ................
-00000670: 878c e588 97e5 87ba 0d0a 290d 0a         ..........)..
+000001a0: 878c e6b7 bbe5 8aa0 0d0a 2020 2020 656e  ..........    en
+000001b0: 7472 795f 706f 696e 7473 3d7b 0d0a 2020  try_points={..  
+000001c0: 2020 2020 2020 2263 6f6e 736f 6c65 5f73        "console_s
+000001d0: 6372 6970 7473 223a 205b 0d0a 2020 2020  cripts": [..    
+000001e0: 2020 2020 2020 2020 226d 795f 7363 7269          "my_scri
+000001f0: 7074 203d 206d 7970 6163 6b61 6765 2e73  pt = mypackage.s
+00000200: 6372 6970 743a 6d61 696e 220d 0a20 2020  cript:main"..   
+00000210: 2020 2020 205d 0d0a 2020 2020 7d2c 0d0a       ]..    },..
+00000220: 2020 2020 6b65 7977 6f72 6473 3d5b 2770      keywords=['p
+00000230: 7974 686f 6e27 2c27 7461 626c 6527 2c27  ython','table','
+00000240: 7765 6274 6162 6c65 272c 2773 6372 6177  webtable','scraw
+00000250: 6c65 7227 5d2c 0d0a 2020 2020 7079 7468  ler'],..    pyth
+00000260: 6f6e 5f72 6571 7569 7265 733d 273e 3d33  on_requires='>=3
+00000270: 2e36 272c 2020 2320 e68c 87e5 ae9a e694  .6',  # ........
+00000280: afe6 8c81 e79a 8450 7974 686f 6ee7 8988  .......Python...
+00000290: e69c ac0d 0a20 2020 2061 7574 686f 723d  .....    author=
+000002a0: 2747 7561 6e62 6127 2c20 2023 20e6 9bbf  'Guanba',  # ...
+000002b0: e68d a2e4 b8ba e4bd a0e7 9a84 e590 8de5  ................
+000002c0: ad97 0d0a 2020 2020 6175 7468 6f72 5f65  ....    author_e
+000002d0: 6d61 696c 3d27 6261 6967 7561 6e62 6140  mail='baiguanba@
+000002e0: 6f75 746c 6f6f 6b2e 636f 6d27 2c20 2023  outlook.com',  #
+000002f0: 20e6 9bbf e68d a2e4 b8ba e4bd a0e7 9a84   ...............
+00000300: e794 b5e5 ad90 e982 aee4 bbb6 e59c b0e5  ................
+00000310: 9d80 0d0a 2020 2020 6465 7363 7269 7074  ....    descript
+00000320: 696f 6e3d 4445 5343 5249 5054 494f 4e2c  ion=DESCRIPTION,
+00000330: 2020 2320 e5ba 93e7 9a84 e7ae 80e7 9fad    # ............
+00000340: e68f 8fe8 bfb0 0d0a 2020 2020 6c6f 6e67  ........    long
+00000350: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+00000360: 7465 6e74 5f74 7970 653d 2774 6578 742f  tent_type='text/
+00000370: 6d61 726b 646f 776e 272c 2020 2320 e68c  markdown',  # ..
+00000380: 87e5 ae9a e995 bfe6 8f8f e8bf b0e7 9a84  ................
+00000390: e6a0 bce5 bc8f 0d0a 2020 2020 7572 6c3d  ........    url=
+000003a0: 2768 7474 7073 3a2f 2f67 6974 6875 622e  'https://github.
+000003b0: 636f 6d2f 6261 6967 7561 6e62 612f 7461  com/baiguanba/ta
+000003c0: 626c 6573 6861 7265 272c 2020 2320 e5ba  bleshare',  # ..
+000003d0: 93e7 9a84 e4b8 bbe9 a1b5 e688 96e6 ba90  ................
+000003e0: e4bb a3e7 a081 e4bb 93e5 ba93 e993 bee6  ................
+000003f0: 8ea5 0d0a 2020 2020 636c 6173 7369 6669  ....    classifi
+00000400: 6572 733d 5b20 2023 20e9 8089 e68b a9e9  ers=[  # .......
+00000410: 8082 e5bd 93e7 9a84 e588 86e7 b1bb e599  ................
+00000420: a80d 0a20 2020 2020 2020 2027 4465 7665  ...        'Deve
+00000430: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+00000440: 3a20 3320 2d20 416c 7068 6127 2c0d 0a20  : 3 - Alpha',.. 
+00000450: 2020 2020 2020 2027 496e 7465 6e64 6564         'Intended
+00000460: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000470: 656c 6f70 6572 7327 2c0d 0a20 2020 2020  elopers',..     
+00000480: 2020 2027 546f 7069 6320 3a3a 2053 6f66     'Topic :: Sof
+00000490: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+000004a0: 7420 3a3a 204c 6962 7261 7269 6573 203a  t :: Libraries :
+000004b0: 3a20 5079 7468 6f6e 204d 6f64 756c 6573  : Python Modules
+000004c0: 272c 0d0a 2020 2020 2020 2020 274c 6963  ',..        'Lic
+000004d0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000004e0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000004f0: 6e73 6527 2c0d 0a20 2020 2020 2020 2027  nse',..        '
+00000500: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000510: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000520: 3a20 332e 3627 2c0d 0a20 2020 2020 2020  : 3.6',..       
+00000530: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
+00000540: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000550: 203a 3a20 332e 3727 2c0d 0a20 2020 2020   :: 3.7',..     
+00000560: 2020 2027 5072 6f67 7261 6d6d 696e 6720     'Programming 
+00000570: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000580: 6f6e 203a 3a20 332e 3827 2c0d 0a20 2020  on :: 3.8',..   
+00000590: 2020 2020 2027 5072 6f67 7261 6d6d 696e       'Programmin
+000005a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000005b0: 7468 6f6e 203a 3a20 332e 3927 2c0d 0a20  thon :: 3.9',.. 
+000005c0: 2020 2020 2020 2027 5072 6f67 7261 6d6d         'Programm
+000005d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000005e0: 5079 7468 6f6e 203a 3a20 332e 3130 272c  Python :: 3.10',
+000005f0: 0d0a 2020 2020 5d2c 0d0a 2020 2020 6c69  ..    ],..    li
+00000600: 6365 6e73 653d 274d 4954 272c 2020 2320  cense='MIT',  # 
+00000610: e4bd a0e7 9a84 e5ba 93e4 bdbf e794 a8e7  ................
+00000620: 9a84 e8ae b8e5 8faf e8af 810d 0a20 2020  .............   
+00000630: 2070 726f 6a65 6374 5f75 726c 733d 7b20   project_urls={ 
+00000640: 2023 20e9 a1b9 e79b aee9 93be e68e a50d   # .............
+00000650: 0a20 2020 2020 2020 2022 4275 6720 5472  .        "Bug Tr
+00000660: 6163 6b65 7222 3a20 2268 7474 7073 3a2f  acker": "https:/
+00000670: 2f67 6974 6875 622e 636f 6d2f 6261 6967  /github.com/baig
+00000680: 7561 6e62 612f 7461 626c 6573 6861 7265  uanba/tableshare
+00000690: 2f69 7373 7565 7322 0d0a 2020 2020 7d2c  /issues"..    },
+000006a0: 0d0a 2020 2020 7363 7269 7074 733d 5b5d  ..    scripts=[]
+000006b0: 2c20 2023 20e5 a682 e69e 9ce4 bda0 e79a  ,  # ...........
+000006c0: 84e5 ba93 e58c 85e5 90ab e58f afe6 89a7  ................
+000006d0: e8a1 8ce6 9687 e4bb b6ef bc8c e8af b7e5  ................
+000006e0: 9ca8 e8bf 99e9 878c e588 97e5 87ba 0d0a  ................
+000006f0: 290d 0a                                  )..
```

### Comparing `tableshare-1.1.2/tableshare.egg-info/PKG-INFO` & `tableshare-1.1.3/tableshare.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableshare
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for scraping and sharing table data from web pages.
 Home-page: https://github.com/baiguanba/tableshare
 Author: Guanba
 Author-email: baiguanba@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baiguanba/tableshare/issues
 Keywords: python,table,webtable,scrawler
```

