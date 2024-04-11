# Comparing `tmp/Antares_Launcher-1.3.2.tar.gz` & `tmp/Antares_Launcher-1.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Antares_Launcher-1.3.2.tar", last modified: Thu Apr 11 17:20:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

