# Comparing `tmp/dayone_to_obsidian-0.4.7.tar.gz` & `tmp/dayone_to_obsidian-0.4.8.tar.gz`

## Comparing `dayone_to_obsidian-0.4.7.tar` & `dayone_to_obsidian-0.4.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/Makefile
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/requirements-dev.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/requirements-test.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.github/dependabot.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.github/pr-labeler.yml
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.github/workflows/pr-labeler.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/__init__.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/cli.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/helpers.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/models.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/options.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/py.typed
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/__init__.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/entry.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/journal.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/__init__.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/audio.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/base.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/pdf.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/photo.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/video.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/conftest.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/constants.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/test_cli.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/test_entry.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/test_journal.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/test_media.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/test_utils.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/assets/MyJournal.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/assets/invalid.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/assets/audios/a2c335fa03eb95c9a5444ff862ffd839.m4a
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/assets/pdfs/bccec75c303608619bc641f3c90b135a.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/assets/photos/6e8f17a1cd2fd963d5843aca794e2287.jpeg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/tests/assets/videos/62bb62c6ccb2571f2270dc5abfdf7f94.mp4
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/LICENSE
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/README.md
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/Makefile
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/requirements-dev.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/requirements-test.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.github/pr-labeler.yml
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.github/workflows/pr-labeler.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/__init__.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/cli.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/helpers.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/models.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/options.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/__init__.py
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/entry.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/journal.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/__init__.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/audio.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/base.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/pdf.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/photo.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/video.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/conftest.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/constants.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/test_cli.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/test_entry.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/test_journal.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/test_media.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/test_utils.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/assets/MyJournal.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/assets/invalid.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/assets/audios/a2c335fa03eb95c9a5444ff862ffd839.m4a
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/assets/pdfs/bccec75c303608619bc641f3c90b135a.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/assets/photos/6e8f17a1cd2fd963d5843aca794e2287.jpeg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/tests/assets/videos/62bb62c6ccb2571f2270dc5abfdf7f94.mp4
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/LICENSE
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/README.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 dayone_to_obsidian-0.4.8/PKG-INFO
```

### Comparing `dayone_to_obsidian-0.4.7/.pre-commit-config.yaml` & `dayone_to_obsidian-0.4.8/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 default_language_version:
   python: python3.11
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-toml
       - id: check-yaml
         args:
           - --unsafe
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.5
     hooks:
       - id: ruff
         args:
           - --fix
           - --exit-non-zero-on-fix
   - repo: https://github.com/psf/black
     rev: 24.3.0
```

### Comparing `dayone_to_obsidian-0.4.7/Makefile` & `dayone_to_obsidian-0.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/.github/workflows/ci.yml` & `dayone_to_obsidian-0.4.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/.github/workflows/pr-labeler.yml` & `dayone_to_obsidian-0.4.8/.github/workflows/pr-labeler.yml`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/.github/workflows/publish.yml` & `dayone_to_obsidian-0.4.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/cli.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/cli.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/models.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/models.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/entry.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/entry.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/journal.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/journal.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/utils.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/utils.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/audio.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/audio.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/base.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/base.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/pdf.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/pdf.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/photo.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/photo.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/dayone_to_obsidian/processors/media/video.py` & `dayone_to_obsidian-0.4.8/dayone_to_obsidian/processors/media/video.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/conftest.py` & `dayone_to_obsidian-0.4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/test_cli.py` & `dayone_to_obsidian-0.4.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/test_entry.py` & `dayone_to_obsidian-0.4.8/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/test_journal.py` & `dayone_to_obsidian-0.4.8/tests/test_journal.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/test_media.py` & `dayone_to_obsidian-0.4.8/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/test_utils.py` & `dayone_to_obsidian-0.4.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/tests/assets/MyJournal.json` & `dayone_to_obsidian-0.4.8/tests/assets/MyJournal.json`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/.gitignore` & `dayone_to_obsidian-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/LICENSE` & `dayone_to_obsidian-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/README.md` & `dayone_to_obsidian-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/pyproject.toml` & `dayone_to_obsidian-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dayone_to_obsidian-0.4.7/PKG-INFO` & `dayone_to_obsidian-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dayone-to-obsidian
-Version: 0.4.7
+Version: 0.4.8
 Summary: Convert a JSON export from Day One into individual notes for Obsidian.
 Project-URL: Homepage, https://github.com/kulapard/dayone-to-obsidian
 Project-URL: Documentation, https://github.com/kulapard/dayone-to-obsidian
 Project-URL: Repository, https://github.com/kulapard/dayone-to-obsidian
 Author-email: Taras Drapalyuk <taras@drapalyuk.com>
 License-Expression: MIT
 License-File: LICENSE
```

