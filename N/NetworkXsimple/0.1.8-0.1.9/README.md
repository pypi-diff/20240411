# Comparing `tmp/NetworkXsimple-0.1.8.tar.gz` & `tmp/NetworkXsimple-0.1.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetworkXsimple-0.1.8.tar", last modified: Wed Apr 10 11:24:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

