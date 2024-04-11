# Comparing `tmp/bitmat-tl-0.2.9.tar.gz` & `tmp/bitmat-tl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.2.9.tar", last modified: Thu Apr  4 10:06:02 2024, max compression
+gzip compressed data, was "bitmat-tl-0.3.0.tar", last modified: Thu Apr 11 18:40:52 2024, max compression
```

## Comparing `bitmat-tl-0.2.9.tar` & `bitmat-tl-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-04 10:06:02.102405 bitmat-tl-0.2.9/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.2.9/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-04 10:06:02.102405 bitmat-tl-0.2.9/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     3858 2024-04-03 15:23:23.000000 bitmat-tl-0.2.9/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-04 10:06:02.098405 bitmat-tl-0.2.9/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-02 10:34:53.000000 bitmat-tl-0.2.9/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     3594 2024-04-03 15:45:15.000000 bitmat-tl-0.2.9/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-04 10:06:02.098405 bitmat-tl-0.2.9/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.9/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12407 2024-04-04 10:00:42.000000 bitmat-tl-0.2.9/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-01 22:08:01.000000 bitmat-tl-0.2.9/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-01 22:08:01.000000 bitmat-tl-0.2.9/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-04 10:06:02.098405 bitmat-tl-0.2.9/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-01 22:08:01.000000 bitmat-tl-0.2.9/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2661 2024-04-03 15:23:23.000000 bitmat-tl-0.2.9/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-02 10:12:51.000000 bitmat-tl-0.2.9/bitmat/utils/convert_hf_model.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-04 10:06:02.098405 bitmat-tl-0.2.9/bitmat/utils/model_hijacks/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-03 09:15:16.000000 bitmat-tl-0.2.9/bitmat/utils/model_hijacks/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-03 11:12:23.000000 bitmat-tl-0.2.9/bitmat/utils/model_hijacks/gemma_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73359 2024-04-03 15:57:20.000000 bitmat-tl-0.2.9/bitmat/utils/model_hijacks/llama_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64378 2024-04-03 15:57:11.000000 bitmat-tl-0.2.9/bitmat/utils/model_hijacks/mistral_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-02 12:56:59.000000 bitmat-tl-0.2.9/bitmat/utils/pack_model_before_save.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-02 15:23:36.000000 bitmat-tl-0.2.9/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-03 11:10:02.000000 bitmat-tl-0.2.9/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-04 10:06:02.102405 bitmat-tl-0.2.9/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     4490 2024-04-04 10:06:02.000000 bitmat-tl-0.2.9/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      708 2024-04-04 10:06:02.000000 bitmat-tl-0.2.9/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-04 10:06:02.000000 bitmat-tl-0.2.9/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-04 10:06:02.000000 bitmat-tl-0.2.9/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-04 10:06:02.000000 bitmat-tl-0.2.9/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-04 10:06:02.102405 bitmat-tl-0.2.9/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-04 10:05:31.000000 bitmat-tl-0.2.9/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.364899 bitmat-tl-0.3.0/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.3.0/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     4347 2024-04-11 18:40:52.364899 bitmat-tl-0.3.0/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3715 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.356899 bitmat-tl-0.3.0/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     3594 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.360899 bitmat-tl-0.3.0/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    13754 2024-04-09 14:18:20.000000 bitmat-tl-0.3.0/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.360899 bitmat-tl-0.3.0/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2661 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/utils/convert_hf_model.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.360899 bitmat-tl-0.3.0/bitmat/utils/model_hijacks/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-09 15:08:28.000000 bitmat-tl-0.3.0/bitmat/utils/model_hijacks/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-09 15:08:28.000000 bitmat-tl-0.3.0/bitmat/utils/model_hijacks/gemma_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73359 2024-04-09 15:08:28.000000 bitmat-tl-0.3.0/bitmat/utils/model_hijacks/llama_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64378 2024-04-09 15:08:28.000000 bitmat-tl-0.3.0/bitmat/utils/model_hijacks/mistral_1_58b.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.360899 bitmat-tl-0.3.0/bitmat/utils/modeling/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       76 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/bitmat/utils/modeling/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1740 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/bitmat/utils/modeling/automodel.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.364899 bitmat-tl-0.3.0/bitmat/utils/modeling/model_hijacks/
+-rw-rw-r--   0 marco     (1000) marco     (1000)      139 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/bitmat/utils/modeling/model_hijacks/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    61145 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73363 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64382 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/utils/pack_model_before_save.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-05 08:31:48.000000 bitmat-tl-0.3.0/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:40:52.364899 bitmat-tl-0.3.0/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     4347 2024-04-11 18:40:52.000000 bitmat-tl-0.3.0/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      980 2024-04-11 18:40:52.000000 bitmat-tl-0.3.0/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-11 18:40:52.000000 bitmat-tl-0.3.0/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-11 18:40:52.000000 bitmat-tl-0.3.0/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-11 18:40:52.000000 bitmat-tl-0.3.0/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-11 18:40:52.364899 bitmat-tl-0.3.0/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-04 14:43:19.000000 bitmat-tl-0.3.0/setup.py
```

### Comparing `bitmat-tl-0.2.9/LICENSE` & `bitmat-tl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/PKG-INFO` & `bitmat-tl-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.9
+Version: 0.3.0
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,16 +16,14 @@
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
-## ⚠️ We're currently investigating as the method .to() seems not working, hold on tight while we fix it
-
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
@@ -48,21 +46,21 @@
 model= AutoModelForCausalLM.from_pretrained("some-repo/some-model")
 # Convert the model to use BitLinear layers
 model = convert_hf_model(model)
 # Save the converted model
 model.save_pretrained('some_local_folder')
 ```
 ### Loading the converted 1.58Bit Model
-To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to import the specific model class from the library. Below is an example demonstrating how to load the Mistral158ForCausalLM model from a local directory:
+To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to load the model from the AutoClass. Below is an example demonstrating how to load the model from a local directory:
 
 ```python
-from bitmat import Mistral158ForCausalLM
+from bitmat import Auto158ModelForCausalLM
 
 # Replace 'path_to_your_model' with the actual path to your model's directory
-model = Mistral158ForCausalLM.from_pretrained('path_to_your_model')
+model = Auto158ModelForCausalLM.from_pretrained('path_to_your_model')
 ```
 Once loaded, the model operates in two distinct modes:
 
 - Evaluation Mode: By default, the model employs quantized weights, optimizing performance for inference tasks. Activate this mode using model.eval().
 
 - Training Mode: Switching to this mode, via model.train(), allows the model to leverage full-precision weights, which is essential for training and fine-tuning processes, ensuring accurate gradient calculations and effective model updates.
```

### Comparing `bitmat-tl-0.2.9/README.md` & `bitmat-tl-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
-## ⚠️ We're currently investigating as the method .to() seems not working, hold on tight while we fix it
-
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
@@ -28,21 +26,21 @@
 model= AutoModelForCausalLM.from_pretrained("some-repo/some-model")
 # Convert the model to use BitLinear layers
 model = convert_hf_model(model)
 # Save the converted model
 model.save_pretrained('some_local_folder')
 ```
 ### Loading the converted 1.58Bit Model
-To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to import the specific model class from the library. Below is an example demonstrating how to load the Mistral158ForCausalLM model from a local directory:
+To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to load the model from the AutoClass. Below is an example demonstrating how to load the model from a local directory:
 
 ```python
-from bitmat import Mistral158ForCausalLM
+from bitmat import Auto158ModelForCausalLM
 
 # Replace 'path_to_your_model' with the actual path to your model's directory
-model = Mistral158ForCausalLM.from_pretrained('path_to_your_model')
+model = Auto158ModelForCausalLM.from_pretrained('path_to_your_model')
 ```
 Once loaded, the model operates in two distinct modes:
 
 - Evaluation Mode: By default, the model employs quantized weights, optimizing performance for inference tasks. Activate this mode using model.eval().
 
 - Training Mode: Switching to this mode, via model.train(), allows the model to leverage full-precision weights, which is essential for training and fine-tuning processes, ensuring accurate gradient calculations and effective model updates.
```

### Comparing `bitmat-tl-0.2.9/bitmat/bitlinear.py` & `bitmat-tl-0.3.0/bitmat/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.3.0/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,14 +88,50 @@
     offs_cn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
     c_ptrs = c_ptr + stride_cm * offs_cm[:, None] + stride_cn * offs_cn[None, :]
     c_mask = (offs_cm[:, None] < M) & (offs_cn[None, :] < N)
     tl.store(c_ptrs, c, mask=c_mask)
 
 
 
+def bitmat(a, b, int_per_2_bits=4, activation=""):
+    """
+        a: int8 tensor (M, K)
+        b: int8 packed tensor (K // int_per_2_bit, N)
+        n_bits: int, number of bits that each element in b represents
+    """
+    # Check constraints.
+    assert a.shape[1] == b.shape[0] * int_per_2_bits, "Incompatible dimensions"
+    assert a.dim() == 2, "Matrix A must be 2D"
+    assert b.dim() == 2, "Matrix B must be 2D"
+    assert a.is_contiguous(), "A must be contiguous"
+    assert b.is_contiguous(), "B must be contiguous"
+    assert int_per_2_bits in [4, 8, 16, 32], "n_bits must be 4, 8, 16, 32"
+    M, K = a.shape
+    _, N = b.shape
+
+    # Allocates output.
+    c = torch.empty((M, N), device=a.device, dtype=torch.float16).contiguous()
+    # 1D launch kernel where each block gets its own program.
+    grid = lambda META: (
+        triton.cdiv(M, META['BLOCK_SIZE_M']) * triton.cdiv(N, META['BLOCK_SIZE_N']),
+    )
+
+    # print(f"Launching kernel with M = {M}, N = {N}, K = {K}, n_bits = {n_bits}, activation = {activation}")
+
+    _ternary_mm_kernel[grid](
+        a, b, c,
+        M, N, K,
+        int_per_2_bits,
+        a.stride(0), a.stride(1),
+        b.stride(0), b.stride(1),
+        c.stride(0), c.stride(1),
+        ACTIVATION=activation
+    )
+    return c
+
 
 @triton.autotune(
     configs=[
         triton.Config({'BLOCK_SIZE_M': 128, 'BLOCK_SIZE_N': 128, 'BLOCK_SIZE_K': 64, 'GROUP_SIZE_M': 8}, num_stages=8, num_warps=8),
         triton.Config({'BLOCK_SIZE_M': 64, 'BLOCK_SIZE_N': 64, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
         triton.Config({'BLOCK_SIZE_M': 32, 'BLOCK_SIZE_N': 32, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
         triton.Config({'BLOCK_SIZE_M': 16, 'BLOCK_SIZE_N': 16, 'BLOCK_SIZE_K': 32, 'GROUP_SIZE_M': 8}, num_stages=4, num_warps=4),
@@ -169,17 +205,17 @@
     # We accumulate into a `[BLOCK_SIZE_M, BLOCK_SIZE_N]` block
     # of fp32 values for higher accuracy.
     # `accumulator` will be converted back to fp16 after the loop.
     accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
     for k in range(0, tl.cdiv(K, BLOCK_SIZE_K)):
         # Load the next block of A and B, generate a mask by checking the K dimension.
         # If it is out of bounds, set it to 0.
-        a = tl.load(a_ptrs, mask=offs_k[None, :] < K - k * BLOCK_SIZE_K, other=0.0)
+        a = tl.load(a_ptrs, mask=offs_k[None, :] < K - k * BLOCK_SIZE_K + BLOCK_SIZE_K - 1, other=0.0)
         # b = tl.load(b_ptrs, mask=offs_k[:, None] < K - k * BLOCK_SIZE_K, other=0)
-        b = tl.load(b_ptrs)
+        b = tl.load(b_ptrs, mask=offs_k[:, None] < K - k * BLOCK_SIZE_K, other=0)
 
         # Convert B from int to a.dtype, for each bit in B, 0 becomes -1.0, 1 becomes 1.0
         # b: (BLOCK_SIZE_K, BLOCK_SIZE_N)
         # We extract the 2 bits of each element in the int matrix
         b = (b >> shifter) & 0x3
         # We need to map back the value 2 -> -1
         b = tl.where(b == 0x2, -1, b)
```

### Comparing `bitmat-tl-0.2.9/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.3.0/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.3.0/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/utils/bitmat.py` & `bitmat-tl-0.3.0/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/utils/convert_hf_model.py` & `bitmat-tl-0.3.0/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/utils/model_hijacks/gemma_1_58b.py` & `bitmat-tl-0.3.0/bitmat/utils/model_hijacks/gemma_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/utils/model_hijacks/llama_1_58b.py` & `bitmat-tl-0.3.0/bitmat/utils/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/utils/model_hijacks/mistral_1_58b.py` & `bitmat-tl-0.3.0/bitmat/utils/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat/utils/packing.py` & `bitmat-tl-0.3.0/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.2.9/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.3.0/bitmat_tl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.2.9
+Version: 0.3.0
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,16 +16,14 @@
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
-## ⚠️ We're currently investigating as the method .to() seems not working, hold on tight while we fix it
-
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
@@ -48,21 +46,21 @@
 model= AutoModelForCausalLM.from_pretrained("some-repo/some-model")
 # Convert the model to use BitLinear layers
 model = convert_hf_model(model)
 # Save the converted model
 model.save_pretrained('some_local_folder')
 ```
 ### Loading the converted 1.58Bit Model
-To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to import the specific model class from the library. Below is an example demonstrating how to load the Mistral158ForCausalLM model from a local directory:
+To utilize the converted 1.58Bit model, such as a customized version of Mistral in this exmaple, you will need to load the model from the AutoClass. Below is an example demonstrating how to load the model from a local directory:
 
 ```python
-from bitmat import Mistral158ForCausalLM
+from bitmat import Auto158ModelForCausalLM
 
 # Replace 'path_to_your_model' with the actual path to your model's directory
-model = Mistral158ForCausalLM.from_pretrained('path_to_your_model')
+model = Auto158ModelForCausalLM.from_pretrained('path_to_your_model')
 ```
 Once loaded, the model operates in two distinct modes:
 
 - Evaluation Mode: By default, the model employs quantized weights, optimizing performance for inference tasks. Activate this mode using model.eval().
 
 - Training Mode: Switching to this mode, via model.train(), allows the model to leverage full-precision weights, which is essential for training and fine-tuning processes, ensuring accurate gradient calculations and effective model updates.
```

### Comparing `bitmat-tl-0.2.9/setup.py` & `bitmat-tl-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.2.9',
+    version='0.3.0',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

