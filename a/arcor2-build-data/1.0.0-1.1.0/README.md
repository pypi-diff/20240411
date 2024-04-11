# Comparing `tmp/arcor2_build_data-1.0.0.tar.gz` & `tmp/arcor2_build_data-1.1.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_build_data-1.0.0.tar", last modified: Tue Feb 14 12:55:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

