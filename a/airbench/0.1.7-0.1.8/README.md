# Comparing `tmp/airbench-0.1.7.tar.gz` & `tmp/airbench-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbench-0.1.7.tar", last modified: Thu Mar 28 11:34:58 2024, max compression
+gzip compressed data, was "airbench-0.1.8.tar", last modified: Thu Apr 11 20:36:30 2024, max compression
```

## Comparing `airbench-0.1.7.tar` & `airbench-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-28 11:34:58.664934 airbench-0.1.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5455 2024-03-28 11:34:58.664934 airbench-0.1.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3679 2024-03-26 09:42:33.000000 airbench-0.1.7/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-28 11:34:58.664934 airbench-0.1.7/airbench/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      542 2024-03-22 00:04:22.000000 airbench-0.1.7/airbench/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6050 2024-03-28 10:59:02.000000 airbench-0.1.7/airbench/lib_airbench93.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2024-03-28 10:59:07.000000 airbench-0.1.7/airbench/lib_airbench94.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5963 2024-03-28 10:59:20.000000 airbench-0.1.7/airbench/lib_airbench95.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6214 2024-03-28 10:59:29.000000 airbench-0.1.7/airbench/lib_airbench96.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14897 2024-03-28 11:01:48.000000 airbench-0.1.7/airbench/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-28 11:34:58.664934 airbench-0.1.7/airbench.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5455 2024-03-28 11:34:58.000000 airbench-0.1.7/airbench.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2024-03-28 11:34:58.000000 airbench-0.1.7/airbench.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-28 11:34:58.000000 airbench-0.1.7/airbench.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-03-28 11:34:58.000000 airbench-0.1.7/airbench.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-28 11:34:58.664934 airbench-0.1.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1110 2024-03-28 11:34:46.000000 airbench-0.1.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-11 20:36:30.055373 airbench-0.1.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6151 2024-04-11 20:36:30.055373 airbench-0.1.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4335 2024-04-11 20:36:07.000000 airbench-0.1.8/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-11 20:36:30.055373 airbench-0.1.8/airbench/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      542 2024-03-22 00:04:22.000000 airbench-0.1.8/airbench/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6096 2024-04-11 20:32:27.000000 airbench-0.1.8/airbench/lib_airbench93.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6008 2024-04-11 20:32:53.000000 airbench-0.1.8/airbench/lib_airbench94.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6009 2024-04-11 20:33:05.000000 airbench-0.1.8/airbench/lib_airbench95.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6260 2024-04-11 20:33:15.000000 airbench-0.1.8/airbench/lib_airbench96.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14897 2024-03-28 11:01:48.000000 airbench-0.1.8/airbench/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-11 20:36:30.055373 airbench-0.1.8/airbench.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6151 2024-04-11 20:36:29.000000 airbench-0.1.8/airbench.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2024-04-11 20:36:30.000000 airbench-0.1.8/airbench.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-11 20:36:29.000000 airbench-0.1.8/airbench.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-11 20:36:29.000000 airbench-0.1.8/airbench.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-11 20:36:30.055373 airbench-0.1.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1110 2024-04-11 20:36:20.000000 airbench-0.1.8/setup.py
```

### Comparing `airbench-0.1.7/PKG-INFO` & `airbench-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 Metadata-Version: 2.1
 Name: airbench
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utilities and baselines for fast neural network training on CIFAR-10
 Home-page: https://github.com/KellerJordan/cifar10-airbench
 Author: Keller Jordan
 Author-email: kjordan4077@gmail.com
 License: UNKNOWN
 Description: # CIFAR-10 Airbench 💨
         
-        Fast training baselines for CIFAR-10.
+        Training methods for CIFAR-10 with state-of-the-art speed.
         
+        | Script | Mean accuracy | Time | PFLOPs |
+        | - | - | - | - |
+        | `airbench94_compiled.py` | 94.01% | 3.29s | 0.36 |
+        | `airbench94.py` | 94.01% | 3.83s | 0.36 |
+        | `airbench95.py` | 95.01% | 10.4s | 1.4 |
+        | `airbench96.py` | 96.05% | 46.3s | 7.5 |
+        
+        Timings are on a single NVIDIA A100 GPU.
+        Note that the first run of training will be slower due to GPU warmup.
+        
+        `airbench94_compiled.py` and `airbench94.py` are equivalent (i.e., yield the same distribution of trained networks), and differ only in that the first uses `torch.compile` to improve GPU utilization. The former is intended for experiments where many networks are trained at once in order to amortize the one-time compilation cost.
+        
+        Paper: https://arxiv.org/abs/2404.00498
         
         ## How to run
         
         To train a neural network with 94% accuracy, run either
         
         ```
         git clone https://github.com/KellerJordan/cifar10-airbench.git
         python airbench/airbench94.py
         ```
         
         or
         
         ```
         pip install airbench
-        python -c "import airbench; airbench.train94()"
+        python -c "import airbench; airbench.warmup94(); airbench.train94()"
         ```
         
         
         ## Motivation
         
         CIFAR-10 is among the most widely used datasets in machine learning, facilitating thousands of research projects per year. 
         This repo provides three fast and stable training baselines for CIFAR-10 in order to help accelerate small-scale neural network research.
         The trainings are provided as easily runnable dependency-free PyTorch scripts, and can replace classic baselines like training ResNet-20 or ResNet-18.
         
         
-        ## Training methods
-        
-        | Script | Mean accuracy | Time | PFLOPs |
-        | - | - | - | - |
-        | `airbench94_compiled.py` | 94.01% | 3.29s | 0.36 |
-        | `airbench94.py` | 94.01% | 3.83s | 0.36 |
-        | `airbench95.py` | 95.01% | 10.4s | 1.4 |
-        | `airbench96.py` | 96.05% | 46.3s | 7.5 |
-        
-        Timings are on a single NVIDIA A100 GPU.
-        Note that the first run of training is slower due to GPU warmup.
-        
-        
         ## Using the GPU-accelerated dataloader independently
         
         For writing custom CIFAR-10 experiments or trainings, you may find it useful to use the GPU-accelerated dataloader independently.
         ```
         import airbench
         train_loader = airbench.CifarLoader('/tmp/cifar10', train=True, aug=dict(flip=True, translate=4, cutout=16), batch_size=500)
         test_loader = airbench.CifarLoader('/tmp/cifar10', train=False, batch_size=1000)
@@ -100,14 +100,19 @@
         mask = (conf < conf.float().quantile(0.6))
         print('Training on %d images selected based on minimum confidence' % mask.sum())
         train_loader.images = train_loader.images[mask]
         train_loader.labels = train_loader.labels[mask]
         train94(train_loader, epochs=16) # yields around 94% accuracy => low-confidence sampling is better than random.
         ```
         
+        ## Prior work
+        
+        This project builds on the excellent previous record https://github.com/tysam-code/hlb-CIFAR10 (6.3 A100-seconds).
+        
+        Which itself builds on the amazing series https://myrtle.ai/learn/how-to-train-your-resnet/ (26 V100-seconds = >8 A100-seconds)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `airbench-0.1.7/README.md` & `airbench-0.1.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # CIFAR-10 Airbench 💨
 
-Fast training baselines for CIFAR-10.
+Training methods for CIFAR-10 with state-of-the-art speed.
 
+| Script | Mean accuracy | Time | PFLOPs |
+| - | - | - | - |
+| `airbench94_compiled.py` | 94.01% | 3.29s | 0.36 |
+| `airbench94.py` | 94.01% | 3.83s | 0.36 |
+| `airbench95.py` | 95.01% | 10.4s | 1.4 |
+| `airbench96.py` | 96.05% | 46.3s | 7.5 |
+
+Timings are on a single NVIDIA A100 GPU.
+Note that the first run of training will be slower due to GPU warmup.
+
+`airbench94_compiled.py` and `airbench94.py` are equivalent (i.e., yield the same distribution of trained networks), and differ only in that the first uses `torch.compile` to improve GPU utilization. The former is intended for experiments where many networks are trained at once in order to amortize the one-time compilation cost.
+
+Paper: https://arxiv.org/abs/2404.00498
 
 ## How to run
 
 To train a neural network with 94% accuracy, run either
 
 ```
 git clone https://github.com/KellerJordan/cifar10-airbench.git
 python airbench/airbench94.py
 ```
 
 or
 
 ```
 pip install airbench
-python -c "import airbench; airbench.train94()"
+python -c "import airbench; airbench.warmup94(); airbench.train94()"
 ```
 
 
 ## Motivation
 
 CIFAR-10 is among the most widely used datasets in machine learning, facilitating thousands of research projects per year. 
 This repo provides three fast and stable training baselines for CIFAR-10 in order to help accelerate small-scale neural network research.
 The trainings are provided as easily runnable dependency-free PyTorch scripts, and can replace classic baselines like training ResNet-20 or ResNet-18.
 
 
-## Training methods
-
-| Script | Mean accuracy | Time | PFLOPs |
-| - | - | - | - |
-| `airbench94_compiled.py` | 94.01% | 3.29s | 0.36 |
-| `airbench94.py` | 94.01% | 3.83s | 0.36 |
-| `airbench95.py` | 95.01% | 10.4s | 1.4 |
-| `airbench96.py` | 96.05% | 46.3s | 7.5 |
-
-Timings are on a single NVIDIA A100 GPU.
-Note that the first run of training is slower due to GPU warmup.
-
-
 ## Using the GPU-accelerated dataloader independently
 
 For writing custom CIFAR-10 experiments or trainings, you may find it useful to use the GPU-accelerated dataloader independently.
 ```
 import airbench
 train_loader = airbench.CifarLoader('/tmp/cifar10', train=True, aug=dict(flip=True, translate=4, cutout=16), batch_size=500)
 test_loader = airbench.CifarLoader('/tmp/cifar10', train=False, batch_size=1000)
@@ -92,7 +92,12 @@
 mask = (conf < conf.float().quantile(0.6))
 print('Training on %d images selected based on minimum confidence' % mask.sum())
 train_loader.images = train_loader.images[mask]
 train_loader.labels = train_loader.labels[mask]
 train94(train_loader, epochs=16) # yields around 94% accuracy => low-confidence sampling is better than random.
 ```
 
+## Prior work
+
+This project builds on the excellent previous record https://github.com/tysam-code/hlb-CIFAR10 (6.3 A100-seconds).
+
+Which itself builds on the amazing series https://myrtle.ai/learn/how-to-train-your-resnet/ (26 V100-seconds = >8 A100-seconds)
```

### Comparing `airbench-0.1.7/airbench/__init__.py` & `airbench-0.1.8/airbench/__init__.py`

 * *Files identical despite different names*

### Comparing `airbench-0.1.7/airbench/lib_airbench93.py` & `airbench-0.1.8/airbench/lib_airbench93.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,17 +132,19 @@
             mod.float()
     return net
 
 ############################################
 #             Train and Eval               #
 ############################################
 
-def train93(train_loader=CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True),
-            epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
+def train93(train_loader=None, epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
             learning_rate=hyp['opt']['lr'], bias_scaler=hyp['opt']['bias_scaler'],
             momentum=hyp['opt']['momentum'], weight_decay=hyp['opt']['weight_decay'],
             whiten_bias_epochs=hyp['opt']['whiten_bias_epochs'], tta_level=hyp['net']['tta_level'],
             make_net=make_net93, run=0, verbose=True):
 
+    if train_loader is None:
+        train_loader = CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True)
+
     return train(train_loader, epochs, label_smoothing, learning_rate, bias_scaler, momentum, weight_decay,
                  whiten_bias_epochs, tta_level, make_net, run, verbose)
```

### Comparing `airbench-0.1.7/airbench/lib_airbench94.py` & `airbench-0.1.8/airbench/lib_airbench94.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,19 @@
             mod.float()
     return net
 
 ############################################
 #             Train and Eval               #
 ############################################
 
-def train94(train_loader=CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True),
-            epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
+def train94(train_loader=None, epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
             learning_rate=hyp['opt']['lr'], bias_scaler=hyp['opt']['bias_scaler'],
             momentum=hyp['opt']['momentum'], weight_decay=hyp['opt']['weight_decay'],
             whiten_bias_epochs=hyp['opt']['whiten_bias_epochs'], tta_level=hyp['net']['tta_level'],
             make_net=make_net94, run=0, verbose=True):
 
+    if train_loader is None:
+        train_loader = CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True)
+
     return train(train_loader, epochs, label_smoothing, learning_rate, bias_scaler, momentum, weight_decay,
                  whiten_bias_epochs, tta_level, make_net, run, verbose)
```

### Comparing `airbench-0.1.7/airbench/lib_airbench95.py` & `airbench-0.1.8/airbench/lib_airbench95.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,17 +131,19 @@
             mod.float()
     return net
 
 ############################################
 #             Train and Eval               #
 ############################################
 
-def train95(train_loader=CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True),
-            epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
+def train95(train_loader=None, epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
             learning_rate=hyp['opt']['lr'], bias_scaler=hyp['opt']['bias_scaler'],
             momentum=hyp['opt']['momentum'], weight_decay=hyp['opt']['weight_decay'],
             whiten_bias_epochs=hyp['opt']['whiten_bias_epochs'], tta_level=hyp['net']['tta_level'],
             make_net=make_net95, run=0, verbose=True):
 
+    if train_loader is None:
+        train_loader = CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True)
+
     return train(train_loader, epochs, label_smoothing, learning_rate, bias_scaler, momentum, weight_decay,
                  whiten_bias_epochs, tta_level, make_net, run, verbose)
```

### Comparing `airbench-0.1.7/airbench/lib_airbench96.py` & `airbench-0.1.8/airbench/lib_airbench96.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,19 @@
             mod.float()
     return net
 
 ############################################
 #             Train and Eval               #
 ############################################
 
-def train96(train_loader=CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True),
-            epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
+def train96(train_loader=None, epochs=hyp['opt']['train_epochs'], label_smoothing=hyp['opt']['label_smoothing'],
             learning_rate=hyp['opt']['lr'], bias_scaler=hyp['opt']['bias_scaler'],
             momentum=hyp['opt']['momentum'], weight_decay=hyp['opt']['weight_decay'],
             whiten_bias_epochs=hyp['opt']['whiten_bias_epochs'], tta_level=hyp['net']['tta_level'],
             make_net=make_net96, run=0, verbose=True):
 
+    if train_loader is None:
+        train_loader = CifarLoader('cifar10', train=True, batch_size=hyp['opt']['batch_size'], aug=hyp['aug'], altflip=True)
+
     return train(train_loader, epochs, label_smoothing, learning_rate, bias_scaler, momentum, weight_decay,
                  whiten_bias_epochs, tta_level, make_net, run, verbose)
```

### Comparing `airbench-0.1.7/airbench/utils.py` & `airbench-0.1.8/airbench/utils.py`

 * *Files identical despite different names*

### Comparing `airbench-0.1.7/airbench.egg-info/PKG-INFO` & `airbench-0.1.8/airbench.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 Metadata-Version: 2.1
 Name: airbench
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utilities and baselines for fast neural network training on CIFAR-10
 Home-page: https://github.com/KellerJordan/cifar10-airbench
 Author: Keller Jordan
 Author-email: kjordan4077@gmail.com
 License: UNKNOWN
 Description: # CIFAR-10 Airbench 💨
         
-        Fast training baselines for CIFAR-10.
+        Training methods for CIFAR-10 with state-of-the-art speed.
         
+        | Script | Mean accuracy | Time | PFLOPs |
+        | - | - | - | - |
+        | `airbench94_compiled.py` | 94.01% | 3.29s | 0.36 |
+        | `airbench94.py` | 94.01% | 3.83s | 0.36 |
+        | `airbench95.py` | 95.01% | 10.4s | 1.4 |
+        | `airbench96.py` | 96.05% | 46.3s | 7.5 |
+        
+        Timings are on a single NVIDIA A100 GPU.
+        Note that the first run of training will be slower due to GPU warmup.
+        
+        `airbench94_compiled.py` and `airbench94.py` are equivalent (i.e., yield the same distribution of trained networks), and differ only in that the first uses `torch.compile` to improve GPU utilization. The former is intended for experiments where many networks are trained at once in order to amortize the one-time compilation cost.
+        
+        Paper: https://arxiv.org/abs/2404.00498
         
         ## How to run
         
         To train a neural network with 94% accuracy, run either
         
         ```
         git clone https://github.com/KellerJordan/cifar10-airbench.git
         python airbench/airbench94.py
         ```
         
         or
         
         ```
         pip install airbench
-        python -c "import airbench; airbench.train94()"
+        python -c "import airbench; airbench.warmup94(); airbench.train94()"
         ```
         
         
         ## Motivation
         
         CIFAR-10 is among the most widely used datasets in machine learning, facilitating thousands of research projects per year. 
         This repo provides three fast and stable training baselines for CIFAR-10 in order to help accelerate small-scale neural network research.
         The trainings are provided as easily runnable dependency-free PyTorch scripts, and can replace classic baselines like training ResNet-20 or ResNet-18.
         
         
-        ## Training methods
-        
-        | Script | Mean accuracy | Time | PFLOPs |
-        | - | - | - | - |
-        | `airbench94_compiled.py` | 94.01% | 3.29s | 0.36 |
-        | `airbench94.py` | 94.01% | 3.83s | 0.36 |
-        | `airbench95.py` | 95.01% | 10.4s | 1.4 |
-        | `airbench96.py` | 96.05% | 46.3s | 7.5 |
-        
-        Timings are on a single NVIDIA A100 GPU.
-        Note that the first run of training is slower due to GPU warmup.
-        
-        
         ## Using the GPU-accelerated dataloader independently
         
         For writing custom CIFAR-10 experiments or trainings, you may find it useful to use the GPU-accelerated dataloader independently.
         ```
         import airbench
         train_loader = airbench.CifarLoader('/tmp/cifar10', train=True, aug=dict(flip=True, translate=4, cutout=16), batch_size=500)
         test_loader = airbench.CifarLoader('/tmp/cifar10', train=False, batch_size=1000)
@@ -100,14 +100,19 @@
         mask = (conf < conf.float().quantile(0.6))
         print('Training on %d images selected based on minimum confidence' % mask.sum())
         train_loader.images = train_loader.images[mask]
         train_loader.labels = train_loader.labels[mask]
         train94(train_loader, epochs=16) # yields around 94% accuracy => low-confidence sampling is better than random.
         ```
         
+        ## Prior work
+        
+        This project builds on the excellent previous record https://github.com/tysam-code/hlb-CIFAR10 (6.3 A100-seconds).
+        
+        Which itself builds on the amazing series https://myrtle.ai/learn/how-to-train-your-resnet/ (26 V100-seconds = >8 A100-seconds)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `airbench-0.1.7/setup.py` & `airbench-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airbench',
-    version='0.1.7',
+    version='0.1.8',
     author='Keller Jordan',
     author_email='kjordan4077@gmail.com',
     description='Utilities and baselines for fast neural network training on CIFAR-10',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KellerJordan/cifar10-airbench',
     packages=find_packages(),
```

