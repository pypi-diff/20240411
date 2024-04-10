# Comparing `tmp/gattlib-py-0.6.0.tar.gz` & `tmp/gattlib_py-0.7.0-cp37-cp37m-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattlib-py-0.6.0.tar", last modified: Sun Apr  7 22:52:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

