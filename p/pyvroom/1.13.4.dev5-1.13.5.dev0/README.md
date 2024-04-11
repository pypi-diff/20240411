# Comparing `tmp/pyvroom-1.13.4.dev5.tar.gz` & `tmp/pyvroom-1.13.5.dev0-cp39-cp39-manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvroom-1.13.4.dev5.tar", last modified: Thu Feb 15 13:59:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

