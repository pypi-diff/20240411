# Comparing `tmp/tiny-match-snapshot-0.0.1.tar.gz` & `tmp/tiny-match-snapshot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny-match-snapshot-0.0.1.tar", last modified: Tue Apr  2 01:47:49 2024, max compression
+gzip compressed data, was "tiny-match-snapshot-0.0.2.tar", last modified: Wed Apr 10 22:51:02 2024, max compression
```

## Comparing `tiny-match-snapshot-0.0.1.tar` & `tiny-match-snapshot-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:47:49.017902 tiny-match-snapshot-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 01:47:44.000000 tiny-match-snapshot-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 01:47:44.000000 tiny-match-snapshot-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-02 01:47:49.017902 tiny-match-snapshot-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:47:49.017902 tiny-match-snapshot-0.0.1/match_snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-02 01:47:44.000000 tiny-match-snapshot-0.0.1/match_snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-02 01:47:44.000000 tiny-match-snapshot-0.0.1/match_snapshot/match_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-02 01:47:44.000000 tiny-match-snapshot-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:47:49.017902 tiny-match-snapshot-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:47:49.017902 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-02 01:47:49.000000 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 01:47:49.000000 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:47:49.000000 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:47:48.000000 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 01:47:49.000000 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 01:47:49.000000 tiny-match-snapshot-0.0.1/tiny_match_snapshot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:51:02.829337 tiny-match-snapshot-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 22:50:58.000000 tiny-match-snapshot-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 22:50:58.000000 tiny-match-snapshot-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-10 22:51:02.829337 tiny-match-snapshot-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-10 22:50:58.000000 tiny-match-snapshot-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:51:02.825337 tiny-match-snapshot-0.0.2/match_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 22:50:58.000000 tiny-match-snapshot-0.0.2/match_snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-10 22:50:58.000000 tiny-match-snapshot-0.0.2/match_snapshot/match_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 22:50:58.000000 tiny-match-snapshot-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:51:02.829337 tiny-match-snapshot-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:51:02.829337 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-10 22:51:02.000000 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 22:51:02.000000 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:51:02.000000 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:51:02.000000 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 22:51:02.000000 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 22:51:02.000000 tiny-match-snapshot-0.0.2/tiny_match_snapshot.egg-info/top_level.txt
```

### Comparing `tiny-match-snapshot-0.0.1/LICENSE` & `tiny-match-snapshot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny-match-snapshot-0.0.1/match_snapshot/match_snapshot.py` & `tiny-match-snapshot-0.0.2/match_snapshot/match_snapshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,25 +128,38 @@
 
         Args:
             id: a unique id to gets the file name.
             image_type: a image type to gets the file name.
         """
         return os.path.join(self.failed_path, f"{id}/{image_type}.png")
 
+    def _grant_error_path_exists(self, id: str):
+        """
+        Check if the error path exists and if not, create it.
+
+        Args:
+            id: a unique id to gets the path name.
+        """
+        error_path = os.path.join(self.failed_path, id)
+        if not os.path.exists(error_path):
+            os.makedirs(error_path)
+
     def _save_failed_images(self, id: str, image, comparison, diff, threshold_diff):
         """
         Save snapshot, comparison, difference and thresholded difference images.
 
         Args:
             id: a unique id to gets the file names.
             image: the snapshot image.
             comparison: the comparison image.
             diff: the difference image.
             threshold_diff: the thresholded difference image.
         """
+        self._grant_error_path_exists(id)
+
         if image:
             image.save(self._get_failed_filename(id, "snapshot"))
         if comparison:
             comparison.save(self._get_failed_filename(id, "comparison"))
         if diff:
             diff.save(self._get_failed_filename(id, "difference"))
         if threshold_diff:
```

### Comparing `tiny-match-snapshot-0.0.1/pyproject.toml` & `tiny-match-snapshot-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">= 3.8"
 name = 'tiny-match-snapshot'
-version = '0.0.1'
+version = '0.0.2'
 description='Tiny snapshot assertion for tests'
 dependencies = ["Pillow"]
 authors = [{name = "Eduardo Oliveira", email = "eduardo_y05@outlook.com"}]
 maintainers = [{name = "Eduardo Oliveira", email = "eduardo_y05@outlook.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["snapshot", "test", "image", "match", "assertion", "playwright", "selenium"]
```

