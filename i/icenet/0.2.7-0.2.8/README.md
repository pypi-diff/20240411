# Comparing `tmp/icenet-0.2.7.tar.gz` & `tmp/icenet-0.2.8-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jambyr/code/ai-lab/icenet/icenet/dist/.tmp-062siymy/icenet-0.2.7.tar", last modified: Sat Jan 20 12:48:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

