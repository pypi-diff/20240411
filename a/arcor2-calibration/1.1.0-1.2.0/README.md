# Comparing `tmp/arcor2_calibration-1.1.0.tar.gz` & `tmp/arcor2_calibration-1.2.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_calibration-1.1.0.tar", last modified: Wed Feb  7 11:55:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

