# Comparing `tmp/aioxdl-0.0.3.tar.gz` & `tmp/aioxdl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.3.tar", last modified: Wed Apr 10 07:19:31 2024, max compression
+gzip compressed data, was "aioxdl-0.0.4.tar", last modified: Wed Apr 10 14:16:36 2024, max compression
```

## Comparing `aioxdl-0.0.3.tar` & `aioxdl-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.973878 aioxdl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 07:19:23.000000 aioxdl-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-10 07:19:31.973878 aioxdl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-10 07:19:23.000000 aioxdl-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.969878 aioxdl-0.0.3/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 07:19:23.000000 aioxdl-0.0.3/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-10 07:19:23.000000 aioxdl-0.0.3/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.973878 aioxdl-0.0.3/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-10 07:19:31.000000 aioxdl-0.0.3/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 07:19:31.000000 aioxdl-0.0.3/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:19:31.000000 aioxdl-0.0.3/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:19:31.000000 aioxdl-0.0.3/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 07:19:31.000000 aioxdl-0.0.3/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 07:19:31.000000 aioxdl-0.0.3/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:19:31.973878 aioxdl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 07:19:23.000000 aioxdl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:16:36.734083 aioxdl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 14:16:29.000000 aioxdl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-10 14:16:36.734083 aioxdl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-10 14:16:29.000000 aioxdl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:16:36.734083 aioxdl-0.0.4/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 14:16:29.000000 aioxdl-0.0.4/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-10 14:16:29.000000 aioxdl-0.0.4/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:16:36.734083 aioxdl-0.0.4/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-10 14:16:36.000000 aioxdl-0.0.4/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 14:16:36.000000 aioxdl-0.0.4/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:16:36.000000 aioxdl-0.0.4/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:16:36.000000 aioxdl-0.0.4/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 14:16:36.000000 aioxdl-0.0.4/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:16:36.000000 aioxdl-0.0.4/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:16:36.734083 aioxdl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 14:16:29.000000 aioxdl-0.0.4/setup.py
```

### Comparing `aioxdl-0.0.3/LICENSE` & `aioxdl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.3/PKG-INFO` & `aioxdl-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.3
+Version: 0.0.4
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,22 @@
 
 async def progress(_, stime, tsize, dsize):
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
-    file = "testfile.mkv"
+    loca = "./Downloads/testfile.mkv"
     link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
-    ou, _ = await core.start(link, file, progress=progress)
-    print(ou)
+    file = await core.start(link, loca, progress=progress)
+    fine = file if core.error == None else core.error
+    print(fine)
 
 asyncio.run(main())
+
+#===[ PROGRESS FUNCTION ]===
+
+# stime = start time
+# tsize = total size
+# dsize = download size
+
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.3 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.4 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -13,11 +13,13 @@
 Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: aiohttp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
 dsize): percentage = round((dsize / tsize) * 100, 2) print("COMPLETED :
-{}%".format(percentage)) async def main(): core = Downloader() file =
-"testfile.mkv" link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" ou, _
-= await core.start(link, file, progress=progress) print(ou) asyncio.run(main())
-```
+{}%".format(percentage)) async def main(): core = Downloader() loca = "./
+Downloads/testfile.mkv" link = "https://www.tg-x.workers.dev/dl/
+18357?hash=AgADIh" file = await core.start(link, loca, progress=progress) fine
+= file if core.error == None else core.error print(fine) asyncio.run(main())
+#===[ PROGRESS FUNCTION ]=== # stime = start time # tsize = total size # dsize
+= download size ```
```

### Comparing `aioxdl-0.0.3/README.md` & `aioxdl-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 
 async def progress(_, stime, tsize, dsize):
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
-    file = "testfile.mkv"
+    loca = "./Downloads/testfile.mkv"
     link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
-    ou, _ = await core.start(link, file, progress=progress)
-    print(ou)
+    file = await core.start(link, loca, progress=progress)
+    fine = file if core.error == None else core.error
+    print(fine)
 
 asyncio.run(main())
+
+#===[ PROGRESS FUNCTION ]===
+
+# stime = start time
+# tsize = total size
+# dsize = download size
+
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
 dsize): percentage = round((dsize / tsize) * 100, 2) print("COMPLETED :
-{}%".format(percentage)) async def main(): core = Downloader() file =
-"testfile.mkv" link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" ou, _
-= await core.start(link, file, progress=progress) print(ou) asyncio.run(main())
-```
+{}%".format(percentage)) async def main(): core = Downloader() loca = "./
+Downloads/testfile.mkv" link = "https://www.tg-x.workers.dev/dl/
+18357?hash=AgADIh" file = await core.start(link, loca, progress=progress) fine
+= file if core.error == None else core.error print(fine) asyncio.run(main())
+#===[ PROGRESS FUNCTION ]=== # stime = start time # tsize = total size # dsize
+= download size ```
```

### Comparing `aioxdl-0.0.3/aioxdl/module.py` & `aioxdl-0.0.4/aioxdl/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import time, aiohttp
-#=======================================================================================================
+#=================================================================================================
 
 class Downloader:
 
-    def __init__(self, imsg=None):
+    def __init__(self, message=None):
         self.tsize = 0
         self.dsize = 0
+        self.error = None
         self.chunk = 1024
         self.timeo = 1000
-        self.imesg = imsg
+        self.imssg = message
         self.stime = time.time()
 
-#=======================================================================================================
+#=================================================================================================
 
     async def getsizes(self, response):
         return int(response.headers.get("Content-Length", 0)) or 0
 
     async def checkurl(self, url, timeout=20):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 return 200 if response.status == 200 else response.status
 
     async def display(self, progress):
-        await progress(self.imesg, self.stime, self.tsize, self.dsize) if progress else None
+        await progress(self.imssg, self.stime, self.tsize, self.dsize) if progress else None
 
-#=======================================================================================================
+#=================================================================================================
 
     async def download(self, url, location, timeout, progress):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 self.tsize += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
@@ -37,20 +38,21 @@
                             break
                         handlexo.write(chunks)
                         self.dsize += self.chunk
                         await self.display(progress)
 
                 return location
 
-#=======================================================================================================
+#=================================================================================================
 
     async def start(self, url, location, timeout=1000, progress=None):
         try:
-            messages = None
             location = await self.download(url, location, timeout, progress)
+        except aiohttp.ClientConnectorError as errors:
+            self.error = errors
         except Exception as errors:
-            messages = errors
-        
-        return messages, location
+            self.error = errors
 
-#=======================================================================================================
+        return location
+
+#=================================================================================================
```

### Comparing `aioxdl-0.0.3/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.4/aioxdl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.3
+Version: 0.0.4
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,22 @@
 
 async def progress(_, stime, tsize, dsize):
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
-    file = "testfile.mkv"
+    loca = "./Downloads/testfile.mkv"
     link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
-    ou, _ = await core.start(link, file, progress=progress)
-    print(ou)
+    file = await core.start(link, loca, progress=progress)
+    fine = file if core.error == None else core.error
+    print(fine)
 
 asyncio.run(main())
+
+#===[ PROGRESS FUNCTION ]===
+
+# stime = start time
+# tsize = total size
+# dsize = download size
+
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.3 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.4 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -13,11 +13,13 @@
 Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: aiohttp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
 dsize): percentage = round((dsize / tsize) * 100, 2) print("COMPLETED :
-{}%".format(percentage)) async def main(): core = Downloader() file =
-"testfile.mkv" link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" ou, _
-= await core.start(link, file, progress=progress) print(ou) asyncio.run(main())
-```
+{}%".format(percentage)) async def main(): core = Downloader() loca = "./
+Downloads/testfile.mkv" link = "https://www.tg-x.workers.dev/dl/
+18357?hash=AgADIh" file = await core.start(link, loca, progress=progress) fine
+= file if core.error == None else core.error print(fine) asyncio.run(main())
+#===[ PROGRESS FUNCTION ]=== # stime = start time # tsize = total size # dsize
+= download size ```
```

### Comparing `aioxdl-0.0.3/setup.py` & `aioxdl-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.3',
+    version='0.0.4',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     install_requires=['aiohttp'],
     long_description=long_description,
```

