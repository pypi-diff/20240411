# Comparing `tmp/software_development_project_team1-0.1.0.tar.gz` & `tmp/software_development_project_team1-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "software_development_project_team1-0.1.0.tar", last modified: Thu Apr 11 16:35:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

