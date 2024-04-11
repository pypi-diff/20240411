# Comparing `tmp/ast_grep_py-0.20.4.tar.gz` & `tmp/ast_grep_py-0.20.5-cp311-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

