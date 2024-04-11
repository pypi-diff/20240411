# Comparing `tmp/mapper_parser-1.0.tar.gz` & `tmp/mapper_parser-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapper_parser-1.0.tar", last modified: Mon Apr  8 05:17:19 2024, max compression
+gzip compressed data, was "mapper_parser-1.1.tar", last modified: Thu Apr 11 01:56:50 2024, max compression
```

## Comparing `mapper_parser-1.0.tar` & `mapper_parser-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.795507 mapper_parser-1.0/
--rw-rw-rw-   0        0        0     1016 2024-04-08 05:17:19.794507 mapper_parser-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-08-04 08:07:08.000000 mapper_parser-1.0/README.md
--rw-rw-rw-   0        0        0      642 2024-04-08 05:16:59.000000 mapper_parser-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 05:17:19.795507 mapper_parser-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.778506 mapper_parser-1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.783507 mapper_parser-1.0/src/mapper_parser/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 mapper_parser-1.0/src/mapper_parser/__init__.py
--rw-rw-rw-   0        0        0     4270 2024-04-08 05:16:00.000000 mapper_parser-1.0/src/mapper_parser/mapper_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-08 05:17:19.792509 mapper_parser-1.0/src/mapper_parser.egg-info/
--rw-rw-rw-   0        0        0     1016 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-08 05:17:19.000000 mapper_parser-1.0/src/mapper_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 01:56:50.608038 mapper_parser-1.1/
+-rw-rw-rw-   0        0        0     1016 2024-04-11 01:56:50.606039 mapper_parser-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-08-04 08:07:08.000000 mapper_parser-1.1/README.md
+-rw-rw-rw-   0        0        0      642 2024-04-11 01:54:50.000000 mapper_parser-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 01:56:50.608038 mapper_parser-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 01:56:50.593044 mapper_parser-1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 01:56:50.598038 mapper_parser-1.1/src/mapper_parser/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 mapper_parser-1.1/src/mapper_parser/__init__.py
+-rw-rw-rw-   0        0        0     4415 2024-04-11 01:55:59.000000 mapper_parser-1.1/src/mapper_parser/mapper_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:56:50.605039 mapper_parser-1.1/src/mapper_parser.egg-info/
+-rw-rw-rw-   0        0        0     1016 2024-04-11 01:56:50.000000 mapper_parser-1.1/src/mapper_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-04-11 01:56:50.000000 mapper_parser-1.1/src/mapper_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 01:56:50.000000 mapper_parser-1.1/src/mapper_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 01:56:50.000000 mapper_parser-1.1/src/mapper_parser.egg-info/top_level.txt
```

### Comparing `mapper_parser-1.0/PKG-INFO` & `mapper_parser-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapper_parser
-Version: 1.0
+Version: 1.1
 Summary: Mybatis mapper xml file parser
 Author-email: Oliver Li <441640312@qq.com>
 Project-URL: Homepage, https://github.com/baikaishuipp/mapper-parser
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/mapper-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mapper_parser-1.0/pyproject.toml` & `mapper_parser-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapper_parser"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Mybatis mapper xml file parser"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.0"
```

### Comparing `mapper_parser-1.0/src/mapper_parser/mapper_parser.py` & `mapper_parser-1.1/src/mapper_parser/mapper_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,20 @@
     match = re.search(pattern, string)
     if match:
         value = match.group(1)
         return value
     else:
         return None
 
+def check_string(tag, id_str, string):
+    pattern = r'^' + tag + '.*?id\s*=\s*"' + id_str + '"'
+    match = re.search(pattern, string)
+    return bool(match)
+
+
 def parse(filepath):
     # 读取XML文件内容
     with open(filepath, "r", encoding="utf-8") as file:
         xml_content = file.read()
 
     # 解析XML文件
     tree = ET.ElementTree(ET.fromstring(xml_content))
@@ -56,29 +62,29 @@
 
     # 获取resultMap的id以及起始行号和截止行号
     for element in root.findall(".//resultMap"):
         result_map_id = element.attrib["id"]
         start_line = 0
         end_line = 0
         for i, line in enumerate(xml_content.splitlines(), start=1):
-            if line.strip().startswith('<resultMap') and f'id="{result_map_id}"' in line:
+            if check_string('<resultMap', result_map_id, line.strip()):
                 start_line = i
             if f'</resultMap>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         result_map_info.append(MapperElement(result_map_id, 'resultMap', start_line, end_line, content))
 
     # 获取resultMap的id以及起始行号和截止行号
     for sql_element in root.findall(".//sql"):
         sql_id = sql_element.attrib["id"]
         start_line = 0
         end_line = 0
         for i, line in enumerate(xml_content.splitlines(), start=1):
-            if line.strip().startswith('<sql') and f'id="{sql_id}"' in line:
+            if check_string('<sql', sql_id, line.strip()):
                 start_line = i
             if f'</sql>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         sql_info.append(MapperElement(sql_id, 'sql', start_line, end_line, content))
 
@@ -87,15 +93,15 @@
     for statement_element in statements:
         statement_id = statement_element.attrib["id"]
         start_line = 0
         end_line = 0
         result_map = None
         include_sql = None
         for i, line in enumerate(xml_content.splitlines(), start=1):
-            if f'<{statement_element.tag} id="{statement_id}"' in line:
+            if check_string('<' + statement_element.tag, statement_id, line.strip()):
                 start_line = i
             if f'resultMap="' in line and start_line != 0:
                 result_map = extract_value(line, 'resultMap')
             if line.strip().startswith('<include') and start_line != 0:
                 include_sql = extract_value(line, 'refid')
             if f'</{statement_element.tag}>' in line and start_line != 0:
                 end_line = i
```

### Comparing `mapper_parser-1.0/src/mapper_parser.egg-info/PKG-INFO` & `mapper_parser-1.1/src/mapper_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapper_parser
-Version: 1.0
+Version: 1.1
 Summary: Mybatis mapper xml file parser
 Author-email: Oliver Li <441640312@qq.com>
 Project-URL: Homepage, https://github.com/baikaishuipp/mapper-parser
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/mapper-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

