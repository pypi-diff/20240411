# Comparing `tmp/s3torchconnector-1.2.2.tar.gz` & `tmp/s3torchconnector-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3torchconnector-1.2.2.tar", last modified: Fri Mar 22 12:12:19 2024, max compression
+gzip compressed data, was "s3torchconnector-1.2.3.tar", last modified: Thu Apr 11 11:04:55 2024, max compression
```

## Comparing `s3torchconnector-1.2.2.tar` & `s3torchconnector-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:19.815008 s3torchconnector-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-22 12:12:13.000000 s3torchconnector-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-22 12:12:13.000000 s3torchconnector-1.2.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-22 12:12:19.815008 s3torchconnector-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-03-22 12:12:13.000000 s3torchconnector-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  1875635 2024-03-22 12:12:13.000000 s3torchconnector-1.2.2/THIRD-PARTY-LICENSES
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 12:12:19.815008 s3torchconnector-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:19.807008 s3torchconnector-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:19.811008 s3torchconnector-1.2.2/src/s3torchconnector/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3_bucket_iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3bucket_key_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:19.811008 s3torchconnector-1.2.2/src/s3torchconnector/_s3client/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3client/_mock_s3client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3client/_s3client.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3client/s3client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_s3dataset_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:19.811008 s3torchconnector-1.2.2/src/s3torchconnector/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/lightning/s3_lightning_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/s3checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/s3iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/s3map_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/s3reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-22 12:12:12.000000 s3torchconnector-1.2.2/src/s3torchconnector/s3writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:12:19.811008 s3torchconnector-1.2.2/src/s3torchconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-22 12:12:19.000000 s3torchconnector-1.2.2/src/s3torchconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-22 12:12:19.000000 s3torchconnector-1.2.2/src/s3torchconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 12:12:19.000000 s3torchconnector-1.2.2/src/s3torchconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-22 12:12:19.000000 s3torchconnector-1.2.2/src/s3torchconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-22 12:12:19.000000 s3torchconnector-1.2.2/src/s3torchconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:55.231995 s3torchconnector-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-11 11:04:48.000000 s3torchconnector-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-11 11:04:48.000000 s3torchconnector-1.2.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-11 11:04:55.231995 s3torchconnector-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-04-11 11:04:48.000000 s3torchconnector-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1875635 2024-04-11 11:04:48.000000 s3torchconnector-1.2.3/THIRD-PARTY-LICENSES
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:04:55.235995 s3torchconnector-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:55.227995 s3torchconnector-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:55.231995 s3torchconnector-1.2.3/src/s3torchconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3_bucket_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3bucket_key_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:55.231995 s3torchconnector-1.2.3/src/s3torchconnector/_s3client/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3client/_mock_s3client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3client/_s3client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3client/s3client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_s3dataset_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:55.231995 s3torchconnector-1.2.3/src/s3torchconnector/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/lightning/s3_lightning_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/s3checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/s3iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/s3map_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/s3reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-11 11:04:47.000000 s3torchconnector-1.2.3/src/s3torchconnector/s3writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:04:55.231995 s3torchconnector-1.2.3/src/s3torchconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-11 11:04:55.000000 s3torchconnector-1.2.3/src/s3torchconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-11 11:04:55.000000 s3torchconnector-1.2.3/src/s3torchconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:04:55.000000 s3torchconnector-1.2.3/src/s3torchconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-11 11:04:55.000000 s3torchconnector-1.2.3/src/s3torchconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 11:04:55.000000 s3torchconnector-1.2.3/src/s3torchconnector.egg-info/top_level.txt
```

### Comparing `s3torchconnector-1.2.2/LICENSE` & `s3torchconnector-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/PKG-INFO` & `s3torchconnector-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3torchconnector
-Version: 1.2.2
+Version: 1.2.3
 Summary: S3 connector integration for PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: THIRD-PARTY-LICENSES
 License-File: NOTICE
 Requires-Dist: torch>=2.0.1
-Requires-Dist: s3torchconnectorclient>=1.2.2
+Requires-Dist: s3torchconnectorclient>=1.2.3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: mypy; extra == "test"
```

### Comparing `s3torchconnector-1.2.2/README.md` & `s3torchconnector-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/THIRD-PARTY-LICENSES` & `s3torchconnector-1.2.3/THIRD-PARTY-LICENSES`

 * *Files 0% similar despite different names*

```diff
@@ -39940,15 +39940,15 @@
 0009c030: 4f52 2049 4e20 434f 4e4e 4543 5449 4f4e  OR IN CONNECTION
 0009c040: 2057 4954 4820 5448 450a 534f 4654 5741   WITH THE.SOFTWA
 0009c050: 5245 204f 5220 5448 4520 5553 4520 4f52  RE OR THE USE OR
 0009c060: 204f 5448 4552 2044 4541 4c49 4e47 5320   OTHER DEALINGS 
 0009c070: 494e 2054 4845 2053 4f46 5457 4152 452e  IN THE SOFTWARE.
 0009c080: 0a0a 2d2d 2d2d 0a0a 5061 636b 6167 653a  ..----..Package:
 0009c090: 206d 6f75 6e74 706f 696e 742d 7333 2d63   mountpoint-s3-c
-0009c0a0: 6c69 656e 743a 302e 382e 300a 0a54 6865  lient:0.8.0..The
+0009c0a0: 6c69 656e 743a 302e 382e 310a 0a54 6865  lient:0.8.1..The
 0009c0b0: 2066 6f6c 6c6f 7769 6e67 2063 6f70 7972   following copyr
 0009c0c0: 6967 6874 7320 616e 6420 6c69 6365 6e73  ights and licens
 0009c0d0: 6573 2077 6572 6520 666f 756e 6420 696e  es were found in
 0009c0e0: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
 0009c0f0: 206f 6620 7468 6973 2070 6163 6b61 6765   of this package
 0009c100: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
 0009c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -40658,15 +40658,15 @@
 0009ed10: 6520 7370 6563 6966 6963 206c 616e 6775  e specific langu
 0009ed20: 6167 6520 676f 7665 726e 696e 6720 7065  age governing pe
 0009ed30: 726d 6973 7369 6f6e 7320 616e 640a 2020  rmissions and.  
 0009ed40: 206c 696d 6974 6174 696f 6e73 2075 6e64   limitations und
 0009ed50: 6572 2074 6865 204c 6963 656e 7365 2e0a  er the License..
 0009ed60: 0a2d 2d2d 2d0a 0a50 6163 6b61 6765 3a20  .----..Package: 
 0009ed70: 6d6f 756e 7470 6f69 6e74 2d73 332d 6372  mountpoint-s3-cr
-0009ed80: 743a 302e 362e 320a 0a54 6865 2066 6f6c  t:0.6.2..The fol
+0009ed80: 743a 302e 372e 300a 0a54 6865 2066 6f6c  t:0.7.0..The fol
 0009ed90: 6c6f 7769 6e67 2063 6f70 7972 6967 6874  lowing copyright
 0009eda0: 7320 616e 6420 6c69 6365 6e73 6573 2077  s and licenses w
 0009edb0: 6572 6520 666f 756e 6420 696e 2074 6865  ere found in the
 0009edc0: 2073 6f75 7263 6520 636f 6465 206f 6620   source code of 
 0009edd0: 7468 6973 2070 6163 6b61 6765 3a0a 0a20  this package:.. 
 0009ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0009edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -41376,15 +41376,15 @@
 000a19f0: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
 000a1a00: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
 000a1a10: 7369 6f6e 7320 616e 640a 2020 206c 696d  sions and.   lim
 000a1a20: 6974 6174 696f 6e73 2075 6e64 6572 2074  itations under t
 000a1a30: 6865 204c 6963 656e 7365 2e0a 0a2d 2d2d  he License...---
 000a1a40: 2d0a 0a50 6163 6b61 6765 3a20 6d6f 756e  -..Package: moun
 000a1a50: 7470 6f69 6e74 2d73 332d 6372 742d 7379  tpoint-s3-crt-sy
-000a1a60: 733a 302e 362e 320a 0a54 6865 2066 6f6c  s:0.6.2..The fol
+000a1a60: 733a 302e 372e 300a 0a54 6865 2066 6f6c  s:0.7.0..The fol
 000a1a70: 6c6f 7769 6e67 2063 6f70 7972 6967 6874  lowing copyright
 000a1a80: 7320 616e 6420 6c69 6365 6e73 6573 2077  s and licenses w
 000a1a90: 6572 6520 666f 756e 6420 696e 2074 6865  ere found in the
 000a1aa0: 2073 6f75 7263 6520 636f 6465 206f 6620   source code of 
 000a1ab0: 7468 6973 2070 6163 6b61 6765 3a0a 0a20  this package:.. 
 000a1ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000a1ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -108446,15 +108446,15 @@
 001a79d0: 204f 4620 4f52 2049 4e20 434f 4e4e 4543   OF OR IN CONNEC
 001a79e0: 5449 4f4e 2057 4954 4820 5448 450a 534f  TION WITH THE.SO
 001a79f0: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
 001a7a00: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
 001a7a10: 4e47 5320 494e 2054 4845 2053 4f46 5457  NGS IN THE SOFTW
 001a7a20: 4152 452e 0a0a 2d2d 2d2d 0a0a 5061 636b  ARE...----..Pack
 001a7a30: 6167 653a 2062 6f74 6f33 3a31 2e33 342e  age: boto3:1.34.
-001a7a40: 3638 0a0a 5468 6520 666f 6c6c 6f77 696e  68..The followin
+001a7a40: 3832 0a0a 5468 6520 666f 6c6c 6f77 696e  82..The followin
 001a7a50: 6720 636f 7079 7269 6768 7473 2061 6e64  g copyrights and
 001a7a60: 206c 6963 656e 7365 7320 7765 7265 2066   licenses were f
 001a7a70: 6f75 6e64 2069 6e20 7468 6520 736f 7572  ound in the sour
 001a7a80: 6365 2063 6f64 6520 6f66 2074 6869 7320  ce code of this 
 001a7a90: 7061 636b 6167 653a 0a0a 2020 2020 2020  package:..      
 001a7aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a7ab0: 2020 2020 2020 2020 2020 2041 7061 6368             Apach
@@ -109163,15 +109163,15 @@
 001aa6a0: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
 001aa6b0: 6320 6c61 6e67 7561 6765 2067 6f76 6572  c language gover
 001aa6c0: 6e69 6e67 2070 6572 6d69 7373 696f 6e73  ning permissions
 001aa6d0: 2061 6e64 0a20 2020 6c69 6d69 7461 7469   and.   limitati
 001aa6e0: 6f6e 7320 756e 6465 7220 7468 6520 4c69  ons under the Li
 001aa6f0: 6365 6e73 652e 0a0a 2d2d 2d2d 0a0a 5061  cense...----..Pa
 001aa700: 636b 6167 653a 2062 6f74 6f63 6f72 653a  ckage: botocore:
-001aa710: 312e 3334 2e36 380a 0a54 6865 2066 6f6c  1.34.68..The fol
+001aa710: 312e 3334 2e38 320a 0a54 6865 2066 6f6c  1.34.82..The fol
 001aa720: 6c6f 7769 6e67 2063 6f70 7972 6967 6874  lowing copyright
 001aa730: 7320 616e 6420 6c69 6365 6e73 6573 2077  s and licenses w
 001aa740: 6572 6520 666f 756e 6420 696e 2074 6865  ere found in the
 001aa750: 2073 6f75 7263 6520 636f 6465 206f 6620   source code of 
 001aa760: 7468 6973 2070 6163 6b61 6765 3a0a 0a20  this package:.. 
 001aa770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001aa780: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -111005,15 +111005,15 @@
 001b19c0: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
 001b19d0: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
 001b19e0: 0a53 4f46 5457 4152 4520 4f52 2054 4845  .SOFTWARE OR THE
 001b19f0: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
 001b1a00: 414c 494e 4753 2049 4e20 5448 4520 534f  ALINGS IN THE SO
 001b1a10: 4654 5741 5245 2e0a 0a2d 2d2d 2d0a 0a50  FTWARE...----..P
 001b1a20: 6163 6b61 6765 3a20 6669 6c65 6c6f 636b  ackage: filelock
-001b1a30: 3a33 2e31 332e 310a 0a54 6865 2066 6f6c  :3.13.1..The fol
+001b1a30: 3a33 2e31 332e 340a 0a54 6865 2066 6f6c  :3.13.4..The fol
 001b1a40: 6c6f 7769 6e67 2063 6f70 7972 6967 6874  lowing copyright
 001b1a50: 7320 616e 6420 6c69 6365 6e73 6573 2077  s and licenses w
 001b1a60: 6572 6520 666f 756e 6420 696e 2074 6865  ere found in the
 001b1a70: 2073 6f75 7263 6520 636f 6465 206f 6620   source code of 
 001b1a80: 7468 6973 2070 6163 6b61 6765 3a0a 0a54  this package:..T
 001b1a90: 6869 7320 6973 2066 7265 6520 616e 6420  his is free and 
 001b1aa0: 756e 656e 6375 6d62 6572 6564 2073 6f66  unencumbered sof
@@ -111184,15 +111184,15 @@
 001b24f0: 5741 5920 4f55 5420 4f46 0a54 4845 2055  WAY OUT OF.THE U
 001b2500: 5345 204f 4620 5448 4953 2053 4f46 5457  SE OF THIS SOFTW
 001b2510: 4152 452c 2045 5645 4e20 4946 2041 4456  ARE, EVEN IF ADV
 001b2520: 4953 4544 204f 4620 5448 4520 504f 5353  ISED OF THE POSS
 001b2530: 4942 494c 4954 5920 4f46 2053 5543 4820  IBILITY OF SUCH 
 001b2540: 4441 4d41 4745 2e0a 0a2d 2d2d 2d0a 0a50  DAMAGE...----..P
 001b2550: 6163 6b61 6765 3a20 6879 706f 7468 6573  ackage: hypothes
-001b2560: 6973 3a36 2e39 392e 3131 0a0a 5468 6520  is:6.99.11..The 
+001b2560: 6973 3a36 2e31 3030 2e31 0a0a 5468 6520  is:6.100.1..The 
 001b2570: 666f 6c6c 6f77 696e 6720 636f 7079 7269  following copyri
 001b2580: 6768 7473 2061 6e64 206c 6963 656e 7365  ghts and license
 001b2590: 7320 7765 7265 2066 6f75 6e64 2069 6e20  s were found in 
 001b25a0: 7468 6520 736f 7572 6365 2063 6f64 6520  the source code 
 001b25b0: 6f66 2074 6869 7320 7061 636b 6167 653a  of this package:
 001b25c0: 0a0a 4d6f 7a69 6c6c 6120 5075 626c 6963  ..Mozilla Public
 001b25d0: 204c 6963 656e 7365 2056 6572 7369 6f6e   License Version
@@ -112236,15 +112236,15 @@
 001b66b0: 6465 2046 6f72 6d20 6973 2022 496e 636f  de Form is "Inco
 001b66c0: 6d70 6174 6962 6c65 2057 6974 6820 5365  mpatible With Se
 001b66d0: 636f 6e64 6172 7920 4c69 6365 6e73 6573  condary Licenses
 001b66e0: 222c 2061 730a 2020 6465 6669 6e65 6420  ", as.  defined 
 001b66f0: 6279 2074 6865 204d 6f7a 696c 6c61 2050  by the Mozilla P
 001b6700: 7562 6c69 6320 4c69 6365 6e73 652c 2076  ublic License, v
 001b6710: 2e20 322e 302e 0a0a 2d2d 2d2d 0a0a 5061  . 2.0...----..Pa
-001b6720: 636b 6167 653a 2069 646e 613a 332e 360a  ckage: idna:3.6.
+001b6720: 636b 6167 653a 2069 646e 613a 332e 370a  ckage: idna:3.7.
 001b6730: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2063  .The following c
 001b6740: 6f70 7972 6967 6874 7320 616e 6420 6c69  opyrights and li
 001b6750: 6365 6e73 6573 2077 6572 6520 666f 756e  censes were foun
 001b6760: 6420 696e 2074 6865 2073 6f75 7263 6520  d in the source 
 001b6770: 636f 6465 206f 6620 7468 6973 2070 6163  code of this pac
 001b6780: 6b61 6765 3a0a 0a52 6564 6973 7472 6962  kage:..Redistrib
 001b6790: 7574 696f 6e20 616e 6420 7573 6520 696e  ution and use in
@@ -113479,15 +113479,15 @@
 001bb460: 6865 204c 6963 656e 7365 2066 6f72 2074  he License for t
 001bb470: 6865 2073 7065 6369 6669 6320 6c61 6e67  he specific lang
 001bb480: 7561 6765 2067 6f76 6572 6e69 6e67 2070  uage governing p
 001bb490: 6572 6d69 7373 696f 6e73 2061 6e64 0a20  ermissions and. 
 001bb4a0: 2020 6c69 6d69 7461 7469 6f6e 7320 756e    limitations un
 001bb4b0: 6465 7220 7468 6520 4c69 6365 6e73 652e  der the License.
 001bb4c0: 0a0a 2d2d 2d2d 0a0a 5061 636b 6167 653a  ..----..Package:
-001bb4d0: 2070 696c 6c6f 773a 3130 2e32 2e30 0a0a   pillow:10.2.0..
+001bb4d0: 2070 696c 6c6f 773a 3130 2e33 2e30 0a0a   pillow:10.3.0..
 001bb4e0: 5468 6520 666f 6c6c 6f77 696e 6720 636f  The following co
 001bb4f0: 7079 7269 6768 7473 2061 6e64 206c 6963  pyrights and lic
 001bb500: 656e 7365 7320 7765 7265 2066 6f75 6e64  enses were found
 001bb510: 2069 6e20 7468 6520 736f 7572 6365 2063   in the source c
 001bb520: 6f64 6520 6f66 2074 6869 7320 7061 636b  ode of this pack
 001bb530: 6167 653a 0a0a 5065 726d 6973 7369 6f6e  age:..Permission
 001bb540: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
@@ -116734,15 +116734,15 @@
 001c7fd0: 2049 4e20 414e 5920 5741 5920 4f55 5420   IN ANY WAY OUT 
 001c7fe0: 4f46 0a54 4845 2055 5345 204f 4620 5448  OF.THE USE OF TH
 001c7ff0: 4953 2053 4f46 5457 4152 452c 2045 5645  IS SOFTWARE, EVE
 001c8000: 4e20 4946 2041 4456 4953 4544 204f 4620  N IF ADVISED OF 
 001c8010: 5448 4520 504f 5353 4942 494c 4954 5920  THE POSSIBILITY 
 001c8020: 4f46 2053 5543 4820 4441 4d41 4745 2e0a  OF SUCH DAMAGE..
 001c8030: 0a2d 2d2d 2d0a 0a50 6163 6b61 6765 3a20  .----..Package: 
-001c8040: 746f 7263 683a 322e 322e 310a 0a54 6865  torch:2.2.1..The
+001c8040: 746f 7263 683a 322e 322e 320a 0a54 6865  torch:2.2.2..The
 001c8050: 2066 6f6c 6c6f 7769 6e67 2063 6f70 7972   following copyr
 001c8060: 6967 6874 7320 616e 6420 6c69 6365 6e73  ights and licens
 001c8070: 6573 2077 6572 6520 666f 756e 6420 696e  es were found in
 001c8080: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
 001c8090: 206f 6620 7468 6973 2070 6163 6b61 6765   of this package
 001c80a0: 3a0a 0a52 6564 6973 7472 6962 7574 696f  :..Redistributio
 001c80b0: 6e20 616e 6420 7573 6520 696e 2073 6f75  n and use in sou
@@ -116998,15 +116998,15 @@
 001c9050: 434f 4e4e 4543 5449 4f4e 2057 4954 4820  CONNECTION WITH 
 001c9060: 5448 450a 534f 4654 5741 5245 204f 5220  THE.SOFTWARE OR 
 001c9070: 5448 4520 5553 4520 4f52 204f 5448 4552  THE USE OR OTHER
 001c9080: 2044 4541 4c49 4e47 5320 494e 2054 4845   DEALINGS IN THE
 001c9090: 2053 4f46 5457 4152 452e 0a0a 2d2d 2d2d   SOFTWARE...----
 001c90a0: 0a0a 5061 636b 6167 653a 2074 7970 696e  ..Package: typin
 001c90b0: 672d 6578 7465 6e73 696f 6e73 3a34 2e31  g-extensions:4.1
-001c90c0: 302e 300a 0a54 6865 2066 6f6c 6c6f 7769  0.0..The followi
+001c90c0: 312e 300a 0a54 6865 2066 6f6c 6c6f 7769  1.0..The followi
 001c90d0: 6e67 2063 6f70 7972 6967 6874 7320 616e  ng copyrights an
 001c90e0: 6420 6c69 6365 6e73 6573 2077 6572 6520  d licenses were 
 001c90f0: 666f 756e 6420 696e 2074 6865 2073 6f75  found in the sou
 001c9100: 7263 6520 636f 6465 206f 6620 7468 6973  rce code of this
 001c9110: 2070 6163 6b61 6765 3a0a 0a50 5954 484f   package:..PYTHO
 001c9120: 4e20 534f 4654 5741 5245 2046 4f55 4e44  N SOFTWARE FOUND
 001c9130: 4154 494f 4e20 4c49 4345 4e53 4520 5645  ATION LICENSE VE
```

### Comparing `s3torchconnector-1.2.2/pyproject.toml` & `s3torchconnector-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s3torchconnector"
-version = "1.2.2"
+version = "1.2.3"
 description = "S3 connector integration for PyTorch"
 requires-python = ">=3.8,<3.13"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -19,15 +19,15 @@
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Topic :: Utilities"
 ]
 
 dependencies = [
     "torch >= 2.0.1",
-    "s3torchconnectorclient >= 1.2.2",
+    "s3torchconnectorclient >= 1.2.3",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-timeout",
     "hypothesis",
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/__init__.py` & `s3torchconnector-1.2.3/src/s3torchconnector/__init__.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/_s3_bucket_iterable.py` & `s3torchconnector-1.2.3/src/s3torchconnector/_s3_bucket_iterable.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/_s3client/_mock_s3client.py` & `s3torchconnector-1.2.3/src/s3torchconnector/_s3client/_mock_s3client.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         )
         self._mock_client = MockMountpointS3Client(
             region,
             bucket,
             throughput_target_gbps=self.s3client_config.throughput_target_gbps,
             part_size=self.s3client_config.part_size,
             user_agent_prefix=self.user_agent_prefix,
+            unsigned=self.s3client_config.unsigned,
         )
 
     def add_object(self, key: str, data: bytes) -> None:
         self._mock_client.add_object(key, data)
 
     def remove_object(self, key: str) -> None:
         self._mock_client.remove_object(key)
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/_s3client/_s3client.py` & `s3torchconnector-1.2.3/src/s3torchconnector/_s3client/_s3client.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     def _client_builder(self) -> MountpointS3Client:
         return MountpointS3Client(
             region=self._region,
             endpoint=self._endpoint,
             user_agent_prefix=self._user_agent_prefix,
             throughput_target_gbps=self._s3client_config.throughput_target_gbps,
             part_size=self._s3client_config.part_size,
+            unsigned=self._s3client_config.unsigned,
         )
 
     def get_object(
         self, bucket: str, key: str, *, object_info: Optional[ObjectInfo] = None
     ) -> S3Reader:
         log.debug(f"GetObject s3://{bucket}/{key}, {object_info is None=}")
         if object_info is None:
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/_s3client/s3client_config.py` & `s3torchconnector-1.2.3/src/s3torchconnector/_s3client/s3client_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 @dataclass(frozen=True)
 class S3ClientConfig:
     """A dataclass exposing configurable parameters for the S3 client.
 
     Args:
     throughput_target_gbps(float): Throughput target in Gigabits per second (Gbps) that we are trying to reach.
         10.0 Gbps by default (may change in future).
-    part_size(int): Size, in bytes, of parts that files will be downloaded or uploaded in.
+    part_size(int): Size (bytes) of file parts that will be uploaded/downloaded.
         Note: for saving checkpoints, the inner client will adjust the part size to meet the service limits.
         (max number of parts per upload is 10,000, minimum upload part size is 5 MiB).
         Part size must have values between 5MiB and 5GiB.
-        8MB by default (may change in future).
+        8MiB by default (may change in future).
     """
 
     throughput_target_gbps: float = 10.0
     part_size: int = 8 * 1024 * 1024
+    unsigned: bool = False
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/_s3dataset_common.py` & `s3torchconnector-1.2.3/src/s3torchconnector/_s3dataset_common.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/_user_agent.py` & `s3torchconnector-1.2.3/src/s3torchconnector/_user_agent.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/lightning/s3_lightning_checkpoint.py` & `s3torchconnector-1.2.3/src/s3torchconnector/lightning/s3_lightning_checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 class S3LightningCheckpoint(CheckpointIO):
     """A checkpoint manager for S3 using the :class:`CheckpointIO` interface."""
 
     def __init__(
         self,
         region: str,
         s3client_config: Optional[S3ClientConfig] = None,
+        endpoint: Optional[str] = None,
     ):
         self.region = region
         user_agent = UserAgent(["lightning", lightning.__version__])
         self._client = S3Client(
             region,
             user_agent=user_agent,
             s3client_config=s3client_config,
+            endpoint=endpoint,
         )
 
     def save_checkpoint(
         self,
         checkpoint: Dict[str, Any],
         # We only support `str` arguments for `path`, as `Path` is explicitly for local filesystems
         path: str,  # type: ignore
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/s3checkpoint.py` & `s3torchconnector-1.2.3/src/s3torchconnector/s3checkpoint.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/s3iterable_dataset.py` & `s3torchconnector-1.2.3/src/s3torchconnector/s3iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/s3map_dataset.py` & `s3torchconnector-1.2.3/src/s3torchconnector/s3map_dataset.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/s3reader.py` & `s3torchconnector-1.2.3/src/s3torchconnector/s3reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,14 +49,42 @@
         Raises:
             S3Exception: An error occurred accessing S3.
         """
 
         if self._stream is None:
             self._stream = self._get_stream()
 
+    def readinto(self, buf) -> int:
+        """Read up to len(buf) bytes into a pre-allocated, writable bytes-like object buf.
+        Return the number of bytes read. If no bytes are available, zero is returned.
+
+        Args:
+            buf : writable bytes-like object
+
+        Returns:
+            int : numer of bytes read or zero, if no bytes available
+        """
+        buf_size = len(buf)
+        if self._position_at_end() or buf_size == 0:
+            # If no bytes are available or no place to write data, zero should be returned
+            return 0
+
+        self.prefetch()
+        assert self._stream is not None
+
+        cur_pos = self._position
+        # preload enough bytes in buffer
+        self.seek(buf_size, SEEK_CUR)
+        # restore position, before starting to write into buf
+        self._buffer.seek(cur_pos)
+        size = self._buffer.readinto(buf)
+        self._position = self._buffer.tell()
+
+        return size
+
     def read(self, size: Optional[int] = None) -> bytes:
         """Read up to size bytes from the object and return them.
 
         If size is zero or positive, read that many bytes from S3, or until the end of the object.
         If size is None or negative, read the entire file.
 
         Args:
@@ -78,15 +106,17 @@
 
         self.prefetch()
         assert self._stream is not None
         cur_pos = self._position
         if size is None or size < 0:
             # Special case read() all to use O(n) algorithm
             self._buffer.seek(0, SEEK_END)
-            self._buffer.write(b"".join(self._stream))
+            for batch in self._stream:
+                self._buffer.write(batch)
+
             # Once we've emptied the buffer, we'll always be at EOF!
             self._size = self._buffer.tell()
         else:
             self.seek(size, SEEK_CUR)
 
         self._buffer.seek(cur_pos)
         data = self._buffer.read(size)
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector/s3writer.py` & `s3torchconnector-1.2.3/src/s3torchconnector/s3writer.py`

 * *Files identical despite different names*

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector.egg-info/PKG-INFO` & `s3torchconnector-1.2.3/src/s3torchconnector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3torchconnector
-Version: 1.2.2
+Version: 1.2.3
 Summary: S3 connector integration for PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: THIRD-PARTY-LICENSES
 License-File: NOTICE
 Requires-Dist: torch>=2.0.1
-Requires-Dist: s3torchconnectorclient>=1.2.2
+Requires-Dist: s3torchconnectorclient>=1.2.3
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: mypy; extra == "test"
```

### Comparing `s3torchconnector-1.2.2/src/s3torchconnector.egg-info/SOURCES.txt` & `s3torchconnector-1.2.3/src/s3torchconnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

