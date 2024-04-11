# Comparing `tmp/polars_hash-0.4.7.tar.gz` & `tmp/polars_hash-0.4.8.tar.gz`

## Comparing `polars_hash-0.4.7.tar` & `polars_hash-0.4.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 polars_hash-0.4.7/Cargo.toml
--rw-r--r--   0     1001      127      933 2024-03-24 00:06:47.000000 polars_hash-0.4.7/Makefile
--rw-r--r--   0     1001      127     3173 2024-03-24 00:06:47.000000 polars_hash-0.4.7/README.md
--rw-r--r--   0     1001      127     7389 2024-03-24 00:06:47.000000 polars_hash-0.4.7/polars_hash/__init__.py
--rw-r--r--   0     1001      127       17 2024-03-24 00:06:47.000000 polars_hash-0.4.7/polars_hash/_internal.pyi
--rw-r--r--   0     1001      127        0 2024-03-24 00:06:47.000000 polars_hash-0.4.7/polars_hash/py.typed
--rw-r--r--   0     1001      127       37 2024-03-24 00:06:47.000000 polars_hash-0.4.7/requirements.txt
--rw-r--r--   0     1001      127     7914 2024-03-24 00:06:47.000000 polars_hash-0.4.7/src/expressions.rs
--rw-r--r--   0     1001      127     4140 2024-03-24 00:06:47.000000 polars_hash-0.4.7/src/geohashers.rs
--rw-r--r--   0     1001      127      396 2024-03-24 00:06:47.000000 polars_hash-0.4.7/src/lib.rs
--rw-r--r--   0     1001      127     1403 2024-03-24 00:06:47.000000 polars_hash-0.4.7/src/sha_hashers.rs
--rw-r--r--   0     1001      127     4799 2024-03-24 00:06:47.000000 polars_hash-0.4.7/tests/test_hash.py
--rw-r--r--   0     1001      127    51482 2024-03-24 00:06:58.000000 polars_hash-0.4.7/Cargo.lock
--rw-r--r--   0     1001      127      897 2024-03-24 00:06:47.000000 polars_hash-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     3834 1970-01-01 00:00:00.000000 polars_hash-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 polars_hash-0.4.8/Cargo.toml
+-rw-r--r--   0     1001      127      933 2024-04-11 20:28:28.000000 polars_hash-0.4.8/Makefile
+-rw-r--r--   0     1001      127     3173 2024-04-11 20:28:28.000000 polars_hash-0.4.8/README.md
+-rw-r--r--   0     1001      127     7950 2024-04-11 20:28:28.000000 polars_hash-0.4.8/polars_hash/__init__.py
+-rw-r--r--   0     1001      127       17 2024-04-11 20:28:28.000000 polars_hash-0.4.8/polars_hash/_internal.pyi
+-rw-r--r--   0     1001      127        0 2024-04-11 20:28:28.000000 polars_hash-0.4.8/polars_hash/py.typed
+-rw-r--r--   0     1001      127       37 2024-04-11 20:28:28.000000 polars_hash-0.4.8/requirements.txt
+-rw-r--r--   0     1001      127     9561 2024-04-11 20:28:28.000000 polars_hash-0.4.8/src/expressions.rs
+-rw-r--r--   0     1001      127     4140 2024-04-11 20:28:28.000000 polars_hash-0.4.8/src/geohashers.rs
+-rw-r--r--   0     1001      127     1615 2024-04-11 20:28:28.000000 polars_hash-0.4.8/src/h3.rs
+-rw-r--r--   0     1001      127      404 2024-04-11 20:28:28.000000 polars_hash-0.4.8/src/lib.rs
+-rw-r--r--   0     1001      127     1403 2024-04-11 20:28:28.000000 polars_hash-0.4.8/src/sha_hashers.rs
+-rw-r--r--   0     1001      127     5314 2024-04-11 20:28:28.000000 polars_hash-0.4.8/tests/test_hash.py
+-rw-r--r--   0     1001      127    53372 2024-04-11 20:28:32.000000 polars_hash-0.4.8/Cargo.lock
+-rw-r--r--   0     1001      127      897 2024-04-11 20:28:28.000000 polars_hash-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     3834 1970-01-01 00:00:00.000000 polars_hash-0.4.8/PKG-INFO
```

### Comparing `polars_hash-0.4.7/Cargo.toml` & `polars_hash-0.4.8/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_hash"
-version = "0.4.7"
+version = "0.4.8"
 edition = "2021"
 
 [lib]
 name = "polars_hash"
 crate-type = ["cdylib"]
 
 [dependencies]
@@ -16,11 +16,12 @@
 wyhash = { version = "0.5.0" }
 geohash = { version = "0.13.0" }
 sha1 = { version = "0.10.6" }
 sha2 = { version = "0.10.8" }
 sha3 = { version = "0.10.8" }
 blake3 = { version = "1.5.0" }
 md5 = {version = "0.7.0"}
+h3o = { version = "0.6.2" }
 
 
 [target.'cfg(target_os = "linux")'.dependencies]
 jemallocator = { version = "0.5", features = ["disable_initial_exec_tls"] }
```

### Comparing `polars_hash-0.4.7/Makefile` & `polars_hash-0.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `polars_hash-0.4.7/README.md` & `polars_hash-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `polars_hash-0.4.7/polars_hash/__init__.py` & `polars_hash-0.4.8/polars_hash/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,27 +174,46 @@
             plugin_path=Path(__file__).parent,
             function_name="ghash_neighbors",
             args=self._expr,
             is_elementwise=True,
         )
 
 
+@pl.api.register_expr_namespace("h3")
+class H3NameSpace:
+    def __init__(self, expr: pl.Expr):
+        self._expr = expr
+
+    def from_coords(self, len: int = 12) -> pl.Expr:
+        """Takes Struct with latitude, longitude as input and returns utf8 H3 spatial index."""
+        return register_plugin_function(
+            plugin_path=Path(__file__).parent,
+            args=[self._expr, len],
+            function_name="h3_encode",
+            is_elementwise=True,
+        )
+
+
 class HExpr(pl.Expr):
     @property
     def chash(self) -> CryptographicHashingNameSpace:
         return CryptographicHashingNameSpace(self)
 
     @property
     def nchash(self) -> NonCryptographicHashingNameSpace:
         return NonCryptographicHashingNameSpace(self)
 
     @property
     def geohash(self) -> GeoHashingNameSpace:
         return GeoHashingNameSpace(self)
 
+    @property
+    def h3(self) -> H3NameSpace:
+        return H3NameSpace(self)
+
 
 class HashColumn(Protocol):
     def __call__(
         self,
         name: str | PolarsDataType | Iterable[str] | Iterable[PolarsDataType],
         *more_names: str | PolarsDataType,
     ) -> HExpr: ...
```

### Comparing `polars_hash-0.4.7/src/expressions.rs` & `polars_hash-0.4.8/src/expressions.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use crate::geohashers::{geohash_decoder, geohash_encoder, geohash_neighbors};
+use crate::h3::h3_encoder;
 use crate::sha_hashers::*;
 use polars::{
     chunked_array::ops::arity::{try_binary_elementwise, try_ternary_elementwise},
     prelude::*,
 };
 use polars_core::datatypes::{
     DataType::{Float64, String, Struct},
@@ -208,14 +209,57 @@
             )),
         },
         _ => try_ternary_elementwise(ca_lat, ca_long, len, geohash_encoder),
     }?;
     Ok(out.into_series())
 }
 
+#[polars_expr(output_type=String)]
+fn h3_encode(inputs: &[Series]) -> PolarsResult<Series> {
+    let ca = inputs[0].struct_()?;
+    let len = match inputs[1].dtype() {
+        DataType::Int64 => inputs[1].clone(),
+        DataType::Int32 => inputs[1].cast(&DataType::Int64)?,
+        DataType::Int16 => inputs[1].cast(&DataType::Int64)?,
+        DataType::Int8 => inputs[1].cast(&DataType::Int64)?,
+        _ => polars_bail!(InvalidOperation:"Length input needs to be integer"),
+    };
+    let len = len.i64()?;
+
+    let lat = ca.field_by_name("latitude")?;
+    let long = ca.field_by_name("longitude")?;
+    let lat = match lat.dtype() {
+        DataType::Float32 => lat.cast(&DataType::Float64)?,
+        DataType::Float64 => lat,
+        _ => polars_bail!(InvalidOperation:"Latitude input needs to be float"),
+    };
+
+    let long = match long.dtype() {
+        DataType::Float32 => long.cast(&DataType::Float64)?,
+        DataType::Float64 => long,
+        _ => polars_bail!(InvalidOperation:"Longitude input needs to be float"),
+    };
+
+    let ca_lat = lat.f64()?;
+    let ca_long = long.f64()?;
+
+    let out: StringChunked = match len.len() {
+        1 => match unsafe { len.get_unchecked(0) } {
+            Some(len) => try_binary_elementwise(ca_lat, ca_long, |ca_lat_opt, ca_long_opt| {
+                h3_encoder(ca_lat_opt, ca_long_opt, Some(len))
+            }),
+            _ => Err(PolarsError::ComputeError(
+                "Length may not be null".to_string().into(),
+            )),
+        },
+        _ => try_ternary_elementwise(ca_lat, ca_long, len, h3_encoder),
+    }?;
+    Ok(out.into_series())
+}
+
 pub fn geohash_decode_output(field: &[Field]) -> PolarsResult<Field> {
     let v: Vec<Field> = vec![
         Field::new("longitude", Float64),
         Field::new("latitude", Float64),
     ];
     Ok(Field::new(field[0].name(), Struct(v)))
 }
```

### Comparing `polars_hash-0.4.7/src/geohashers.rs` & `polars_hash-0.4.8/src/geohashers.rs`

 * *Files identical despite different names*

### Comparing `polars_hash-0.4.7/src/sha_hashers.rs` & `polars_hash-0.4.8/src/sha_hashers.rs`

 * *Files identical despite different names*

### Comparing `polars_hash-0.4.7/tests/test_hash.py` & `polars_hash-0.4.8/tests/test_hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,34 @@
     assert_frame_equal(result, expected)
     assert_frame_equal(
         df.select(pl.col("coord").geohash.from_coords(12).geohash.to_coords()),
         df,  # type: ignore
     )
 
 
+def test_h3():
+    df = pl.DataFrame(
+        {"coord": [{"longitude": -120.6623, "latitude": 35.3003}]},
+        schema={
+            "coord": pl.Struct(
+                [pl.Field("longitude", pl.Float64), pl.Field("latitude", pl.Float64)]
+            ),
+        },
+    )
+
+    result = df.select(pl.col("coord").h3.from_coords(5))  # type: ignore
+
+    expected = pl.DataFrame(
+        [
+            pl.Series("coord", ["8529adc7fffffff"], dtype=pl.Utf8),
+        ]
+    )
+    assert_frame_equal(result, expected)
+
+
 def test_lazy_name():
     result = (
         pl.from_dicts({"h1": "sp1xk2m6194y"})
         .lazy()
         .with_columns(pl.col("h1").geohash.neighbors())
         .unnest("h1")
         .collect()
```

### Comparing `polars_hash-0.4.7/Cargo.lock` & `polars_hash-0.4.8/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [[package]]
 name = "ahash"
 version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
+ "const-random",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
@@ -94,17 +95,17 @@
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
@@ -140,17 +141,17 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
@@ -161,15 +162,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -178,33 +179,33 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "windows-targets 0.52.4",
 ]
 
@@ -228,25 +229,45 @@
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
 name = "comfy-table"
-version = "7.1.0"
+version = "7.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c64043d6c7b7a4c58e39e7efccfdea7b93d885a795d0c054a69dbbf4dd52686"
+checksum = "b34115915337defe99b2aff5c2ce6771e5fbc4079f4b506301f5cf394c8452f7"
 dependencies = [
  "crossterm",
  "strum",
- "strum_macros",
+ "strum_macros 0.26.2",
  "unicode-width",
 ]
 
 [[package]]
+name = "const-random"
+version = "0.1.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87e00182fe74b066627d63b85fd550ac2998d4b0bd86bfed477a0ae4c7c71359"
+dependencies = [
+ "const-random-macro",
+]
+
+[[package]]
+name = "const-random-macro"
+version = "0.1.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9d839f2a20b0aee515dc581a6172f2321f96cab76c1a38a4c584a194955390e"
+dependencies = [
+ "getrandom",
+ "once_cell",
+ "tiny-keccak",
+]
+
+[[package]]
 name = "constant_time_eq"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
 
 [[package]]
 name = "core-foundation-sys"
@@ -325,14 +346,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acdd7c62a3665c7f6830a51635d9ac9b23ed385797f70a83bb8bafe9c572ab2b"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
@@ -358,22 +385,22 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.12"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -393,14 +420,20 @@
 [[package]]
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
+name = "float_eq"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "28a80e3145d8ad11ba0995949bbcf48b9df2be62772b3d351ef017dff6ecb853"
+
+[[package]]
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "generic-array"
@@ -431,17 +464,17 @@
 dependencies = [
  "geo-types",
  "libm",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -449,14 +482,33 @@
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
+name = "h3o"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d55005adb5818b0ed10969a17f87610a3be88d7c00c0a6fa950f045c990c8a46"
+dependencies = [
+ "ahash",
+ "either",
+ "float_eq",
+ "h3o-bit",
+ "libm",
+]
+
+[[package]]
+name = "h3o-bit"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fb45e8060378c0353781abf67e1917b545a6b710d0342d85b70c125af7ef320"
+
+[[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
  "ahash",
  "allocator-api2",
@@ -527,17 +579,17 @@
 name = "iter-read"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "itoap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9028f49264629065d057f340a86acb84867925865f73bbf8d47b4d149a7e88b8"
 
@@ -559,17 +611,17 @@
 dependencies = [
  "jemalloc-sys",
  "libc",
 ]
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "f08474e32172238f2827bd160c67871cdb2801430f65c3979184dc362e3ca118"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -640,32 +692,32 @@
 name = "md5"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "490cc448043f947bae3cbee9c203358d62dbee0db12107a74be5c30ccfd09771"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "multiversion"
 version = "0.7.4"
@@ -1117,15 +1169,15 @@
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
  "regex",
  "smartstring",
- "strum_macros",
+ "strum_macros 0.25.3",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1193,18 +1245,19 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_hash"
-version = "0.4.7"
+version = "0.4.8"
 dependencies = [
  "blake3",
  "geohash",
+ "h3o",
  "jemallocator",
  "md5",
  "polars",
  "polars-arrow",
  "pyo3",
  "pyo3-polars",
  "serde",
@@ -1278,28 +1331,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-polars"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6ab8ad08494161085fb0d2d9de82c7fde7398da1778ee7e7a5a596ff4201f5b"
@@ -1322,22 +1375,22 @@
 checksum = "56c67d6b47b05d3827ef8e5f4449ae1a1861f5d7086ee18c5429e347b0d03c19"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1385,17 +1438,17 @@
 checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1437,23 +1490,23 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -1495,22 +1548,22 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1608,29 +1661,42 @@
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
 name = "strum"
-version = "0.25.0"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
+checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 
 [[package]]
 name = "strum_macros"
 version = "0.25.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.53",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "strum_macros"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1638,28 +1704,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.30.7"
+version = "0.30.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c385888ef380a852a16209afc8cfad22795dd8873d69c9a14d2e2088f118d18"
+checksum = "26d7c217777061d5a2d652aea771fb9ba98b6dade657204b08c4b9604d11555b"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "windows",
@@ -1690,15 +1756,24 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "tiny-keccak"
+version = "2.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
+dependencies = [
+ "crunchy",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
@@ -1774,15 +1849,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1796,15 +1871,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2003,37 +2078,37 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `polars_hash-0.4.7/pyproject.toml` & `polars_hash-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_hash-0.4.7/PKG-INFO` & `polars_hash-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-hash
-Version: 0.4.7
+Version: 0.4.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Summary: Stable non-cryptographic and cryptographic hashing functions for Polars
 Author-email: Ion Koutsours <15728914+ion-elgreco@users.noreply.github.com>
 Requires-Python: >=3.8
```

