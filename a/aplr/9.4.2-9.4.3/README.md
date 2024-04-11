# Comparing `tmp/aplr-9.4.2.tar.gz` & `tmp/aplr-9.4.3-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplr-9.4.2.tar", last modified: Thu Mar 14 16:59:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

