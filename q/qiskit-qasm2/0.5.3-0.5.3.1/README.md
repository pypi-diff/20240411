# Comparing `tmp/qiskit_qasm2-0.5.3.tar.gz` & `tmp/qiskit_qasm2-0.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_qasm2-0.5.3.tar", last modified: Sat Mar 11 01:46:33 2023, max compression
+gzip compressed data, was "qiskit_qasm2-0.5.3.1.tar", last modified: Thu Apr 11 10:57:38 2024, max compression
```

## Comparing `qiskit_qasm2-0.5.3.tar` & `qiskit_qasm2-0.5.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 01:46:33.235727 qiskit_qasm2-0.5.3/src-python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-11 01:46:33.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-11 01:46:33.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 01:46:33.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 01:46:33.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-11 01:46:33.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-11 01:46:33.000000 qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/src-rust/
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-rust/bytecode.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-rust/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)    29102 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-rust/expr.rs
--rw-r--r--   0 runner    (1001) docker     (123)    30408 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-rust/lex.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-rust/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    71059 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/src-rust/parse.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 01:46:33.239727 qiskit_qasm2-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/tests/test_arxiv_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/tests/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30821 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/tests/test_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    54566 2023-03-11 01:46:18.000000 qiskit_qasm2-0.5.3/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:57:38.795392 qiskit_qasm2-0.5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-11 10:57:38.795392 qiskit_qasm2-0.5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-11 10:57:38.795392 qiskit_qasm2-0.5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:57:38.787392 qiskit_qasm2-0.5.3.1/src-python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:57:38.791392 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:57:38.795392 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-11 10:57:38.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 10:57:38.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:57:38.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:57:38.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 10:57:38.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 10:57:38.000000 qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:57:38.791392 qiskit_qasm2-0.5.3.1/src-rust/
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-rust/bytecode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-rust/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    29102 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-rust/expr.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    30408 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-rust/lex.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-rust/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    71059 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/src-rust/parse.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:57:38.795392 qiskit_qasm2-0.5.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/tests/test_arxiv_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/tests/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30821 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/tests/test_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54566 2024-04-11 10:57:32.000000 qiskit_qasm2-0.5.3.1/tests/test_structure.py
```

### Comparing `qiskit_qasm2-0.5.3/Cargo.lock` & `qiskit_qasm2-0.5.3.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/LICENSE` & `qiskit_qasm2-0.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/PKG-INFO` & `qiskit_qasm2-0.5.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 Metadata-Version: 2.1
 Name: qiskit_qasm2
-Version: 0.5.3
+Version: 0.5.3.1
 Summary: Importer for parsing OpenQASM 2 strings into Qiskit circuits
 Home-page: https://github.com/jakelishman/qiskit-qasm2
 Author: Jake Lishman
 License: Apache 2.0 License
 Project-URL: Bug Tracker, https://github.com/jakelishman/qiskit-qasm2/issues
 Project-URL: Documentation, https://jakelishman.github.io/qiskit-qasm2
 Project-URL: Source Code, https://github.com/jakelishman/qiskit-qasm2
 Description-Content-Type: text/markdown; variant=GFM
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: qiskit-terra>=0.21.0
+Requires-Dist: typing_extensions>=4.1.0
+Provides-Extra: all
 
 # Importer from OpenQASM 2 to Qiskit
 
 [![License](https://img.shields.io/github/license/jakelishman/qiskit-qasm2.svg?style=flat)](https://opensource.org/licenses/Apache-2.0) [![Release](https://img.shields.io/github/release/jakelishman/qiskit-qasm2.svg?style=flat)](https://github.com/jakelishman/qiskit-qasm2/releases) [![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm2.svg?style=flat)](https://pypi.org/project/qiskit-qasm2/) [![Coverage Status](https://coveralls.io/repos/github/jakelishman/qiskit-qasm2/badge.svg?branch=main)](https://coveralls.io/github/jakelishman/qiskit-qasm2?branch=main)
 
+> [!IMPORTANT]
+>
+> This package is obsolete.  It was vendored into Qiskit itself as of `qiskit==0.43.0` (via
+> `qiskit-terra==0.24.0` at the time), at version `0.5.3` of this package.  There is no longer any
+> need to install this package; simply use `qiskit.qasm2.load` or `qiskit.qasm2.loads`.  The Qiskit
+> version is actively developed, and this package is not being updated any more.
+>
+> All references to Qiskit in the README and in the package itself mean Qiskit versions `<0.43`,
+> before this package was vendored into Qiskit.
+
 This repository provides the Python package `qiskit_qasm2`, which provides a
 fast parser of OpenQASM 2 into Qiskit's `QuantumCircuit`.  It is often 10x or
 more faster than Qiskit's native parser.  The API is simple:
 
 - `qiskit_qasm2.load` takes a filename, and returns `QuantumCircuit`;
 - `qiskit_qasm2.loads` takes an OpenQASM 2 program in a string, and returns
   `QuantumCircuit`.
```

### Comparing `qiskit_qasm2-0.5.3/README.md` & `qiskit_qasm2-0.5.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Importer from OpenQASM 2 to Qiskit
 
 [![License](https://img.shields.io/github/license/jakelishman/qiskit-qasm2.svg?style=flat)](https://opensource.org/licenses/Apache-2.0) [![Release](https://img.shields.io/github/release/jakelishman/qiskit-qasm2.svg?style=flat)](https://github.com/jakelishman/qiskit-qasm2/releases) [![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm2.svg?style=flat)](https://pypi.org/project/qiskit-qasm2/) [![Coverage Status](https://coveralls.io/repos/github/jakelishman/qiskit-qasm2/badge.svg?branch=main)](https://coveralls.io/github/jakelishman/qiskit-qasm2?branch=main)
 
+> [!IMPORTANT]
+>
+> This package is obsolete.  It was vendored into Qiskit itself as of `qiskit==0.43.0` (via
+> `qiskit-terra==0.24.0` at the time), at version `0.5.3` of this package.  There is no longer any
+> need to install this package; simply use `qiskit.qasm2.load` or `qiskit.qasm2.loads`.  The Qiskit
+> version is actively developed, and this package is not being updated any more.
+>
+> All references to Qiskit in the README and in the package itself mean Qiskit versions `<0.43`,
+> before this package was vendored into Qiskit.
+
 This repository provides the Python package `qiskit_qasm2`, which provides a
 fast parser of OpenQASM 2 into Qiskit's `QuantumCircuit`.  It is often 10x or
 more faster than Qiskit's native parser.  The API is simple:
 
 - `qiskit_qasm2.load` takes a filename, and returns `QuantumCircuit`;
 - `qiskit_qasm2.loads` takes an OpenQASM 2 program in a string, and returns
   `QuantumCircuit`.
```

### Comparing `qiskit_qasm2-0.5.3/pyproject.toml` & `qiskit_qasm2-0.5.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/setup.cfg` & `qiskit_qasm2-0.5.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-python/qiskit_qasm2/__init__.py` & `qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-python/qiskit_qasm2/parse.py` & `qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2/parse.py`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/PKG-INFO` & `qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 Metadata-Version: 2.1
-Name: qiskit-qasm2
-Version: 0.5.3
+Name: qiskit_qasm2
+Version: 0.5.3.1
 Summary: Importer for parsing OpenQASM 2 strings into Qiskit circuits
 Home-page: https://github.com/jakelishman/qiskit-qasm2
 Author: Jake Lishman
 License: Apache 2.0 License
 Project-URL: Bug Tracker, https://github.com/jakelishman/qiskit-qasm2/issues
 Project-URL: Documentation, https://jakelishman.github.io/qiskit-qasm2
 Project-URL: Source Code, https://github.com/jakelishman/qiskit-qasm2
 Description-Content-Type: text/markdown; variant=GFM
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: qiskit-terra>=0.21.0
+Requires-Dist: typing_extensions>=4.1.0
+Provides-Extra: all
 
 # Importer from OpenQASM 2 to Qiskit
 
 [![License](https://img.shields.io/github/license/jakelishman/qiskit-qasm2.svg?style=flat)](https://opensource.org/licenses/Apache-2.0) [![Release](https://img.shields.io/github/release/jakelishman/qiskit-qasm2.svg?style=flat)](https://github.com/jakelishman/qiskit-qasm2/releases) [![Downloads](https://img.shields.io/pypi/dm/qiskit-qasm2.svg?style=flat)](https://pypi.org/project/qiskit-qasm2/) [![Coverage Status](https://coveralls.io/repos/github/jakelishman/qiskit-qasm2/badge.svg?branch=main)](https://coveralls.io/github/jakelishman/qiskit-qasm2?branch=main)
 
+> [!IMPORTANT]
+>
+> This package is obsolete.  It was vendored into Qiskit itself as of `qiskit==0.43.0` (via
+> `qiskit-terra==0.24.0` at the time), at version `0.5.3` of this package.  There is no longer any
+> need to install this package; simply use `qiskit.qasm2.load` or `qiskit.qasm2.loads`.  The Qiskit
+> version is actively developed, and this package is not being updated any more.
+>
+> All references to Qiskit in the README and in the package itself mean Qiskit versions `<0.43`,
+> before this package was vendored into Qiskit.
+
 This repository provides the Python package `qiskit_qasm2`, which provides a
 fast parser of OpenQASM 2 into Qiskit's `QuantumCircuit`.  It is often 10x or
 more faster than Qiskit's native parser.  The API is simple:
 
 - `qiskit_qasm2.load` takes a filename, and returns `QuantumCircuit`;
 - `qiskit_qasm2.loads` takes an OpenQASM 2 program in a string, and returns
   `QuantumCircuit`.
```

### Comparing `qiskit_qasm2-0.5.3/src-python/qiskit_qasm2.egg-info/SOURCES.txt` & `qiskit_qasm2-0.5.3.1/src-python/qiskit_qasm2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-rust/bytecode.rs` & `qiskit_qasm2-0.5.3.1/src-rust/bytecode.rs`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-rust/error.rs` & `qiskit_qasm2-0.5.3.1/src-rust/error.rs`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-rust/expr.rs` & `qiskit_qasm2-0.5.3.1/src-rust/expr.rs`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-rust/lex.rs` & `qiskit_qasm2-0.5.3.1/src-rust/lex.rs`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-rust/lib.rs` & `qiskit_qasm2-0.5.3.1/src-rust/lib.rs`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/src-rust/parse.rs` & `qiskit_qasm2-0.5.3.1/src-rust/parse.rs`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/tests/test_arxiv_examples.py` & `qiskit_qasm2-0.5.3.1/tests/test_arxiv_examples.py`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/tests/test_expression.py` & `qiskit_qasm2-0.5.3.1/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/tests/test_lexer.py` & `qiskit_qasm2-0.5.3.1/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/tests/test_parse_errors.py` & `qiskit_qasm2-0.5.3.1/tests/test_parse_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_qasm2-0.5.3/tests/test_structure.py` & `qiskit_qasm2-0.5.3.1/tests/test_structure.py`

 * *Files identical despite different names*

