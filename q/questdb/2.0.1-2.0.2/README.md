# Comparing `tmp/questdb-2.0.1.tar.gz` & `tmp/questdb-2.0.2-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-2.0.1.tar", last modified: Thu Apr  4 14:16:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

