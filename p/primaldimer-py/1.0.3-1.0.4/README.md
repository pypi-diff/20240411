# Comparing `tmp/primaldimer_py-1.0.3.tar.gz` & `tmp/primaldimer_py-1.0.4.tar.gz`

## Comparing `primaldimer_py-1.0.3.tar` & `primaldimer_py-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 primaldimer_py-1.0.3/Cargo.toml
--rw-r--r--   0     1001      127     2825 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      104 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/.gitmodules
--rw-r--r--   0     1001      127    20131 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/LICENSE
--rw-r--r--   0     1001      127      179 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/README.md
--rw-r--r--   0     1001      127      554 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/measure.py
--rw-r--r--   0     1001      127    48016 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/profile.svg
--rw-r--r--   0     1001      127     1077 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/src/lib.rs
--rw-r--r--   0     1001      127     8574 2023-11-30 12:44:42.000000 primaldimer_py-1.0.3/Cargo.lock
--rw-r--r--   0     1001      127      320 2023-11-30 12:44:27.000000 primaldimer_py-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 primaldimer_py-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 primaldimer_py-1.0.4/Cargo.toml
+-rw-r--r--   0     1001      127     2825 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      104 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/.gitmodules
+-rw-r--r--   0     1001      127    20131 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/LICENSE
+-rw-r--r--   0     1001      127      179 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/README.md
+-rw-r--r--   0     1001      127      554 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/measure.py
+-rw-r--r--   0     1001      127    48016 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/profile.svg
+-rw-r--r--   0     1001      127     1077 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/src/lib.rs
+-rw-r--r--   0     1001      127     8574 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/Cargo.lock
+-rw-r--r--   0     1001      127      320 2024-04-10 22:07:05.000000 primaldimer_py-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 primaldimer_py-1.0.4/PKG-INFO
```

### Comparing `primaldimer_py-1.0.3/.github/workflows/CI.yml` & `primaldimer_py-1.0.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `primaldimer_py-1.0.3/LICENSE` & `primaldimer_py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `primaldimer_py-1.0.3/measure.py` & `primaldimer_py-1.0.4/measure.py`

 * *Files identical despite different names*

### Comparing `primaldimer_py-1.0.3/profile.svg` & `primaldimer_py-1.0.4/profile.svg`

 * *Files identical despite different names*

### Comparing `primaldimer_py-1.0.3/src/lib.rs` & `primaldimer_py-1.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `primaldimer_py-1.0.3/Cargo.lock` & `primaldimer_py-1.0.4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.12.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25db6b064527c5d482d0423354fcd07a89a2dfe07b67892e62411946db7f07b0"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
@@ -102,26 +102,26 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "primaldimer_py"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = [
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "primaldimer_rs",
  "pyo3",
 ]
 
 [[package]]
 name = "primaldimer_rs"
-version = "0.1.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d22df8a5178c071ca5d1d342621c0578036ab0a42d41147e21b62a2b1208111"
+checksum = "49e6051ab22611855ec6a3e94244336f5e6b7cdbf6645a836f72b5bf30450ad7"
 dependencies = [
  "itertools 0.10.5",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.58"
```

### Comparing `primaldimer_py-1.0.3/PKG-INFO` & `primaldimer_py-1.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: primaldimer_py
-Version: 1.0.3
+Version: 1.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

