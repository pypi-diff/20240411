# Comparing `tmp/libcom-0.0.1.post9.tar.gz` & `tmp/libcom-0.0.2-cp38-cp38-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libcom-0.0.1.post9.tar", last modified: Thu Jan 25 01:31:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

