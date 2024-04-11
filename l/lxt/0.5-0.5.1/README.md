# Comparing `tmp/lxt-0.5.tar.gz` & `tmp/lxt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxt-0.5.tar", last modified: Fri Apr  5 15:43:28 2024, max compression
+gzip compressed data, was "lxt-0.5.1.tar", last modified: Thu Apr 11 16:18:35 2024, max compression
```

## Comparing `lxt-0.5.tar` & `lxt-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2156 2024-04-05 14:07:44.000000 lxt-0.5/LICENSE
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5948 2024-04-05 15:43:28.900796 lxt-0.5/PKG-INFO
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5545 2024-04-05 15:40:42.000000 lxt-0.5/README.md
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/lxt/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 14:07:44.000000 lxt-0.5/lxt/__init__.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      785 2024-04-05 14:18:02.000000 lxt-0.5/lxt/check.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    15189 2024-04-05 14:07:45.000000 lxt-0.5/lxt/core.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    14635 2024-04-05 14:16:05.000000 lxt-0.5/lxt/functional.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2678 2024-04-05 14:07:45.000000 lxt-0.5/lxt/modules.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    13091 2024-04-05 14:28:12.000000 lxt-0.5/lxt/rules.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3435 2024-04-05 14:44:58.000000 lxt-0.5/lxt/utils.py
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/lxt.egg-info/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5948 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/PKG-INFO
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      305 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/SOURCES.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        1 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/dependency_links.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       63 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/requires.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        4 2024-04-05 15:43:28.000000 lxt-0.5/lxt.egg-info/top_level.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       38 2024-04-05 15:43:28.900796 lxt-0.5/setup.cfg
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      598 2024-04-05 15:20:00.000000 lxt-0.5/setup.py
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 15:43:28.900796 lxt-0.5/tests/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3799 2024-04-05 14:13:59.000000 lxt-0.5/tests/test_functional.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      717 2024-04-05 14:12:50.000000 lxt-0.5/tests/test_rules.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2156 2024-04-05 14:07:44.000000 lxt-0.5.1/LICENSE
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5812 2024-04-11 16:18:35.473678 lxt-0.5.1/PKG-INFO
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5560 2024-04-11 13:37:53.000000 lxt-0.5.1/README.md
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/lxt/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 14:07:44.000000 lxt-0.5.1/lxt/__init__.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      785 2024-04-05 14:18:02.000000 lxt-0.5.1/lxt/check.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    15189 2024-04-05 14:07:45.000000 lxt-0.5.1/lxt/core.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    20440 2024-04-11 16:00:37.000000 lxt-0.5.1/lxt/functional.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3081 2024-04-11 16:15:12.000000 lxt-0.5.1/lxt/modules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    13091 2024-04-05 14:28:12.000000 lxt-0.5.1/lxt/rules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3435 2024-04-05 14:44:58.000000 lxt-0.5.1/lxt/utils.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/lxt.egg-info/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5812 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/PKG-INFO
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      327 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/SOURCES.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        1 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/dependency_links.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       63 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/requires.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        4 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/top_level.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       38 2024-04-11 16:18:35.473678 lxt-0.5.1/setup.cfg
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      600 2024-04-11 16:07:52.000000 lxt-0.5.1/setup.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/tests/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5262 2024-04-11 16:03:47.000000 lxt-0.5.1/tests/test_functional.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      943 2024-04-11 16:16:01.000000 lxt-0.5.1/tests/test_modules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      758 2024-04-11 15:35:57.000000 lxt-0.5.1/tests/test_rules.py
```

### Comparing `lxt-0.5/LICENSE` & `lxt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lxt-0.5/PKG-INFO` & `lxt-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: lxt
-Version: 0.5
+Version: 0.5.1
 Summary: LRP explains Transformers
 Home-page: https://github.com/rachtibat/LRP-for-Transformers
 Author: Reduan Achtibat
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: transformers
-Requires-Dist: accelerate
-Requires-Dist: tabulate
-Requires-Dist: matplotlib
-Requires-Dist: bitsandbytes
 
 <div align="center">
   <img src="docs/source/_static/lxt_logo.png" width="300"/>
   <p>Layer-wise Relevance Propagation (LRP) extended to handle attention layers in Large Language Models (LLMs) and Vision Transformers (ViTs)</p>
 </div>
 
 [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)](https://pytorch.org)
-[![Read the Docs](https://img.shields.io/badge/-Docs-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white&link=https://inseq.org)](https://google.de)
+[![Read the Docs](https://img.shields.io/badge/-Docs-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white)](https://lxt.readthedocs.io)
 
 #### 🔥 Faithful Attributions
 
 Attention-aware LRP (AttnLRP) **outperforms** gradient- and perturbation-based methods, provides faithful attributions for the **entirety** of a black-box transformer model while scaling in computational complexitiy $O(1)$ and memory requirements $O(\sqrt{N})$ with respect to the number of layers.
 
 #### 🔎 Latent Feature Attribution & Visualization
 Since we get relevance values for each neuron in the model as a by-product, we know exactly how important each neuron is for the prediction of the model. Combined with Activation Maximization, we can label neurons in LLMs and even steer the generation process of the LLM by activating specialized knowledge neurons in latent space!
@@ -70,15 +64,15 @@
 $ git clone https://github.com/rachtibat/LRP-for-Transformers
 $ pip install ./lxt
 ```
 
 Tested with ``transformers==4.39.3``, ``torch==2.2.2``, ``python==3.11``
 
 ### 💡 How does the code work?
-Layer-wise Relevance Propagation is a rule-based backpropagation algorithm. This means, that we can implement LRP in a singular backward pass!
+Layer-wise Relevance Propagation is a rule-based backpropagation algorithm. This means, that we can implement LRP in a single backward pass!
 To achieve this, we have implemented [custom PyTorch autograd Functions](https://pytorch.org/tutorials/beginner/examples_autograd/two_layer_net_custom_function.html) for commonly used operations in transformers. These functions behave identically in the forward pass, but compute LRP attributions in the backward pass. To compute the $\varepsilon$-LRP rule for a linear function $y = W x + b$, you can simply write
 ```python
 import lxt.functional as lf
 
 y = lf.linear_epsilon(x.requires_grad_(), W, b)
 y.backward(y)
 
@@ -120,16 +114,16 @@
 Applying LRP to new models can be tricky! We provide some basic debugging tools to help you out!
 
 ### ⚙️ Tuning Vision Transformers
 ViTs are vulnerable to noisy attributions, hence we must denoise the heatmap.
 We propose to use the $\gamma$-LRP rule, where the $\gamma$ parameter must be tuned to the model and dataset!
 
 ## Documentaion
-A documentation of LXT is available, however we will add more in the coming months!
+A [documentation of LXT is available](https://lxt.readthedocs.io), however we will add more in the coming months!
 The Roadmap lists what is still missing.
 
 ## Contribution
 Feel free to explore the code and experiment with different datasets and models. We encourage contributions and feedback from the community. We are especially grateful for providing support for new model architectures! 🙏
 
 
 ## Acknowledgements
-The code is heavily inspired by [Zennit](https://github.com/chr5tphr/zennit), a tool for LRP attributions in PyTorch using hooks. Zennit is 100% compatible wit LXT and offers even more LRP rules 🎉 If you like LXT, consider also liking Zennit ;)
+The code is heavily inspired by [Zennit](https://github.com/chr5tphr/zennit), a tool for LRP attributions in PyTorch using hooks. Zennit is 100% compatible with LXT and offers even more LRP rules 🎉 If you like LXT, consider also liking Zennit ;)
```

### Comparing `lxt-0.5/README.md` & `lxt-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
   <img src="docs/source/_static/lxt_logo.png" width="300"/>
   <p>Layer-wise Relevance Propagation (LRP) extended to handle attention layers in Large Language Models (LLMs) and Vision Transformers (ViTs)</p>
 </div>
 
 [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)](https://pytorch.org)
-[![Read the Docs](https://img.shields.io/badge/-Docs-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white&link=https://inseq.org)](https://google.de)
+[![Read the Docs](https://img.shields.io/badge/-Docs-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white)](https://lxt.readthedocs.io)
 
 #### 🔥 Faithful Attributions
 
 Attention-aware LRP (AttnLRP) **outperforms** gradient- and perturbation-based methods, provides faithful attributions for the **entirety** of a black-box transformer model while scaling in computational complexitiy $O(1)$ and memory requirements $O(\sqrt{N})$ with respect to the number of layers.
 
 #### 🔎 Latent Feature Attribution & Visualization
 Since we get relevance values for each neuron in the model as a by-product, we know exactly how important each neuron is for the prediction of the model. Combined with Activation Maximization, we can label neurons in LLMs and even steer the generation process of the LLM by activating specialized knowledge neurons in latent space!
@@ -54,15 +54,15 @@
 $ git clone https://github.com/rachtibat/LRP-for-Transformers
 $ pip install ./lxt
 ```
 
 Tested with ``transformers==4.39.3``, ``torch==2.2.2``, ``python==3.11``
 
 ### 💡 How does the code work?
-Layer-wise Relevance Propagation is a rule-based backpropagation algorithm. This means, that we can implement LRP in a singular backward pass!
+Layer-wise Relevance Propagation is a rule-based backpropagation algorithm. This means, that we can implement LRP in a single backward pass!
 To achieve this, we have implemented [custom PyTorch autograd Functions](https://pytorch.org/tutorials/beginner/examples_autograd/two_layer_net_custom_function.html) for commonly used operations in transformers. These functions behave identically in the forward pass, but compute LRP attributions in the backward pass. To compute the $\varepsilon$-LRP rule for a linear function $y = W x + b$, you can simply write
 ```python
 import lxt.functional as lf
 
 y = lf.linear_epsilon(x.requires_grad_(), W, b)
 y.backward(y)
 
@@ -104,16 +104,16 @@
 Applying LRP to new models can be tricky! We provide some basic debugging tools to help you out!
 
 ### ⚙️ Tuning Vision Transformers
 ViTs are vulnerable to noisy attributions, hence we must denoise the heatmap.
 We propose to use the $\gamma$-LRP rule, where the $\gamma$ parameter must be tuned to the model and dataset!
 
 ## Documentaion
-A documentation of LXT is available, however we will add more in the coming months!
+A [documentation of LXT is available](https://lxt.readthedocs.io), however we will add more in the coming months!
 The Roadmap lists what is still missing.
 
 ## Contribution
 Feel free to explore the code and experiment with different datasets and models. We encourage contributions and feedback from the community. We are especially grateful for providing support for new model architectures! 🙏
 
 
 ## Acknowledgements
-The code is heavily inspired by [Zennit](https://github.com/chr5tphr/zennit), a tool for LRP attributions in PyTorch using hooks. Zennit is 100% compatible wit LXT and offers even more LRP rules 🎉 If you like LXT, consider also liking Zennit ;)
+The code is heavily inspired by [Zennit](https://github.com/chr5tphr/zennit), a tool for LRP attributions in PyTorch using hooks. Zennit is 100% compatible with LXT and offers even more LRP rules 🎉 If you like LXT, consider also liking Zennit ;)
```

### Comparing `lxt-0.5/lxt/check.py` & `lxt-0.5.1/lxt/check.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5/lxt/core.py` & `lxt-0.5.1/lxt/core.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5/lxt/functional.py` & `lxt-0.5.1/lxt/functional.py`

 * *Files 19% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     inplace: bool
         Whether to perform the operation in place during the backward pass, will overwrite the relevance at the output
     epsilon: float
         Small value to stabilize the denominator
     """
     
     return add2_tensors_fn.apply(input_a, input_b, inplace, epsilon)
-    # return add2_fn_OLD.apply(input_a, input_b, inplace, epsilon)
 
 @torch.fx.wrap
 def softmax(input, dim, dtype=None, inplace=False):
     """
     Computes Relevance using Deep Taylor Decomposition at x (with bias) according to Proposition 3.1 of the paper
     'AttnLRP: Attention-Aware Layer-wise Relevance Propagation for Transformers'
 
@@ -156,14 +155,91 @@
     input_b: torch.Tensor
         The second input tensor
     inplace: bool
         Whether to perform the operation in place during the backward pass, will overwrite the relevance at the output
     """
     return mul2_fn.apply(input_a, input_b, inplace)
 
+@torch.fx.wrap
+def mean(x, dim, keep_dim, epsilon=1e-6):
+    """
+    Epsilon LRP rule for the mean operation.
+
+    Parameters:
+    -----------
+    x: torch.Tensor
+        The input tensor
+    dim: int
+        The dimension to apply the mean function
+    keep_dim: bool
+        Whether to keep the dimension after applying the mean function
+    epsilon: float
+        Small value to stabilize the denominator
+    """
+    
+    return mean_fn.apply(x, dim, keep_dim, epsilon)
+
+@torch.fx.wrap
+def layer_norm(hidden_states, weight, bias, variance_epsilon):
+    """
+    A mixture of identity and epsilon rules for standard nn.LayerNorm operations:
+    Idenitiy rule for element-wise (y * weight) because single input single output. Identity rule on 1/std because of Proposition 3.4 of the paper
+    'AttnLRP: Attention-Aware Layer-wise Relevance Propagation for Transformers'. 
+    (x - mean) is a linear operation, so we apply the epsilon rule on it.
+
+    To implement this, we do a trick: We differentiate the whole layer, while detaching the std operation from the graph.
+    This is then equivalent to all the rules discussed above! This is slightly faster than implementing everything in pure lxt.
+    See _layer_norm_slower for the pure lxt implementation.
+
+    Parameters:
+    -----------
+    hidden_states: torch.Tensor
+        The input tensor
+    weight: torch.Tensor
+        The weight tensor
+    variance_epsilon: float
+        Small value to stabilize the denominator
+    """
+
+    return layer_norm_grad_fn.apply(hidden_states, weight, bias, variance_epsilon)
+
+@torch.fx.wrap
+def _layer_norm_slower(hidden_states, weight, bias, variance_epsilon):
+    """
+    A mixture of identity and epsilon rules for standard nn.LayerNorm operations:
+    Idenitiy rule for element-wise (y * weight) because single input single output. Identity rule on 1/std because of Proposition 3.4 of the paper
+    'AttnLRP: Attention-Aware Layer-wise Relevance Propagation for Transformers'. 
+    (x - mean) is a linear operation, so we apply the epsilon rule on it.
+
+    This implementation is slower than the layer_norm function because it is implemented in pure lxt instead of using torch.autograd.
+
+    Parameters:
+    -----------
+    hidden_states: torch.Tensor
+        The input tensor
+    weight: torch.Tensor
+        The weight tensor
+    variance_epsilon: float
+        Small value to stabilize the denominator
+    """
+
+    
+    x_mean = mean(hidden_states, -1, keep_dim=True)
+
+    # no relevance will flow through std because we detach!
+    var = ((hidden_states - x_mean) ** 2).mean(dim=-1, keepdim=True)
+    std = (var + variance_epsilon).sqrt().detach()
+    
+    y = add2(hidden_states, mul2(x_mean, -1))
+    # mul2 is identity if the second input does not require gradients
+    y = mul2(y, 1/std)
+    y = mul2(y, weight)
+    y = add2(y, bias)
+
+    return y
 
 ###############################
 ### AUTOGRAD IMPLEMENTATION ###
 ###############################
 
 def _stabilize(input, epsilon=1e-6, inplace=False):
     """
@@ -426,8 +502,107 @@
 
         if ctx.inplace:
             out_relevance = out_relevance[0].div_(n_required)
         else:
             out_relevance = out_relevance[0] / n_required
 
         # only return relevance at requires_grad indices else None
-        return tuple(out_relevance if i in ctx.requires_grads else None for i in range(2)) + (None,)
+        return tuple(out_relevance if i in ctx.requires_grads else None for i in range(2)) + (None,)
+
+
+class mean_fn(Function):
+    """
+    Epsilon LRP rule for the mean operation.
+
+    Parameters:
+    -----------
+    x: torch.Tensor
+        The input tensor
+    dim: int
+        The dimension to apply the mean function
+    keep_dim: bool
+        Whether to keep the dimension after applying the mean function
+    epsilon: float
+        Small value to stabilize the denominator
+    """
+
+    @staticmethod
+    def forward(ctx, x, dim, keepdim, epsilon=1e-6):
+
+        y = x.mean(dim, keepdim)
+    
+        ctx.save_for_backward(x)
+        ctx.epsilon, ctx.dim, ctx.keepdim = epsilon, dim, keepdim
+
+        return y
+
+    @staticmethod
+    @conservation_check_wrap
+    def backward(ctx, *out_relevance):
+
+        x, = ctx.saved_tensors
+
+        x_sum = x.sum(ctx.dim, keepdim=True)
+
+        if ctx.keepdim is False:
+            out_relevance = out_relevance[0].unsqueeze(ctx.dim)
+        else:
+            out_relevance = out_relevance[0]
+
+        relevance = x * out_relevance / _stabilize(x_sum, ctx.epsilon, inplace=True)
+
+        if ctx.keepdim is False:
+            relevance = relevance.squeeze(ctx.dim)
+
+        return (relevance, None, None, None)
+    
+
+class layer_norm_grad_fn(Function):
+    """
+    A mixture of identity and epsilon rules for standard nn.LayerNorm operations:
+    Idenitiy rule for element-wise (y * weight) because single input single output. Identity rule on 1/std because of Proposition 3.4 of the paper
+    'AttnLRP: Attention-Aware Layer-wise Relevance Propagation for Transformers'. 
+    (x - mean) is a linear operation, so we apply the epsilon rule on it.
+
+    To implement this, we do a trick: We differentiate the whole layer, while detaching the std operation from the graph.
+    This is then equivalent to all the rules discussed above! This is slightly faster than implementing everything in pure lxt.
+
+    Parameters:
+    -----------
+    hidden_states: torch.Tensor
+        The input tensor
+    weight: torch.Tensor
+        The weight tensor
+    variance_epsilon: float
+        Small value to stabilize the denominator
+    """
+
+    @staticmethod
+    def forward(ctx, x, weight, bias, variance_epsilon, epsilon=1e-6):
+
+        with torch.enable_grad():
+
+            mean = x.mean(dim=-1, keepdim=True)
+            var = ((x - mean) ** 2).mean(dim=-1, keepdim=True)
+            std = (var + variance_epsilon).sqrt()
+            y = (x - mean) / std.detach() # detach std operation will remove it from computational graph i.e. identity rule on x/std
+            if weight is not None:
+                y *= weight
+            if bias is not None:
+                y += bias
+
+            ctx.save_for_backward(x, y)
+            ctx.epsilon = epsilon
+
+        return y.detach()
+
+    @staticmethod
+    @conservation_check_wrap
+    def backward(ctx, *out_relevance):
+
+        x, y = ctx.saved_tensors
+
+        relevance_norm = out_relevance[0] / _stabilize(y, ctx.epsilon, False)
+
+        grads, = torch.autograd.grad(y, x, relevance_norm)
+
+        return (grads*x, None, None, None, None)
```

### Comparing `lxt-0.5/lxt/modules.py` & `lxt-0.5.1/lxt/modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,23 @@
         self.weight = nn.Parameter(torch.ones(hidden_size))
         self.variance_epsilon = eps
 
     def forward(self, hidden_states):
         return lf.rms_norm_identity_fn.apply(hidden_states, self.weight, self.variance_epsilon)
     
 
+class LayerNormEpsilon(nn.LayerNorm):
+
+    def __init__(self, normalized_shape, eps: float = 0.00001, elementwise_affine: bool = True, bias: bool = True, device=None, dtype=None):
+        super().__init__(normalized_shape, eps, elementwise_affine, bias, device, dtype)
+
+    def forward(self, x):
+        return lf.layer_norm(x, self.weight, self.bias, self.eps)
+    
+
 
 ##########################
 ### Initialize Modules ###
 ##########################
 
 def copy_parameters_and_buffers_(original, replacement):
     """
@@ -70,15 +79,15 @@
 
     replacement = replacement(**kwargs)
     copy_parameters_and_buffers_(original, replacement)
 
     return replacement
 
 
-def initialize_linear(original, replacement):
+def initialize_bias(original, replacement):
     """
     Initialize the LinearEpsilon module correctly with the bias argument.
     """
 
     kwargs = {}
     for arg in inspect.signature(original.__init__).parameters.keys():
         if hasattr(original, arg):
@@ -90,10 +99,11 @@
     copy_parameters_and_buffers_(original, replacement)
 
     return replacement
 
 
 INIT_MODULE_MAPPING = {
     SoftmaxDT: initialize_generic,
-    LinearEpsilon: initialize_linear,
-    RMSNormIdentity: initialize_generic
+    LinearEpsilon: initialize_bias,
+    RMSNormIdentity: initialize_generic,
+    LayerNormEpsilon: initialize_bias
 }
```

### Comparing `lxt-0.5/lxt/rules.py` & `lxt-0.5.1/lxt/rules.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5/lxt/utils.py` & `lxt-0.5.1/lxt/utils.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5/lxt.egg-info/PKG-INFO` & `lxt-0.5.1/lxt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: lxt
-Version: 0.5
+Version: 0.5.1
 Summary: LRP explains Transformers
 Home-page: https://github.com/rachtibat/LRP-for-Transformers
 Author: Reduan Achtibat
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: transformers
-Requires-Dist: accelerate
-Requires-Dist: tabulate
-Requires-Dist: matplotlib
-Requires-Dist: bitsandbytes
 
 <div align="center">
   <img src="docs/source/_static/lxt_logo.png" width="300"/>
   <p>Layer-wise Relevance Propagation (LRP) extended to handle attention layers in Large Language Models (LLMs) and Vision Transformers (ViTs)</p>
 </div>
 
 [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)](https://pytorch.org)
-[![Read the Docs](https://img.shields.io/badge/-Docs-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white&link=https://inseq.org)](https://google.de)
+[![Read the Docs](https://img.shields.io/badge/-Docs-blue?style=for-the-badge&logo=Read-the-Docs&logoColor=white)](https://lxt.readthedocs.io)
 
 #### 🔥 Faithful Attributions
 
 Attention-aware LRP (AttnLRP) **outperforms** gradient- and perturbation-based methods, provides faithful attributions for the **entirety** of a black-box transformer model while scaling in computational complexitiy $O(1)$ and memory requirements $O(\sqrt{N})$ with respect to the number of layers.
 
 #### 🔎 Latent Feature Attribution & Visualization
 Since we get relevance values for each neuron in the model as a by-product, we know exactly how important each neuron is for the prediction of the model. Combined with Activation Maximization, we can label neurons in LLMs and even steer the generation process of the LLM by activating specialized knowledge neurons in latent space!
@@ -70,15 +64,15 @@
 $ git clone https://github.com/rachtibat/LRP-for-Transformers
 $ pip install ./lxt
 ```
 
 Tested with ``transformers==4.39.3``, ``torch==2.2.2``, ``python==3.11``
 
 ### 💡 How does the code work?
-Layer-wise Relevance Propagation is a rule-based backpropagation algorithm. This means, that we can implement LRP in a singular backward pass!
+Layer-wise Relevance Propagation is a rule-based backpropagation algorithm. This means, that we can implement LRP in a single backward pass!
 To achieve this, we have implemented [custom PyTorch autograd Functions](https://pytorch.org/tutorials/beginner/examples_autograd/two_layer_net_custom_function.html) for commonly used operations in transformers. These functions behave identically in the forward pass, but compute LRP attributions in the backward pass. To compute the $\varepsilon$-LRP rule for a linear function $y = W x + b$, you can simply write
 ```python
 import lxt.functional as lf
 
 y = lf.linear_epsilon(x.requires_grad_(), W, b)
 y.backward(y)
 
@@ -120,16 +114,16 @@
 Applying LRP to new models can be tricky! We provide some basic debugging tools to help you out!
 
 ### ⚙️ Tuning Vision Transformers
 ViTs are vulnerable to noisy attributions, hence we must denoise the heatmap.
 We propose to use the $\gamma$-LRP rule, where the $\gamma$ parameter must be tuned to the model and dataset!
 
 ## Documentaion
-A documentation of LXT is available, however we will add more in the coming months!
+A [documentation of LXT is available](https://lxt.readthedocs.io), however we will add more in the coming months!
 The Roadmap lists what is still missing.
 
 ## Contribution
 Feel free to explore the code and experiment with different datasets and models. We encourage contributions and feedback from the community. We are especially grateful for providing support for new model architectures! 🙏
 
 
 ## Acknowledgements
-The code is heavily inspired by [Zennit](https://github.com/chr5tphr/zennit), a tool for LRP attributions in PyTorch using hooks. Zennit is 100% compatible wit LXT and offers even more LRP rules 🎉 If you like LXT, consider also liking Zennit ;)
+The code is heavily inspired by [Zennit](https://github.com/chr5tphr/zennit), a tool for LRP attributions in PyTorch using hooks. Zennit is 100% compatible with LXT and offers even more LRP rules 🎉 If you like LXT, consider also liking Zennit ;)
```

### Comparing `lxt-0.5/setup.py` & `lxt-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='lxt',  
-    version='0.5',
+    version='0.5.1',
     install_requires=[
         'torch',
         'transformers',
         'accelerate',
         'tabulate',
         'matplotlib',
         'bitsandbytes'
```

### Comparing `lxt-0.5/tests/test_functional.py` & `lxt-0.5.1/tests/test_functional.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import torch
-import lxt.functional as functional
+import lxt.functional as lf
 from torch.nn import functional as F
 import torch.nn as nn
 
 
 def test_softmax():
 
     x = torch.randn(16, 10, 32, requires_grad=True)
@@ -12,52 +12,50 @@
 
     y_gt = F.softmax(x, -1)
 
     # implement Proposition 3.1 of AttnLRP paper
     relevance_gt = x.float() * (init_relevance - y_gt * init_relevance.sum(-1, keepdim=True))
 
     # test inplace=False
-    y_lxt = functional.softmax.apply(x, -1, torch.float32, False)
+    y_lxt = lf.softmax(x, -1, torch.float32, False)
     relevance_lxt, = torch.autograd.grad(y_lxt, x, init_relevance)
     assert torch.allclose(relevance_gt, relevance_lxt, rtol=0, atol=1e-5)
 
     # test inplace=True
-    y_lxt = functional.softmax.apply(x, -1, torch.float32, True)
+    y_lxt = lf.softmax(x, -1, torch.float32, True)
     relevance_lxt, = torch.autograd.grad(y_lxt, x, init_relevance)
     assert torch.allclose(relevance_gt, relevance_lxt, rtol=0, atol=1e-5)
 
-    print("softmax test passed")
-
 
 def test_matmul():
 
     epsilon = 1e-9
 
-    a = torch.randn(16, 10, 32, requires_grad=True)
-    b = torch.randn(16, 32, 5, requires_grad=True)
+    a = torch.randn(2, 10, 32, requires_grad=True)
+    b = torch.randn(2, 32, 5, requires_grad=True)
 
-    init_relevance = torch.randn(16, 10, 5, requires_grad=True)
+    init_relevance = torch.randn(2, 10, 5, requires_grad=True)
 
     y_gt = torch.matmul(a, b)
 
     # implement Proposition 3.3 of AttnLRP paper
     relevance_a_gt = torch.einsum("bji, bip, bjp -> bji", a, b, init_relevance / (2*y_gt + epsilon))
     relevance_b_gt = torch.einsum("bji, bip, bjp -> bip", a, b, init_relevance / (2*y_gt + epsilon))
 
     # test inplace=False
-    y_lxt = functional.matmul.apply(a, b, False, epsilon)
+    y_lxt = lf.matmul(a, b, False, epsilon)
     relevance_a_lxt, relevance_b_lxt = torch.autograd.grad(y_lxt, (a, b), init_relevance)
-    assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-5)
-    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-5)
+    assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-4)
+    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-4)
 
     # test inplace=True
-    y_lxt = functional.matmul.apply(a, b, True, epsilon)
+    y_lxt = lf.matmul(a, b, True, epsilon)
     relevance_a_lxt, relevance_b_lxt = torch.autograd.grad(y_lxt, (a, b), init_relevance)
-    assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-5)
-    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-5)
+    assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-4)
+    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-4)
 
 
 def test_linear():
 
     epsilon = 1e-9
 
     x = torch.randn(16, 10, requires_grad=True)
@@ -68,18 +66,18 @@
 
     y_gt = F.linear(x, weight, bias)
 
     # implement Equation 8 of AttnLRP paper
     relevace_gt = torch.einsum("ji, bi, bj -> bi", weight, x, init_relevance / (y_gt + epsilon))
 
     # test inplace=False
-    y_lxt = functional.linear_epsilon.apply(x, weight, bias, epsilon)
+    y_lxt = lf.linear_epsilon(x, weight, bias, epsilon)
     relevance_lxt, = torch.autograd.grad(y_lxt, x, init_relevance)
 
-    assert torch.allclose(relevace_gt, relevance_lxt, rtol=0, atol=1e-5)
+    assert torch.allclose(relevace_gt, relevance_lxt, rtol=0, atol=1e-4)
 
 
 def test_sum():
 
     epsilon = 1e-9
 
     a = torch.randn(16, 10, 32, requires_grad=True)
@@ -90,19 +88,78 @@
     y_gt = a + b
 
     # implement epsilon rule for summation
     relevance_a_gt = a * (init_relevance / (y_gt + epsilon))
     relevance_b_gt = b * (init_relevance / (y_gt + epsilon))
 
     # test inplace=False
-    y_lxt = functional.add2.apply(a, b, False, epsilon)
+    y_lxt = lf.add2(a, b, False, epsilon)
     relevance_a_lxt, relevance_b_lxt = torch.autograd.grad(y_lxt, (a, b), init_relevance)
 
-    assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-5)
-    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-5)
+    assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-4)
+    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-4)
 
     # test inplace=True
-    y_lxt = functional.add2.apply(a, b, True, epsilon)
+    y_lxt = lf.add2(a, b, True, epsilon)
     relevance_a_lxt, relevance_b_lxt = torch.autograd.grad(y_lxt, (a, b), init_relevance)
 
     assert torch.allclose(relevance_a_gt, relevance_a_lxt, rtol=0, atol=1e-5)
-    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-5)
+    assert torch.allclose(relevance_b_gt, relevance_b_lxt, rtol=0, atol=1e-5)
+
+
+def test_mean():
+
+    epsilon = 1e-9
+
+    a = torch.randn(1, 8, 32, requires_grad=True)
+    init_relevance = torch.randn(1, 8)
+
+    # implement epsilon rule for mean
+    relevance_gt = a * (init_relevance.unsqueeze(-1) / (a.sum(-1).unsqueeze(-1) + epsilon))
+
+    ## --- test keep_dim=True
+    y_lxt = lf.mean(a, -1, True, epsilon)
+    relevance_lxt, = torch.autograd.grad(y_lxt, a, init_relevance.unsqueeze(-1))
+
+    assert torch.allclose(relevance_gt, relevance_lxt, rtol=0, atol=1e-4)
+
+    ## --- test keep_dim=False
+    y_lxt = lf.mean(a, -1, False, epsilon)
+    relevance_lxt, = torch.autograd.grad(y_lxt, a, init_relevance)
+
+    assert torch.allclose(relevance_gt, relevance_lxt, rtol=0, atol=1e-4)
+
+
+def test_layernorm():
+
+    x = torch.randn(1, 4, 32, requires_grad=True)
+    init_relevance = torch.randn(1, 4, 32)
+
+    layer = torch.nn.LayerNorm(32)
+    weight = torch.randn_like(layer.weight)
+    bias = torch.randn_like(layer.bias)
+    layer.weight = nn.Parameter(weight)
+    layer.bias = nn.Parameter(bias)
+    layer.weight.requires_grad_(False)
+    layer.bias.requires_grad_(False)
+
+    ### round truth
+    y = lf.layer_norm(x, weight, bias, layer.eps)
+    relevance_gt, = torch.autograd.grad(y, x, init_relevance)
+
+    ### lxt
+    y = lf._layer_norm_slower(x, weight, bias, layer.eps)
+    relevance_lxt, = torch.autograd.grad(y, x, init_relevance)
+
+    assert torch.allclose(relevance_lxt, relevance_gt, rtol=0, atol=1e-3)
+
+
+if __name__ == "__main__":
+
+    test_softmax()
+    test_matmul()
+    test_linear()
+    test_sum()
+    test_mean()
+    test_layernorm()
+
+    print("ALL TESTS PASSED")
```

### Comparing `lxt-0.5/tests/test_rules.py` & `lxt-0.5.1/tests/test_rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
 import torch
 import lxt.rules as rules
-import lxt.functional as functional
+import lxt.functional as lf
 from torch.nn import functional as F
 import torch.nn as nn
+from functools import partial
 
 def test_epsilon_rule():
 
     x = torch.randn(1, 5, requires_grad=True)
     weights = torch.randn(5, 5, requires_grad=False)
     bias = torch.randn(5, requires_grad=False)
 
     init_relevance = torch.randn(1, 5, requires_grad=True)
 
-    y_gt = functional.linear_epsilon.apply(x, weights, bias)
+    y_gt = lf.linear_epsilon(x, weights, bias)
     relevance_gt, = torch.autograd.grad(y_gt, x, init_relevance)
 
-    y_lxt = rules.EpsilonRule.apply(F.linear, x, weights, bias)
+    layer = rules.EpsilonRule(partial(F.linear, weight=weights, bias=bias))
+    y_lxt = layer(x)
     relevance_lxt, = torch.autograd.grad(y_lxt, x, init_relevance)
 
     assert torch.allclose(relevance_gt, relevance_lxt, rtol=0, atol=1e-5)
```

