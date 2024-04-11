# Comparing `tmp/bitlinear-1.0.0.tar.gz` & `tmp/bitlinear-1.0.1.tar.gz`

## Comparing `bitlinear-1.0.0.tar` & `bitlinear-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.0.0/bitlinear/__init__.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 bitlinear-1.0.0/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bitlinear-1.0.0/bitlinear/kernels.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bitlinear-1.0.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.0.0/LICENSE
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bitlinear-1.0.0/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 bitlinear-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.0.1/bitlinear/__init__.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 bitlinear-1.0.1/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bitlinear-1.0.1/bitlinear/kernels.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bitlinear-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.0.1/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.0.1/PKG-INFO
```

### Comparing `bitlinear-1.0.0/bitlinear/bitlinear.py` & `bitlinear-1.0.1/bitlinear/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.0.0/bitlinear/kernels.py` & `bitlinear-1.0.1/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.0.0/LICENSE` & `bitlinear-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.0.0/README.md` & `bitlinear-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,22 +19,33 @@
 ```
 from bitlinear import replace_modules
 from transformers import AutoModelForCausalLM
 model = AutoModelForCausalLM.from_pretrained("HuggingFaceM4/tiny-random-LlamaForCausalLM")
 replace_modules(model)
 ```
 
-A more elaborate example is available under `examples`, including training and evaluating a binary classifer:
+More elaborate examples are available under `examples/classifier`, including training and evaluating a binary classifer:
 ```
-python examples/train.py
-python examples/eval.py
+pip install -r examples/classifier/requirements.txt
+python examples/classifier/train.py
+python examples/classifier/eval.py
+```
+There is also an MNIST classifier:
+```
+pip install -r examples/classifier/requirements.txt
+python examples/mnist/train.py
 ```
 
 # comparison to other work
 There are other implementations of bit-linear layers, most of which get at least some of the details wrong at the time of this writing (April 2024).
 
 The focus of this implementation is to develop:
 * a flexible production-ready drop-in replacemenbt for torch.nn.LinearLayer,
 * efficient fused kernels for training, and
 * efficient fused kernels for inference with 2-bit weights and 8-bit activations.
 
 Furthermore, this implementation is meant to serve as a testbed for research on low-bit quantization aware training and inference.
+
+# future work
+* further examples (vision, llm)
+* efficient fused kernels for GPU/AVX/CPU training
+* efficient fused kernels for GPU/AVX/CPU inferenc
```

### Comparing `bitlinear-1.0.0/pyproject.toml` & `bitlinear-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.0.0/PKG-INFO` & `bitlinear-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.0.0
+Version: 1.0.1
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,22 +34,33 @@
 ```
 from bitlinear import replace_modules
 from transformers import AutoModelForCausalLM
 model = AutoModelForCausalLM.from_pretrained("HuggingFaceM4/tiny-random-LlamaForCausalLM")
 replace_modules(model)
 ```
 
-A more elaborate example is available under `examples`, including training and evaluating a binary classifer:
+More elaborate examples are available under `examples/classifier`, including training and evaluating a binary classifer:
 ```
-python examples/train.py
-python examples/eval.py
+pip install -r examples/classifier/requirements.txt
+python examples/classifier/train.py
+python examples/classifier/eval.py
+```
+There is also an MNIST classifier:
+```
+pip install -r examples/classifier/requirements.txt
+python examples/mnist/train.py
 ```
 
 # comparison to other work
 There are other implementations of bit-linear layers, most of which get at least some of the details wrong at the time of this writing (April 2024).
 
 The focus of this implementation is to develop:
 * a flexible production-ready drop-in replacemenbt for torch.nn.LinearLayer,
 * efficient fused kernels for training, and
 * efficient fused kernels for inference with 2-bit weights and 8-bit activations.
 
 Furthermore, this implementation is meant to serve as a testbed for research on low-bit quantization aware training and inference.
+
+# future work
+* further examples (vision, llm)
+* efficient fused kernels for GPU/AVX/CPU training
+* efficient fused kernels for GPU/AVX/CPU inferenc
```

