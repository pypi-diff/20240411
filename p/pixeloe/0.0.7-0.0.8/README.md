# Comparing `tmp/pixeloe-0.0.7.tar.gz` & `tmp/pixeloe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeloe-0.0.7.tar", last modified: Sat Apr  6 13:40:55 2024, max compression
+gzip compressed data, was "pixeloe-0.0.8.tar", last modified: Thu Apr 11 02:59:08 2024, max compression
```

## Comparing `pixeloe-0.0.7.tar` & `pixeloe-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:40:55.725833 pixeloe-0.0.7/
--rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2024-03-29 05:43:29.000000 pixeloe-0.0.7/LICENSE
--rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-06 13:40:55.725540 pixeloe-0.0.7/PKG-INFO
--rw-r--r--   0 kblueleaf   (501) staff       (20)     7508 2024-04-01 04:05:40.000000 pixeloe-0.0.7/README.md
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:40:55.715857 pixeloe-0.0.7/pixeloe/
--rw-r--r--   0 kblueleaf   (501) staff       (20)       31 2024-03-29 05:43:29.000000 pixeloe-0.0.7/pixeloe/__init__.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     3637 2024-04-06 13:40:12.000000 pixeloe-0.0.7/pixeloe/cli.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     2223 2024-04-06 13:28:46.000000 pixeloe-0.0.7/pixeloe/color.py
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:40:55.724800 pixeloe-0.0.7/pixeloe/downscale/
--rw-r--r--   0 kblueleaf   (501) staff       (20)      363 2024-03-31 16:49:46.000000 pixeloe-0.0.7/pixeloe/downscale/__init__.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1113 2024-03-31 16:49:46.000000 pixeloe-0.0.7/pixeloe/downscale/center.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1554 2024-03-31 16:49:46.000000 pixeloe-0.0.7/pixeloe/downscale/contrast_based.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)      894 2024-03-31 16:49:46.000000 pixeloe-0.0.7/pixeloe/downscale/conventional.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1772 2024-03-31 16:49:46.000000 pixeloe-0.0.7/pixeloe/downscale/k_centroid.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     3189 2024-04-06 13:31:59.000000 pixeloe-0.0.7/pixeloe/outline.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)     1915 2024-04-06 13:39:38.000000 pixeloe-0.0.7/pixeloe/pixelize.py
--rw-r--r--   0 kblueleaf   (501) staff       (20)      951 2024-04-06 13:31:13.000000 pixeloe-0.0.7/pixeloe/utils.py
-drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:40:55.725193 pixeloe-0.0.7/pixeloe.egg-info/
--rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-06 13:40:55.000000 pixeloe-0.0.7/pixeloe.egg-info/PKG-INFO
--rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-06 13:40:55.000000 pixeloe-0.0.7/pixeloe.egg-info/SOURCES.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-04-06 13:40:55.000000 pixeloe-0.0.7/pixeloe.egg-info/dependency_links.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)       96 2024-04-06 13:40:55.000000 pixeloe-0.0.7/pixeloe.egg-info/entry_points.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-03-29 05:49:33.000000 pixeloe-0.0.7/pixeloe.egg-info/not-zip-safe
--rw-r--r--   0 kblueleaf   (501) staff       (20)       27 2024-04-06 13:40:55.000000 pixeloe-0.0.7/pixeloe.egg-info/requires.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2024-04-06 13:40:55.000000 pixeloe-0.0.7/pixeloe.egg-info/top_level.txt
--rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2024-04-06 13:40:55.725890 pixeloe-0.0.7/setup.cfg
--rw-r--r--   0 kblueleaf   (501) staff       (20)      707 2024-04-06 13:40:42.000000 pixeloe-0.0.7/setup.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.951105 pixeloe-0.0.8/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2024-03-29 05:43:29.000000 pixeloe-0.0.8/LICENSE
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-11 02:59:08.950801 pixeloe-0.0.8/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     7517 2024-04-11 02:57:31.000000 pixeloe-0.0.8/README.md
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.947085 pixeloe-0.0.8/pixeloe/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:57:08.000000 pixeloe-0.0.8/pixeloe/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3637 2024-04-06 13:40:12.000000 pixeloe-0.0.8/pixeloe/cli.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2193 2024-04-06 13:44:10.000000 pixeloe-0.0.8/pixeloe/color.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.950133 pixeloe-0.0.8/pixeloe/downscale/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      363 2024-03-31 16:49:46.000000 pixeloe-0.0.8/pixeloe/downscale/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1113 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/center.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1554 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/contrast_based.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      894 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/conventional.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1772 2024-04-06 13:42:55.000000 pixeloe-0.0.8/pixeloe/downscale/k_centroid.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3189 2024-04-06 13:42:41.000000 pixeloe-0.0.8/pixeloe/outline.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1915 2024-04-06 13:39:38.000000 pixeloe-0.0.8/pixeloe/pixelize.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      903 2024-04-06 13:59:07.000000 pixeloe-0.0.8/pixeloe/utils.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-11 02:59:08.950508 pixeloe-0.0.8/pixeloe.egg-info/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/SOURCES.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/dependency_links.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       96 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/entry_points.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-03-29 05:49:33.000000 pixeloe-0.0.8/pixeloe.egg-info/not-zip-safe
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       27 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/requires.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2024-04-11 02:59:08.000000 pixeloe-0.0.8/pixeloe.egg-info/top_level.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2024-04-11 02:59:08.951166 pixeloe-0.0.8/setup.cfg
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      699 2024-04-11 02:59:04.000000 pixeloe-0.0.8/setup.py
```

### Comparing `pixeloe-0.0.7/LICENSE` & `pixeloe-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.7/README.md` & `pixeloe-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 ---
 
 Or you can import it into your code:
 
 ```python
 import cv2
-from pixeloe import pixelize
+from pixeloe.pixelize import pixelize
 
 img = cv2.imread("img/test.png")
 img = pixelize(img, target_size=256, patch_size=8)
 cv2.imwrite("img/test2.png", img)
 ```
 
 ## Algorithm Explanation
```

### Comparing `pixeloe-0.0.7/pixeloe/cli.py` & `pixeloe-0.0.8/pixeloe/cli.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.7/pixeloe/color.py` & `pixeloe-0.0.8/pixeloe/color.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,45 +18,45 @@
     source[:, :, 0] = wavelet_colorfix(source[:, :, 0], target[:, :, 0])
     source[:, :, 1] = wavelet_colorfix(source[:, :, 1], target[:, :, 1])
     source[:, :, 2] = wavelet_colorfix(source[:, :, 2], target[:, :, 2])
     output = source
     return output.clip(0, 255).astype(np.uint8)
 
 
-def wavelet_colorfix(input, target):
-    input_high, _ = wavelet_decomposition(input, 5)
+def wavelet_colorfix(inp, target):
+    inp_high, _ = wavelet_decomposition(inp, 5)
     _, target_low = wavelet_decomposition(target, 5)
-    output = input_high + target_low
+    output = inp_high + target_low
     return output
 
 
-def wavelet_decomposition(input, levels):
-    high_freq = np.zeros_like(input)
+def wavelet_decomposition(inp, levels):
+    high_freq = np.zeros_like(inp)
     for i in range(1, levels + 1):
         radius = 2**i
-        low_freq = wavelet_blur(input, radius)
-        high_freq = high_freq + (input - low_freq)
-        input = low_freq
+        low_freq = wavelet_blur(inp, radius)
+        high_freq = high_freq + (inp - low_freq)
+        inp = low_freq
     return high_freq, low_freq
 
 
-def wavelet_blur(input, radius):
+def wavelet_blur(inp, radius):
     kernel_size = 2 * radius + 1
-    output = cv2.GaussianBlur(input, (kernel_size, kernel_size), 0)
+    output = cv2.GaussianBlur(inp, (kernel_size, kernel_size), 0)
     return output
 
 
-def color_styling(input, saturation=1.2, contrast=1.1):
-    output = input.copy()
+def color_styling(inp, saturation=1.2, contrast=1.1):
+    output = inp.copy()
     output = cv2.cvtColor(output, cv2.COLOR_BGR2HSV)
     output[:, :, 1] = output[:, :, 1] * saturation
     output[:, :, 2] = output[:, :, 2] * contrast - (contrast - 1)
     output = np.clip(output, 0, 1)
     output = cv2.cvtColor(output, cv2.COLOR_HSV2BGR)
     return output
 
 
-def kmeans_color_quant(input, colors=32):
-    img = cv2.cvtColor(input, cv2.COLOR_BGR2RGB)
+def kmeans_color_quant(inp, colors=32):
+    img = cv2.cvtColor(inp, cv2.COLOR_BGR2RGB)
     img_pil = Image.fromarray(img)
     img_quant = img_pil.quantize(colors, 1, kmeans=colors).convert("RGB")
     return cv2.cvtColor(np.array(img_quant), cv2.COLOR_RGB2BGR)
```

### Comparing `pixeloe-0.0.7/pixeloe/downscale/center.py` & `pixeloe-0.0.8/pixeloe/downscale/center.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..utils import apply_chunk
 
 
 def center_downscale(
     img,
     target_size=128,
 ):
-    H, W, C = img.shape
+    H, W, _ = img.shape
 
     ratio = W / H
     target_size = (target_size**2 / ratio) ** 0.5
     target_hw = (int(target_size * ratio), int(target_size))
     patch_size = max(int(round(H // target_hw[1])), int(round(W // target_hw[0])))
 
     img_lab = cv2.cvtColor(img, cv2.COLOR_BGR2LAB).astype(np.float32)
```

### Comparing `pixeloe-0.0.7/pixeloe/downscale/contrast_based.py` & `pixeloe-0.0.8/pixeloe/downscale/contrast_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return output
 
 
 def contrast_based_downscale(
     img,
     target_size=128,
 ):
-    H, W, C = img.shape
+    H, W, _ = img.shape
 
     ratio = W / H
     target_size = (target_size**2 / ratio) ** 0.5
     target_hw = (int(target_size * ratio), int(target_size))
     patch_size = max(int(round(H // target_hw[1])), int(round(W // target_hw[0])))
 
     img_lab = cv2.cvtColor(img, cv2.COLOR_BGR2LAB).astype(np.float32)
```

### Comparing `pixeloe-0.0.7/pixeloe/downscale/conventional.py` & `pixeloe-0.0.8/pixeloe/downscale/conventional.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from PIL import Image
 
 
 def nearest(
     img,
     target_size=128,
 ):
-    H, W, C = img.shape
+    H, W, _ = img.shape
 
     ratio = W / H
     target_size = (target_size**2 / ratio) ** 0.5
     target_hw = (int(target_size * ratio), int(target_size))
     img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
     img = Image.fromarray(img_rgb)
     img_sm = img.resize(target_hw, Image.NEAREST)
@@ -19,15 +19,15 @@
     return img_sm
 
 
 def bicubic(
     img,
     target_size=128,
 ):
-    H, W, C = img.shape
+    H, W, _ = img.shape
 
     ratio = W / H
     target_size = (target_size**2 / ratio) ** 0.5
     target_hw = (int(target_size * ratio), int(target_size))
     img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
     img = Image.fromarray(img_rgb)
     img_sm = img.resize(target_hw, Image.BICUBIC)
```

### Comparing `pixeloe-0.0.7/pixeloe/downscale/k_centroid.py` & `pixeloe-0.0.8/pixeloe/downscale/k_centroid.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def k_centroid_downscale(cv2img, target_size=128, centroids=2):
     """
     k-centroid downscaling algorithm from Astropulse, under MIT License.
     https://github.com/Astropulse/pixeldetector/blob/6e88e18ddbd16529b5dd85b1c615cbb2e5778bf2/k-centroid.py#L19-L44
     """
-    H, W, C = cv2img.shape
+    H, W, _ = cv2img.shape
 
     ratio = W / H
     target_size = (target_size**2 / ratio) ** 0.5
     height = int(target_size)
     width = int(target_size * ratio)
 
     # Perform outline expansion and color matching
```

### Comparing `pixeloe-0.0.7/pixeloe/outline.py` & `pixeloe-0.0.8/pixeloe/outline.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     output = cv2.erode(output, kernel_smoothing, iterations=erode)
 
     return output
 
 
 if __name__ == "__main__":
     img = cv2.imread("img/dragon-girl.png")
-    H, W, C = img.shape
+    H, W, _ = img.shape
     ratio = W / H
     target_pixel_count = (1024**2 / ratio) ** 0.5
     img = cv2.resize(img, (int(target_pixel_count * ratio), int(target_pixel_count)))
     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
     weight_mat = expansion_weight(img, 8, 2, 9, 3)
     img_out = outline_expansion(img, 1, 1)
```

### Comparing `pixeloe-0.0.7/pixeloe/pixelize.py` & `pixeloe-0.0.8/pixeloe/pixelize.py`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.7/pixeloe/utils.py` & `pixeloe-0.0.8/pixeloe/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,12 +33,8 @@
 
 
 def sigmoid(x):
     return 1 / (1 + np.exp(-x))
 
 
 def isiterable(x):
-    try:
-        _ = iter(x)
-        return True
-    except:
-        return False
+    return hasattr(x, "__iter__")
```

### Comparing `pixeloe-0.0.7/pixeloe.egg-info/SOURCES.txt` & `pixeloe-0.0.8/pixeloe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixeloe-0.0.7/setup.py` & `pixeloe-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
-from pixeloe.cli import command_map
+from pixeloe import cli
 
 
 setup(
     name="pixeloe",
     packages=find_packages(),
-    version="0.0.7",
+    version="0.0.8",
     url="https://github.com/KohakuBlueleaf/PixelOE",
     description="Detail-Oriented Pixelization based on Contrast-Aware Outline Expansion.",
     license="Apache License 2.0",
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=["opencv-python", "numpy", "pillow"],
     entry_points={
         "console_scripts": [
             f"pixeloe.{command}=pixeloe.cli:{func}"
-            for command, func in command_map.items()
+            for command, func in cli.command_map.items()
         ]
     },
     python_requires=">=3.10",
 )
```

