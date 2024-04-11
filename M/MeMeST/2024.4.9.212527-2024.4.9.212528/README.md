# Comparing `tmp/MeMeST-2024.4.9.212527.tar.gz` & `tmp/MeMeST-2024.4.9.212528-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeMeST-2024.4.9.212527.tar", last modified: Tue Apr  9 13:25:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

