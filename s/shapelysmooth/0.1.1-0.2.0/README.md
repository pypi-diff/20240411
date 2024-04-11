# Comparing `tmp/shapelysmooth-0.1.1.tar.gz` & `tmp/shapelysmooth-0.2.0-pp310-pypy310_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelysmooth-0.1.1.tar", last modified: Tue Jan 24 11:34:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

