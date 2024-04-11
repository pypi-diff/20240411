# Comparing `tmp/geohaye-0.0.1.tar.gz` & `tmp/geohaye-0.0.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geohaye-0.0.1.tar", last modified: Mon Feb 19 18:32:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

