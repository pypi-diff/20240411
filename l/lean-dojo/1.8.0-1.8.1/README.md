# Comparing `tmp/lean_dojo-1.8.0.tar.gz` & `tmp/lean_dojo-1.8.1.tar.gz`

## Comparing `lean_dojo-1.8.0.tar` & `lean_dojo-1.8.1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/mypy.ini
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tmp.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/constants.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/container.py
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/utils.py
--rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/ExtractData.lean
--rw-r--r--   0        0        0    48595 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/ast.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/build_lean4_repo.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/cache.py
--rw-r--r--   0        0        0    20689 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/lean.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/trace.py
--rw-r--r--   0        0        0    43534 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/traced_data.py
--rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/interaction/Lean4Repl.lean
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/interaction/dojo.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/interaction/parse_goals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/data_extraction/test_trace.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_commands.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_imports.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_init_errors.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_parse_goals.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_sorry.py
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_tactics.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_timeout.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/LICENSE
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/README.md
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/mypy.ini
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/constants.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/container.py
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/utils.py
+-rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/ExtractData.lean
+-rw-r--r--   0        0        0    48595 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/ast.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/build_lean4_repo.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/cache.py
+-rw-r--r--   0        0        0    20689 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/lean.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/trace.py
+-rw-r--r--   0        0        0    43534 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/data_extraction/traced_data.py
+-rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/interaction/Lean4Repl.lean
+-rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/interaction/dojo.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/src/lean_dojo/interaction/parse_goals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/conftest.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/data_extraction/test_trace.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_commands.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_imports.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_init_errors.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_parse_goals.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_sorry.py
+-rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_tactics.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/tests/interaction/test_timeout.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/LICENSE
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/README.md
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7897 2020-02-02 00:00:00.000000 lean_dojo-1.8.1/PKG-INFO
```

### Comparing `lean_dojo-1.8.0/.readthedocs.yaml` & `lean_dojo-1.8.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/__init__.py` & `lean_dojo-1.8.1/src/lean_dojo/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import logger
 from .data_extraction.trace import (
     trace,
     get_traced_repo_path,
     is_available_in_cache,
 )
 
 from .data_extraction.traced_data import (
@@ -25,8 +26,8 @@
     ProofGivenUp,
 )
 from .interaction.parse_goals import Declaration, Goal, parse_goals
 from .data_extraction.lean import get_latest_commit, LeanGitRepo, LeanFile, Theorem, Pos
 from .constants import __version__
 
 if os.geteuid() == 0:
-    raise RuntimeError("LeanDojo should not be run as root.")
+    logger.warning("Running LeanDojo as the root user may cause unexpected issues. Proceed with caution.")
```

### Comparing `lean_dojo-1.8.0/src/lean_dojo/constants.py` & `lean_dojo-1.8.1/src/lean_dojo/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 from typing import Tuple
 from loguru import logger
 from dotenv import load_dotenv
 
 load_dotenv()
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 logger.remove()
 if "VERBOSE" in os.environ or "DEBUG" in os.environ:
     logger.add(sys.stderr, level="DEBUG")
 else:
     logger.add(sys.stderr, level="INFO")
```

### Comparing `lean_dojo-1.8.0/src/lean_dojo/container.py` & `lean_dojo-1.8.1/src/lean_dojo/container.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/utils.py` & `lean_dojo-1.8.1/src/lean_dojo/utils.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/ExtractData.lean` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/ExtractData.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/ast.py` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/ast.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/build_lean4_repo.py` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/build_lean4_repo.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/cache.py` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/cache.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/lean.py` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/lean.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/trace.py` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/trace.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/data_extraction/traced_data.py` & `lean_dojo-1.8.1/src/lean_dojo/data_extraction/traced_data.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/interaction/Lean4Repl.lean` & `lean_dojo-1.8.1/src/lean_dojo/interaction/Lean4Repl.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/src/lean_dojo/interaction/dojo.py` & `lean_dojo-1.8.1/src/lean_dojo/interaction/dojo.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,15 @@
 
         Returns:
             Dict[str, Any]: _description_
         """
         if self.proc.stdin is None:
             raise RuntimeError("self.proc.stdin is not initialized")
         self._check_alive()
+        logger.debug(req)
         self.proc.stdin.write(req + "\n")
         try:
             res, msg = self._read_next_line()
         except EOFError:
             raise DojoCrashError("Unexpected EOF")
         try:
             result: Dict[str, Any] = json.loads(res)
```

### Comparing `lean_dojo-1.8.0/src/lean_dojo/interaction/parse_goals.py` & `lean_dojo-1.8.1/src/lean_dojo/interaction/parse_goals.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/tests/conftest.py` & `lean_dojo-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/tests/interaction/test_commands.py` & `lean_dojo-1.8.1/tests/interaction/test_commands.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/tests/interaction/test_imports.py` & `lean_dojo-1.8.1/tests/interaction/test_imports.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/tests/interaction/test_init_errors.py` & `lean_dojo-1.8.1/tests/interaction/test_init_errors.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/tests/interaction/test_sorry.py` & `lean_dojo-1.8.1/tests/interaction/test_sorry.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/tests/interaction/test_tactics.py` & `lean_dojo-1.8.1/tests/interaction/test_tactics.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/.gitignore` & `lean_dojo-1.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/LICENSE` & `lean_dojo-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.0/README.md` & `lean_dojo-1.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## Requirements
 
 * Supported platforms: Linux, Windows WSL, and macOS
 * Git >= 2.25
 * 3.9 <= Python < 3.11
 * wget
 * [elan](https://github.com/leanprover/elan)
-* Strongly Rrecommended: Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
+* Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
 
 
 ## Installation
 
 LeanDojo is available on [PyPI](https://pypi.org/project/lean-dojo/) and can be installed via pip:
 ```bash
 pip install lean-dojo
```

### Comparing `lean_dojo-1.8.0/pyproject.toml` & `lean_dojo-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "/docs",
   "/images",
   "/scripts",
 ]
 
 [project]
 name = "lean-dojo"
-version = "1.8.0"
+version = "1.8.1"
 authors = [
   { name="Kaiyu Yang", email="kaiyuy@caltech.edu" },
 ]
 description = "LeanDojo: Machine Learning for Theorem Proving in Lean"
 keywords = ["theorem proving", "machine learning", "Lean"]
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `lean_dojo-1.8.0/PKG-INFO` & `lean_dojo-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lean-dojo
-Version: 1.8.0
+Version: 1.8.1
 Summary: LeanDojo: Machine Learning for Theorem Proving in Lean
 Project-URL: Homepage, https://leandojo.org/
 Project-URL: Bug Tracker, https://github.com/lean-dojo/LeanDojo/issues
 Author-email: Kaiyu Yang <kaiyuy@caltech.edu>
 License: MIT License
         
         Copyright (c) 2023 LeanDojo Team
@@ -85,15 +85,15 @@
 ## Requirements
 
 * Supported platforms: Linux, Windows WSL, and macOS
 * Git >= 2.25
 * 3.9 <= Python < 3.11
 * wget
 * [elan](https://github.com/leanprover/elan)
-* Strongly Rrecommended: Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
+* Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
 
 
 ## Installation
 
 LeanDojo is available on [PyPI](https://pypi.org/project/lean-dojo/) and can be installed via pip:
 ```bash
 pip install lean-dojo
```

