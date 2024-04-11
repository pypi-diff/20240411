# Comparing `tmp/ring-attention-pytorch-0.3.8.tar.gz` & `tmp/ring-attention-pytorch-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.8.tar", last modified: Tue Apr  9 15:28:21 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.9.tar", last modified: Wed Apr 10 13:59:20 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.8.tar` & `ring-attention-pytorch-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18348 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:59:20.484446 ring-attention-pytorch-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-10 13:59:20.484446 ring-attention-pytorch-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:59:20.480446 ring-attention-pytorch-0.3.9/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:59:20.480446 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 13:59:20.000000 ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:59:20.484446 ring-attention-pytorch-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 13:59:15.000000 ring-attention-pytorch-0.3.9/setup.py
```

### Comparing `ring-attention-pytorch-0.3.8/LICENSE` & `ring-attention-pytorch-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.8/PKG-INFO` & `ring-attention-pytorch-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.8
+Version: 0.3.9
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.8/README.md` & `ring-attention-pytorch-0.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     - [x] cuda backwards pass must have same dq, dk, dv as naive
 - [x] fix naive flash attention backwards
 - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise flash attention is ineffective
 - [x] for cuda striped attention, for backwards hack, pad the extra token once and index out when passing into Tri's cuda kernel
 - [x] find a machine with 8 GPUs and test with a quarter million tokens first
 
-- [ ] see for cuda version whether softmax_D can be computed once and cached over the ring reduce. go for modified triton backwards if notattn)
+- [ ] see for cuda version whether softmax_D can be computed once and cached over the ring reduce. go for modified triton backwards if not
 - [ ] think about how to craft a special `Dataset` that shards across sequence length (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some cuda ring reduce impl
 - [ ] figure out how to pytest distributed pytorch
 - [ ] use sdp context manager to validate when it is possible to use `ring_flash_attn_cuda`, otherwise assert out
 
 ## Citations
```

#### html2text {}

```diff
@@ -55,15 +55,15 @@
 cuda backwards pass must have same dq, dk, dv as naive - [x] fix naive flash
 attention backwards - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise
 flash attention is ineffective - [x] for cuda striped attention, for backwards
 hack, pad the extra token once and index out when passing into Tri's cuda
 kernel - [x] find a machine with 8 GPUs and test with a quarter million tokens
 first - [ ] see for cuda version whether softmax_D can be computed once and
-cached over the ring reduce. go for modified triton backwards if notattn) - [ ]
+cached over the ring reduce. go for modified triton backwards if not - [ ]
 think about how to craft a special `Dataset` that shards across sequence length
 (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some
 cuda ring reduce impl - [ ] figure out how to pytest distributed pytorch - [ ]
 use sdp context manager to validate when it is possible to use
 `ring_flash_attn_cuda`, otherwise assert out ## Citations ```bibtex @article
 {Liu2023RingAW, title = {Ring Attention with Blockwise Transformers for Near-
```

### Comparing `ring-attention-pytorch-0.3.8/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.9/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,44 +142,56 @@
 @autocast(enabled = False)
 def apply_rotary_pos_emb(pos, t):
     pos = rearrange(pos, 'n d -> n 1 d')
     return t * pos.cos() + rotate_half(t) * pos.sin()
 
 # batch to sequence sharding and back
 
+def pad_at_dim(
+    t: Tensor,
+    pad: Tuple[int, int],
+    *,
+    dim = -1,
+    value = 0.
+):
+    dims_from_right = (- dim - 1) if dim < 0 else (t.ndim - dim - 1)
+    zeros = ((0, 0) * dims_from_right)
+    return F.pad(t, (*zeros, *pad), value = value)
+
 def pad_to_multiple(
     x: Tensor,
     length: int,
     pad_value = 0
 ):
-    seq_len = x.shape[-1]
+    seq_len = x.shape[1]
     remainder = seq_len % length
 
     if remainder == 0:
         return x, 0
 
     pad_length = length - remainder
-    return F.pad(x, (0, pad_length), value = pad_value), pad_length
+    return pad_at_dim(x, (0, pad_length), value = pad_value, dim = 1), pad_length
 
 def maybe_pad_seq_and_mask(
     x: Tensor,
     mask: Optional[Tensor],
     seq_size: int
 ):
-    orig_x, seq_len = x, x.shape[-1]
+    orig_x, shape = x, x.shape[:2]
+    seq_len = shape[-1]
 
     # auto pad sequence and mask, as ring passing makes assumption tensor is all same shape
 
     x, pad_length = pad_to_multiple(x, seq_size)
 
     if pad_length == 0:
         return x, mask
 
     if not exists(mask):
-        mask = torch.ones_like(orig_x).bool()
+        mask = torch.ones(shape).bool()
 
     mask, _ = pad_to_multiple(mask, seq_size, pad_value = False)
 
     return x, mask
 
 def sharded_batch_to_sharded_seq(
     x: Tensor,
@@ -197,25 +209,25 @@
     if exists(mask):
         mask, _ = all_gather(mask)
 
     # first make sure world size is divisible by the sequence size
 
     world_size = get_world_size()
 
-    total_split_seq = x.shape[-1] // seq_size
+    total_split_seq = x.shape[1] // seq_size
 
     assert divisible_by(world_size, total_split_seq)
 
     num_sharded_batches = world_size // total_split_seq
 
-    x = rearrange(x, '(b s) n -> b (s n)', s = num_sharded_batches)
+    x = rearrange(x, '(b s) n ... -> b (s n) ...', s = num_sharded_batches)
 
     # then split sequence across machines
 
-    x = x.split(seq_size, dim = -1)
+    x = x.split(seq_size, dim = 1)
 
     x, _ = split_by_rank(x)
 
     if exists(mask):
         mask = rearrange(mask, '(b s) n -> b (s n)', s = num_sharded_batches)
         mask = mask.split(seq_size, dim = -1)
         mask, _ = split_by_rank(mask)
@@ -334,26 +346,26 @@
         ring_size = default(ring_size, get_world_size())
         ring_attn = self.ring_attn & is_distributed()
         auto_shard_seq = self.auto_shard_seq & is_distributed()
 
         using_striped_ring_cuda = x.is_cuda and self.using_striped_ring_cuda
         striped_bucket_size = self.bucket_size if not using_striped_ring_cuda else self.ring_seq_size
 
-        seq_len = x.shape[-1]
+        seq_len = x.shape[1]
 
         if auto_shard_seq:
             x, mask = maybe_pad_seq_and_mask(x, mask, self.ring_seq_size)
 
             if self.striped_ring_attn:
                 x = rearrange(x, 'b (i j) d -> b (j i) d', i = striped_bucket_size)
 
                 if exists(mask):
                     mask = rearrange(mask, 'b (i j) -> b (j i)', i = striped_bucket_size)
 
-            (x, mask), batch_sizes = sharded_batch_to_sharded_seq(x, mask, self.ring_seq_size)
+            (x, mask), batch_sizes, num_sharded_batches = sharded_batch_to_sharded_seq(x, mask, self.ring_seq_size)
 
         device = x.device
 
         qkv = self.to_qkv(x)
         q, k, v = rearrange(qkv, 'b n (qkv h d) -> qkv b n h d', qkv = 3, h = self.heads)
 
         # rotary relative positions
@@ -400,18 +412,18 @@
 
         # combine heads
 
         out = rearrange(out, 'b n h d -> b n (h d)')
         out = self.to_out(out)
 
         if auto_shard_seq:
-            out, _ = sharded_seq_to_sharded_batch(out, batch_sizes)
+            out = sharded_seq_to_sharded_batch(out, batch_sizes, num_sharded_batches)
 
             if self.striped_ring_attn:
-                out = rearrange('b (j i) d -> b (i j) d', out, i = striped_bucket_size)
+                out = rearrange(out, 'b (j i) d -> b (i j) d', i = striped_bucket_size)
 
             out = out[:, :seq_len]
 
         return out
 
 # simple transformer for end2end testing
 
@@ -449,14 +461,15 @@
         ring_attn: bool = False,
         striped_ring_attn: bool = False,
         ring_seq_size: int = 512,
         auto_shard_seq: Optional[bool] = None,
         max_lookback_seq_len: Optional[Union[Tuple[int, ...], int]] = None,
         rotary_embed_theta: int = 10000,    # will need to be changed for the million token context
         ignore_index: int = -1,
+        force_regular_attn: bool = False,
         use_cuda_kernel: Optional[bool] = None
     ):
         super().__init__()
 
         use_cuda_kernel = default(use_cuda_kernel, torch.cuda.is_available())
         self.use_cuda_kernel = use_cuda_kernel
         assert not (use_cuda_kernel and not torch.cuda.is_available())
@@ -501,14 +514,15 @@
                     dim_head = dim_head,
                     heads = heads,
                     bucket_size = bucket_size,
                     ring_attn = ring_attn,
                     ring_seq_size = ring_seq_size,
                     max_lookback_seq_len = layer_max_lookback_seq_len,
                     striped_ring_attn = striped_ring_attn,
+                    force_regular_attn = force_regular_attn,
                     use_cuda_kernel = self.use_cuda_kernel,
                     auto_shard_seq = False,
                 ),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
         self.to_logits = nn.Sequential(
```

### Comparing `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.9/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.9/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.8
+Version: 0.3.9
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.8/setup.py` & `ring-attention-pytorch-0.3.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.8',
+  version = '0.3.9',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

