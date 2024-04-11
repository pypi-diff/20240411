# Comparing `tmp/rs1090-0.1.3.tar.gz` & `tmp/rs1090-0.2.0.tar.gz`

## Comparing `rs1090-0.1.3.tar` & `rs1090-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,68 @@
--rw-r--r--   0     1001      127      897 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/Cargo.toml
--rw-r--r--   0     1001      127     2869 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/benches/long_flight.rs
--rw-r--r--   0     1001      127 10186581 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/data/long_flight.csv
--rw-r--r--   0     1001      127      319 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/examples/basic.rs
--rw-r--r--   0     1001      127     2263 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/examples/flight.rs
--rw-r--r--   0     1001      127     2423 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/readme.md
--rw-r--r--   0     1001      127     4956 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/adsb.rs
--rw-r--r--   0     1001      127     4794 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds05.rs
--rw-r--r--   0     1001      127     5334 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds06.rs
--rw-r--r--   0     1001      127     7757 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds08.rs
--rw-r--r--   0     1001      127    14730 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds09.rs
--rw-r--r--   0     1001      127     4676 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds10.rs
--rw-r--r--   0     1001      127     6121 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds17.rs
--rw-r--r--   0     1001      127     1723 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds20.rs
--rw-r--r--   0     1001      127     5789 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds30.rs
--rw-r--r--   0     1001      127     5096 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds40.rs
--rw-r--r--   0     1001      127     5848 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds44.rs
--rw-r--r--   0     1001      127     6574 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds50.rs
--rw-r--r--   0     1001      127     7095 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds60.rs
--rw-r--r--   0     1001      127     2461 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds61.rs
--rw-r--r--   0     1001      127     8978 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds62.rs
--rw-r--r--   0     1001      127    12441 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/bds65.rs
--rw-r--r--   0     1001      127      493 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/bds/mod.rs
--rw-r--r--   0     1001      127     6285 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/commb.rs
--rw-r--r--   0     1001      127    15802 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/cpr.rs
--rw-r--r--   0     1001      127     6422 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/crc.rs
--rw-r--r--   0     1001      127        1 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/flarm.rs
--rw-r--r--   0     1001      127    26840 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/decode/mod.rs
--rw-r--r--   0     1001      127      997 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/lib.rs
--rw-r--r--   0     1001      127     3639 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/source/beast.rs
--rw-r--r--   0     1001      127       15 2024-03-08 19:08:27.000000 rs1090-0.1.3/crates/rs1090/src/source/mod.rs
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 rs1090-0.1.3/python/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/.gitignore
--rw-r--r--   0     1001      127      651 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/examples/basic_bench.py
--rw-r--r--   0     1001      127      753 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/examples/long_flight.py
--rw-r--r--   0     1001      127   732057 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/examples/minimal.parquet
--rw-r--r--   0     1001      127     1112 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/readme.md
--rw-r--r--   0     1001      127     1736 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/rs1090/__init__.py
--rw-r--r--   0     1001      127      502 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/rs1090/_rust.pyi
--rw-r--r--   0     1001      127        0 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/rs1090/py.typed
--rw-r--r--   0     1001      127     3938 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/src/lib.rs
--rw-r--r--   0     1001      127     1509 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/tests/test_adsb.py
--rw-r--r--   0     1001      127     1010 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/tests/test_commb.py
--rw-r--r--   0     1001      127     1082 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/tests/test_common.py
--rw-r--r--   0     1001      127      423 2024-03-08 19:08:27.000000 rs1090-0.1.3/python/tests/test_full.py
--rw-r--r--   0     1001      127    39709 2024-03-08 19:08:27.000000 rs1090-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rs1090-0.1.3/Cargo.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 rs1090-0.1.3/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-03-08 19:08:27.000000 rs1090-0.1.3/rs1090/py.typed
--rw-r--r--   0     1001      127      502 2024-03-08 19:08:27.000000 rs1090-0.1.3/rs1090/_rust.pyi
--rw-r--r--   0     1001      127     1736 2024-03-08 19:08:27.000000 rs1090-0.1.3/rs1090/__init__.py
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 rs1090-0.1.3/PKG-INFO
+-rw-r--r--   0     1001      127     1097 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/Cargo.toml
+-rw-r--r--   0     1001      127     2869 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/benches/long_flight.rs
+-rw-r--r--   0     1001      127  1829500 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/data/airports.json
+-rw-r--r--   0     1001      127 13658890 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/data/flarm.csv
+-rw-r--r--   0     1001      127 10186581 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/data/long_flight.csv
+-rw-r--r--   0     1001      127    56601 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/data/patterns.json
+-rw-r--r--   0     1001      127      640 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/examples/airports.rs
+-rw-r--r--   0     1001      127      319 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/examples/basic.rs
+-rw-r--r--   0     1001      127     2341 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/examples/flight.rs
+-rw-r--r--   0     1001      127     4427 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/readme.md
+-rw-r--r--   0     1001      127     1414 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/data/airports.rs
+-rw-r--r--   0     1001      127       50 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/data/mod.rs
+-rw-r--r--   0     1001      127     1132 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/data/patterns.rs
+-rw-r--r--   0     1001      127    16778 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/data/tail.rs
+-rw-r--r--   0     1001      127     4956 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/adsb.rs
+-rw-r--r--   0     1001      127     4794 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds05.rs
+-rw-r--r--   0     1001      127     5338 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds06.rs
+-rw-r--r--   0     1001      127     7761 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds08.rs
+-rw-r--r--   0     1001      127    14592 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds09.rs
+-rw-r--r--   0     1001      127     4713 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds10.rs
+-rw-r--r--   0     1001      127     6158 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds17.rs
+-rw-r--r--   0     1001      127     1760 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds20.rs
+-rw-r--r--   0     1001      127     5945 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds30.rs
+-rw-r--r--   0     1001      127     5133 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds40.rs
+-rw-r--r--   0     1001      127     5885 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds44.rs
+-rw-r--r--   0     1001      127     6611 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds50.rs
+-rw-r--r--   0     1001      127     7132 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds60.rs
+-rw-r--r--   0     1001      127     2461 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds61.rs
+-rw-r--r--   0     1001      127     8982 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds62.rs
+-rw-r--r--   0     1001      127    12441 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/bds65.rs
+-rw-r--r--   0     1001      127      225 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/bds/mod.rs
+-rw-r--r--   0     1001      127     6285 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/commb.rs
+-rw-r--r--   0     1001      127    19245 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/cpr.rs
+-rw-r--r--   0     1001      127     6422 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/crc.rs
+-rw-r--r--   0     1001      127    14003 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/flarm.rs
+-rw-r--r--   0     1001      127    27430 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/decode/mod.rs
+-rw-r--r--   0     1001      127     1172 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/lib.rs
+-rw-r--r--   0     1001      127     3963 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/source/beast.rs
+-rw-r--r--   0     1001      127       78 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/source/mod.rs
+-rw-r--r--   0     1001      127     2422 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/source/radarcape.rs
+-rw-r--r--   0     1001      127    20992 2024-04-11 06:32:34.000000 rs1090-0.2.0/crates/rs1090/src/source/rtlsdr.rs
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 rs1090-0.2.0/python/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/.gitignore
+-rw-r--r--   0     1001      127     8431 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/examples/bench_pms.py
+-rw-r--r--   0     1001      127     2255 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/examples/benchmark.py
+-rw-r--r--   0     1001      127    15135 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/examples/benchmark.svg
+-rw-r--r--   0     1001      127    54306 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/examples/flarm.png
+-rw-r--r--   0     1001      127     2266 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/examples/flarm.py
+-rw-r--r--   0     1001      127      753 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/examples/long_flight.py
+-rw-r--r--   0     1001      127     1654 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/readme.md
+-rw-r--r--   0     1001      127     4333 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/rs1090/__init__.py
+-rw-r--r--   0     1001      127      589 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/rs1090/_rust.pyi
+-rw-r--r--   0     1001      127        0 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/rs1090/py.typed
+-rw-r--r--   0     1001      127    18575 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/rs1090/stubs.py
+-rw-r--r--   0     1001      127     4555 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/src/lib.rs
+-rw-r--r--   0     1001      127     2091 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/tests/test_adsb.py
+-rw-r--r--   0     1001      127     1340 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/tests/test_commb.py
+-rw-r--r--   0     1001      127     1282 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/tests/test_common.py
+-rw-r--r--   0     1001      127     1554 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/tests/test_flarm.py
+-rw-r--r--   0     1001      127      423 2024-04-11 06:32:34.000000 rs1090-0.2.0/python/tests/test_full.py
+-rw-r--r--   0     1001      127    64586 2024-04-11 06:32:34.000000 rs1090-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 rs1090-0.2.0/Cargo.toml
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rs1090-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      127     4333 2024-04-11 06:32:34.000000 rs1090-0.2.0/rs1090/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-11 06:32:34.000000 rs1090-0.2.0/rs1090/py.typed
+-rw-r--r--   0     1001      127      589 2024-04-11 06:32:34.000000 rs1090-0.2.0/rs1090/_rust.pyi
+-rw-r--r--   0     1001      127    18575 2024-04-11 06:32:34.000000 rs1090-0.2.0/rs1090/stubs.py
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 rs1090-0.2.0/PKG-INFO
```

### Comparing `rs1090-0.1.3/crates/rs1090/Cargo.toml` & `rs1090-0.2.0/crates/rs1090/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,37 @@
 keywords = ["aircraft", "ADS-B", "Mode-S", "decoding"]
 readme = "readme.md"
 authors.workspace = true
 version.workspace = true
 license.workspace = true
 edition.workspace = true
 
+[features]
+rtlsdr = ['soapysdr']
+
 [dependencies]
+ansi_term = "0.12.1"
 async-stream = "0.3.5"
 deku = "0.16.0"
 futures = "0.3.30"
 futures-util = "0.3.30"
+hex = "0.4.3"
 libm = "0.2.8"
+num-complex = "0.4.5"
+once_cell = "1.19.0"
 rayon = "1.9.0"
-serde = { version="1.0.197", features = ["derive"] }
+regex = "1.10.3"
+serde = { version = "1.0.197", features = ["derive"] }
 serde_json = "1.0.114"
-tokio = { version="1.36.0", features = ["full"] }
+soapysdr = { version = "0.4.0", optional = true }
+tokio = { version = "1.36.0", features = ["full"] }
 
 [dev-dependencies]
 approx = "0.5.1"
 criterion = "0.5.1"
-hex = "0.4.3"
 hexlit = "0.5.5"
 
 [[bench]]
 name = "long_flight"
 harness = false
 
 [[example]]
@@ -38,7 +46,10 @@
 [[example]]
 name = "decode_file"
 path = "examples/flight.rs"
 test = false
 
 # [[example]]
 # name = "tcas_incidents"
+
+[[example]]
+name = "airports"
```

### Comparing `rs1090-0.1.3/crates/rs1090/benches/long_flight.rs` & `rs1090-0.2.0/crates/rs1090/benches/long_flight.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/data/long_flight.csv` & `rs1090-0.2.0/crates/rs1090/data/long_flight.csv`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/examples/flight.rs` & `rs1090-0.2.0/crates/rs1090/examples/flight.rs`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,17 @@
                     parts.next().unwrap().parse::<f64>().expect("not a float");
                 let msg = parts.next().unwrap();
                 let hex = &mut msg.to_string()[18..].to_string();
                 let bytes = hex::decode(&hex).unwrap();
                 let (_, msg) = Message::from_bytes((&bytes, 0)).unwrap();
                 res.push(TimedMessage {
                     timestamp,
-                    message: msg,
+                    frame: hex.to_string(),
+                    message: Some(msg),
+                    idx: 0,
                 });
             }
             res
         })
         .flat_map(|v| v)
         .collect();
```

### Comparing `rs1090-0.1.3/crates/rs1090/readme.md` & `rs1090-0.2.0/python/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,60 @@
 # rs1090
 
-rs1090 is a Rust library to decode Mode S and ADS-B messages.
+rs1090 is a Python binding to the [rs1090](https://docs.rs/rs1090/) Rust library to decode Mode S, ADS-B and FLARM messages. It takes its inspiration from the Python [pyModeS](https://github.com/junzis/pyModeS) library.
 
-It takes its inspiration from the Python [pyModeS](https://github.com/junzis/pyModeS) library, and uses [deku](https://github.com/sharksforarms/deku) in order to decode binary data in a clean declarative way.
-
-The project started as a fork of a very similar project called [adsb-deku](https://crates.io/crates/adsb_deku), but modules have been refactored to match [pyModeS](https://github.com/junzis/pyModeS) design, implementations extensively reviewed, simplified, corrected, and completed.
-
-The direction ambitioned by rs1090 boil down to:
+The direction ambitioned by rs1090 boils down to:
 
 - improving the performance of Mode S decoding in Python;
 - exporting trajectory data to cross-platform formats such as JSON or parquet;
 - providing efficient multi-receiver Mode S decoding;
 - serving real-time enriched trajectory data to external applications.
 
-If you just want to decode ADS-B messages from your Raspberry and visualize the data on a map, you may want to stick to one of the dump0190 implementations.
-
-The rs1090 library comes with a companion application [decode1090](https://crates.io/crates/decode1090) and a Python binding [rs1090](https://pypi.org/project/rs1090).
-
 ## Installation
 
-Run the following Cargo command in your project directory:
-
-```sh
-cargo add rs1090
-```
-
-Or add the following line to your `Cargo.toml`:
-
-```toml
-rs1090 = "0.2.0"  # check for the latest version
-```
-
-For the Python binding:
-
 ```sh
 pip install rs1090
 ```
 
 ## Usage
 
-In Rust:
-
-```rust
-use hexlit::hex;
-use rs1090::prelude::*;
-
-fn main() {
-    let bytes: [u8; 14] = hex!("8c4841753a9a153237aef0f275be");
-    // ADS-B decoding
-    if let Ok((_, msg)) = Message::from_bytes((&bytes, 0)) {
-        // JSON output
-        let json = serde_json::to_string(&msg).expect("JSON error");
-        println!("{}", json);
-    }
-}
-```
-
-In Python:
+For single messages:
 
 ```pycon
 >>> import rs1090
 >>> rs1090.decode("8c4841753a9a153237aef0f275be")
 {'df': '17', 'icao24': '484175', 'bds': '06', 'NUCp': 7, 'groundspeed': 17.0, 'track': 92.8125, 'parity': 'odd', 'lat_cpr': 39195, 'lon_cpr': 110320}
 ```
 
-For large sets of messages in Python (e.g. what you can download through [pyopensky](https://github.com/open-aviation/pyopensky)):
+For batches of messages:
 
 ```pycon
 >>> import rs1090
+>>> rs1090.decode(msg_list)
+...
 >>> rs1090.decode(msg_list, ts_list)  # includes CPR to position decoding
 ...
 >>> rs1090.decode(msg_list, ts_list, reference=(lat0, lon0))  # useful for surface messages
 ...
 ```
+
+For FLARM messages (also as batches):
+
+```pycon
+>>> msg = "7bf2381040ccc7e2395ecaa28e033a655d47e1d91d0bf986e1b0"
+>>> rs1090.flarm(msg, 1655279476, 43.61924, 5.11755)
+{'timestamp': 1655279476,
+ 'reference_lat': 43.61924,
+ 'reference_lon': 5.11755,
+ 'icao24': '38f27b',
+ 'is_icao24': True,
+ 'actype': 'Glider',
+ 'latitude': 43.6812864,
+ 'longitude': 5.150585599999999,
+ 'geoaltitude': 970,
+ 'vertical_speed': 1.0,
+ 'groundspeed': 18.698261951315153,
+ 'track': 29.655457935479006,
+ 'no_track': False,
+ 'stealth': False,
+ 'gps': 129}
+```
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/adsb.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/adsb.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds05.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds05.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds06.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds06.rs`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     use hexlit::hex;
 
     #[test]
     fn test_surface_position() {
         let bytes = hex!("8c4841753a9a153237aef0f275be");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
         if let ExtendedSquitterADSB(adsb_msg) = msg.df {
-            if let BDS06(SurfacePosition {
+            if let ME::BDS06(SurfacePosition {
                 track, groundspeed, ..
             }) = adsb_msg.message
             {
                 assert_eq!(track, Some(92.8125));
                 assert_eq!(groundspeed, Some(17.));
                 return;
             }
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds08.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds08.rs`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     use hexlit::hex;
 
     #[test]
     fn test_callsign() {
         let bytes = hex!("8d406b902015a678d4d220aa4bda");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
         if let ExtendedSquitterADSB(adsb_msg) = msg.df {
-            if let BDS08(AircraftIdentification {
+            if let ME::BDS08(AircraftIdentification {
                 tc,
                 ca,
                 callsign,
                 wake_vortex,
             }) = adsb_msg.message
             {
                 assert_eq!(format!("{tc}{ca}"), "A0");
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds09.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds09.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #![allow(clippy::suspicious_else_formatting)]
 
 use deku::bitvec::{BitSlice, Msb0};
 use deku::prelude::*;
-use serde::ser::{Serialize, SerializeStruct, Serializer};
+use serde::ser::SerializeStruct;
+use serde::Serialize;
 use std::fmt;
 
 /**
  * ## Airborne Velocity (BDS 0,9)
  *
  * Airborne velocities are all transmitted with Type Code 19. Four different
  * subtypes are defined in bits 6-8 of the ME field. All sub-types share a
@@ -21,15 +22,15 @@
  * Subtypes 2 and 4 are designed for supersonic aircraft. Their message
  * structures are identical to subtypes 1 and 3, but with the speed resolution
  * of 4 kt instead of 1 kt. However, since there are no operational supersonic
  * airliners currently, there is no ADS-B airborne velocity message with
  * subtypes 2 and 4 at this moment.
  *
  */
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
 pub struct AirborneVelocity {
     #[deku(bits = "3")]
     #[serde(skip)]
     /// The subtype value
     pub subtype: u8,
 
     #[deku(bits = "1")]
@@ -100,32 +101,30 @@
         }
     } else {
         None
     };
     Ok((rest, value))
 }
 
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
 #[deku(ctx = "subtype: u8", id = "subtype")]
 #[serde(untagged)]
 pub enum AirborneVelocitySubType {
     #[deku(id = "0")]
-    #[serde(skip)]
     Reserved0(#[deku(bits = "22")] u32),
 
     #[deku(id_pat = "1..=2")]
     GroundSpeedDecoding(GroundSpeedDecoding),
 
     #[deku(id = "3")]
     AirspeedSubsonic(AirspeedSubsonicDecoding),
     #[deku(id = "4")]
     AirspeedSupersonic(AirspeedSupersonicDecoding),
 
     #[deku(id_pat = "5..=7")]
-    #[serde(skip)]
     Reserved1(#[deku(bits = "22")] u32),
 }
 
 #[derive(Debug, PartialEq, DekuRead, Copy, Clone)]
 #[deku(type = "u8", bits = "1")]
 pub enum Sign {
     Positive = 0,
@@ -151,15 +150,15 @@
                 Self::Positive => "",
                 Self::Negative => "-",
             }
         )
     }
 }
 
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Copy, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 pub struct GroundSpeedDecoding {
     #[serde(skip)]
     pub ew_sign: Sign,
     #[deku(
         endian = "big",
         bits = "10",
         map = "|val: u16| -> Result<_, DekuError> {
@@ -201,18 +200,18 @@
     #[deku(bits = "1")]
     pub status_heading: bool,
 
     #[deku(
         endian = "big",
         bits = "10",
         map = "|val: u16| -> Result<_, DekuError> {
-            Ok(if *status_heading { Some(val as f32 * 360. / 1024.) } else { None })
+            Ok(if *status_heading { Some(val as f64 * 360. / 1024.) } else { None })
         }"
     )]
-    pub heading: Option<f32>,
+    pub heading: Option<f64>,
 
     pub airspeed_type: AirspeedType,
 
     #[deku(
         endian = "big",
         bits = "10",
         map = "|value: u16| -> Result<_, DekuError> {
@@ -222,15 +221,15 @@
     )]
     pub airspeed: Option<u16>,
 }
 
 impl Serialize for AirspeedSubsonicDecoding {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
-        S: Serializer,
+        S: serde::ser::Serializer,
     {
         let mut state = serializer.serialize_struct("Message", 2)?;
         if let Some(heading) = &self.heading {
             state.serialize_field("heading", heading)?;
         }
         if let Some(airspeed) = &self.airspeed {
             match &self.airspeed_type {
@@ -272,15 +271,15 @@
     )]
     pub airspeed: Option<u16>,
 }
 
 impl Serialize for AirspeedSupersonicDecoding {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
-        S: Serializer,
+        S: serde::ser::Serializer,
     {
         let mut state = serializer.serialize_struct("Message", 2)?;
         if let Some(heading) = &self.heading {
             state.serialize_field("heading", heading)?;
         }
         if let Some(airspeed) = &self.airspeed {
             match &self.airspeed_type {
@@ -326,15 +325,15 @@
 #[derive(Copy, Clone, Debug, PartialEq, DekuRead)]
 #[deku(type = "u8", bits = "1")]
 pub enum DirectionNS {
     SouthToNorth = 0,
     NorthToSouth = 1,
 }
 
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Copy, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 #[deku(type = "u8", bits = "1")]
 pub enum VerticalRateSource {
     #[serde(rename = "barometric")]
     BarometricPressureAltitude = 0,
 
     #[serde(rename = "GNSS")]
     GeometricAltitude = 1,
@@ -370,19 +369,15 @@
                     writeln!(
                         f,
                         "  {}:           {} kt",
                         v.airspeed_type, value
                     )?;
                 }
                 if let Some(value) = v.heading {
-                    writeln!(
-                        f,
-                        "  Heading:       {}°",
-                        libm::round(value as f64)
-                    )?;
+                    writeln!(f, "  Heading:       {}°", libm::round(value))?;
                 }
             }
             AirborneVelocitySubType::AirspeedSupersonic(v) => {
                 if let Some(value) = v.airspeed {
                     writeln!(
                         f,
                         "  {}:           {} kt",
@@ -419,15 +414,15 @@
     use hexlit::hex;
 
     #[test]
     fn test_groundspeed_velocity() {
         let bytes = hex!("8D485020994409940838175B284F");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
         if let ExtendedSquitterADSB(adsb_msg) = msg.df {
-            if let BDS09(velocity) = adsb_msg.message {
+            if let ME::BDS09(velocity) = adsb_msg.message {
                 if let AirborneVelocitySubType::GroundSpeedDecoding(_gsd) =
                     velocity.velocity
                 {
                     assert_relative_eq!(
                         _gsd.groundspeed,
                         159.,
                         max_relative = 1e-2
@@ -468,15 +463,15 @@
     }
 
     #[test]
     fn test_airspeed_velocity() {
         let bytes = hex!("8DA05F219B06B6AF189400CBC33F");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
         if let ExtendedSquitterADSB(adsb_msg) = msg.df {
-            if let BDS09(velocity) = adsb_msg.message {
+            if let ME::BDS09(velocity) = adsb_msg.message {
                 if let AirborneVelocitySubType::AirspeedSubsonic(asd) =
                     velocity.velocity
                 {
                     assert_eq!(asd.airspeed.unwrap(), 375);
                     assert_relative_eq!(
                         asd.heading.unwrap(),
                         244.,
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds10.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds10.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  * Mode S transponder.
  *
  * In the data link capability report, the first eight bits indicate the BDS
  * number, which is 1,0, or 0001 0000 in binary format.
  */
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "10")]
 pub struct DataLinkCapability {
     #[deku(bits = "8", map = "fail_if_not10")]
     #[serde(skip)]
     /// The first eight bits indicate the BDS code 1000 0000 (1,0 in hexadecimal).
     pub bds: u8,
 
     #[deku(bits = "1")]
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds17.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds17.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  * A bit when the corresponding register has a valid input that has been updated
  * at the required rate. This means that the same aircraft would respond with
  * different GICB reports due to the availability of the relevant data.
  *
  */
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
+#[serde(tag = "bds", rename = "17")]
 pub struct GICBCapabilityReport {
     #[deku(bits = "1")]
     #[serde(skip_serializing_if = "is_false")]
     /// Extended squitter airborne position
     pub bds05: bool,
 
     #[deku(bits = "1")]
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds20.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds20.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
  * ## Aircraft identification (BDS 2,0)
  *
  * Similar to an ADS-B aircraft identification message, the callsign of an
  * aircraft can be decoded from BDS 2,0 messages.
  */
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "20")]
 pub struct AircraftIdentification {
     #[deku(bits = "8", map = "fail_if_not20")]
     #[serde(skip)]
     /// The first eight bits indicate the BDS code 0010 0000 (2,0 in hexadecimal).
     pub bds: u8,
 
     #[deku(reader = "bds08::callsign_read(deku::rest)")]
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds30.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds30.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
  * ## ACAS active resolution advisory (BDS 3,0)
  *
  * The BDS 3,0 message is used to report resolution advisories (RA) generated by
  * ACAS equipment.
  */
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "30")]
 pub struct ACASResolutionAdvisory {
     #[deku(bits = "8", map = "fail_if_not30")]
     #[serde(skip)]
     /// The first eight bits indicate the BDS code 0011 0000 (3,0 in hexadecimal).
     pub bds: u8,
 
     #[deku(bits = "1")]
@@ -174,33 +175,36 @@
     #[serde(skip)]
     pub zeros: u8,
 }
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
 pub struct ThreatOrientation {
     /// Altitude code on 13 bits
+    #[serde(rename = "threat_altitude")]
     altitude: AC13Field,
 
     #[deku(
         bits = "7",
         map = "|n: u8| -> Result<_, DekuError> {
             if n == 0 { Ok(None) } else { Ok(Some((n as f32 - 1.) / 10.)) }
         }"
     )]
     /// Most recent threat range from ACAS (max 12.55 nautical miles)
+    #[serde(rename = "threat_range")]
     range: Option<f32>,
 
     #[deku(
         bits = "6",
         map = "|n: u16| -> Result<_, DekuError> {
             if n == 0 { Ok(None) } else { Ok(Some(6 * (n - 1) + 3)) }
         }"
     )]
     /// Most recent estimated bearing of the threat aircraft,
     /// relative to their own heading (3 degree precision)
+    #[serde(rename = "threat_bearing")]
     bearing: Option<u16>,
 }
 
 fn fail_if_not30(value: u8) -> Result<u8, DekuError> {
     if value == 0x30 {
         Ok(value)
     } else {
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds40.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds40.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
  * The selected vertical intention message is designed for air traffic control
  * to obtain an aircraft’s current vertical intentions. For example, an aircraft
  * controller can use this information to check whether an aircraft is complying
  * with an altitude command.
  */
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "40")]
 pub struct SelectedVerticalIntention {
     #[deku(reader = "read_selected(deku::rest)")]
     #[serde(rename = "selected_mcp", skip_serializing_if = "Option::is_none")]
     pub selected_altitude_mcp: Option<u16>, // 1+12
 
     #[deku(reader = "read_selected(deku::rest)")]
     #[serde(rename = "selected_fms", skip_serializing_if = "Option::is_none")]
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds44.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds44.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use serde::Serialize;
 
 /**
  * ## Meteorological Routine Air Report (BDS 4,4)
  */
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "44")]
 pub struct MeteorologicalRoutineAirReport {
     /// Figure of merit / source
     #[deku(bits = 4)]
     #[serde(skip)]
     pub figure_of_merit: u8,
 
     #[deku(reader = "read_wind_speed(deku::rest)")]
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds50.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds50.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 use deku::prelude::*;
 use serde::Serialize;
 
 /**
  * ## Track and turn report (BDS 5,0)
  */
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "50")]
 pub struct TrackAndTurnReport {
     #[deku(reader = "read_roll(deku::rest)")] // 11 bits
     #[serde(rename = "roll")]
     // Roll angle (negative sign means left wing down)
     pub roll_angle: Option<f64>,
 
     #[deku(reader = "read_track(deku::rest)")] // 12 bits
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds60.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds60.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 * - Inertial vertical velocity:
 *   1. Flight Management Computer / GNSS integrated
 *   2. Flight Management Computer (General)
 *   3. Inertial Reference System/Flight Management System
 *
 */
 #[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
+#[serde(tag = "bds", rename = "60")]
 pub struct HeadingAndSpeedReport {
     #[deku(reader = "read_heading(deku::rest)")] // 12 bits
     /// The magnetic heading is the aircraft's heading with respect to the magnetic North
     #[serde(rename = "heading", skip_serializing_if = "Option::is_none")]
     pub magnetic_heading: Option<f64>,
 
     #[deku(reader = "read_ias(deku::rest)")] // 11 bits
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds61.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds61.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds62.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds62.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     #[serde(rename = "source")]
     /// The source for the selected altitude (FMS or MCP/FCU)
     pub alt_source: AltSource, // bit 8
 
     #[deku(
         bits = "11",// bit 9..20
         endian = "big",
-        map = "|altitude: u32| -> Result<_, DekuError> {
+        map = "|altitude: u16| -> Result<_, DekuError> {
             Ok(
                 if altitude > 1 {Some(((altitude - 1) * 32 + 16) / 100 * 100)}
                 else {None}
             )
         }"
     )]
     #[serde(skip_serializing_if = "Option::is_none")]
     /// The selected altitude in the FMS or MCP/FCU, in feet
     /// (encoded as a multiple of 32 + 16, but rounded to the closest 100 ft)
-    pub selected_altitude: Option<u32>,
+    pub selected_altitude: Option<u16>,
 
     #[deku(
         bits = "9", // bit 20..29
         endian = "big",
         map = "|qnh: u32| -> Result<_, DekuError> {
             if qnh == 0 { Ok(None) }
             else { Ok(Some(800.0 + ((qnh - 1) as f32) * 0.8)) }
@@ -236,15 +236,15 @@
     use hexlit::hex;
 
     #[test]
     fn test_surface_position() {
         let bytes = hex!("8DA05629EA21485CBF3F8CADAEEB");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
         if let ExtendedSquitterADSB(adsb_msg) = msg.df {
-            if let BDS62(TargetStateAndStatusInformation {
+            if let ME::BDS62(TargetStateAndStatusInformation {
                 selected_altitude,
                 alt_source,
                 barometric_setting,
                 selected_heading,
                 mode_status,
                 autopilot,
                 vnav_mode,
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/bds/bds65.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/bds/bds65.rs`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 pub enum AircraftOperationStatus {
     #[deku(id = "0")]
     Airborne(OperationStatusAirborne),
 
     #[deku(id = "1")]
     Surface(OperationStatusSurface),
 
-    #[serde(skip)]
     #[deku(id_pat = "2..=7")]
     Reserved(#[deku(bits = "5")] u8, [u8; 5]),
 }
 
 impl fmt::Display for AircraftOperationStatus {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         writeln!(f, "  Aircraft Operation Status (BDS 6,5)")?;
@@ -256,27 +255,27 @@
 /// around 2008 (DO-260A), and version 2 around 2012 (DO-260B). Version 3 is
 /// currently being developed.
 #[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 #[deku(type = "u8", bits = "3")]
 #[serde(tag = "version")]
 pub enum ADSBVersionAirborne {
     #[deku(id = "0")]
-    #[serde(skip)] // useless, never happens
+    #[serde(rename = "0")] // useless, never happens
     /// ADS-B version 0 (BDS 6,5 undefined, so these messages should not happen)
     DOC9871AppendixA(Empty),
     #[deku(id = "1")]
     #[serde(rename = "1")]
     /// ADS-B version 1 (2008)
     DOC9871AppendixB(AirborneV1),
     #[deku(id = "2")]
     #[serde(rename = "2")]
     /// ADS-B version 2 (2012)
     DOC9871AppendixC(AirborneV2),
     #[deku(id_pat = "3..=7")]
-    #[serde(skip)]
+    #[serde(rename = "3to7")]
     Reserved(Empty),
 }
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 pub struct AirborneV1 {
     #[deku(bits = "1")]
     #[serde(rename = "NICs")]
@@ -310,15 +309,15 @@
     pub horizontal_reference_direction: u8,
 }
 
 #[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 pub struct AirborneV2 {
     #[deku(bits = "1")]
     #[serde(rename = "NICa")]
-    /// NIC supplement A (NICs)
+    /// NIC supplement A (NICa)
     pub nic_a: u8,
 
     #[deku(bits = "4")]
     #[serde(rename = "NACp")]
     /// Navigation Accuracy Category for position (NACp)
     pub nac_p: u8,
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/commb.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/commb.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/cpr.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/cpr.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-use super::{
-    adsb::ME,
-    bds::{bds05::AirbornePosition, bds06::SurfacePosition},
-    TimedMessage, DF, ICAO,
-};
+use super::adsb::ME;
+use super::bds::bds05::AirbornePosition;
+use super::bds::bds06::SurfacePosition;
+use super::{TimedMessage, DF, ICAO};
+use crate::data::airports::one_airport;
 use deku::prelude::*;
+use regex::Regex;
 use serde::Serialize;
-use std::{collections::BTreeMap, fmt};
+use std::collections::BTreeMap;
+use std::fmt;
+use std::str::FromStr;
 
 /**
 * The position information is encoded in a Compact Position Reporting (CPR)
 * format, which requires fewer bits to encode positions with higher resolution.
 * The CPR offers a trade-off between global position ambiguity and local
 * position accuracy. Two types of position messages (identified by the odd and
 * even frame bit) are broadcast alternately.
@@ -47,16 +50,47 @@
 
 #[derive(Debug, PartialEq, Serialize, Clone, Copy)]
 pub struct Position {
     pub latitude: f64,
     pub longitude: f64,
 }
 
+impl FromStr for Position {
+    type Err = String;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        let regex_list = [Regex::new(s).unwrap()];
+        if let Some(airport) = one_airport(&regex_list) {
+            return Ok(Position {
+                latitude: airport.lat,
+                longitude: airport.lon,
+            });
+        }
+        let parts: Vec<&str> = s.split(',').map(|p| p.trim()).collect();
+
+        if parts.len() != 2 {
+            return Err("Invalid number of coordinates".to_string());
+        }
+
+        let latitude: f64 = parts[0]
+            .parse()
+            .map_err(|e| format!("Latitude parse error: {}", e))?;
+        let longitude: f64 = parts[1]
+            .parse()
+            .map_err(|e| format!("Longitude parse error: {}", e))?;
+
+        Ok(Position {
+            latitude,
+            longitude,
+        })
+    }
+}
+
 #[derive(Default)]
-struct AircraftState {
+pub struct AircraftState {
     timestamp: f64,
     pos: Option<Position>,
     msg: Option<AirbornePosition>,
 }
 
 /// NZ represents the number of latitude zones between the equator and a pole.
 /// In Mode S, is defined to be 15.
@@ -141,14 +175,24 @@
     if lat < 87.000_000_00 { return 2; }
     1
 }
 
 const D_LAT_EVEN: f64 = 360.0 / (4.0 * NZ);
 const D_LAT_ODD: f64 = 360.0 / (4.0 * NZ - 1.0);
 
+// Main difference for % between Python and Rust is that in Rust, the sign
+// of the result matches the sign of the dividend.
+fn modulo(a: f64, b: f64) -> f64 {
+    if a >= 0. {
+        a % b
+    } else {
+        a % b + libm::fabs(b)
+    }
+}
+
 /**
  * Decode airborne position from a pair of even and odd position message.
  */
 
 pub fn airborne_position(
     oldest: &AirbornePosition,
     latest: &AirbornePosition,
@@ -180,16 +224,16 @@
     let cpr_lat_even = f64::from(even_frame.lat_cpr) / CPR_MAX;
     let cpr_lon_even = f64::from(even_frame.lon_cpr) / CPR_MAX;
     let cpr_lat_odd = f64::from(odd_frame.lat_cpr) / CPR_MAX;
     let cpr_lon_odd = f64::from(odd_frame.lon_cpr) / CPR_MAX;
 
     let j = libm::floor(59.0 * cpr_lat_even - 60.0 * cpr_lat_odd + 0.5);
 
-    let mut lat_even = D_LAT_EVEN * (j % 60.0 + cpr_lat_even);
-    let mut lat_odd = D_LAT_ODD * (j % 59.0 + cpr_lat_odd);
+    let mut lat_even = D_LAT_EVEN * (modulo(j, 60.) + cpr_lat_even);
+    let mut lat_odd = D_LAT_ODD * (modulo(j, 59.) + cpr_lat_odd);
 
     if lat_even >= 270.0 {
         lat_even -= 360.0;
     }
 
     if lat_odd >= 270.0 {
         lat_odd -= 360.0;
@@ -209,16 +253,15 @@
     };
     let ni = std::cmp::max(nl(lat) - p, 1) as f64;
     let m = libm::floor(
         cpr_lon_even * (nl(lat) - 1) as f64 - cpr_lon_odd * nl(lat) as f64
             + 0.5,
     );
 
-    let r = m % ni;
-    let r = if r < 0.0 { r + libm::fabs(ni) } else { r };
+    let r = modulo(m, ni);
 
     let mut lon = (360.0 / ni) * (r + c);
     if lon >= 180.0 {
         lon -= 360.0;
     }
 
     Some(Position {
@@ -245,25 +288,25 @@
     let d_lat = if msg.parity == CPRFormat::Even {
         360. / 60.
     } else {
         360. / 59.
     };
 
     let j = libm::floor(latitude_ref / d_lat)
-        + libm::floor(0.5 + (latitude_ref % d_lat) / d_lat - cpr_lat);
+        + libm::floor(0.5 + modulo(latitude_ref, d_lat) / d_lat - cpr_lat);
 
     let lat = d_lat * (j + cpr_lat);
     let ni = if msg.parity == CPRFormat::Even {
         nl(lat)
     } else {
         nl(lat) - 1
     };
     let d_lon = if ni > 0 { 360. / ni as f64 } else { 360. };
     let m = libm::floor(longitude_ref / d_lon)
-        + libm::floor(0.5 + (longitude_ref % d_lon) / d_lon - cpr_lon);
+        + libm::floor(0.5 + modulo(longitude_ref, d_lon) / d_lon - cpr_lon);
     let lon = d_lon * (m + cpr_lon);
 
     Position {
         latitude: lat,
         longitude: lon,
     }
 }
@@ -286,105 +329,157 @@
     let d_lat = if msg.parity == CPRFormat::Even {
         90. / 60.
     } else {
         90. / 59.
     };
 
     let j = libm::floor(latitude_ref / d_lat)
-        + libm::floor(0.5 + (latitude_ref % d_lat) / d_lat - cpr_lat);
+        + libm::floor(0.5 + modulo(latitude_ref, d_lat) / d_lat - cpr_lat);
 
     let lat = d_lat * (j + cpr_lat);
     let ni = if msg.parity == CPRFormat::Even {
         nl(lat)
     } else {
         nl(lat) - 1
     };
     let d_lon = if ni > 0 { 90. / ni as f64 } else { 90. };
     let m = libm::floor(longitude_ref / d_lon)
-        + libm::floor(0.5 + (longitude_ref % d_lon) / d_lon - cpr_lon);
+        + libm::floor(0.5 + modulo(longitude_ref, d_lon) / d_lon - cpr_lon);
     let lon = d_lon * (m + cpr_lon);
 
     Position {
         latitude: lat,
         longitude: lon,
     }
 }
 
+/**
+ * Mutates the ME message based on recent past positions (parameter `timestamp`)
+ * of the same aircraft (parameter `icao24`). For surface messages, the
+ * reference position will be considered; and possibly updated based on low
+ * altitude positions detected.
+ *
+ * - `aircraft` is a hashmap of aircraft containing their most recent state;
+ * - `reference` is a (possibly None) set of coordinates.
+ */
+
+pub fn decode_position(
+    message: &mut ME,
+    timestamp: f64,
+    icao24: &ICAO,
+    aircraft: &mut BTreeMap<ICAO, AircraftState>,
+    reference: &mut Option<Position>,
+) {
+    let latest = aircraft.entry(*icao24).or_insert(AircraftState {
+        timestamp,
+        pos: None,
+        msg: None,
+    });
+    match message {
+        ME::BDS05(airborne) => {
+            match (latest.timestamp, latest.msg, latest.pos) {
+                (t, _, Some(latest_pos)) if timestamp - t < 10. => {
+                    let pos = airborne_position_with_reference(
+                        airborne,
+                        latest_pos.latitude,
+                        latest_pos.longitude,
+                    );
+                    // First update the message
+                    airborne.latitude = Some(pos.latitude);
+                    airborne.longitude = Some(pos.longitude);
+                    // Then update the reference in aircraft
+                    latest.pos = Some(pos);
+                    latest.msg = Some(*airborne);
+                    latest.timestamp = timestamp;
+                    // If necessary update the reference position
+                    if let Some(alt) = airborne.alt {
+                        if alt < 1000 {
+                            *reference = Some(Position {
+                                latitude: pos.latitude,
+                                longitude: pos.longitude,
+                            })
+                        }
+                    }
+                }
+                (t, Some(oldest), None) if timestamp - t < 10. => {
+                    let pos: Option<Position> =
+                        airborne_position(&oldest, airborne);
+
+                    // First update the message
+                    if let Some(pos) = pos {
+                        airborne.latitude = Some(pos.latitude);
+                        airborne.longitude = Some(pos.longitude);
+                    }
+                    // Then update the reference in aircraft
+                    latest.pos = pos;
+                    latest.msg = Some(*airborne);
+                    latest.timestamp = timestamp;
+                }
+                _ => {
+                    // no airborne position, no position
+                    // or just too old position
+                    latest.msg = Some(*airborne);
+                    latest.timestamp = timestamp;
+                }
+            }
+        }
+        ME::BDS06(surface) => {
+            let pos = match (latest.pos, reference) {
+                (Some(pos), _) => Some(surface_position_with_reference(
+                    surface,
+                    pos.latitude,
+                    pos.longitude,
+                )),
+                (_, Some(reference)) => Some(surface_position_with_reference(
+                    surface,
+                    reference.latitude,
+                    reference.longitude,
+                )),
+                _ => None,
+            };
+            if let Some(pos) = pos {
+                // First update the message
+                surface.latitude = Some(pos.latitude);
+                surface.longitude = Some(pos.longitude);
+                // Then update the reference in aircraft
+                latest.pos = Some(pos);
+                latest.timestamp = timestamp;
+            }
+        }
+        _ => (),
+    }
+}
+
+/**
+ * This function is only used  for the decoding of offline messages.
+ */
 pub fn decode_positions(res: &mut [TimedMessage], reference: Option<Position>) {
     let mut aircraft: BTreeMap<ICAO, AircraftState> = BTreeMap::new();
+    let mut reference = reference;
 
     let _: Vec<()> = res
         .iter_mut()
         .map(|msg| {
-            if let DF::ExtendedSquitterADSB(adsb) = &mut msg.message.df {
-                let icao24 = adsb.icao24;
-                let latest = aircraft.entry(icao24).or_insert(AircraftState {
-                    timestamp: msg.timestamp,
-                    pos: None,
-                    msg: None,
-                });
-
-                match &mut adsb.message {
-                    ME::BDS05(airborne) => {
-                        match (latest.timestamp, latest.msg, latest.pos) {
-                            (t, Some(oldest), _) if msg.timestamp - t < 10. => {
-                                let pos: Option<Position> = if let Some(pos) =
-                                    airborne_position(&oldest, airborne)
-                                {
-                                    Some(pos)
-                                } else {
-                                    latest.pos.map(|latest_pos| {
-                                        airborne_position_with_reference(
-                                            &oldest,
-                                            latest_pos.latitude,
-                                            latest_pos.longitude,
-                                        )
-                                    })
-                                };
-
-                                if let Some(pos) = pos {
-                                    airborne.latitude = Some(pos.latitude);
-                                    airborne.longitude = Some(pos.longitude);
-                                }
-                                latest.pos = pos;
-                                latest.msg = Some(*airborne);
-                                latest.timestamp = msg.timestamp;
-                            }
-                            _ => {
-                                latest.msg = Some(*airborne);
-                                latest.timestamp = msg.timestamp;
-                            }
-                        }
-                    }
-                    ME::BDS06(surface) => {
-                        let pos = match (latest.pos, reference) {
-                            (Some(pos), _) => {
-                                Some(surface_position_with_reference(
-                                    surface,
-                                    pos.latitude,
-                                    pos.longitude,
-                                ))
-                            }
-                            (_, Some(reference)) => {
-                                Some(surface_position_with_reference(
-                                    surface,
-                                    reference.latitude,
-                                    reference.longitude,
-                                ))
-                            }
-                            _ => None,
-                        };
-                        if let Some(pos) = pos {
-                            surface.latitude = Some(pos.latitude);
-                            surface.longitude = Some(pos.longitude);
-                            latest.pos = Some(pos);
-                            latest.timestamp = msg.timestamp;
-                        }
-                    }
-                    _ => (),
+            if let Some(message) = &mut msg.message {
+                match &mut message.df {
+                    DF::ExtendedSquitterADSB(adsb) => decode_position(
+                        &mut adsb.message,
+                        msg.timestamp,
+                        &adsb.icao24,
+                        &mut aircraft,
+                        &mut reference,
+                    ),
+                    DF::ExtendedSquitterTisB { cf, .. } => decode_position(
+                        &mut cf.me,
+                        msg.timestamp,
+                        &cf.aa,
+                        &mut aircraft,
+                        &mut reference,
+                    ),
+                    _ => {}
                 }
             }
         })
         .collect();
 }
 
 #[cfg(test)]
@@ -400,38 +495,62 @@
         let b2 = hex!("8D40058B58C904A87F402D3B8C59");
         let msg1 = Message::from_bytes((&b1, 0)).unwrap().1;
         let msg2 = Message::from_bytes((&b2, 0)).unwrap().1;
 
         let (msg1, msg2) = match (msg1.df, msg2.df) {
             (ExtendedSquitterADSB(msg1), ExtendedSquitterADSB(msg2)) => {
                 match (msg1.message, msg2.message) {
-                    (BDS05(m1), BDS05(m2)) => (m1, m2),
+                    (ME::BDS05(m1), ME::BDS05(m2)) => (m1, m2),
                     _ => unreachable!(),
                 }
             }
             _ => unreachable!(),
         };
 
         let Position {
             latitude,
             longitude,
         } = airborne_position(&msg1, &msg2).unwrap();
 
         assert_relative_eq!(latitude, 49.81755, max_relative = 1e-3);
         assert_relative_eq!(longitude, 6.08442, max_relative = 1e-3);
+
+        let b3 = hex!("8d4d224f58bf07c2d41a9a353d70");
+        let b4 = hex!("8d4d224f58bf003b221b34aa5b8d");
+
+        let msg1 = Message::from_bytes((&b3, 0)).unwrap().1;
+        let msg2 = Message::from_bytes((&b4, 0)).unwrap().1;
+
+        let (msg1, msg2) = match (msg1.df, msg2.df) {
+            (ExtendedSquitterADSB(msg1), ExtendedSquitterADSB(msg2)) => {
+                match (msg1.message, msg2.message) {
+                    (ME::BDS05(m1), ME::BDS05(m2)) => (m1, m2),
+                    _ => unreachable!(),
+                }
+            }
+            _ => unreachable!(),
+        };
+
+        let Position {
+            latitude,
+            longitude,
+        } = airborne_position(&msg1, &msg2).unwrap();
+
+        assert_relative_eq!(latitude, 42.346, max_relative = 1e-3);
+        assert_relative_eq!(longitude, 0.4347, max_relative = 1e-3);
     }
 
     #[test]
     fn decode_airporne_position_with_reference() {
         let bytes = hex!("8D40058B58C901375147EFD09357");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
 
         let msg = match msg.df {
             ExtendedSquitterADSB(msg) => match msg.message {
-                BDS05(msg) => msg,
+                ME::BDS05(msg) => msg,
                 _ => unreachable!(),
             },
             _ => unreachable!(),
         };
 
         let Position {
             latitude,
@@ -442,15 +561,15 @@
         assert_relative_eq!(longitude, 6.06785, max_relative = 1e-3);
 
         let bytes = hex!("8D40058B58C904A87F402D3B8C59");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
 
         let msg = match msg.df {
             ExtendedSquitterADSB(msg) => match msg.message {
-                BDS05(msg) => msg,
+                ME::BDS05(msg) => msg,
                 _ => unreachable!(),
             },
             _ => unreachable!(),
         };
 
         let Position {
             latitude,
@@ -464,15 +583,15 @@
     #[test]
     fn decode_surface_position_with_reference() {
         let bytes = hex!("8c4841753aab238733c8cd4020b1");
         let msg = Message::from_bytes((&bytes, 0)).unwrap().1;
 
         let msg = match msg.df {
             ExtendedSquitterADSB(msg) => match msg.message {
-                BDS06(msg) => msg,
+                ME::BDS06(msg) => msg,
                 _ => unreachable!(),
             },
             _ => unreachable!(),
         };
 
         let Position {
             latitude,
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/crc.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/crc.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/crates/rs1090/src/decode/mod.rs` & `rs1090-0.2.0/crates/rs1090/src/decode/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 pub mod flarm;
 
 use adsb::{ADSB, ME};
 use commb::DataSelector;
 use crc::modes_checksum;
 use deku::bitvec::{BitSlice, Msb0};
 use deku::prelude::*;
-use serde::ser::{Serialize, Serializer};
+use serde::Serialize;
 use std::fmt;
 
 /**
  * DF stands for Downlink Format.
  *
  * A number between 0 and 24 encoding the type of the message, and whether it is
  * short (56 bits) or long (112 bits).
@@ -30,15 +30,15 @@
  * | 18       | [`DF::ExtendedSquitterTisB`]        | 3.1.2.8.7   |
  * | 19       | [`DF::ExtendedSquitterMilitary`]    | 3.1.2.8.8   |
  * | 20       | [`DF::CommBAltitudeReply`]          | 3.1.2.6.6   |
  * | 21       | [`DF::CommBIdentityReply`]          | 3.1.2.6.8   |
  * | 24       | [`DF::CommDExtended`]               | 3.1.2.7.3   |
  */
 
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
 #[deku(type = "u8", bits = "5", ctx = "crc: u32")]
 #[serde(tag = "df")]
 pub enum DF {
     /// DF=0: Short Air-Air Surveillance (3.1.2.8.2)
     #[deku(id = "0")]
     #[serde(rename = "0")]
     ShortAirAirSurveillance {
@@ -274,15 +274,15 @@
         parity: ICAO,
     },
 }
 
 /// The entry point to Mode S and ADS-B decoding
 ///
 /// Use as `Message::from_bytes()` in mostly all applications
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
 pub struct Message {
     /// Calculated from all bits, should be 0 for ADS-B (raises a DekuError),
     /// icao24 otherwise
     #[deku(reader = "Self::read_crc(deku::input_bits)")]
     #[serde(skip)]
     pub crc: u32,
 
@@ -396,20 +396,43 @@
                 writeln!(f, "  ICAO Address:     {crc:x?}")?;
             }
         }
         Ok(())
     }
 }
 
-#[derive(serde::Serialize)]
+#[derive(Serialize)]
 pub struct TimedMessage {
     pub timestamp: f64,
 
+    pub frame: String,
+
     #[serde(flatten)]
-    pub message: Message,
+    pub message: Option<Message>,
+
+    pub idx: usize,
+}
+
+impl fmt::Display for TimedMessage {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        writeln!(f, "{:.0} {}", &self.timestamp, &self.frame)?;
+        if let Some(msg) = &self.message {
+            writeln!(f, "{}", msg)?;
+        }
+        write!(f, "")
+    }
+}
+impl fmt::Debug for TimedMessage {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        writeln!(f, "{:.0} {}", &self.timestamp, &self.frame)?;
+        if let Some(msg) = &self.message {
+            writeln!(f, "{:#}", msg)?;
+        }
+        write!(f, "")
+    }
 }
 
 /// ICAO 24-bit address, commonly use to reference airframes, i.e. tail numbers
 /// of aircraft
 #[derive(PartialEq, Eq, PartialOrd, DekuRead, Hash, Copy, Clone, Ord)]
 #[deku(ctx = "crc: u32")]
 pub struct IcaoParity(
@@ -432,15 +455,15 @@
         Ok(())
     }
 }
 
 impl Serialize for IcaoParity {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
-        S: Serializer,
+        S: serde::ser::Serializer,
     {
         let icao = format!("{:06x}", &self.0);
         serializer.serialize_str(&icao)
     }
 }
 
 impl core::str::FromStr for IcaoParity {
@@ -470,15 +493,15 @@
         Ok(())
     }
 }
 
 impl Serialize for ICAO {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
-        S: Serializer,
+        S: serde::ser::Serializer,
     {
         let icao = format!("{:06x}", &self.0);
         serializer.serialize_str(&icao)
     }
 }
 
 impl core::str::FromStr for ICAO {
@@ -516,23 +539,23 @@
         Ok(())
     }
 }
 
 impl Serialize for IdentityCode {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
-        S: Serializer,
+        S: serde::ser::Serializer,
     {
         let squawk = format!("{:04x}", &self.0);
         serializer.serialize_str(&squawk)
     }
 }
 
 /// 13 bit encoded altitude
-#[derive(Debug, PartialEq, Eq, serde::Serialize, DekuRead, Copy, Clone)]
+#[derive(Debug, PartialEq, Eq, Serialize, DekuRead, Copy, Clone)]
 pub struct AC13Field(#[deku(reader = "Self::read(deku::rest)")] pub u16);
 
 impl AC13Field {
     fn read(
         rest: &BitSlice<u8, Msb0>,
     ) -> Result<(&BitSlice<u8, Msb0>, u16), DekuError> {
         let (rest, ac13field) =
@@ -564,15 +587,15 @@
                 Ok((rest, 0))
             }
         }
     }
 }
 
 /// Transponder level and additional information (3.1.2.5.2.2.1)
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Copy, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 #[deku(type = "u8", bits = "3")]
 #[allow(non_camel_case_types)]
 pub enum Capability {
     /// Level 1 transponder (surveillance only), and either airborne or on the ground
     #[serde(rename = "level1")]
     AG_LEVEL1 = 0x00,
     #[deku(id_pat = "0x01..=0x03")]
@@ -606,15 +629,15 @@
                 Self::AG_DR0 => "DR0",
             }
         )
     }
 }
 
 /// Airborne or Ground and SPI (used in DF=4, 5, 20 or 21)
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Copy, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Copy, Clone)]
 #[deku(type = "u8", bits = "3")]
 #[serde(rename_all = "snake_case")]
 pub enum FlightStatus {
     NoAlertNoSpiAirborne = 0b000,
     NoAlertNoSpiOnGround = 0b001,
     AlertNoSpiAirborne = 0b010,
     AlertNoSpiOnGround = 0b011,
@@ -669,15 +692,15 @@
     NoInformation = 0b00,
     CommB = 0b01,
     CommC = 0b10,
     CommD = 0b11,
 }
 
 /// The control field in TIS-B messages (DF=18)
-#[derive(Debug, PartialEq, serde::Serialize, DekuRead, Clone)]
+#[derive(Debug, PartialEq, Serialize, DekuRead, Clone)]
 pub struct ControlField {
     #[serde(rename = "tisb")]
     pub field_type: ControlFieldType,
     /// AA: Address, Announced
     #[serde(rename = "icao24")]
     pub aa: ICAO,
     /// ME: message, extended squitter
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/lib.rs` & `rs1090-0.2.0/crates/rs1090/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+#![allow(rustdoc::broken_intra_doc_links)]
 #![doc = include_str!("../readme.md")]
+pub mod data;
 pub mod decode;
 pub mod source;
 
 pub mod prelude {
     /// This re-export is necessary to decode messages
     pub use deku::prelude::*;
 
-    pub use crate::decode::adsb::ME::*;
+    pub use crate::decode::adsb::{ADSB, ME};
     pub use crate::decode::bds::bds05::AirbornePosition;
     pub use crate::decode::bds::bds06::SurfacePosition;
     pub use crate::decode::bds::bds08::AircraftIdentification;
     pub use crate::decode::bds::bds09::AirborneVelocity;
     pub use crate::decode::bds::bds61::AircraftStatus;
     pub use crate::decode::bds::bds62::TargetStateAndStatusInformation;
     pub use crate::decode::bds::bds65::AircraftOperationStatus;
     /// The root structure to decode messages
     pub use crate::decode::Message;
-    pub use crate::decode::TimedMessage;
     pub use crate::decode::DF::*;
+    pub use crate::decode::{TimedMessage, ICAO};
 
     /// This re-export is necessary for the following export
     pub use futures_util::stream::StreamExt;
 
     /// Information on the structure of a Beast message
     pub use crate::source::beast;
+    pub use crate::source::radarcape;
+
+    #[cfg(feature = "rtlsdr")]
+    pub use crate::source::rtlsdr;
 }
```

### Comparing `rs1090-0.1.3/crates/rs1090/src/source/beast.rs` & `rs1090-0.2.0/crates/rs1090/src/source/beast.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use async_stream::stream;
 use futures_util::stream::Stream;
 use tokio::io::AsyncReadExt;
-use tokio::net::TcpStream;
+use tokio::net::{TcpStream, UdpSocket};
 
 use std::collections::HashSet;
 
 /// Iterate a Beast binary feed.
 ///
 ///  - esc "1" : 6 byte MLAT timestamp, 1 byte signal level, 2 byte Mode-AC
 ///  - esc "2" : 6 byte MLAT timestamp, 1 byte signal level, 7 byte Mode-S short frame
@@ -14,82 +14,100 @@
 ///
 /// esc esc: true 0x1a
 /// esc is 0x1a, and "1", "2" and "3" are 0x31, 0x32 and 0x33
 ///
 /// Decoding the timestamp:
 /// <https://wiki.modesbeast.com/Radarcape:Firmware_Versions#The_GPS_timestamp>
 
-pub async fn next_msg(mut stream: TcpStream) -> impl Stream<Item = Vec<u8>> {
+pub enum DataSource {
+    Tcp(TcpStream),
+    Udp(UdpSocket),
+}
+
+pub async fn next_msg(mut stream: DataSource) -> impl Stream<Item = Vec<u8>> {
     // Initialize a HashSet to check for valid message types
     let valid_msg_types: HashSet<u8> =
         vec![0x31, 0x32, 0x33, 0x34].into_iter().collect();
 
     let mut data = Vec::new();
     stream! {
-        loop {
-            // Read from the stream into the buffer
-            let mut buffer = [0u8; 1024];
-            let bytes_read = match stream.read(&mut buffer).await {
-                Ok(0) => break, // Connection closed by peer
-                Ok(n) => n,
-                Err(e) => {
-                    println!("Error reading from socket: {}", e);
-                    break;
+    loop {
+        // Read from the stream into the buffer
+        let mut buffer = [0u8; 1024];
+        let bytes_read = match &mut stream {
+            DataSource::Tcp(tcp_stream) => {
+                match tcp_stream.read(&mut buffer).await {
+                    Ok(0) => break, // Connection closed by peer
+                    Ok(n) => n,
+                    Err(e) => {
+                        println!("Error reading from socket: {}", e);
+                        break;
+                    }
                 }
-            };
+            }
+            DataSource::Udp(udp_socket) => {
+                match udp_socket.recv_from(&mut buffer).await {
+                    Ok((n, _)) => n,
+                    Err(e) => {
+                        println!("Error reading from socket: {}", e);
+                        break;
+                    }
+                }
+            }
+        };
 
-            // Extend the data vector with the read bytes
-            data.extend_from_slice(&buffer[..bytes_read]);
+        // Extend the data vector with the read bytes
+        data.extend_from_slice(&buffer[..bytes_read]);
 
-            while data.len() >= 23 {
-                if let Some(it) = data.iter().position(|&x| x == 0x1A) {
-                    data = data.split_off(it);
+        while data.len() >= 23 {
+            if let Some(it) = data.iter().position(|&x| x == 0x1A) {
+                data = data.split_off(it);
 
-                    if data.len() < 23 {
-                        break;
-                    }
+                if data.len() < 23 {
+                    break;
+                }
 
-                    let msg_type = data[1];
-                    if valid_msg_types.contains(&msg_type) {
-                        // Collapse consecutive 0x1A into a single 0x1A
-                        let mut ref_idx = 1;
-                        let mut idx;
-                        let msg_size = match msg_type {
-                            0x31 => 11,
-                            0x32 => 16,
-                            0x33 => 23,
-                            0x34 => 23, // Adjust the message size accordingly
-                            _ => 0,
-                        };
-
-
-                        loop {
-                            idx = data[ref_idx..msg_size.min(data.len())].iter().position(|&x| x == 0x1A);
-                            if let Some(start) = idx.map(|idx| ref_idx + idx) {
-                                ref_idx = start + 1;
-                                if data.get(ref_idx) == Some(&0x1A) {
-                                    data.splice(start..=start, std::iter::empty());
-                                }
-                            } else {
-                                break;
+                let msg_type = data[1];
+                if valid_msg_types.contains(&msg_type) {
+                    // Collapse consecutive 0x1A into a single 0x1A
+                    let mut ref_idx = 1;
+                    let mut idx;
+                    let msg_size = match msg_type {
+                        0x31 => 11,
+                        0x32 => 16,
+                        0x33 => 23,
+                        0x34 => 23, // Adjust the message size accordingly
+                        _ => 0,
+                    };
+
+                    loop {
+                        idx = data[ref_idx..msg_size.min(data.len())]
+                            .iter()
+                            .position(|&x| x == 0x1A);
+                        if let Some(start) = idx.map(|idx| ref_idx + idx) {
+                            ref_idx = start + 1;
+                            if data.get(ref_idx) == Some(&0x1A) {
+                                data.splice(start..=start, std::iter::empty());
                             }
-                        }
-
-                        if idx.is_some() || data.len() < msg_size {
-                            // Move to the next buffer
+                        } else {
                             break;
                         }
+                    }
 
-                        let msg = data.drain(..msg_size).collect::<Vec<u8>>();
-                        yield msg
-                    } else {
-                        // Log a warning for probably corrupted message
-                        println!("Probably corrupted message");
-                        data = data.split_off(1);
+                    if idx.is_some() || data.len() < msg_size {
+                        // Move to the next buffer
+                        break;
                     }
+
+                    let msg = data.drain(..msg_size).collect::<Vec<u8>>();
+                    yield msg
                 } else {
-                    break;
+                    // Probably corrupted message
+                    data = data.split_off(1);
                 }
+            } else {
+                break;
             }
         }
     }
+    }
 }
```

### Comparing `rs1090-0.1.3/python/Cargo.toml` & `rs1090-0.2.0/python/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 name = "_rust"
 crate-type = ["cdylib"]
 
 [dependencies]
 hex = "0.4.3"
 pyo3 = "0.19.0"
 rayon = "1.9.0"
-rs1090 = { version= "0.1.3", path = "../crates/rs1090" }
+rs1090 = { version= "0.2.0", path = "../crates/rs1090" }
 serde-pickle = "1.1.1"
```

### Comparing `rs1090-0.1.3/python/.gitignore` & `rs1090-0.2.0/python/.gitignore`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/python/examples/long_flight.py` & `rs1090-0.2.0/python/examples/long_flight.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.1.3/python/tests/test_adsb.py` & `rs1090-0.2.0/python/tests/test_commb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 from pytest import approx
 
-from rs1090 import decode
+import rs1090
 
 
-def test_icao24():
-    assert decode("8D406B902015A678D4D220AA4BDA")["icao24"] == "406b90"
-
-
-def test_wake_vortex():
-    assert decode("8D406B902015A678D4D220AA4BDA")["wake_vortex"] == "n/a"
-
-
-def test_adsb_callsign():
-    assert decode("8D406B902015A678D4D220AA4BDA")["callsign"] == "EZY85MH"
-
-
-def test_adsb_alt():
-    assert decode("8D40058B58C901375147EFD09357")["altitude"] == 39000
-
-
-def test_adsb_velocity():
-    msg = decode("8D485020994409940838175B284F")
-    assert msg["groundspeed"] == approx(159.2, rel=1e-3)
-    assert msg["vertical_rate"] == -832
-    assert msg["track"] == approx(182.88, rel=1e-3)
-    assert msg["geo_minus_baro"] == 550
-
-    msg = decode("8DA05F219B06B6AF189400CBC33F")
-    assert msg["TAS"] == 375
-    assert msg["vertical_rate"] == -2304
-    assert msg["heading"] == approx(243.98, rel=1e-3)
-
-
-def test_adsb_emergency():
-    msg = decode("8DA2C1B6E112B600000000760759")
-    assert msg["emergency_state"] == "none"
-    assert msg["squawk"] == "6513"
-
-
-def test_adsb_target_state_status():
-    msg = decode("8DA05629EA21485CBF3F8CADAEEB")
-
-    assert msg["selected_altitude"] == 17000
-    assert msg["source"] == "MCP/FCU"
-    assert msg["barometric_setting"] == approx(1012.8)
-    assert msg["selected_heading"] == approx(66.8, 0.1)
-    assert msg["autopilot"]
-    assert msg["vnav_mode"]
-    assert not msg["alt_hold"]
-    assert not msg["approach_mode"]
-    assert msg["lnav_mode"]
-    assert msg["tcas_operational"]
+def test_bds20() -> None:
+    msg = rs1090.decode("A000083E202CC371C31DE0AA1CCF")
+    assert rs1090.is_df20(msg)
+    assert rs1090.is_bds20(msg)
+    assert msg["callsign"] == "KLM1017"
+    msg = rs1090.decode("A0001993202422F2E37CE038738E")
+    assert rs1090.is_df20(msg)
+    assert rs1090.is_bds20(msg)
+    assert msg["callsign"] == "IBK2873"
+
+
+def test_bds40() -> None:
+    msg = rs1090.decode("A000029C85E42F313000007047D3")
+    assert rs1090.is_df20(msg)
+    assert rs1090.is_bds40(msg)
+    assert msg["selected_mcp"] == 3000
+    assert msg["selected_fms"] == 3000
+    assert msg["barometric_setting"] == 1020
+
+
+def test_bds50() -> None:
+    msg = rs1090.decode("A000139381951536E024D4CCF6B5")
+    assert rs1090.is_df20(msg)
+    assert rs1090.is_bds50(msg)
+    assert msg["roll"] == approx(2.11, rel=1e-3)
+    assert msg["track"] == approx(114.2578)
+    assert msg["groundspeed"] == 438
+    assert msg["track_rate"] == 0.125
+    assert msg["TAS"] == 424
+
+
+def test_bds60() -> None:
+    msg = rs1090.decode("A00004128F39F91A7E27C46ADC21")
+    assert rs1090.is_df20(msg)
+    assert rs1090.is_bds60(msg)
+    assert msg["heading"] == approx(42.71484)
+    assert msg["IAS"] == 252
+    assert msg["Mach"] == 0.42
+    assert msg["vrate_barometric"] == -1920
+    assert msg["vrate_inertial"] == -1920
```

### Comparing `rs1090-0.1.3/Cargo.lock` & `rs1090-0.2.0/Cargo.lock`

 * *Files 20% similar despite different names*

```diff
@@ -14,29 +14,71 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "ahash"
+version = "0.8.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+ "version_check",
+ "zerocopy",
+]
+
+[[package]]
 name = "aho-corasick"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+
+[[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
+name = "ansi_term"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "anstream"
 version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e2e1ebcb11de5c03c67de28a7df593d32191b44939c482e97702baaaa6ab6a5"
 dependencies = [
  "anstyle",
  "anstyle-parse",
@@ -129,14 +171,40 @@
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
+name = "base64"
+version = "0.21.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+
+[[package]]
+name = "bindgen"
+version = "0.66.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2b84e06fc203107bfbad243f4aba2af864eb7db3b1cf46ea0a023b0b433d2a7"
+dependencies = [
+ "bitflags 2.4.2",
+ "cexpr",
+ "clang-sys",
+ "lazy_static",
+ "lazycell",
+ "peeking_take_while",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "rustc-hash",
+ "shlex",
+ "syn 2.0.50",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
@@ -153,14 +221,23 @@
  "funty",
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
+name = "block-buffer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "bumpalo"
 version = "3.15.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
 
 [[package]]
 name = "byteorder"
@@ -171,32 +248,70 @@
 [[package]]
 name = "bytes"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
 
 [[package]]
+name = "cassowary"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df8670b8c7b9dae1793364eafadf7239c40d669904660c5960d74cfd80b46a53"
+
+[[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
+name = "castaway"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a17ed5635fc8536268e5d4de1e22e81ac34419e5f052d4d51f4e01dcc263fcc"
+dependencies = [
+ "rustversion",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
 
 [[package]]
+name = "cexpr"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.37"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
+ "js-sys",
+ "num-traits",
+ "wasm-bindgen",
+ "windows-targets 0.52.3",
+]
+
+[[package]]
 name = "ciborium"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
@@ -216,14 +331,25 @@
 checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
+name = "clang-sys"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
+dependencies = [
+ "glob",
+ "libc",
+ "libloading",
+]
+
+[[package]]
 name = "clap"
 version = "4.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
 dependencies = [
  "clap_builder",
  "clap_derive",
@@ -263,26 +389,54 @@
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
+name = "compact_str"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f86b9c4c00838774a6d902ef931eff7470720c51d90c2e32cfe15dc304737b3f"
+dependencies = [
+ "castaway",
+ "cfg-if",
+ "itoa",
+ "ryu",
+ "static_assertions",
+]
+
+[[package]]
+name = "core-foundation-sys"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
+
+[[package]]
+name = "cpufeatures"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "criterion"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
  "cast",
  "ciborium",
  "clap",
  "criterion-plot",
  "is-terminal",
- "itertools",
+ "itertools 0.10.5",
  "num-traits",
  "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
@@ -295,15 +449,15 @@
 [[package]]
 name = "criterion-plot"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
 dependencies = [
  "cast",
- "itertools",
+ "itertools 0.10.5",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
@@ -324,20 +478,56 @@
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
+name = "crossterm"
+version = "0.27.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f476fe445d41c9e991fd07515a6f463074b782242ccf4a5b7b1d1012e70824df"
+dependencies = [
+ "bitflags 2.4.2",
+ "crossterm_winapi",
+ "futures-core",
+ "libc",
+ "mio",
+ "parking_lot",
+ "signal-hook",
+ "signal-hook-mio",
+ "winapi",
+]
+
+[[package]]
+name = "crossterm_winapi"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acdd7c62a3665c7f6830a51635d9ac9b23ed385797f70a83bb8bafe9c572ab2b"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
+name = "crypto-common"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
+dependencies = [
+ "generic-array",
+ "typenum",
+]
+
+[[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -365,16 +555,22 @@
 dependencies = [
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "data-encoding"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+
+[[package]]
 name = "decode1090"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
  "clap",
  "deku",
  "futures-util",
  "hex",
  "rs1090",
  "serde",
@@ -402,20 +598,39 @@
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "digest"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
+name = "encoding_rs"
+version = "0.8.33"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
@@ -430,14 +645,23 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "form_urlencoded"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
+dependencies = [
+ "percent-encoding",
+]
+
+[[package]]
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "futures"
@@ -525,34 +749,108 @@
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
+name = "generic-array"
+version = "0.14.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
+
+[[package]]
+name = "getrandom"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
+name = "h2"
+version = "0.3.25"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "half"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+dependencies = [
+ "ahash",
+ "allocator-api2",
+]
+
+[[package]]
+name = "headers"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06683b93020a07e3dbcf5f8c0f6d40080d725bea7936fc01ad345c01b97dc270"
+dependencies = [
+ "base64",
+ "bytes",
+ "headers-core",
+ "http",
+ "httpdate",
+ "mime",
+ "sha1",
+]
+
+[[package]]
+name = "headers-core"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7f66481bfee273957b1f20485a4ff3362987f85b2c236580d81b4eb7a326429"
+dependencies = [
+ "http",
+]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -571,20 +869,111 @@
 [[package]]
 name = "hexlit"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b6e75c860d4216ac53f9ac88b25c99eaedba075b3a7b2ed31f2adc51a74fffd"
 
 [[package]]
+name = "http"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
+
+[[package]]
+name = "hyper"
+version = "0.14.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
+name = "iana-time-zone"
+version = "0.1.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows-core",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
+name = "idna"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indexmap"
 version = "2.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
 dependencies = [
  "equivalent",
  "hashbrown",
@@ -593,14 +982,20 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "indoc"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
+
+[[package]]
 name = "is-terminal"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
  "hermit-abi",
  "libc",
@@ -619,35 +1014,86 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
+name = "jet1090"
+version = "0.2.0"
+dependencies = [
+ "chrono",
+ "clap",
+ "crossterm",
+ "deku",
+ "futures",
+ "futures-util",
+ "hex",
+ "ratatui",
+ "rs1090",
+ "serde",
+ "serde_json",
+ "soapysdr",
+ "tokio",
+ "warp",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
+name = "lazycell"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
+
+[[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if",
+ "windows-targets 0.52.3",
+]
+
+[[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "linux-raw-sys"
@@ -668,14 +1114,23 @@
 [[package]]
 name = "log"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
+name = "lru"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3262e75e648fce39813cb56ac41f3c3e3f65217ebf3844d818d1f9398cfb0dc"
+dependencies = [
+ "hashbrown",
+]
+
+[[package]]
 name = "memchr"
 version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memoffset"
@@ -683,14 +1138,36 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "mime"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
+
+[[package]]
+name = "mime_guess"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
+dependencies = [
+ "mime",
+ "unicase",
+]
+
+[[package]]
+name = "minimal-lexical"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
+
+[[package]]
 name = "miniz_oxide"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
@@ -698,30 +1175,68 @@
 [[package]]
 name = "mio"
 version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
 dependencies = [
  "libc",
+ "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "multer"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01acbdc23469fd8fe07ab135923371d5f5a422fbf9c522158677c8eb15bc51c2"
+dependencies = [
+ "bytes",
+ "encoding_rs",
+ "futures-util",
+ "http",
+ "httparse",
+ "log",
+ "memchr",
+ "mime",
+ "spin",
+ "version_check",
+]
+
+[[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
+name = "num-complex"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
@@ -786,26 +1301,70 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "paste"
+version = "1.0.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+
+[[package]]
+name = "peeking_take_while"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
+
+[[package]]
+name = "percent-encoding"
+version = "2.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
+
+[[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.50",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "pkg-config"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
 name = "plotters"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
  "num-traits",
  "plotters-backend",
@@ -826,14 +1385,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
 name = "proc-macro-crate"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
 dependencies = [
  "once_cell",
  "toml_edit",
@@ -851,15 +1416,15 @@
 [[package]]
 name = "pyo3"
 version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
 dependencies = [
  "cfg-if",
- "indoc",
+ "indoc 1.0.9",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
@@ -920,14 +1485,64 @@
 [[package]]
 name = "radium"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
+name = "ratatui"
+version = "0.26.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcb12f8fbf6c62614b0d56eb352af54f6a22410c3b079eb53ee93c7b97dd31d8"
+dependencies = [
+ "bitflags 2.4.2",
+ "cassowary",
+ "compact_str",
+ "crossterm",
+ "indoc 2.0.5",
+ "itertools 0.12.1",
+ "lru",
+ "paste",
+ "stability",
+ "strum",
+ "unicode-segmentation",
+ "unicode-width",
+]
+
+[[package]]
 name = "rayon"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
 dependencies = [
  "either",
  "rayon-core",
@@ -979,34 +1594,39 @@
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "rs1090"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
+ "ansi_term",
  "approx",
  "async-stream",
  "criterion",
  "deku",
  "futures",
  "futures-util",
  "hex",
  "hexlit",
  "libm",
+ "num-complex",
+ "once_cell",
  "rayon",
+ "regex",
  "serde",
  "serde_json",
+ "soapysdr",
  "tokio",
 ]
 
 [[package]]
 name = "rs1090-python"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
  "hex",
  "pyo3",
  "rayon",
  "rs1090",
  "serde-pickle",
 ]
@@ -1014,27 +1634,48 @@
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustix"
 version = "0.38.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
 dependencies = [
  "bitflags 2.4.2",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "rustls-pemfile"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
+dependencies = [
+ "base64",
+]
+
+[[package]]
+name = "rustversion"
+version = "1.0.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+
+[[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "same-file"
@@ -1042,14 +1683,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "scoped-tls"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1cf6437eb19a8f4a6cc0f7dca544973b0b78843adbfeb3683d1a94a0024a294"
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
@@ -1092,14 +1739,64 @@
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_urlencoded"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+dependencies = [
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "sha1"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
+name = "shlex"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
+
+[[package]]
+name = "signal-hook"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8621587d4798caf8eb44879d42e56b9a93ea5dcd315a6487c357130095b62801"
+dependencies = [
+ "libc",
+ "signal-hook-registry",
+]
+
+[[package]]
+name = "signal-hook-mio"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29ad2e15f37ec9a6cc544097b78a1ec90001e9f71b81338ca39f430adaca99af"
+dependencies = [
+ "libc",
+ "mio",
+ "signal-hook",
+]
+
+[[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
@@ -1116,36 +1813,102 @@
 [[package]]
 name = "smallvec"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
+name = "soapysdr"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24e2578203d938a532667e3e5d74917e65abd7afb17b4c2ebb7594f75de911ac"
+dependencies = [
+ "log",
+ "num-complex",
+ "soapysdr-sys",
+]
+
+[[package]]
+name = "soapysdr-sys"
+version = "0.7.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "abb5e50f86d0bf0c3312b77fce8737f760ce30adfa22baae97ffdd66a939356b"
+dependencies = [
+ "bindgen",
+ "cc",
+ "pkg-config",
+]
+
+[[package]]
 name = "socket2"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "spin"
+version = "0.9.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
+
+[[package]]
+name = "stability"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ebd1b177894da2a2d9120208c3386066af06a488255caabc5de8ddca22dbc3ce"
+dependencies = [
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "static_assertions"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
+
+[[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "strsim"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
 
 [[package]]
+name = "strum"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
+dependencies = [
+ "strum_macros",
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
+ "syn 2.0.50",
+]
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1182,24 +1945,59 @@
 checksum = "21bebf2b7c9e0a515f6e0f8c51dc0f8e4696391e6f1ff30379559f8365fb0df7"
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "thiserror"
+version = "1.0.58"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.58"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.50",
+]
+
+[[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "tokio"
 version = "1.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
 dependencies = [
  "backtrace",
  "bytes",
@@ -1222,14 +2020,51 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.50",
 ]
 
 [[package]]
+name = "tokio-stream"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "267ac89e0bec6e691e5813911606935d77c476ff49024f98abcea3e7b15e37af"
+dependencies = [
+ "futures-core",
+ "pin-project-lite",
+ "tokio",
+]
+
+[[package]]
+name = "tokio-tungstenite"
+version = "0.20.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "212d5dcb2a1ce06d81107c3d0ffa3121fe974b73f068c8282cb1c32328113b6c"
+dependencies = [
+ "futures-util",
+ "log",
+ "tokio",
+ "tungstenite",
+]
+
+[[package]]
+name = "tokio-util"
+version = "0.7.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "futures-sink",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 
 [[package]]
 name = "toml_edit"
@@ -1239,42 +2074,198 @@
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
+name = "tracing"
+version = "0.1.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
+dependencies = [
+ "log",
+ "pin-project-lite",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-core"
+version = "0.1.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
+dependencies = [
+ "once_cell",
+]
+
+[[package]]
+name = "try-lock"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
+
+[[package]]
+name = "tungstenite"
+version = "0.20.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e3dac10fd62eaf6617d3a904ae222845979aec67c615d1c842b4002c7666fb9"
+dependencies = [
+ "byteorder",
+ "bytes",
+ "data-encoding",
+ "http",
+ "httparse",
+ "log",
+ "rand",
+ "sha1",
+ "thiserror",
+ "url",
+ "utf-8",
+]
+
+[[package]]
+name = "typenum"
+version = "1.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
+
+[[package]]
+name = "unicase"
+version = "2.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7d2d4dafb69621809a81864c9c1b864479e1235c0dd4e199924b9742439ed89"
+dependencies = [
+ "version_check",
+]
+
+[[package]]
+name = "unicode-bidi"
+version = "0.3.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
+name = "unicode-normalization"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
+dependencies = [
+ "tinyvec",
+]
+
+[[package]]
+name = "unicode-segmentation"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
+
+[[package]]
+name = "unicode-width"
+version = "0.1.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "url"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
+]
+
+[[package]]
+name = "utf-8"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
+
+[[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
 name = "walkdir"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
+name = "want"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
+dependencies = [
+ "try-lock",
+]
+
+[[package]]
+name = "warp"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c1e92e22e03ff1230c03a1a8ee37d2f89cd489e2e541b7550d6afad96faed169"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "headers",
+ "http",
+ "hyper",
+ "log",
+ "mime",
+ "mime_guess",
+ "multer",
+ "percent-encoding",
+ "pin-project",
+ "rustls-pemfile",
+ "scoped-tls",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "tokio",
+ "tokio-stream",
+ "tokio-tungstenite",
+ "tokio-util",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
@@ -1368,14 +2359,23 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.3",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
@@ -1516,7 +2516,27 @@
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
+
+[[package]]
+name = "zerocopy"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.50",
+]
```

### Comparing `rs1090-0.1.3/pyproject.toml` & `rs1090-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.4,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rs1090"
 requires-python = ">=3.9"
-dependencies = []
+dependencies = ["pandas>=2.2.0"]
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 
@@ -38,13 +38,12 @@
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [project.optional-dependencies]
 dev = [
   "mypy>=1.8.0",
   "pytest>=8.0.2",
-  "ruff>=0.3.0", 
-  "pandas>=2.2.0"
+  "ruff>=0.3.0"
 ]
 
 [project.urls]
 repository = "https://github.com/xoolive/rs1090"
```

### Comparing `rs1090-0.1.3/PKG-INFO` & `rs1090-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.3
 Name: rs1090
-Version: 0.1.3
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: pandas >=2.2.0
 Requires-Dist: mypy >=1.8.0 ; extra == 'dev'
 Requires-Dist: pytest >=8.0.2 ; extra == 'dev'
 Requires-Dist: ruff >=0.3.0 ; extra == 'dev'
-Requires-Dist: pandas >=2.2.0 ; extra == 'dev'
 Provides-Extra: dev
 Summary: Python binding to rs1090, a library to decode Mode S and ADS-B signals
 Keywords: aircraft,ADS-B,Mode-S,decoding
 Author: Xavier Olive <git@xoolive.org>
 Author-email: Xavier Olive <git@xoolive.org>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/xoolive/rs1090
 
 # rs1090
 
-rs1090 is a Python binding to the [rs1090](https://docs.rs/rs1090/) Rust library to decode Mode S and ADS-B messages.
+rs1090 is a Python binding to the [rs1090](https://docs.rs/rs1090/) Rust library to decode Mode S, ADS-B and FLARM messages. It takes its inspiration from the Python [pyModeS](https://github.com/junzis/pyModeS) library.
 
-It takes its inspiration from the Python [pyModeS](https://github.com/junzis/pyModeS) library. The direction ambitioned by rs1090 boils down to:
+The direction ambitioned by rs1090 boils down to:
 
 - improving the performance of Mode S decoding in Python;
 - exporting trajectory data to cross-platform formats such as JSON or parquet;
 - providing efficient multi-receiver Mode S decoding;
 - serving real-time enriched trajectory data to external applications.
 
 ## Installation
@@ -53,7 +53,29 @@
 ...
 >>> rs1090.decode(msg_list, ts_list)  # includes CPR to position decoding
 ...
 >>> rs1090.decode(msg_list, ts_list, reference=(lat0, lon0))  # useful for surface messages
 ...
 ```
 
+For FLARM messages (also as batches):
+
+```pycon
+>>> msg = "7bf2381040ccc7e2395ecaa28e033a655d47e1d91d0bf986e1b0"
+>>> rs1090.flarm(msg, 1655279476, 43.61924, 5.11755)
+{'timestamp': 1655279476,
+ 'reference_lat': 43.61924,
+ 'reference_lon': 5.11755,
+ 'icao24': '38f27b',
+ 'is_icao24': True,
+ 'actype': 'Glider',
+ 'latitude': 43.6812864,
+ 'longitude': 5.150585599999999,
+ 'geoaltitude': 970,
+ 'vertical_speed': 1.0,
+ 'groundspeed': 18.698261951315153,
+ 'track': 29.655457935479006,
+ 'no_track': False,
+ 'stealth': False,
+ 'gps': 129}
+```
+
```

