# Comparing `tmp/together-1.0.1.tar.gz` & `tmp/together-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-1.0.1.tar", max compression
+gzip compressed data, was "together-1.1.0.tar", max compression
```

## Comparing `together-1.0.1.tar` & `together-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-04-05 19:08:02.492677 together-1.0.1/LICENSE
--rw-r--r--   0        0        0     9667 2024-04-05 19:08:02.492677 together-1.0.1/README.md
--rw-r--r--   0        0        0     1897 2024-04-05 19:08:02.496677 together-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-04-05 19:08:02.496677 together-1.0.1/src/together/__init__.py
--rw-r--r--   0        0        0       57 2024-04-05 19:08:02.496677 together-1.0.1/src/together/abstract/__init__.py
--rw-r--r--   0        0        0    25103 2024-04-05 19:08:02.496677 together-1.0.1/src/together/abstract/api_requestor.py
--rw-r--r--   0        0        0        0 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/__init__.py
--rw-r--r--   0        0        0     7838 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/chat.py
--rw-r--r--   0        0        0     3691 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/completions.py
--rw-r--r--   0        0        0     3186 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/files.py
--rw-r--r--   0        0        0     4954 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/finetune.py
--rw-r--r--   0        0        0     2363 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/images.py
--rw-r--r--   0        0        0     1126 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/models.py
--rw-r--r--   0        0        0     1977 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/cli.py
--rw-r--r--   0        0        0     4774 2024-04-05 19:08:02.496677 together-1.0.1/src/together/client.py
--rw-r--r--   0        0        0      801 2024-04-05 19:08:02.496677 together-1.0.1/src/together/constants.py
--rw-r--r--   0        0        0     5329 2024-04-05 19:08:02.496677 together-1.0.1/src/together/error.py
--rw-r--r--   0        0        0    10916 2024-04-05 19:08:02.496677 together-1.0.1/src/together/filemanager.py
--rw-r--r--   0        0        0        0 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/__init__.py
--rw-r--r--   0        0        0      727 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/base.py
--rw-r--r--   0        0        0     2343 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/complete.py
--rw-r--r--   0        0        0      591 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/embeddings.py
--rw-r--r--   0        0        0     3863 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/files.py
--rw-r--r--   0        0        0     4917 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/finetune.py
--rw-r--r--   0        0        0      582 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/images.py
--rw-r--r--   0        0        0     1053 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/models.py
--rw-r--r--   0        0        0      701 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/__init__.py
--rw-r--r--   0        0        0      617 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/chat/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/chat/completions.py
--rw-r--r--   0        0        0     8403 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/completions.py
--rw-r--r--   0        0        0     2546 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/embeddings.py
--rw-r--r--   0        0        0     4593 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/files.py
--rw-r--r--   0        0        0    12424 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/finetune.py
--rw-r--r--   0        0        0     4775 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/images.py
--rw-r--r--   0        0        0     1786 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/models.py
--rw-r--r--   0        0        0     1319 2024-04-05 19:08:02.496677 together-1.0.1/src/together/together_response.py
--rw-r--r--   0        0        0     1402 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/__init__.py
--rw-r--r--   0        0        0      642 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/abstract.py
--rw-r--r--   0        0        0     3630 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/chat_completions.py
--rw-r--r--   0        0        0     1491 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/common.py
--rw-r--r--   0        0        0     2173 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/completions.py
--rw-r--r--   0        0        0      751 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/embeddings.py
--rw-r--r--   0        0        0      370 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/error.py
--rw-r--r--   0        0        0     1934 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/files.py
--rw-r--r--   0        0        0     5779 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/finetune.py
--rw-r--r--   0        0        0      915 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/images.py
--rw-r--r--   0        0        0     1013 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/models.py
--rw-r--r--   0        0        0      662 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/_log.py
--rw-r--r--   0        0        0     2407 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/api_helpers.py
--rw-r--r--   0        0        0     4835 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/files.py
--rw-r--r--   0        0        0     1788 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/tools.py
--rw-r--r--   0        0        0      126 2024-04-05 19:08:02.500677 together-1.0.1/src/together/version.py
--rw-r--r--   0        0        0    10963 1970-01-01 00:00:00.000000 together-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 23:34:18.446826 together-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9667 2024-04-10 23:34:18.446826 together-1.1.0/README.md
+-rw-r--r--   0        0        0     2439 2024-04-10 23:34:18.446826 together-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-04-10 23:34:18.446826 together-1.1.0/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-10 23:34:18.446826 together-1.1.0/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-04-10 23:34:18.450826 together-1.1.0/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     7838 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     3691 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3186 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     4954 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-04-10 23:34:18.450826 together-1.1.0/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-04-10 23:34:18.450826 together-1.1.0/src/together/client.py
+-rw-r--r--   0        0        0      908 2024-04-10 23:34:18.450826 together-1.1.0/src/together/constants.py
+-rw-r--r--   0        0        0     5329 2024-04-10 23:34:18.450826 together-1.1.0/src/together/error.py
+-rw-r--r--   0        0        0    11438 2024-04-10 23:34:18.450826 together-1.1.0/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3863 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-04-10 23:34:18.450826 together-1.1.0/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    11140 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0     8403 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4593 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/files.py
+-rw-r--r--   0        0        0    12424 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-04-10 23:34:18.450826 together-1.1.0/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-04-10 23:34:18.450826 together-1.1.0/src/together/together_response.py
+-rw-r--r--   0        0        0     1432 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/abstract.py
+-rw-r--r--   0        0        0     3630 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/common.py
+-rw-r--r--   0        0        0     2173 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/error.py
+-rw-r--r--   0        0        0     1954 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/files.py
+-rw-r--r--   0        0        0     5779 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-04-10 23:34:18.450826 together-1.1.0/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     7186 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-04-10 23:34:18.450826 together-1.1.0/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-04-10 23:34:18.454826 together-1.1.0/src/together/version.py
+-rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 together-1.1.0/PKG-INFO
```

### Comparing `together-1.0.1/LICENSE` & `together-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `together-1.0.1/README.md` & `together-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `together-1.0.1/pyproject.toml` & `together-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 [build-system]
-requires = ["poetry"]
+requires = [
+    "poetry",
+    # Starting with NumPy 1.25, NumPy is (by default) as far back compatible
+    # as oldest-support-numpy was (customizable with a NPY_TARGET_VERSION
+    # define).  For older Python versions (where NumPy 1.25 is not yet avaiable)
+    # continue using oldest-support-numpy.
+    "oldest-supported-numpy>=0.14; python_version<'3.9'",
+    "numpy>=1.25; python_version>='3.9'",
+]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
-  "Together AI <support@together.ai>"
+    "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
@@ -27,25 +35,31 @@
 tabulate = "^0.9.0"
 pydantic = "^2.6.3"
 aiohttp = "^3.9.3"
 filelock = "^3.13.1"
 eval-type-backport = "^0.1.3"
 click = "^8.1.7"
 pillow = "^10.3.0"
+pyarrow = ">=10.0.1"
+numpy = [
+    { version = ">=1.23.5", python = "<3.12" },
+    { version = ">=1.26.0", python = ">=3.12" },
+]
 
 [tool.poetry.group.quality]
 optional = true
 
 [tool.poetry.group.quality.dependencies]
 black = ">=23.1,<25.0"
 ruff = "^0.3.2"
 types-tqdm = "^4.65.0.0"
 types-tabulate = "^0.9.0.3"
 pre-commit = "3.5.0"
 types-requests = "^2.31.0.20240218"
+pyarrow-stubs = "^10.0.1.7"
 mypy = "^1.9.0"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 pytest = ">=7.4.2,<9.0.0"
```

### Comparing `together-1.0.1/src/together/__init__.py` & `together-1.1.0/src/together/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/abstract/api_requestor.py` & `together-1.1.0/src/together/abstract/api_requestor.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/api/chat.py` & `together-1.1.0/src/together/cli/api/chat.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/api/completions.py` & `together-1.1.0/src/together/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/api/files.py` & `together-1.1.0/src/together/cli/api/files.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/api/finetune.py` & `together-1.1.0/src/together/cli/api/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/api/images.py` & `together-1.1.0/src/together/cli/api/images.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/api/models.py` & `together-1.1.0/src/together/cli/api/models.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/cli/cli.py` & `together-1.1.0/src/together/cli/cli.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/client.py` & `together-1.1.0/src/together/client.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/constants.py` & `together-1.1.0/src/together/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,7 +22,10 @@
 MIN_SAMPLES = 100
 
 # the number of bytes in a gigabyte, used to convert bytes to GB for readable comparison
 NUM_BYTES_IN_GB = 2**30
 
 # maximum number of GB sized files we support finetuning for
 MAX_FILE_SIZE_GB = 4.9
+
+# expected columns for Parquet files
+PARQUET_EXPECTED_COLUMNS = ["input_ids", "attention_mask", "labels"]
```

### Comparing `together-1.0.1/src/together/error.py` & `together-1.1.0/src/together/error.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/filemanager.py` & `together-1.1.0/src/together/filemanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 from together.error import (
     APIError,
     AuthenticationError,
     DownloadError,
     FileTypeError,
 )
 from together.together_response import TogetherResponse
-from together.types import FilePurpose, FileResponse, TogetherClient, TogetherRequest
+from together.types import (
+    FilePurpose,
+    FileResponse,
+    FileType,
+    TogetherClient,
+    TogetherRequest,
+)
 
 
 def chmod_and_replace(src: Path, dst: Path) -> None:
     """Set correct permission before moving a blob from tmp directory to cache dir.
 
     Do not take into account the `umask` from the process as there is no convenient way
     to get it that is thread-safe.
@@ -256,20 +262,25 @@
             )
         elif response.status_code != 302:
             raise APIError(
                 f"Unexpected error raised by endpoint: {response.content.decode()}, headers: {response.headers}",
                 http_status=response.status_code,
             )
 
-    def redirect_policy(
-        self, url: str, file: Path, purpose: FilePurpose
+    def get_upload_url(
+        self,
+        url: str,
+        file: Path,
+        purpose: FilePurpose,
+        filetype: FileType,
     ) -> Tuple[str, str]:
         data = {
             "purpose": purpose.value,
             "file_name": file.name,
+            "file_type": filetype.value,
         }
 
         requestor = api_requestor.APIRequestor(
             client=self._client,
         )
 
         method = "POST"
@@ -320,15 +331,24 @@
 
         requestor = api_requestor.APIRequestor(
             client=self._client,
         )
 
         redirect_url = None
         if redirect:
-            redirect_url, file_id = self.redirect_policy(url, file, purpose)
+            if file.suffix == ".jsonl":
+                filetype = FileType.jsonl
+            elif file.suffix == ".parquet":
+                filetype = FileType.parquet
+            else:
+                raise FileTypeError(
+                    f"Unknown extension of file {file}. "
+                    "Only files with extensions .jsonl and .parquet are supported."
+                )
+            redirect_url, file_id = self.get_upload_url(url, file, purpose, filetype)
 
         file_size = os.stat(file.as_posix()).st_size
 
         with tqdm(
             total=file_size,
             unit="B",
             unit_scale=True,
```

### Comparing `together-1.0.1/src/together/legacy/base.py` & `together-1.1.0/src/together/legacy/base.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/legacy/complete.py` & `together-1.1.0/src/together/legacy/complete.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/legacy/embeddings.py` & `together-1.1.0/src/together/legacy/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/legacy/files.py` & `together-1.1.0/src/together/legacy/files.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/legacy/finetune.py` & `together-1.1.0/src/together/legacy/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/legacy/images.py` & `together-1.1.0/src/together/legacy/images.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/legacy/models.py` & `together-1.1.0/src/together/legacy/models.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/__init__.py` & `together-1.1.0/src/together/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/chat/__init__.py` & `together-1.1.0/src/together/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/chat/completions.py` & `together-1.1.0/src/together/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/completions.py` & `together-1.1.0/src/together/resources/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/embeddings.py` & `together-1.1.0/src/together/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/files.py` & `together-1.1.0/src/together/resources/files.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/finetune.py` & `together-1.1.0/src/together/resources/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/images.py` & `together-1.1.0/src/together/resources/images.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/resources/models.py` & `together-1.1.0/src/together/resources/models.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/together_response.py` & `together-1.1.0/src/together/together_response.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/__init__.py` & `together-1.1.0/src/together/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from together.types.files import (
     FileDeleteResponse,
     FileList,
     FileObject,
     FilePurpose,
     FileRequest,
     FileResponse,
+    FileType,
 )
 from together.types.finetune import (
     FinetuneDownloadResult,
     FinetuneList,
     FinetuneListEvents,
     FinetuneRequest,
     FinetuneResponse,
@@ -51,11 +52,12 @@
     "FinetuneDownloadResult",
     "FileRequest",
     "FileResponse",
     "FileList",
     "FileDeleteResponse",
     "FileObject",
     "FilePurpose",
+    "FileType",
     "ImageRequest",
     "ImageResponse",
     "ModelObject",
 ]
```

### Comparing `together-1.0.1/src/together/types/abstract.py` & `together-1.1.0/src/together/types/abstract.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/chat_completions.py` & `together-1.1.0/src/together/types/chat_completions.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/common.py` & `together-1.1.0/src/together/types/common.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/completions.py` & `together-1.1.0/src/together/types/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/embeddings.py` & `together-1.1.0/src/together/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/files.py` & `together-1.1.0/src/together/types/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 )
 
 
 class FilePurpose(str, Enum):
     FineTune = "fine-tune"
 
 
+class FileType(str, Enum):
+    jsonl = "jsonl"
+    parquet = "parquet"
+
+
 class FileRequest(BaseModel):
     """
     Files request type
     """
 
     # training file ID
     training_file: str
@@ -39,29 +44,25 @@
 
 
 class FileResponse(BaseModel):
     """
     Files API response type
     """
 
-    # file id
     id: str
-    # object type
     object: Literal[ObjectType.File]
     # created timestamp
     created_at: int | None = None
-    # file purpose
+    type: FileType | None = None
     purpose: FilePurpose | None = None
-    # file-name
     filename: str | None = None
     # file byte size
     bytes: int | None = None
     # JSONL line count
     line_count: int | None = Field(None, alias="LineCount")
-    # is processed
     processed: bool | None = Field(None, alias="Processed")
 
 
 class FileList(BaseModel):
     # object type
     object: Literal["list"] | None = None
     # list of fine-tune job objects
```

### Comparing `together-1.0.1/src/together/types/finetune.py` & `together-1.1.0/src/together/types/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/images.py` & `together-1.1.0/src/together/types/images.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/types/models.py` & `together-1.1.0/src/together/types/models.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/utils/__init__.py` & `together-1.1.0/src/together/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/utils/_log.py` & `together-1.1.0/src/together/utils/_log.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/utils/api_helpers.py` & `together-1.1.0/src/together/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/src/together/utils/files.py` & `together-1.1.0/src/together/utils/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from __future__ import annotations
 
 import json
 import os
 from pathlib import Path
+from traceback import format_exc
 from typing import Any, Dict
 
-from together.constants import MAX_FILE_SIZE_GB, MIN_SAMPLES, NUM_BYTES_IN_GB
+from pyarrow import ArrowInvalid, parquet
+
+from together.constants import (
+    MAX_FILE_SIZE_GB,
+    MIN_SAMPLES,
+    NUM_BYTES_IN_GB,
+    PARQUET_EXPECTED_COLUMNS,
+)
 
 
 def check_file(
     file: Path | str,
 ) -> Dict[str, Any]:
     if not isinstance(file, Path):
         file = Path(file)
@@ -46,14 +54,33 @@
         report_dict["message"] = "File is empty"
         report_dict["file_size"] = 0
         report_dict["is_check_passed"] = False
         return report_dict
     else:
         report_dict["file_size"] = file_size
 
+    if file.suffix == ".jsonl":
+        report_dict["filetype"] = "jsonl"
+        data_report_dict = _check_jsonl(file)
+    elif file.suffix == ".parquet":
+        report_dict["filetype"] = "parquet"
+        data_report_dict = _check_parquet(file)
+    else:
+        report_dict["filetype"] = (
+            f"Unknown extension of file {file}. "
+            "Only files with extensions .jsonl and .parquet are supported."
+        )
+        report_dict["is_check_passed"] = False
+
+    report_dict.update(data_report_dict)
+    return report_dict
+
+
+def _check_jsonl(file: Path) -> Dict[str, Any]:
+    report_dict: Dict[str, Any] = {}
     # Check that the file is UTF-8 encoded. If not report where the error occurs.
     try:
         with file.open(encoding="utf-8") as f:
             f.read()
         report_dict["utf8"] = True
     except UnicodeDecodeError as e:
         report_dict["utf8"] = False
@@ -67,43 +94,43 @@
         try:
             for idx, line in enumerate(f):
                 json_line = json.loads(line)  # each line in jsonlines should be a json
 
                 if not isinstance(json_line, dict):
                     report_dict["line_type"] = False
                     report_dict["message"] = (
-                        f"Error parsing file. Invalid format on line {idx+1} of the input file. "
+                        f"Error parsing file. Invalid format on line {idx + 1} of the input file. "
                         'Example of valid json: {"text": "my sample string"}. '
                     )
 
                     report_dict["is_check_passed"] = False
 
                 if "text" not in json_line.keys():
                     report_dict["text_field"] = False
                     report_dict["message"] = (
-                        f"Missing 'text' field was found on line {idx+1} of the the input file. "
+                        f"Missing 'text' field was found on line {idx + 1} of the the input file. "
                         "Expected format: {'text': 'my sample string'}. "
                     )
                     report_dict["is_check_passed"] = False
                 else:
                     # check to make sure the value of the "text" key is a string
                     if not isinstance(json_line["text"], str):
                         report_dict["key_value"] = False
                         report_dict["message"] = (
-                            f'Invalid value type for "text" key on line {idx+1}. '
+                            f'Invalid value type for "text" key on line {idx + 1}. '
                             f'Expected string. Found {type(json_line["text"])}.'
                         )
 
                         report_dict["is_check_passed"] = False
 
             # make sure this is outside the for idx, line in enumerate(f): for loop
             if idx + 1 < MIN_SAMPLES:
                 report_dict["min_samples"] = False
                 report_dict["message"] = (
-                    f"Processing {file} resulted in only {idx+1} samples. "
+                    f"Processing {file} resulted in only {idx + 1} samples. "
                     f"Our minimum is {MIN_SAMPLES} samples. "
                 )
                 report_dict["is_check_passed"] = False
             else:
                 report_dict["num_samples"] = idx + 1
                 report_dict["min_samples"] = True
 
@@ -114,19 +141,64 @@
             if idx < 0:
                 report_dict["message"] = (
                     "Unable to decode file. "
                     "File may be empty or in an unsupported format. "
                 )
             else:
                 report_dict["message"] = (
-                    f"Error parsing json payload. Unexpected format on line {idx+1}."
+                    f"Error parsing json payload. Unexpected format on line {idx + 1}."
                 )
             report_dict["is_check_passed"] = False
 
     if report_dict["text_field"] is not False:
         report_dict["text_field"] = True
     if report_dict["line_type"] is not False:
         report_dict["line_type"] = True
     if report_dict["key_value"] is not False:
         report_dict["key_value"] = True
+    return report_dict
+
+
+def _check_parquet(file: Path) -> Dict[str, Any]:
+    report_dict: Dict[str, Any] = {}
+
+    try:
+        table = parquet.read_table(str(file), memory_map=True)
+    except ArrowInvalid:
+        report_dict["load_parquet"] = (
+            f"An exception has occurred when loading the Parquet file {file}. Please check the file for corruption. "
+            f"Exception trace:\n{format_exc()}"
+        )
+        report_dict["is_check_passed"] = False
+        return report_dict
+
+    column_names = table.schema.names
+    if "input_ids" not in column_names:
+        report_dict["load_parquet"] = (
+            f"Parquet file {file} does not contain the `input_ids` column."
+        )
+        report_dict["is_check_passed"] = False
+        return report_dict
+
+    for column_name in column_names:
+        if column_name not in PARQUET_EXPECTED_COLUMNS:
+            report_dict["load_parquet"] = (
+                f"Parquet file {file} contains an unexpected column {column_name}. "
+                f"Only columns {PARQUET_EXPECTED_COLUMNS} are supported."
+            )
+            report_dict["is_check_passed"] = False
+            return report_dict
+
+    num_samples = len(table)
+    if num_samples < MIN_SAMPLES:
+        report_dict["min_samples"] = (
+            f"Processing {file} resulted in only {num_samples} samples. "
+            f"Our minimum is {MIN_SAMPLES} samples. "
+        )
+        report_dict["is_check_passed"] = False
+        return report_dict
+    else:
+        report_dict["num_samples"] = num_samples
+
+    report_dict["is_check_passed"] = True
 
     return report_dict
```

### Comparing `together-1.0.1/src/together/utils/tools.py` & `together-1.1.0/src/together/utils/tools.py`

 * *Files identical despite different names*

### Comparing `together-1.0.1/PKG-INFO` & `together-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python client for Together's Cloud Platform!
 Home-page: https://github.com/togethercomputer/together-python
 License: Apache-2.0
 Author: Together AI
 Author-email: support@together.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,15 +15,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0)
 Requires-Dist: filelock (>=3.13.1,<4.0.0)
+Requires-Dist: numpy (>=1.23.5) ; python_version < "3.12"
+Requires-Dist: numpy (>=1.26.0) ; python_version >= "3.12"
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
+Requires-Dist: pyarrow (>=10.0.1)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.9,<0.13)
 Project-URL: Bug Tracker, https://github.com/togethercomputer/together-python/issues
 Project-URL: Repository, https://github.com/togethercomputer/together-python
```

