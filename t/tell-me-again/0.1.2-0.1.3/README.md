# Comparing `tmp/tell_me_again-0.1.2.tar.gz` & `tmp/tell_me_again-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tell_me_again-0.1.2.tar", max compression
+gzip compressed data, was "tell_me_again-0.1.3.tar", max compression
```

## Comparing `tell_me_again-0.1.2.tar` & `tell_me_again-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1483 2024-04-11 17:43:05.293971 tell_me_again-0.1.2/README.md
--rw-r--r--   0        0        0      544 2024-04-11 17:45:17.839012 tell_me_again-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       75 2024-01-31 15:05:29.848817 tell_me_again-0.1.2/tell_me_again/__init__.py
--rw-r--r--   0        0        0    15960 2024-04-11 17:43:05.293971 tell_me_again-0.1.2/tell_me_again/dataset.py
--rw-r--r--   0        0        0      816 2024-03-12 16:11:35.642169 tell_me_again-0.1.2/tell_me_again/util.py
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 tell_me_again-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1483 2024-04-11 17:43:05.293971 tell_me_again-0.1.3/README.md
+-rw-r--r--   0        0        0      544 2024-04-11 17:55:33.566951 tell_me_again-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-01-31 15:05:29.848817 tell_me_again-0.1.3/tell_me_again/__init__.py
+-rw-r--r--   0        0        0    15976 2024-04-11 17:53:50.062283 tell_me_again-0.1.3/tell_me_again/dataset.py
+-rw-r--r--   0        0        0      816 2024-03-12 16:11:35.642169 tell_me_again-0.1.3/tell_me_again/util.py
+-rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 tell_me_again-0.1.3/PKG-INFO
```

### Comparing `tell_me_again-0.1.2/README.md` & `tell_me_again-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tell_me_again-0.1.2/pyproject.toml` & `tell_me_again-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tell-me-again"
-version = "0.1.2"
+version = "0.1.3"
 description = "Dataset for the paper 'Tell me again! A Large-Scale Dataset of Multiple Summaries for the"
 authors = ["Same Story"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tell_me_again-0.1.2/tell_me_again/dataset.py` & `tell_me_again-0.1.3/tell_me_again/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         return len(self.stories)
 
     def perform_splits(self):
         split_ids = {}
         for split in ["train", "dev", "test"]:
             zip_file = zipfile.ZipFile(self.data_path)
             in_file = zip_file.open(split + "_stories.csv")
-            split_ids[split] = [l.strip() for l in in_file.readlines()]
+            split_ids[split] = [l.decode("utf-8").strip() for l in in_file.readlines()]
         train_stories = {k: self.stories[k] for k in split_ids["train"]}
         dev_stories = {k: self.stories[k] for k in split_ids["dev"]}
         test_stories = {k: self.stories[k] for k in split_ids["test"]}
         return {
             k: self.__class__(data_path=None, stories=s)
             for k, s in [
                 ("train", train_stories),
```

### Comparing `tell_me_again-0.1.2/tell_me_again/util.py` & `tell_me_again-0.1.3/tell_me_again/util.py`

 * *Files identical despite different names*

### Comparing `tell_me_again-0.1.2/PKG-INFO` & `tell_me_again-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tell-me-again
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dataset for the paper 'Tell me again! A Large-Scale Dataset of Multiple Summaries for the
 License: MIT
 Author: Same Story
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

