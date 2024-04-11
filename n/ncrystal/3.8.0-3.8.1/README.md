# Comparing `tmp/ncrystal-3.8.0.tar.gz` & `tmp/ncrystal-3.8.1-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncrystal-3.8.0.tar", last modified: Sun Dec  3 13:31:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

