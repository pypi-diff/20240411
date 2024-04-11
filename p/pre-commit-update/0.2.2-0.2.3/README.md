# Comparing `tmp/pre_commit_update-0.2.2.tar.gz` & `tmp/pre_commit_update-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.2.2.tar", max compression
+gzip compressed data, was "pre_commit_update-0.2.3.tar", max compression
```

## Comparing `pre_commit_update-0.2.2.tar` & `pre_commit_update-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1058 2024-03-14 22:21:56.722257 pre_commit_update-0.2.2/LICENSE
--rw-r--r--   0        0        0     6121 2024-04-08 20:24:09.734523 pre_commit_update-0.2.2/README.md
--rw-r--r--   0        0        0     1660 2024-04-11 09:31:50.560168 pre_commit_update-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 18:52:38.000000 pre_commit_update-0.2.2/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0    10852 2024-04-11 09:32:10.876625 pre_commit_update-0.2.2/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.2.2/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     7665 1970-01-01 00:00:00.000000 pre_commit_update-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-14 22:21:56.722257 pre_commit_update-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6121 2024-04-08 20:24:09.734523 pre_commit_update-0.2.3/README.md
+-rw-r--r--   0        0        0     1660 2024-04-11 11:58:32.472296 pre_commit_update-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-08 18:52:38.000000 pre_commit_update-0.2.3/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0    11039 2024-04-11 11:58:09.552302 pre_commit_update-0.2.3/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.2.3/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     7665 1970-01-01 00:00:00.000000 pre_commit_update-0.2.3/PKG-INFO
```

### Comparing `pre_commit_update-0.2.2/LICENSE` & `pre_commit_update-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.2.2/README.md` & `pre_commit_update-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.2.2/pyproject.toml` & `pre_commit_update-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.2.2"
+version = "0.2.3"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
 repository = "https://gitlab.com/vojko.pribudic/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
```

### Comparing `pre_commit_update-0.2.2/src/pre_commit_update/cli.py` & `pre_commit_update-0.2.3/src/pre_commit_update/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,42 +102,47 @@
         # Credit goes to Levon (https://stackoverflow.com/users/1209279/levon)
         # for this idea: <https://stackoverflow.com/a/11592279/7593853>.
         return all(character in string.hexdigits for character in ver)
 
 
 def _get_target_ver(repo: Dict, tags: List, all_versions: bool) -> str:
     current_ver: str = repo["rev"]
-    if current_ver in tags:
+    try:
+        parse_version(current_ver)
         return _get_target_tag(tags, all_versions)
-    elif _is_a_hash(current_ver):
+    except InvalidVersion:
+        pass
+    if _is_a_hash(current_ver):
         return _get_repo_head_hash(repo)
     return current_ver
 
 
 def _get_fixed_tag_versions(tag_versions: List) -> List:
     # Due to various prefixes that devs choose for tags, strip them down to semantic version numbers only.
     # Store it inside the dict ("ver1.2.3": "1.2.3") and parse the value to get the correct sort.
     # Return the original value (key) once everything is parsed/sorted.
     fixed_tag_versions: Dict = {}
     for tag in tag_versions:
         for prefix in re.findall("([a-zA-Z ]*)\\d*.*", tag):
-            if not prefix:
+            prefix = prefix.strip()
+            # Remove invalid suffix/tag values like "-test" or "split"
+            try:
+                version: str = tag[len(prefix) :]
+                parse_version(version)
+                fixed_tag_versions[tag] = version
+            except InvalidVersion:
                 continue
-            fixed_tag_versions[tag] = tag[len(prefix) :]
-    try:
-        fixed_tag_versions = {
-            k: v
-            for k, v in sorted(
-                fixed_tag_versions.items(),
-                key=lambda item: parse_version(item[1]),
-                reverse=True,
-            )
-        }
-    except InvalidVersion:
-        pass
+    fixed_tag_versions = {
+        k: v
+        for k, v in sorted(
+            fixed_tag_versions.items(),
+            key=lambda item: parse_version(item[1]),
+            reverse=True,
+        )
+    }
     return list(fixed_tag_versions.keys())
 
 
 def _output_display_message(value: DisplayMessageType) -> None:
     try:
         click.echo("\n".join(x["message"] for x in value))
     except UnicodeEncodeError:
```

### Comparing `pre_commit_update-0.2.2/PKG-INFO` & `pre_commit_update-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-update
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple CLI tool to check and update pre-commit hooks.
 Home-page: https://gitlab.com/vojko.pribudic/pre-commit-update
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pre-commit-update Version: 0.2.2 Summary: Simple
+Metadata-Version: 2.1 Name: pre-commit-update Version: 0.2.3 Summary: Simple
 CLI tool to check and update pre-commit hooks. Home-page: https://gitlab.com/
 vojko.pribudic/pre-commit-update License: MIT Author: Vojko PribudiÄ Author-
 email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ Maintainer-email:
 dmanthing@gmail.com Requires-Python: >=3.8 Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
```

