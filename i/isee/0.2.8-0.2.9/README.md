# Comparing `tmp/isee-0.2.8.tar.gz` & `tmp/isee-0.2.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isee-0.2.8.tar", last modified: Thu Feb 29 13:41:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

