# Comparing `tmp/silence_lint_error-1.3.0.tar.gz` & `tmp/silence_lint_error-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silence_lint_error-1.3.0.tar", last modified: Fri Dec 15 23:42:20 2023, max compression
+gzip compressed data, was "silence_lint_error-1.4.0.tar", last modified: Thu Apr 11 09:48:15 2024, max compression
```

## Comparing `silence_lint_error-1.3.0.tar` & `silence_lint_error-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2023-12-15 23:42:20.742559 silence_lint_error-1.3.0/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1078 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/LICENSE
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2764 2023-12-15 23:42:20.742471 silence_lint_error-1.3.0/PKG-INFO
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2141 2023-12-15 23:41:05.000000 silence_lint_error-1.3.0/README.md
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1420 2023-12-15 23:42:20.742913 silence_lint_error-1.3.0/setup.cfg
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       74 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/setup.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2023-12-15 23:42:20.738848 silence_lint_error-1.3.0/silence_lint_error/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/silence_lint_error/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3996 2023-12-15 23:41:05.000000 silence_lint_error-1.3.0/silence_lint_error/comments.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     4866 2023-12-15 23:41:05.000000 silence_lint_error-1.3.0/silence_lint_error/fix_silenced_error.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     9378 2023-12-11 17:21:55.000000 silence_lint_error-1.3.0/silence_lint_error/silence_lint_error.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2023-12-15 23:42:20.742191 silence_lint_error-1.3.0/silence_lint_error.egg-info/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2764 2023-12-15 23:42:20.000000 silence_lint_error-1.3.0/silence_lint_error.egg-info/PKG-INFO
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)      743 2023-12-15 23:42:20.000000 silence_lint_error-1.3.0/silence_lint_error.egg-info/SOURCES.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        1 2023-12-15 23:42:20.000000 silence_lint_error-1.3.0/silence_lint_error.egg-info/dependency_links.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)      146 2023-12-15 23:42:20.000000 silence_lint_error-1.3.0/silence_lint_error.egg-info/entry_points.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       18 2023-12-15 23:42:20.000000 silence_lint_error-1.3.0/silence_lint_error.egg-info/requires.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       25 2023-12-15 23:42:20.000000 silence_lint_error-1.3.0/silence_lint_error.egg-info/top_level.txt
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2023-12-15 23:42:20.740136 silence_lint_error-1.3.0/tests/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/tests/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     4095 2023-12-15 23:41:05.000000 silence_lint_error-1.3.0/tests/comments_test.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2023-12-15 23:42:20.740770 silence_lint_error-1.3.0/tests/fix_silenced_error/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/tests/fix_silenced_error/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1725 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/tests/fix_silenced_error/fixit_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1308 2023-12-15 23:41:05.000000 silence_lint_error-1.3.0/tests/fix_silenced_error/ruff_test.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2023-12-15 23:42:20.741661 silence_lint_error-1.3.0/tests/silence_lint_error/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.3.0/tests/silence_lint_error/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     6387 2023-12-11 17:21:55.000000 silence_lint_error-1.3.0/tests/silence_lint_error/fixit_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2065 2023-11-24 18:42:18.000000 silence_lint_error-1.3.0/tests/silence_lint_error/flake8_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1898 2023-11-24 18:42:18.000000 silence_lint_error-1.3.0/tests/silence_lint_error/ruff_test.py
+drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.656846 silence_lint_error-1.4.0/
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1078 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/LICENSE
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3196 2024-04-11 09:48:15.656731 silence_lint_error-1.4.0/PKG-INFO
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2573 2024-04-11 09:47:00.000000 silence_lint_error-1.4.0/README.md
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1420 2024-04-11 09:48:15.657194 silence_lint_error-1.4.0/setup.cfg
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       74 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/setup.py
+drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.653324 silence_lint_error-1.4.0/silence_lint_error/
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/silence_lint_error/__init__.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3996 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/silence_lint_error/comments.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     4866 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/silence_lint_error/fix_silenced_error.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)    11052 2024-04-11 09:47:00.000000 silence_lint_error-1.4.0/silence_lint_error/silence_lint_error.py
+drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.656385 silence_lint_error-1.4.0/silence_lint_error.egg-info/
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3196 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/PKG-INFO
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)      784 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/SOURCES.txt
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        1 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/dependency_links.txt
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)      146 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/entry_points.txt
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       18 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/requires.txt
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       25 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/top_level.txt
+drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.654441 silence_lint_error-1.4.0/tests/
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/__init__.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     4095 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/tests/comments_test.py
+drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.654877 silence_lint_error-1.4.0/tests/fix_silenced_error/
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/fix_silenced_error/__init__.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1725 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/fix_silenced_error/fixit_test.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1308 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/tests/fix_silenced_error/ruff_test.py
+drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.655771 silence_lint_error-1.4.0/tests/silence_lint_error/
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/silence_lint_error/__init__.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     6387 2023-12-11 17:21:55.000000 silence_lint_error-1.4.0/tests/silence_lint_error/fixit_test.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2065 2023-11-24 18:42:18.000000 silence_lint_error-1.4.0/tests/silence_lint_error/flake8_test.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1898 2023-11-24 18:42:18.000000 silence_lint_error-1.4.0/tests/silence_lint_error/ruff_test.py
+-rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2347 2024-04-11 09:47:00.000000 silence_lint_error-1.4.0/tests/silence_lint_error/semgrep_test.py
```

### Comparing `silence_lint_error-1.3.0/LICENSE` & `silence_lint_error-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/PKG-INFO` & `silence_lint_error-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,17 @@
-Metadata-Version: 2.1
-Name: silence_lint_error
-Version: 1.3.0
-Summary: silence linting errors by adding ignore/fixme comments
-Home-page: https://github.com/samueljsb/silence-lint-error
-Author: Samuel Searles-Bryant
-Author-email: sam@samueljsb.co.uk
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: attrs
-Requires-Dist: tokenize-rt
-
 # silence-lint-error
 
 Silent linting errors by adding `ignore` or `fixme` comments.
 
 This tool currently works with:
 
 - [`fixit`](https://github.com/Instagram/Fixit)
 - [`flake8`](https://github.com/PyCQA/flake8) (silence only)
 - [`ruff`](https://docs.astral.sh/ruff/)
+- [`semgrep`](https://semgrep.dev/docs/) (silence only)
 
 ## Usage
 
 Install with pip:
 
 ```shell
 python -m pip install silence-lint-error
@@ -56,14 +39,24 @@
 
 To add `noqa: F401` comments to ignore the `F401` rule in `ruff`, run:
 
 ```shell
 silence-lint-error ruff F401 path/to/files/ path/to/more/files/
 ```
 
+To add `nosemgrep: python.lang.best-practice.sleep.arbitrary-sleep` comments to
+ignore the `python.lang.best-practice.sleep.arbitrary-sleep` rule in `semgrep`,
+run:
+
+```shell
+SEMGREP_RULES=r/python silence-lint-error semgrep python.lang.best-practice.sleep.arbitrary-sleep path/to/files/ path/to/more/files/
+```
+
+N.B. The rules must be configured in an environment variable.
+
 ### fix silenced errors
 
 If there is an auto-fix for a linting error, you can remove the `ignore` or
 `fixme` comments and apply the auto-fix.
 
 For example, to remove all `lint-fixme: CollapseIsinstanceChecks` comments and
 apply the auto-fix for that rule, run:
```

### Comparing `silence_lint_error-1.3.0/setup.cfg` & `silence_lint_error-1.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = silence_lint_error
-version = 1.3.0
+version = 1.4.0
 description = silence linting errors by adding ignore/fixme comments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/samueljsb/silence-lint-error
 author = Samuel Searles-Bryant
 author_email = sam@samueljsb.co.uk
 license = MIT
```

### Comparing `silence_lint_error-1.3.0/silence_lint_error/comments.py` & `silence_lint_error-1.4.0/silence_lint_error/comments.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/silence_lint_error/fix_silenced_error.py` & `silence_lint_error-1.4.0/silence_lint_error/fix_silenced_error.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/silence_lint_error/silence_lint_error.py` & `silence_lint_error-1.4.0/silence_lint_error/silence_lint_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -209,19 +209,74 @@
         self, src: str, violations: Sequence[Violation],
     ) -> str:
         [rule_name] = {violation.rule_name for violation in violations}
         linenos_to_silence = {violation.lineno for violation in violations}
         return comments.add_noqa_comments(src, linenos_to_silence, rule_name)
 
 
+class Semgrep:
+    name = 'semgrep'
+
+    def find_violations(
+        self, rule_name: RuleName, filenames: Sequence[FileName],
+    ) -> dict[FileName, list[Violation]]:
+        proc = subprocess.run(
+            (
+                'semgrep', 'scan',
+                '--metrics=off', '--oss-only',
+                '--json',
+                *filenames,
+            ),
+            capture_output=True,
+            text=True,
+        )
+
+        if proc.returncode:
+            raise ErrorRunningTool(proc)
+
+        # extract filenames and line numbers
+        results: dict[FileName, list[Violation]] = defaultdict(list)
+        data = json.loads(proc.stdout)
+        for result in data['results']:
+            if result['check_id'] != rule_name:
+                continue
+
+            results[result['path']].append(
+                Violation(
+                    rule_name=result['check_id'],
+                    lineno=result['start']['line'],
+                ),
+            )
+
+        return dict(results)
+
+    def silence_violations(
+        self, src: str, violations: Sequence[Violation],
+    ) -> str:
+        [rule_name] = {violation.rule_name for violation in violations}
+        linenos_to_silence = {violation.lineno for violation in violations}
+
+        lines = src.splitlines(keepends=True)
+
+        new_lines = []
+        for current_lineno, line in enumerate(lines, start=1):
+            if current_lineno in linenos_to_silence:
+                leading_ws = line.removesuffix(line.lstrip())
+                new_lines.append(f'{leading_ws}# nosemgrep: {rule_name}\n')
+            new_lines.append(line)
+
+        return ''.join(new_lines)
+
+
 LINTERS: dict[str, type[Linter]] = {
     'fixit': Fixit,
     'fixit-inline': FixitInline,
     'flake8': Flake8,
     'ruff': Ruff,
+    'semgrep': Semgrep,
 }
 
 
 # CLI
 # ===
 
 class Context(NamedTuple):
```

### Comparing `silence_lint_error-1.3.0/silence_lint_error.egg-info/PKG-INFO` & `silence_lint_error-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: silence-lint-error
-Version: 1.3.0
+Name: silence_lint_error
+Version: 1.4.0
 Summary: silence linting errors by adding ignore/fixme comments
 Home-page: https://github.com/samueljsb/silence-lint-error
 Author: Samuel Searles-Bryant
 Author-email: sam@samueljsb.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,15 @@
 Silent linting errors by adding `ignore` or `fixme` comments.
 
 This tool currently works with:
 
 - [`fixit`](https://github.com/Instagram/Fixit)
 - [`flake8`](https://github.com/PyCQA/flake8) (silence only)
 - [`ruff`](https://docs.astral.sh/ruff/)
+- [`semgrep`](https://semgrep.dev/docs/) (silence only)
 
 ## Usage
 
 Install with pip:
 
 ```shell
 python -m pip install silence-lint-error
@@ -56,14 +57,24 @@
 
 To add `noqa: F401` comments to ignore the `F401` rule in `ruff`, run:
 
 ```shell
 silence-lint-error ruff F401 path/to/files/ path/to/more/files/
 ```
 
+To add `nosemgrep: python.lang.best-practice.sleep.arbitrary-sleep` comments to
+ignore the `python.lang.best-practice.sleep.arbitrary-sleep` rule in `semgrep`,
+run:
+
+```shell
+SEMGREP_RULES=r/python silence-lint-error semgrep python.lang.best-practice.sleep.arbitrary-sleep path/to/files/ path/to/more/files/
+```
+
+N.B. The rules must be configured in an environment variable.
+
 ### fix silenced errors
 
 If there is an auto-fix for a linting error, you can remove the `ignore` or
 `fixme` comments and apply the auto-fix.
 
 For example, to remove all `lint-fixme: CollapseIsinstanceChecks` comments and
 apply the auto-fix for that rule, run:
```

### Comparing `silence_lint_error-1.3.0/silence_lint_error.egg-info/SOURCES.txt` & `silence_lint_error-1.4.0/silence_lint_error.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 tests/comments_test.py
 tests/fix_silenced_error/__init__.py
 tests/fix_silenced_error/fixit_test.py
 tests/fix_silenced_error/ruff_test.py
 tests/silence_lint_error/__init__.py
 tests/silence_lint_error/fixit_test.py
 tests/silence_lint_error/flake8_test.py
-tests/silence_lint_error/ruff_test.py
+tests/silence_lint_error/ruff_test.py
+tests/silence_lint_error/semgrep_test.py
```

### Comparing `silence_lint_error-1.3.0/tests/comments_test.py` & `silence_lint_error-1.4.0/tests/comments_test.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/tests/fix_silenced_error/fixit_test.py` & `silence_lint_error-1.4.0/tests/fix_silenced_error/fixit_test.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/tests/fix_silenced_error/ruff_test.py` & `silence_lint_error-1.4.0/tests/fix_silenced_error/ruff_test.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/tests/silence_lint_error/fixit_test.py` & `silence_lint_error-1.4.0/tests/silence_lint_error/fixit_test.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/tests/silence_lint_error/flake8_test.py` & `silence_lint_error-1.4.0/tests/silence_lint_error/flake8_test.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.3.0/tests/silence_lint_error/ruff_test.py` & `silence_lint_error-1.4.0/tests/silence_lint_error/ruff_test.py`

 * *Files identical despite different names*

