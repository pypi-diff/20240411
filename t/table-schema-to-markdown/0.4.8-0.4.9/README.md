# Comparing `tmp/table_schema_to_markdown-0.4.8-py3-none-any.whl.zip` & `tmp/table_schema_to_markdown-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 8523 bytes, number of entries: 7
--rw-r--r--  2.0 unx    13802 b- defN 24-Apr-08 09:36 table_schema_to_markdown/__init__.py
--rwxr-xr-x  2.0 unx     1056 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md
--rw-r--r--  2.0 unx     1072 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     5402 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/WHEEL
--rwxr--r--  2.0 unx       25 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      684 b- defN 24-Apr-08 09:45 table_schema_to_markdown-0.4.8.dist-info/RECORD
-7 files, 22133 bytes uncompressed, 7285 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx    13824 b- defN 24-Apr-09 11:40 table_schema_to_markdown/__init__.py
+-rwxr-xr-x  2.0 unx     1056 b- defN 24-Apr-09 11:40 table_schema_to_markdown-0.4.9.data/scripts/table-schema-to-md
+-rw-r--r--  2.0 unx     1072 b- defN 24-Apr-09 11:40 table_schema_to_markdown-0.4.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5402 b- defN 24-Apr-09 11:40 table_schema_to_markdown-0.4.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 11:40 table_schema_to_markdown-0.4.9.dist-info/WHEEL
+-rwxr--r--  2.0 unx       25 b- defN 24-Apr-09 11:40 table_schema_to_markdown-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      684 b- defN 24-Apr-09 11:40 table_schema_to_markdown-0.4.9.dist-info/RECORD
+7 files, 22155 bytes uncompressed, 7285 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: table_schema_to_markdown/__init__.py
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md
+Filename: table_schema_to_markdown-0.4.9.data/scripts/table-schema-to-md
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.8.dist-info/LICENSE
+Filename: table_schema_to_markdown-0.4.9.dist-info/LICENSE
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.8.dist-info/METADATA
+Filename: table_schema_to_markdown-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.8.dist-info/WHEEL
+Filename: table_schema_to_markdown-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.8.dist-info/top_level.txt
+Filename: table_schema_to_markdown-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: table_schema_to_markdown-0.4.8.dist-info/RECORD
+Filename: table_schema_to_markdown-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## table_schema_to_markdown/__init__.py

```diff
@@ -402,16 +402,16 @@
                 if len(listenums) > 0:
                     out_fd.write("\n- Valeurs autorisées : ")
                     for enum in listenums:
                         # to prevent weird display due
                         # to markdown quoting mechanism
                         out_fd.write(
                             "\n    - {}".format(
-                                enum if not enum.startswith(">")
-                                else "\\" + enum
+                                "\\" + enum if isinstance(enum, str) and enum.startswith(">")
+                                else enum
                             )
                         )
                 if intervals != "":
                     out_fd.write(f"\n- {intervals}")
                 if sizes != "":
                     out_fd.write(f"\n- {sizes}")
                 if pattern != "":
```

## Comparing `table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md` & `table_schema_to_markdown-0.4.9.data/scripts/table-schema-to-md`

 * *Files identical despite different names*

## Comparing `table_schema_to_markdown-0.4.8.dist-info/LICENSE` & `table_schema_to_markdown-0.4.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `table_schema_to_markdown-0.4.8.dist-info/METADATA` & `table_schema_to_markdown-0.4.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: table-schema-to-markdown
-Version: 0.4.8
+Version: 0.4.9
 Summary: Generate Markdown documentation from a table schema file from Frictionless Data
 Home-page: https://github.com/geoffreyaldebert/table-schema-to-markdown
 Author: Antoine Augusti, Geoffrey Aldebert
 Author-email: hi@antoine-augusti.fr, geoffrey.aldebert@data.gouv.fr
 License: MIT
 Keywords: frictionlessdata,documentation,tableschema,table-schema,frictionless data,open data,json schema,json table schema,data package,tabular data package
 Platform: UNKNOWN
```

## Comparing `table_schema_to_markdown-0.4.8.dist-info/RECORD` & `table_schema_to_markdown-0.4.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-table_schema_to_markdown/__init__.py,sha256=Qq0avn1hX81N6zInMdpqScm4Ncr2-uaSBGsz_EryjX4,13802
-table_schema_to_markdown-0.4.8.data/scripts/table-schema-to-md,sha256=c2IgvuLFUBBrwY8LxvO9GrADX6ZIT5-_SVW8-0iErwU,1056
-table_schema_to_markdown-0.4.8.dist-info/LICENSE,sha256=qV08noOLMZNHkulCB6KzZKm-aPGZjbP-sYJqmz2dUeM,1072
-table_schema_to_markdown-0.4.8.dist-info/METADATA,sha256=x2zeKQKdOrpep7yAra_k3cbq5rUUvlMmczmgqQlDBcU,5402
-table_schema_to_markdown-0.4.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-table_schema_to_markdown-0.4.8.dist-info/top_level.txt,sha256=jsrAX2CW2-lFIx28kPUYPlwep72sLHxmjd13pvAHS-c,25
-table_schema_to_markdown-0.4.8.dist-info/RECORD,,
+table_schema_to_markdown/__init__.py,sha256=kML8j9y-xym4tblpSULn9Z7lNcIwhMLr5FJA-N8wqCg,13824
+table_schema_to_markdown-0.4.9.data/scripts/table-schema-to-md,sha256=c2IgvuLFUBBrwY8LxvO9GrADX6ZIT5-_SVW8-0iErwU,1056
+table_schema_to_markdown-0.4.9.dist-info/LICENSE,sha256=qV08noOLMZNHkulCB6KzZKm-aPGZjbP-sYJqmz2dUeM,1072
+table_schema_to_markdown-0.4.9.dist-info/METADATA,sha256=hbK-ukuXXNrY8S2rAjsxRsJ3gSElsrhB4mvdU_GBnw0,5402
+table_schema_to_markdown-0.4.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+table_schema_to_markdown-0.4.9.dist-info/top_level.txt,sha256=jsrAX2CW2-lFIx28kPUYPlwep72sLHxmjd13pvAHS-c,25
+table_schema_to_markdown-0.4.9.dist-info/RECORD,,
```

