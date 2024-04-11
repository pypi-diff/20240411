# Comparing `tmp/five_strips_of_bacon-0.1.2.tar.gz` & `tmp/five_strips_of_bacon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_strips_of_bacon-0.1.2.tar", max compression
+gzip compressed data, was "five_strips_of_bacon-0.1.4.tar", max compression
```

## Comparing `five_strips_of_bacon-0.1.2.tar` & `five_strips_of_bacon-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1118 2024-04-09 18:02:12.474693 five_strips_of_bacon-0.1.2/README.md
--rw-r--r--   0        0        0      552 2024-04-11 02:01:58.318511 five_strips_of_bacon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2256 2023-10-20 03:40:16.732000 five_strips_of_bacon-0.1.2/src/bacon.py
--rw-r--r--   0        0        0     2866 2024-04-09 18:08:34.450000 five_strips_of_bacon-0.1.2/src/decode_five_strips_of_bacon.py
--rw-r--r--   0        0        0     7878 2024-04-11 01:35:20.243192 five_strips_of_bacon-0.1.2/src/main.py
--rw-r--r--   0        0        0    29094 2024-03-08 05:34:01.619000 five_strips_of_bacon-0.1.2/src/resources/bacon_five.png
--rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 five_strips_of_bacon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1118 2024-04-09 18:02:12.474693 five_strips_of_bacon-0.1.4/README.md
+-rw-r--r--   0        0        0      636 2024-04-11 03:29:00.914683 five_strips_of_bacon-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2256 2023-10-20 03:40:16.732000 five_strips_of_bacon-0.1.4/src/bacon.py
+-rw-r--r--   0        0        0     2866 2024-04-09 18:08:34.450000 five_strips_of_bacon-0.1.4/src/decode_five_strips_of_bacon.py
+-rw-r--r--   0        0        0     7954 2024-04-11 03:25:02.307806 five_strips_of_bacon-0.1.4/src/main.py
+-rw-r--r--   0        0        0    29094 2024-03-08 05:34:01.619000 five_strips_of_bacon-0.1.4/src/resources/bacon_five.png
+-rw-r--r--   0        0        0     1762 1970-01-01 00:00:00.000000 five_strips_of_bacon-0.1.4/PKG-INFO
```

### Comparing `five_strips_of_bacon-0.1.2/README.md` & `five_strips_of_bacon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.2/pyproject.toml` & `five_strips_of_bacon-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "five-strips-of-bacon"
-version = "0.1.2"
-description = ""
+version = "0.1.4"
+description = "Encode/Decode messages using five simultaneous bacon ciphers."
 authors = ["Odyhibit <josh.2990@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "src/main.py"},
     { include = "src/bacon.py"},
     { include = "src/decode_five_strips_of_bacon.py"},
-    { include = "src/resources/*"},
+    { include = "bacon_five.png", from="src/resources"},
 ]
 
+
+
 [tool.poetry.dependencies]
 python = "^3.8"
 customtkinter = "^5.2.2"
 pillow = "^10.3.0"
 
 [tool.poetry.scripts]
 five-strips-of-bacon = "src.main:main"
```

### Comparing `five_strips_of_bacon-0.1.2/src/bacon.py` & `five_strips_of_bacon-0.1.4/src/bacon.py`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.2/src/decode_five_strips_of_bacon.py` & `five_strips_of_bacon-0.1.4/src/decode_five_strips_of_bacon.py`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.2/src/main.py` & `five_strips_of_bacon-0.1.4/src/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 class MainWindow:
 
     def __init__(self, root):
 
         tabcontrol = CTkTabview(root)
         tabcontrol.pack(expand=True)
-        #icon_path = ImageTk.PhotoImage(file="resources/bacon_five.png")
-        #root.wm_iconbitmap()
-        #root.iconphoto(False, icon_path)
+        icon_path = ImageTk.PhotoImage(file="five-strips-of-bacon/src/resources/bacon_five.png")
+        root.wm_iconbitmap()
+        root.iconphoto(False, icon_path)
         root.title("Five Strips of Bacon")
         tabcontrol.pack(padx=20, pady=20)
         tabcontrol.add("Encode")
         tabcontrol.add("Decode")
 
         def convert_hidden(e):
             temp = hidden_text.get("1.0", "end-1c").upper()
@@ -38,17 +38,17 @@
             hidden_str = hidden_text.get("1.0", "end-1c").replace(" ", "")
             cover = 0
             for letter in cover_str:
                 if letter.isalpha():
                     cover += 1
             # print("cover:", cover, "len(hidden):", len(hidden_str))
             if cover >= len(hidden_str):
-                calc_button.configure(state="normal")
+                calc_button.configure(state="normal", text="Calculate cipher")
             else:
-                calc_button.configure(state="disabled")
+                calc_button.configure(state="disabled", text="Need more cover text")
 
         def calculate_cipher():
             # BISCUT Bold Italic Strikethrough Capital Underline - Text
             word_joiner = "\u2060"
             no_break_space = "\ufeff"
             hidden_str = hidden_text.get("1.0", "end-1c")
             secret_bin_str = bacon.get_bit_mask(hidden_text.get("1.0", "end -1c").lower(),
```

### Comparing `five_strips_of_bacon-0.1.2/src/resources/bacon_five.png` & `five_strips_of_bacon-0.1.4/src/resources/bacon_five.png`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.2/PKG-INFO` & `five_strips_of_bacon-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: five-strips-of-bacon
-Version: 0.1.2
-Summary: 
+Version: 0.1.4
+Summary: Encode/Decode messages using five simultaneous bacon ciphers.
 Author: Odyhibit
 Author-email: josh.2990@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

