# Comparing `tmp/arcor2_execution-1.2.0.tar.gz` & `tmp/arcor2_execution-1.3.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_execution-1.2.0.tar", last modified: Wed Jan  3 13:03:08 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

