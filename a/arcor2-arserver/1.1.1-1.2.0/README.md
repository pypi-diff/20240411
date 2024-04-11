# Comparing `tmp/arcor2_arserver-1.1.1.tar.gz` & `tmp/arcor2_arserver-1.2.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_arserver-1.1.1.tar", last modified: Tue Jan 23 12:49:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

