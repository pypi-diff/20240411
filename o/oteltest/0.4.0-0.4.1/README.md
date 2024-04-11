# Comparing `tmp/oteltest-0.4.0.tar.gz` & `tmp/oteltest-0.4.1.tar.gz`

## Comparing `oteltest-0.4.0.tar` & `oteltest-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.4.0/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1584 2020-02-02 00:00:00.000000 oteltest-0.4.0/example_scripts/simple_loop.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/__init__.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/common.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/main.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/sink.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.4.0/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.4.0/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.4.1/example_scripts/simple_loop.json
+-rwxr-xr-x   0        0        0     1584 2020-02-02 00:00:00.000000 oteltest-0.4.1/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.1/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 oteltest-0.4.1/src/oteltest/common.py
+-rw-r--r--   0        0        0     7025 2020-02-02 00:00:00.000000 oteltest-0.4.1/src/oteltest/main.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.4.1/src/oteltest/sink.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.4.1/src/oteltest/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.4.1/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.4.1/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.4.1/PKG-INFO
```

### Comparing `oteltest-0.4.0/example_scripts/simple_loop.json` & `oteltest-0.4.1/example_scripts/simple_loop.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996279761904763%*

 * *Differences: {"'trace_reqs'": "{0: {'request': {'resourceSpans': {0: {'scopeSpans': {0: {'spans': {0: "*

 * *                 "{'traceId': 'Kz0gw9vAHz8cMIBWQi7rMA==', 'spanId': 'uYs4lqZdcbU=', "*

 * *                 "'startTimeUnixNano': '1712771403864599000', 'endTimeUnixNano': "*

 * *                 "'1712771404368311000'}, 1: {'traceId': 'DGwojjkCC5VMySsLvJnI6A==', 'spanId': "*

 * *                 "'dpQILryJATU=', 'startTimeUnixNano': '1712771404368461000', 'endTimeUnixNano': "*

 * *                 "'1712771404868739000'}, 2: {'traceId': […]*

```diff
@@ -46,93 +46,93 @@
                         "scopeSpans": [
                             {
                                 "scope": {
                                     "name": "my-tracer"
                                 },
                                 "spans": [
                                     {
-                                        "endTimeUnixNano": "1712759491354281000",
+                                        "endTimeUnixNano": "1712771404368311000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "GFQ0Y/1usHw=",
-                                        "startTimeUnixNano": "1712759490850426000",
+                                        "spanId": "uYs4lqZdcbU=",
+                                        "startTimeUnixNano": "1712771403864599000",
                                         "status": {},
-                                        "traceId": "wKn+9uYSu732Bvp/d6soig=="
+                                        "traceId": "Kz0gw9vAHz8cMIBWQi7rMA=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759491857068000",
+                                        "endTimeUnixNano": "1712771404868739000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "9g/OJxA/XS4=",
-                                        "startTimeUnixNano": "1712759491354586000",
+                                        "spanId": "dpQILryJATU=",
+                                        "startTimeUnixNano": "1712771404368461000",
                                         "status": {},
-                                        "traceId": "TlfIBrx/au+g7z9/g8c6JA=="
+                                        "traceId": "DGwojjkCC5VMySsLvJnI6A=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759492359400000",
+                                        "endTimeUnixNano": "1712771405372377000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "dkWwAUyNjO8=",
-                                        "startTimeUnixNano": "1712759491857207000",
+                                        "spanId": "Kx69+pAheSc=",
+                                        "startTimeUnixNano": "1712771404868993000",
                                         "status": {},
-                                        "traceId": "h+YaJ65EcB6Kf9qD1XLpYA=="
+                                        "traceId": "uWqKMpLH9g2YUJJpsURDsw=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759492863414000",
+                                        "endTimeUnixNano": "1712771405873316000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "4tqPOx4B+Eo=",
-                                        "startTimeUnixNano": "1712759492359552000",
+                                        "spanId": "81bvQR+8eo0=",
+                                        "startTimeUnixNano": "1712771405372558000",
                                         "status": {},
-                                        "traceId": "x73Excz4sdxygBM+ID69+w=="
+                                        "traceId": "fDElFIEP6p5f+UmYH5jwdA=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759493368265000",
+                                        "endTimeUnixNano": "1712771406377606000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "R2a/Swb/XBY=",
-                                        "startTimeUnixNano": "1712759492863667000",
+                                        "spanId": "h5PXI5uUHPI=",
+                                        "startTimeUnixNano": "1712771405873638000",
                                         "status": {},
-                                        "traceId": "kp7/+JXh/sDqCH6bsesshg=="
+                                        "traceId": "3lYBDP60jpXKeeKufKLlzw=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759493871011000",
+                                        "endTimeUnixNano": "1712771406879339000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "ei+dgcuqSRY=",
-                                        "startTimeUnixNano": "1712759493368418000",
+                                        "spanId": "T+x9zY3O8Vw=",
+                                        "startTimeUnixNano": "1712771406377782000",
                                         "status": {},
-                                        "traceId": "rla9nswFh1ONlj3ktaaQVg=="
+                                        "traceId": "2oWdp6sPAYDFmDeWMsNz3Q=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759494372957000",
+                                        "endTimeUnixNano": "1712771407384479000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "u1oBpdXkEsY=",
-                                        "startTimeUnixNano": "1712759493871273000",
+                                        "spanId": "NDDVNmpv5fI=",
+                                        "startTimeUnixNano": "1712771406879594000",
                                         "status": {},
-                                        "traceId": "aar/fPoP1SbWePlkuUAHlQ=="
+                                        "traceId": "UGb/YVlHrusY24GfHTThxA=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759494873477000",
+                                        "endTimeUnixNano": "1712771407888121000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "TnHUM/kRZt8=",
-                                        "startTimeUnixNano": "1712759494373152000",
+                                        "spanId": "L6h4ufSHEuw=",
+                                        "startTimeUnixNano": "1712771407384738000",
                                         "status": {},
-                                        "traceId": "lj5EHWo9ElfkBu/kSznVeg=="
+                                        "traceId": "/8V/0lgsqgMSwX82gnyYVA=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759495373978000",
+                                        "endTimeUnixNano": "1712771408391338000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "8e109dTowyk=",
-                                        "startTimeUnixNano": "1712759494873735000",
+                                        "spanId": "FpYmJwYEYJA=",
+                                        "startTimeUnixNano": "1712771407888311000",
                                         "status": {},
-                                        "traceId": "+vDpXIG67rjtv8lrS8SpEQ=="
+                                        "traceId": "eTxlcqgXOrF9rNY8GnNZ6g=="
                                     }
                                 ]
                             }
                         ]
                     }
                 ]
             }
@@ -181,39 +181,39 @@
                         "scopeSpans": [
                             {
                                 "scope": {
                                     "name": "my-tracer"
                                 },
                                 "spans": [
                                     {
-                                        "endTimeUnixNano": "1712759495877969000",
+                                        "endTimeUnixNano": "1712771408895990000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "ddV2pt1uCLE=",
-                                        "startTimeUnixNano": "1712759495374180000",
+                                        "spanId": "CaAE4sWLCmQ=",
+                                        "startTimeUnixNano": "1712771408391594000",
                                         "status": {},
-                                        "traceId": "+p/vEXWXA3e9pOP6k6EdhQ=="
+                                        "traceId": "948AEvKAHh0xcpE1BdwBgQ=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759496381277000",
+                                        "endTimeUnixNano": "1712771409401061000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "IrKP3d5WENQ=",
-                                        "startTimeUnixNano": "1712759495878226000",
+                                        "spanId": "gA+fILGF1XQ=",
+                                        "startTimeUnixNano": "1712771408896275000",
                                         "status": {},
-                                        "traceId": "TNr46zLbAWYZcwB5kmnJ8g=="
+                                        "traceId": "KNyT8YzR7GKJixSeTWYKug=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712759496884624000",
+                                        "endTimeUnixNano": "1712771409902388000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "fy0SEmyae3k=",
-                                        "startTimeUnixNano": "1712759496381403000",
+                                        "spanId": "VjhxzmiJWX4=",
+                                        "startTimeUnixNano": "1712771409401317000",
                                         "status": {},
-                                        "traceId": "3eEzf3zfr/vdfqRC9aaV7A=="
+                                        "traceId": "hw2l3DwGnKDkILoeCXSjYg=="
                                     }
                                 ]
                             }
                         ]
                     }
                 ]
             }
```

### Comparing `oteltest-0.4.0/example_scripts/simple_loop.py` & `oteltest-0.4.1/example_scripts/simple_loop.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/src/oteltest/__init__.py` & `oteltest-0.4.1/src/oteltest/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/src/oteltest/common.py` & `oteltest-0.4.1/src/oteltest/common.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/src/oteltest/main.py` & `oteltest-0.4.1/src/oteltest/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,36 +116,42 @@
 
 
 def run_python_script(script, script_dir, oteltest_instance: OtelTest, v):
     python_script_cmd = [
         v.path_to_executable("python"),
         str(Path(script_dir) / script),
     ]
-    script = oteltest_instance.wrapper_script()
-    if script is not None:
-        python_script_cmd.insert(0, v.path_to_executable(script))
+
+    wrapper_script = oteltest_instance.wrapper_script()
+    if wrapper_script is not None:
+        python_script_cmd.insert(0, v.path_to_executable(wrapper_script))
 
     process = subprocess.Popen(
         python_script_cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         env=oteltest_instance.environment_variables(),
     )
 
     oteltest_instance.run_client()
 
-    # wait for the process to terminate
     timeout = oteltest_instance.max_wait()
     if timeout is None:
-        print("- Will wait indefinitely for script to finish (max_wait() returned None)")
+        print(
+            f"- Will wait indefinitely for {script} to finish (max_wait is None)"
+        )
     else:
-        print(f"- Will wait up to {timeout} seconds for script to finish")
-    stdout, stderr = process.communicate(timeout=timeout)
+        print(f"- Will wait up to {timeout} seconds for {script} to finish")
 
-    print_result(process.returncode, stderr, stdout)
+    try:
+        stdout, stderr = process.communicate(timeout=timeout)
+        print_result(process.returncode, stderr, stdout)
+    except subprocess.TimeoutExpired as ex:
+        print(f"- Script '{script}' was force terminated")
+        print_result(process.returncode, ex.stderr, ex.stdout)
 
 
 def run_subprocess(args, env_vars=None):
     print(f"- Subprocess: {args}")
     print(f"- Environment: {env_vars}")
     result = subprocess.run(
         args,
```

### Comparing `oteltest-0.4.0/src/oteltest/sink.py` & `oteltest-0.4.1/src/oteltest/sink.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/src/oteltest/version.py` & `oteltest-0.4.1/src/oteltest/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `oteltest-0.4.0/tests/__init__.py` & `oteltest-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/.gitignore` & `oteltest-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/LICENSE.txt` & `oteltest-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/README.md` & `oteltest-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/pyproject.toml` & `oteltest-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.4.0/PKG-INFO` & `oteltest-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.4.0
+Version: 0.4.1
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

