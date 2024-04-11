# Comparing `tmp/tell_me_again-0.1.1.tar.gz` & `tmp/tell_me_again-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tell_me_again-0.1.1.tar", max compression
+gzip compressed data, was "tell_me_again-0.1.2.tar", max compression
```

## Comparing `tell_me_again-0.1.1.tar` & `tell_me_again-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1334 2024-03-07 20:03:05.013756 tell_me_again-0.1.1/README.md
--rw-r--r--   0        0        0      544 2024-03-12 16:14:18.871085 tell_me_again-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       75 2024-01-31 15:05:29.848817 tell_me_again-0.1.1/tell_me_again/__init__.py
--rw-r--r--   0        0        0    15967 2024-03-12 16:11:35.645503 tell_me_again-0.1.1/tell_me_again/dataset.py
--rw-r--r--   0        0        0      816 2024-03-12 16:11:35.642169 tell_me_again-0.1.1/tell_me_again/util.py
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 tell_me_again-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1483 2024-04-11 17:43:05.293971 tell_me_again-0.1.2/README.md
+-rw-r--r--   0        0        0      544 2024-04-11 17:45:17.839012 tell_me_again-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-01-31 15:05:29.848817 tell_me_again-0.1.2/tell_me_again/__init__.py
+-rw-r--r--   0        0        0    15960 2024-04-11 17:43:05.293971 tell_me_again-0.1.2/tell_me_again/dataset.py
+-rw-r--r--   0        0        0      816 2024-03-12 16:11:35.642169 tell_me_again-0.1.2/tell_me_again/util.py
+-rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 tell_me_again-0.1.2/PKG-INFO
```

### Comparing `tell_me_again-0.1.1/README.md` & `tell_me_again-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Tell me again!
 
 A dataset of multiple summaries for the same story.
 
 The summaries are scraped from Wikipedia and come in various languages.
 We also provide automatically created translation and anonymized versions of the summaries (without identifiable names).
+For further details, check out the corresponding paper [here](https://www.inf.uni-hamburg.de/en/inst/ab/lt/publications/2024-hatzel-et-al-lrec.pdf).
 
 
 When using this dataset please cite the following paper:
 ```
 @inproceedings{hatzel-etal-2024-tellme,
     title = "Tell me again! A Large-Scale Dataset of Multiple Summaries for the Same Story"
     booktitle = "Proceedings of the Forteenth Language Resources and Evaluation Conference",
```

### Comparing `tell_me_again-0.1.1/pyproject.toml` & `tell_me_again-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tell-me-again"
-version = "0.1.1"
+version = "0.1.2"
 description = "Dataset for the paper 'Tell me again! A Large-Scale Dataset of Multiple Summaries for the"
 authors = ["Same Story"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tell_me_again-0.1.1/tell_me_again/dataset.py` & `tell_me_again-0.1.2/tell_me_again/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,17 +226,16 @@
 
     def __len__(self):
         return len(self.stories)
 
     def perform_splits(self):
         split_ids = {}
         for split in ["train", "dev", "test"]:
-            in_file = open(
-                self.data_path / Path(split + "_stories.csv")
-            )  # TODO: fix path
+            zip_file = zipfile.ZipFile(self.data_path)
+            in_file = zip_file.open(split + "_stories.csv")
             split_ids[split] = [l.strip() for l in in_file.readlines()]
         train_stories = {k: self.stories[k] for k in split_ids["train"]}
         dev_stories = {k: self.stories[k] for k in split_ids["dev"]}
         test_stories = {k: self.stories[k] for k in split_ids["test"]}
         return {
             k: self.__class__(data_path=None, stories=s)
             for k, s in [
```

### Comparing `tell_me_again-0.1.1/tell_me_again/util.py` & `tell_me_again-0.1.2/tell_me_again/util.py`

 * *Files identical despite different names*

### Comparing `tell_me_again-0.1.1/PKG-INFO` & `tell_me_again-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tell-me-again
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dataset for the paper 'Tell me again! A Large-Scale Dataset of Multiple Summaries for the
 License: MIT
 Author: Same Story
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -17,14 +17,15 @@
 
 # Tell me again!
 
 A dataset of multiple summaries for the same story.
 
 The summaries are scraped from Wikipedia and come in various languages.
 We also provide automatically created translation and anonymized versions of the summaries (without identifiable names).
+For further details, check out the corresponding paper [here](https://www.inf.uni-hamburg.de/en/inst/ab/lt/publications/2024-hatzel-et-al-lrec.pdf).
 
 
 When using this dataset please cite the following paper:
 ```
 @inproceedings{hatzel-etal-2024-tellme,
     title = "Tell me again! A Large-Scale Dataset of Multiple Summaries for the Same Story"
     booktitle = "Proceedings of the Forteenth Language Resources and Evaluation Conference",
```

