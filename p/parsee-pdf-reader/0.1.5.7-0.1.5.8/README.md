# Comparing `tmp/parsee_pdf_reader-0.1.5.7.tar.gz` & `tmp/parsee_pdf_reader-0.1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsee_pdf_reader-0.1.5.7.tar", max compression
+gzip compressed data, was "parsee_pdf_reader-0.1.5.8.tar", max compression
```

## Comparing `parsee_pdf_reader-0.1.5.7.tar` & `parsee_pdf_reader-0.1.5.8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     2103 2024-03-14 16:22:53.928158 parsee_pdf_reader-0.1.5.7/README.md
--rw-r--r--   0        0        0       75 2024-03-05 15:48:26.078726 parsee_pdf_reader-0.1.5.7/pdf_reader/__init__.py
--rw-r--r--   0        0        0     7938 2024-03-19 11:07:45.223684 parsee_pdf_reader-0.1.5.7/pdf_reader/converter.py
--rw-r--r--   0        0        0    35261 2024-03-15 15:33:11.382995 parsee_pdf_reader-0.1.5.7/pdf_reader/custom_dataclasses.py
--rw-r--r--   0        0        0     4673 2024-03-15 16:32:11.639123 parsee_pdf_reader-0.1.5.7/pdf_reader/extract.py
--rw-r--r--   0        0        0     4341 2024-03-14 11:57:22.437409 parsee_pdf_reader-0.1.5.7/pdf_reader/helper.py
--rw-r--r--   0        0        0    47790 2024-03-15 16:01:25.561217 parsee_pdf_reader-0.1.5.7/pdf_reader/pdf_page.py
--rw-r--r--   0        0        0     1653 2024-03-15 16:32:17.079506 parsee_pdf_reader-0.1.5.7/pdf_reader/visualisation.py
--rw-r--r--   0        0        0      502 2024-03-19 11:07:57.246721 parsee_pdf_reader-0.1.5.7/pyproject.toml
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 parsee_pdf_reader-0.1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-21 12:36:41.365473 parsee_pdf_reader-0.1.5.8/LICENSE
+-rw-r--r--   0        0        0     2103 2024-03-14 16:22:53.928158 parsee_pdf_reader-0.1.5.8/README.md
+-rw-r--r--   0        0        0       75 2024-03-05 15:48:26.078726 parsee_pdf_reader-0.1.5.8/pdf_reader/__init__.py
+-rw-r--r--   0        0        0     8019 2024-04-11 16:41:06.009187 parsee_pdf_reader-0.1.5.8/pdf_reader/converter.py
+-rw-r--r--   0        0        0    35261 2024-04-11 16:37:14.422122 parsee_pdf_reader-0.1.5.8/pdf_reader/custom_dataclasses.py
+-rw-r--r--   0        0        0     4673 2024-04-11 16:37:14.422411 parsee_pdf_reader-0.1.5.8/pdf_reader/extract.py
+-rw-r--r--   0        0        0     4341 2024-03-14 11:57:22.437409 parsee_pdf_reader-0.1.5.8/pdf_reader/helper.py
+-rw-r--r--   0        0        0    47790 2024-04-11 16:37:14.422701 parsee_pdf_reader-0.1.5.8/pdf_reader/pdf_page.py
+-rw-r--r--   0        0        0     1653 2024-03-15 16:32:17.079506 parsee_pdf_reader-0.1.5.8/pdf_reader/visualisation.py
+-rw-r--r--   0        0        0      502 2024-04-11 16:42:06.321822 parsee_pdf_reader-0.1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 parsee_pdf_reader-0.1.5.8/PKG-INFO
```

### Comparing `parsee_pdf_reader-0.1.5.7/README.md` & `parsee_pdf_reader-0.1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `parsee_pdf_reader-0.1.5.7/pdf_reader/converter.py` & `parsee_pdf_reader-0.1.5.8/pdf_reader/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,26 +154,27 @@
 def get_elements_from_image(image_path: str) -> Tuple[Rect, List[LTChar]]:
     CONF_THRESHOLD = 60
 
     output = []
 
     # start tesseract
     img = cv2.imread(image_path)
+    height, width, channels = img.shape
     tesseract_data = pytesseract.image_to_data(img, output_type=Output.DICT, config="--psm 11")
     for k, conf in enumerate(tesseract_data["conf"]):
         if conf < 0:
             continue
         x0 = tesseract_data["left"][k]
         x1 = tesseract_data["left"][k] + tesseract_data["width"][k]
         y0 = tesseract_data["top"][k]
         y1 = tesseract_data["top"][k] + tesseract_data["height"][k]
         if CONF_THRESHOLD > conf >= 0:
             # crop the text and resize, then run tesseract just on that text piece again
             padding = 2
-            crop_img = img[y0 - padding:y1 + padding, x0 - padding:x1 + padding]
+            crop_img = img[max(y0 - padding, 0):min(y1 + padding, height), max(x0 - padding, 0):min(x1 + padding, width)]
             crop_img = cv2.resize(crop_img, None, fx=3, fy=3, interpolation=cv2.INTER_CUBIC)
             data_cropped_img = pytesseract.image_to_data(crop_img, output_type=Output.DICT, config="--psm 7")
             new_text = " ".join([x for k, x in enumerate(data_cropped_img["text"]) if data_cropped_img["conf"][k] >= 0])
             # replace in dictionary
             tesseract_data["text"][k] = new_text
         text = tesseract_data["text"][k]
```

### Comparing `parsee_pdf_reader-0.1.5.7/pdf_reader/custom_dataclasses.py` & `parsee_pdf_reader-0.1.5.8/pdf_reader/custom_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_pdf_reader-0.1.5.7/pdf_reader/extract.py` & `parsee_pdf_reader-0.1.5.8/pdf_reader/extract.py`

 * *Files identical despite different names*

### Comparing `parsee_pdf_reader-0.1.5.7/pdf_reader/helper.py` & `parsee_pdf_reader-0.1.5.8/pdf_reader/helper.py`

 * *Files identical despite different names*

### Comparing `parsee_pdf_reader-0.1.5.7/pdf_reader/pdf_page.py` & `parsee_pdf_reader-0.1.5.8/pdf_reader/pdf_page.py`

 * *Files identical despite different names*

### Comparing `parsee_pdf_reader-0.1.5.7/pdf_reader/visualisation.py` & `parsee_pdf_reader-0.1.5.8/pdf_reader/visualisation.py`

 * *Files identical despite different names*

### Comparing `parsee_pdf_reader-0.1.5.7/PKG-INFO` & `parsee_pdf_reader-0.1.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsee-pdf-reader
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: 
 Home-page: https://parsee.ai
 Author: Parsee.ai
 Author-email: info@parsee.ai
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

