# Comparing `tmp/arcor2_fanuc-0.3.0.tar.gz` & `tmp/arcor2_fanuc-0.4.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_fanuc-0.3.0.tar", last modified: Fri Oct 28 16:08:25 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

