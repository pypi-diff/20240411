# Comparing `tmp/arcor2_fit_demo-1.2.0.tar.gz` & `tmp/arcor2_fit_demo-1.5.0-py311-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_fit_demo-1.2.0.tar", last modified: Thu Jul 20 11:09:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

