# Comparing `tmp/VisionCraftAPI-1.0.4.tar.gz` & `tmp/VisionCraftAPI-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraftAPI-1.0.4.tar", last modified: Tue Apr  9 20:34:30 2024, max compression
+gzip compressed data, was "VisionCraftAPI-1.0.5.tar", last modified: Thu Apr 11 19:08:07 2024, max compression
```

## Comparing `VisionCraftAPI-1.0.4.tar` & `VisionCraftAPI-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.149083 VisionCraftAPI-1.0.4/
--rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2542 2024-04-09 20:34:30.150082 VisionCraftAPI-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 VisionCraftAPI-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.105083 VisionCraftAPI-1.0.4/VisionCraftAPI/
--rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/__init__.py
--rw-rw-rw-   0        0        0    20169 2024-04-09 20:33:12.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/api.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.125082 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/
--rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/__init__.py
--rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/modes.py
--rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/task_statuses.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.131080 VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/
--rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/types.py
--rw-rw-rw-   0        0        0     2067 2024-04-05 14:57:20.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/http_client.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.143083 VisionCraftAPI-1.0.4/VisionCraftAPI/models/
--rw-rw-rw-   0        0        0      303 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/__init__.py
--rw-rw-rw-   0        0        0      336 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/limits.py
--rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/llm.py
--rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/midjourney.py
--rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/whisper.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.146081 VisionCraftAPI-1.0.4/VisionCraftAPI/utils/
--rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/utils/__init__.py
--rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/utils/checker.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.119085 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/
--rw-rw-rw-   0        0        0     2542 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 20:34:30.152091 VisionCraftAPI-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-04-09 20:33:17.000000 VisionCraftAPI-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:07.005238 VisionCraftAPI-1.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2542 2024-04-11 19:08:07.006241 VisionCraftAPI-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 VisionCraftAPI-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.951244 VisionCraftAPI-1.0.5/VisionCraftAPI/
+-rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/__init__.py
+-rw-rw-rw-   0        0        0    20917 2024-04-11 18:50:01.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.976238 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/
+-rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/modes.py
+-rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/task_statuses.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.981240 VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/
+-rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/types.py
+-rw-rw-rw-   0        0        0     2067 2024-04-05 14:57:20.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/http_client.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.997240 VisionCraftAPI-1.0.5/VisionCraftAPI/models/
+-rw-rw-rw-   0        0        0      303 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/__init__.py
+-rw-rw-rw-   0        0        0      336 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/limits.py
+-rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/llm.py
+-rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/midjourney.py
+-rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/whisper.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:07.004239 VisionCraftAPI-1.0.5/VisionCraftAPI/utils/
+-rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/utils/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/utils/checker.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.969246 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/
+-rw-rw-rw-   0        0        0     2542 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 19:08:07.008240 VisionCraftAPI-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-04-11 19:07:26.000000 VisionCraftAPI-1.0.5/setup.py
```

### Comparing `VisionCraftAPI-1.0.4/LICENSE` & `VisionCraftAPI-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/PKG-INFO` & `VisionCraftAPI-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VisionCraftAPI-1.0.4/README.md` & `VisionCraftAPI-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI/api.py` & `VisionCraftAPI-1.0.5/VisionCraftAPI/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,25 @@
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/llm-models/available-models
         SDK Docs: https://vision.b2k.tech/docs/api-methods/large-language-models-llms/get_llm_models
         
         :return: A list of LLM models
         """
         return await self.__get(f'{self.API_HOST}/models-llm')
     
+    async def get_upscale_models(self) -> list:
+        """
+        Get list of all upscale models.
+        
+        API Docs: https://docs.visioncraft.top/interacting-with-the-api/image-upscale/available-models
+        SDK Docs: https://vision.b2k.tech/docs/api-methods/image-upscale/get_upscale_models
+        
+        :return: A list of upscale models
+        """
+        return await self.__get(f'{self.API_HOST}/models-upscale')
+
     async def get_samplers(self) -> list:
         """
         Get list of all samplers for StableDiffusion 1.x models.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/stablediffusion-1.x-models/available-samplers
         SDK Docs: https://vision.b2k.tech/docs/api-methods/stablediffusion-1.x-models/get_samplers
         
@@ -294,32 +305,38 @@
             "token": self.api_key
         }
         
         result = await self.__post(f'{self.API_HOST}/midjourney/result', json=json)
         return MidjourneyResult(**result)
     
     async def image_upscaling(self,
-                              image: str | bytes) -> bytes:     
+                              image: str | bytes,
+                              model: str,
+                              resize: Optional[int] = 2) -> bytes:     
         """
         Upscale an image.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/image-upscale/upscale
         SDK Docs: https://vision.b2k.tech/docs/api-methods/image-upscale/image_upscaling
         
         :param image: A URL or bytes object of the image to upscale
+        :param model: An upscale model from the list of available models
+        :param resize: How many times to improve a photo (2 or 4)
         
         :return: A bytes object of the upscaled image
         """   
         
         if type(image) == bytes:
             image = base64.b64encode(image).decode('utf-8')
         
         json = {
             "image": image,
-            "token": self.api_key
+            "token": self.api_key,
+            "model": model,
+            "resize": resize
         }
         
         return await self.__post(f'{self.API_HOST}/upscale', json=json)
     
     async def image2image(self,
                           image: str | bytes,
                           prompt: str,
```

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/types.py` & `VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/types.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI/http_client.py` & `VisionCraftAPI-1.0.5/VisionCraftAPI/http_client.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI/models/whisper.py` & `VisionCraftAPI-1.0.5/VisionCraftAPI/models/whisper.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI/utils/checker.py` & `VisionCraftAPI-1.0.5/VisionCraftAPI/utils/checker.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/PKG-INFO` & `VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/SOURCES.txt` & `VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.4/setup.py` & `VisionCraftAPI-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.4'
+version = '1.0.5'
 
 with open('README.md', 'r') as f:
       long_description = f.read()
 
 setup(name='VisionCraftAPI',
       version=version,
```

