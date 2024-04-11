# Comparing `tmp/python-mecab-ko-1.3.3.tar.gz` & `tmp/python_mecab_ko-1.3.5-cp39-cp39-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mecab-ko-1.3.3.tar", last modified: Fri Dec 30 07:19:48 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

