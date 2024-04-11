# Comparing `tmp/easyofd-0.1.1.4.tar.gz` & `tmp/easyofd-0.1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyofd-0.1.1.4.tar", last modified: Tue Mar 19 06:17:27 2024, max compression
+gzip compressed data, was "easyofd-0.1.1.5.tar", last modified: Thu Apr 11 03:20:39 2024, max compression
```

## Comparing `easyofd-0.1.1.4.tar` & `easyofd-0.1.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 06:17:27.658357 easyofd-0.1.1.4/
--rw-rw-rw-   0        0        0    11550 2023-10-07 08:01:17.000000 easyofd-0.1.1.4/LICENSE
--rw-rw-rw-   0        0        0     1875 2024-03-19 06:17:27.657363 easyofd-0.1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1439 2024-03-14 10:29:52.000000 easyofd-0.1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 06:17:27.628349 easyofd-0.1.1.4/easyofd/
--rw-rw-rw-   0        0        0       41 2023-10-23 03:28:51.000000 easyofd-0.1.1.4/easyofd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:17:27.632338 easyofd-0.1.1.4/easyofd/draw/
--rw-rw-rw-   0        0        0      492 2023-10-31 09:09:18.000000 easyofd-0.1.1.4/easyofd/draw/__init__.py
--rw-rw-rw-   0        0        0     4746 2023-12-06 06:05:56.000000 easyofd-0.1.1.4/easyofd/draw/draw_ofd.py
--rw-rw-rw-   0        0        0    16089 2024-02-01 12:38:40.000000 easyofd-0.1.1.4/easyofd/draw/draw_pdf.py
--rw-rw-rw-   0        0        0     2974 2023-10-26 07:49:17.000000 easyofd-0.1.1.4/easyofd/draw/font_tools.py
--rw-rw-rw-   0        0        0    11957 2023-12-05 08:02:52.000000 easyofd-0.1.1.4/easyofd/draw/ofdtemplate.py
--rw-rw-rw-   0        0        0    33496 2023-10-31 09:01:30.000000 easyofd-0.1.1.4/easyofd/draw/pdf_parse.py
--rw-rw-rw-   0        0        0     3904 2023-11-17 02:43:10.000000 easyofd-0.1.1.4/easyofd/ofd.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:17:27.634348 easyofd-0.1.1.4/easyofd/parser_ofd/
--rw-rw-rw-   0        0        0     1021 2023-10-21 09:56:30.000000 easyofd-0.1.1.4/easyofd/parser_ofd/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-11-09 02:42:47.000000 easyofd-0.1.1.4/easyofd/parser_ofd/file_deal.py
--rw-rw-rw-   0        0        0    10238 2023-12-06 08:37:56.000000 easyofd-0.1.1.4/easyofd/parser_ofd/file_parser.py
--rw-rw-rw-   0        0        0    11119 2024-03-19 05:59:26.000000 easyofd-0.1.1.4/easyofd/parser_ofd/ofd_parser.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:17:27.630343 easyofd-0.1.1.4/easyofd.egg-info/
--rw-rw-rw-   0        0        0     1875 2024-03-19 06:17:27.000000 easyofd-0.1.1.4/easyofd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-03-19 06:17:27.000000 easyofd-0.1.1.4/easyofd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 06:17:27.000000 easyofd-0.1.1.4/easyofd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-03-19 06:17:27.000000 easyofd-0.1.1.4/easyofd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-19 06:17:27.000000 easyofd-0.1.1.4/easyofd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 06:17:27.658357 easyofd-0.1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1008 2024-03-19 06:17:25.000000 easyofd-0.1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:17:27.635330 easyofd-0.1.1.4/test/
--rw-rw-rw-   0        0        0      815 2023-10-26 06:35:50.000000 easyofd-0.1.1.4/test/test.py
--rw-rw-rw-   0        0        0     1282 2023-10-26 06:23:17.000000 easyofd-0.1.1.4/test/test_muty.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.624474 easyofd-0.1.1.5/
+-rw-rw-rw-   0        0        0    11550 2023-10-07 08:01:17.000000 easyofd-0.1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1875 2024-04-11 03:20:39.623472 easyofd-0.1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1439 2024-03-14 10:29:52.000000 easyofd-0.1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.381949 easyofd-0.1.1.5/easyofd/
+-rw-rw-rw-   0        0        0       41 2023-10-23 03:28:51.000000 easyofd-0.1.1.5/easyofd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.495237 easyofd-0.1.1.5/easyofd/draw/
+-rw-rw-rw-   0        0        0      492 2023-10-31 09:09:18.000000 easyofd-0.1.1.5/easyofd/draw/__init__.py
+-rw-rw-rw-   0        0        0     4746 2023-12-06 06:05:56.000000 easyofd-0.1.1.5/easyofd/draw/draw_ofd.py
+-rw-rw-rw-   0        0        0    16450 2024-04-11 03:18:54.000000 easyofd-0.1.1.5/easyofd/draw/draw_pdf.py
+-rw-rw-rw-   0        0        0     2974 2023-10-26 07:49:17.000000 easyofd-0.1.1.5/easyofd/draw/font_tools.py
+-rw-rw-rw-   0        0        0    11957 2023-12-05 08:02:52.000000 easyofd-0.1.1.5/easyofd/draw/ofdtemplate.py
+-rw-rw-rw-   0        0        0    33496 2023-10-31 09:01:30.000000 easyofd-0.1.1.5/easyofd/draw/pdf_parse.py
+-rw-rw-rw-   0        0        0     3904 2023-11-17 02:43:10.000000 easyofd-0.1.1.5/easyofd/ofd.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.599536 easyofd-0.1.1.5/easyofd/parser_ofd/
+-rw-rw-rw-   0        0        0     1021 2023-10-21 09:56:30.000000 easyofd-0.1.1.5/easyofd/parser_ofd/__init__.py
+-rw-rw-rw-   0        0        0     2963 2023-11-09 02:42:47.000000 easyofd-0.1.1.5/easyofd/parser_ofd/file_deal.py
+-rw-rw-rw-   0        0        0    10238 2023-12-06 08:37:56.000000 easyofd-0.1.1.5/easyofd/parser_ofd/file_parser.py
+-rw-rw-rw-   0        0        0    11119 2024-03-19 05:59:26.000000 easyofd-0.1.1.5/easyofd/parser_ofd/ofd_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.398907 easyofd-0.1.1.5/easyofd.egg-info/
+-rw-rw-rw-   0        0        0     1875 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 03:20:39.000000 easyofd-0.1.1.5/easyofd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 03:20:39.624474 easyofd-0.1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2024-04-11 03:19:40.000000 easyofd-0.1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:39.613500 easyofd-0.1.1.5/test/
+-rw-rw-rw-   0        0        0      815 2023-10-26 06:35:50.000000 easyofd-0.1.1.5/test/test.py
+-rw-rw-rw-   0        0        0     1282 2023-10-26 06:23:17.000000 easyofd-0.1.1.5/test/test_muty.py
```

### Comparing `easyofd-0.1.1.4/LICENSE` & `easyofd-0.1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/PKG-INFO` & `easyofd-0.1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyofd
-Version: 0.1.1.4
+Version: 0.1.1.5
 Summary: easy operate OFD
 Home-page: https://github.com/renoyuan/easyofd
 Author: renoyuan
 Author-email: renoyuan@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyofd-0.1.1.4/README.md` & `easyofd-0.1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/draw/draw_ofd.py` & `easyofd-0.1.1.5/easyofd/draw/draw_ofd.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/draw/draw_pdf.py` & `easyofd-0.1.1.5/easyofd/draw/draw_pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,38 +143,42 @@
             # 原点在页面的左下角 
             color = line_dict.get("color",[0,0,0])
             c.setFillColorRGB(int(color[0])/255,int(color[1])/255, int(color[2])/255)
             c.setStrokeColorRGB(int(color[0])/255,int(color[1])/255, int(color[2])/255)
             
             DeltaX = line_dict.get("DeltaX","")
             DeltaY = line_dict.get("DeltaY","")
+            # print("DeltaX",DeltaX)
             X = line_dict.get("X","")
             Y = line_dict.get("Y","")
-            CTM = line_dict.get("CTM","") # 因为ofd 的傻逼 增加这个字符缩放
+            CTM = line_dict.get("CTM","") # 因为ofd 增加这个字符缩放
             resizeX =1
             resizeY =1
+            # CTM =None # 有的数据不使用这个CTM
             if CTM :
                 resizeX = float(CTM.split(" ")[0])
                 resizeY = float(CTM.split(" ")[3])
         
             x_list = self.cmp_offset(line_dict.get("pos")[0], X, DeltaX, text, resizeX)
             y_list = self.cmp_offset(line_dict.get("pos")[1], Y, DeltaY, text, resizeY)
             
-
+            # print("x_list",x_list)
+            # print("y_list",y_list)
+            # print("Y",page_size[3])
+            # print("x",page_size[2])
             # if line_dict.get("Glyphs_d") and  FontFilePath.get(line_dict["font"])  and font_f not in FONTS:
             if False:  # 对于自定义字体 写入字形 drawPath 性能差暂时作废
                 Glyphs = [int(i) for i in line_dict.get("Glyphs_d").get("Glyphs").split(" ")]
                 for idx,Glyph_id in enumerate(Glyphs):
                     _cahr_x= float(x_list[idx])*self.OP
                     _cahr_y= (float(page_size[3])-(float(y_list[idx])))*self.OP
                     imageFile = draw_Glyph( FontFilePath.get(line_dict["font"]), Glyph_id,text[idx])
                     
                     # font_img_info.append((FontFilePath.get(line_dict["font"]), Glyph_id,text[idx],_cahr_x,_cahr_y,-line_dict["size"]*Op*2,line_dict["size"]*Op*2))
                     c.drawImage(imageFile,_cahr_x,_cahr_y,-line_dict["size"]*self.OP*2,line_dict["size"]*self.OP*2  )
-                    
             else:
                 if len(text) > len(x_list) or len(text) > len(y_list):
                     text = re.sub("[^\u4e00-\u9fa5]", "", text)
                 try:
                     # 按行写入  最后一个字符y  算出来大于 y轴  最后一个字符x  算出来大于 x轴 
                     if y_list[-1]*self.OP > page_size[3]*self.OP or x_list[-1]*self.OP > page_size[2]*self.OP or x_list[-1] < 0 or y_list[-1]<0 :
                         # print("line wtite")
@@ -183,16 +187,18 @@
                         c.drawString(x_p,  y_p, text, mode=0) # mode=3 文字不可见 0可見
                     
                         # text_write.append((x_p,  y_p, text))
                     # 按字符写入
                     else:
                         for cahr_id, _cahr_ in enumerate(text):
                             # print("char wtite")
+                            c.setFont(font, line_dict["size"] * self.OP *resizeX)
                             _cahr_x = float(x_list[cahr_id])*self.OP
                             _cahr_y = (float(page_size[3])-(float(y_list[cahr_id])))*self.OP
+                            print(_cahr_x,  _cahr_y, _cahr_)
                             c.drawString(_cahr_x,  _cahr_y, _cahr_, mode=0)  # mode=3 文字不可见 0可見
                         
                             # text_write.append((_cahr_x,  _cahr_y, _cahr_))
                     
                 except Exception as e:
                     logger.error(f"{e}")
                     traceback.print_exc()
```

### Comparing `easyofd-0.1.1.4/easyofd/draw/font_tools.py` & `easyofd-0.1.1.5/easyofd/draw/font_tools.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/draw/ofdtemplate.py` & `easyofd-0.1.1.5/easyofd/draw/ofdtemplate.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/draw/pdf_parse.py` & `easyofd-0.1.1.5/easyofd/draw/pdf_parse.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/ofd.py` & `easyofd-0.1.1.5/easyofd/ofd.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/parser_ofd/__init__.py` & `easyofd-0.1.1.5/easyofd/parser_ofd/__init__.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/parser_ofd/file_deal.py` & `easyofd-0.1.1.5/easyofd/parser_ofd/file_deal.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/parser_ofd/file_parser.py` & `easyofd-0.1.1.5/easyofd/parser_ofd/file_parser.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd/parser_ofd/ofd_parser.py` & `easyofd-0.1.1.5/easyofd/parser_ofd/ofd_parser.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/easyofd.egg-info/PKG-INFO` & `easyofd-0.1.1.5/easyofd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyofd
-Version: 0.1.1.4
+Version: 0.1.1.5
 Summary: easy operate OFD
 Home-page: https://github.com/renoyuan/easyofd
 Author: renoyuan
 Author-email: renoyuan@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyofd-0.1.1.4/easyofd.egg-info/SOURCES.txt` & `easyofd-0.1.1.5/easyofd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/setup.py` & `easyofd-0.1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="easyofd", 
-    version="0.1.1.4",
+    version="0.1.1.5",
     author="renoyuan",    
     author_email="renoyuan@foxmail.com",    
     description="easy operate OFD",
     long_description=long_description,   
     long_description_content_type="text/markdown",
     url="https://github.com/renoyuan/easyofd",    
     packages=setuptools.find_packages(exclude=["README.md",".vscode", ".vscode.*", ".git", ".git.*"]),
```

### Comparing `easyofd-0.1.1.4/test/test.py` & `easyofd-0.1.1.5/test/test.py`

 * *Files identical despite different names*

### Comparing `easyofd-0.1.1.4/test/test_muty.py` & `easyofd-0.1.1.5/test/test_muty.py`

 * *Files identical despite different names*

