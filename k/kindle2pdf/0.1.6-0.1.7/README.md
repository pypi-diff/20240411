# Comparing `tmp/kindle2pdf-0.1.6.tar.gz` & `tmp/kindle2pdf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kindle2pdf-0.1.6.tar", max compression
+gzip compressed data, was "kindle2pdf-0.1.7.tar", max compression
```

## Comparing `kindle2pdf-0.1.6.tar` & `kindle2pdf-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      718 2024-04-07 18:34:12.317348 kindle2pdf-0.1.6/README.md
--rw-r--r--   0        0        0    14579 2024-04-08 07:27:54.880220 kindle2pdf-0.1.6/kindle2pdf.py
--rw-r--r--   0        0        0      461 2024-04-08 07:28:25.809149 kindle2pdf-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 kindle2pdf-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-04-07 18:34:12.317348 kindle2pdf-0.1.7/README.md
+-rw-r--r--   0        0        0    15303 2024-04-11 19:59:20.962120 kindle2pdf-0.1.7/kindle2pdf.py
+-rw-r--r--   0        0        0      461 2024-04-11 19:48:55.015409 kindle2pdf-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 kindle2pdf-0.1.7/PKG-INFO
```

### Comparing `kindle2pdf-0.1.6/README.md` & `kindle2pdf-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kindle2pdf-0.1.6/kindle2pdf.py` & `kindle2pdf-0.1.7/kindle2pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,28 +47,40 @@
 
     def __init__(
         self,
         asin: str,
         font_size: int = 12,
         page_size: tuple[float, float] = A4,
         dpi: int = 160,
+        left_margin: float = 0.5,
+        right_margin: float = 0.5,
+        top_margin: float = 0.5,
+        bottom_margin: float = 0.5,
     ) -> None:
         """
         Initializes the Kindle2PDF object with the specified ASIN and starts a reading session.
 
         Args:
             asin (str): The ASIN of the book to convert.
             font_size (int): The font size to use for rendering the book.
             page_size (tuple[float, float]): The size of the PDF pages.
             dpi (int): The DPI to use for rendering images.
+            left_margin (float): The left margin of the PDF pages in inches.
+            right_margin (float): The right margin of the PDF pages in inches.
+            top_margin (float): The top margin of the PDF pages in inches.
+            bottom_margin (float): The bottom margin of the PDF pages in inches.
         """
         self.asin = asin
         self.font_size = font_size
         self.page_size = page_size
         self.dpi = dpi
+        self.left_margin = left_margin
+        self.right_margin = right_margin
+        self.top_margin = top_margin
+        self.bottom_margin = bottom_margin
         self.session = self.start_reading_session()
 
     def start_reading_session(self) -> dict:
         """
         Starts a new reading session by authenticating with Amazon and retrieving session tokens.
 
         Returns:
@@ -167,18 +179,18 @@
             "revision": self.session["version"],
             "fontFamily": "Bookerly",
             "fontSize": str(self.font_size),
             "lineHeight": "1.4",
             "dpi": str(self.dpi),
             "height": str(int(self.page_size[1] * self.dpi / 72)),
             "width": str(int(self.page_size[0] * self.dpi / 72)),
-            "marginBottom": "0",
-            "marginLeft": "9",
-            "marginRight": "9",
-            "marginTop": "0",
+            "marginBottom": str(int(self.bottom_margin * 72)),
+            "marginLeft": str(int(self.left_margin * 72)),
+            "marginRight": str(int(self.right_margin * 72)),
+            "marginTop": str(int(self.top_margin * 72)),
             "maxNumberColumns": "1",
             "theme": "default",
             "locationMap": "true",
             "packageType": "TAR",
             "encryptionVersion": "NONE",
             "numPage": num_pages,
             "skipPageCount": 0,
```

### Comparing `kindle2pdf-0.1.6/PKG-INFO` & `kindle2pdf-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kindle2pdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Robert Dargavel Smith
 Author-email: teticio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

