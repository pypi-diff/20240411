# Comparing `tmp/arcor2_build-1.3.1.tar.gz` & `tmp/arcor2_build-1.4.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_build-1.3.1.tar", last modified: Tue Jan 30 14:59:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

