# Comparing `tmp/kkpyai-0.4.0.tar.gz` & `tmp/kkpyai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.4.0.tar", max compression
+gzip compressed data, was "kkpyai-0.5.0.tar", max compression
```

## Comparing `kkpyai-0.4.0.tar` & `kkpyai-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.4.0/LICENSE
--rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.4.0/README.md
--rw-r--r--   0        0        0     8190 2024-04-11 18:26:15.665996 kkpyai-0.4.0/kkpyai/kktorch.py
--rw-r--r--   0        0        0      420 2024-04-11 18:27:55.534516 kkpyai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 kkpyai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.5.0/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.5.0/README.md
+-rw-r--r--   0        0        0     9553 2024-04-11 19:25:17.524948 kkpyai-0.5.0/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      420 2024-04-11 19:08:10.389722 kkpyai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 kkpyai-0.5.0/PKG-INFO
```

### Comparing `kkpyai-0.4.0/LICENSE` & `kkpyai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyai-0.4.0/kkpyai/kktorch.py` & `kkpyai-0.5.0/kkpyai/kktorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import os.path as osp
 import typing
 # 3rd party
 import kkpyutil as util
 import torch as tc
 import matplotlib.pyplot as plt
+import numpy as np
 
 
 # region globals
 
 def find_fastest_device():
     """
     - Apple Silicon uses Apple's own Metal Performance Shaders (MPS) instead of CUDA
@@ -95,14 +96,15 @@
 class Model(Loggable):
     def __init__(self, model, lossfn_name='L1Loss', optm_name='SGD', learning_rate=0.01, device_name=None, logger=None):
         super().__init__(logger)
         self.device = device_name or find_fastest_device()
         self.model = model.to(self.device)
         self.lossFunction = eval(f'tc.nn.{lossfn_name}()')
         self.optimizer = eval(f'tc.optim.{optm_name}(self.model.parameters(), lr={learning_rate})')
+        self.plot = Plot()
 
     def set_lossfunction(self, lossfn_name='L1Loss'):
         """
         - ref: https://pytorch.org/docs/stable/nn.html#loss-functions
         """
         self.lossFunction = eval(f'nn.{lossfn_name}()')
 
@@ -113,14 +115,15 @@
         self.optimizer = eval(f'tc.optim.{opt_name}(self.model.parameters(), lr={learning_rate})')
 
     def train(self, train_set, test_set=None, n_epochs=1000, seed=42, verbose=False, log_every_n_epochs=100):
         tc.manual_seed(seed)
         X_train = train_set['data'].to(self.device)
         y_train = train_set['labels'].to(self.device)
         pred = {'preds': None, 'loss': None}
+        losses = {'train': [], 'test': []}
         if test_set:
             X_test = test_set['data'].to(self.device)
             y_test = test_set['labels'].to(self.device)
         for epoch in range(n_epochs):
             # Training
             # - train mode is on by default after construction
             self.model.train()
@@ -132,62 +135,79 @@
             self.optimizer.zero_grad()
             # - backpropagation
             loss.backward()
             # - update weights and biases
             self.optimizer.step()
             if test_set:
                 pred = self.evaluate(test_set)
+                if verbose:
+                    losses['train'].append(loss.cpu().detach().numpy())
+                    losses['test'].append(pred['loss'].cpu().detach().numpy())
             if verbose and epoch % log_every_n_epochs == 0:
                 msg = f"Epoch: {epoch} | Train Loss: {loss} | Test Loss: {pred['loss']}" if test_set else f"Epoch: {epoch} | Train Loss: {loss}"
                 self.logger.info(msg)
+        if verbose:
+            # plot predictions
+            self.plot.unblock()
+            self.plot.plot_predictions(train_set, test_set, pred['pred'])
+            self.plot.plot_learning(losses['train'], losses['test'])
         # final test predictions
         return pred
 
-    def evaluate(self, test_set):
+    def evaluate(self, test_set, verbose=False):
+        """
+        - test_set must contain ground-truth labels
+        """
         X_test = test_set['data'].to(self.device)
         y_test = test_set['labels'].to(self.device)
         # Testing
         # - eval mode is on by default after construction
         self.model.eval()
         # - forward pass
         with tc.inference_mode():
             test_pred = self.model(X_test)
             # - compute loss
             test_loss = self.lossFunction(test_pred, y_test)
+        if verbose:
+            self.logger.info(f'Test Loss: {test_loss}')
+            self.plot.unblock()
+            self.plot.plot_predictions(None, test_set, test_pred)
         return {'pred': test_pred, 'loss': test_loss}
 
     def predict(self, test_set):
         """
-        - we predict when test_set has no labels
-        - otherwise we evaluate the model
+        - test_set can have no labels
         """
         X_test = test_set['data'].to(self.device)
         test_set['labels'] = test_set['labels'].to(self.device)
         # Testing
         # - eval mode is on by default after construction
         self.model.eval()
         # - forward pass
         with tc.inference_mode():
             predictions = self.model(X_test)
         return predictions.to(self.device)
 
+    def close_plot(self):
+        self.plot.close()
+
     def save(self, model_basename=None, optimized=True):
         ext = '.pth' if optimized else '.pt'
         path = self._compose_model_name(model_basename, ext)
         os.makedirs(osp.dirname(path), exist_ok=True)
         tc.save(self.model.state_dict(), path)
 
     def load(self, model_basename=None, optimized=True):
         ext = '.pth' if optimized else '.pt'
         path = self._compose_model_name(model_basename, ext)
         self.model.load_state_dict(tc.load(path))
 
     @staticmethod
     def _compose_model_name(model_basename, ext):
-        return osp.join(util.get_platform_tmp_dir(), 'torch', f'{model_basename}.{ext}')
+        return osp.join(util.get_platform_tmp_dir(), 'torch', f'{model_basename}{ext}')
 
 # endregion
 
 
 # region visualization
 
 class Plot:
@@ -196,18 +216,32 @@
         self.useBlocking = True
 
     def plot_predictions(self, train_set, test_set, predictions=None):
         """
         - sets contain data and labels
         """
         fig, ax = plt.subplots(figsize=(10, 7))
-        ax.scatter(train_set['data'], train_set['labels'], s=4, color='blue', label='Training Data')
-        ax.scatter(test_set['data'], test_set['labels'], s=4, color='green', label='Testing Data')
+        if train_set:
+            ax.scatter(train_set['data'].cpu(), train_set['labels'].cpu(), s=4, color='blue', label='Training Data')
+        if test_set:
+            ax.scatter(test_set['data'].cpu(), test_set['labels'].cpu(), s=4, color='green', label='Testing Data')
         if predictions is not None:
-            ax.scatter(test_set['data'], predictions, s=4, color='red', label='Predictions')
+            ax.scatter(test_set['data'].cpu(), predictions.cpu(), s=4, color='red', label='Predictions')
+        ax.legend(prop=self.legendConfig['prop'])
+        plt.show(block=self.useBlocking)
+
+    def plot_learning(self, train_losses, test_losses=None):
+        fig, ax = plt.subplots(figsize=(10, 7))
+        if train_losses is not None:
+            ax.plot(train_losses, label='Training Loss', color='blue')
+        if test_losses is not None:
+            ax.plot(test_losses, label='Testing Loss', color='orange')
+        ax.set_title('Learning Curves')
+        ax.set_ylabel("Loss")
+        ax.set_xlabel("Epochs")
         ax.legend(prop=self.legendConfig['prop'])
         plt.show(block=self.useBlocking)
 
     def block(self):
         self.useBlocking = True
 
     def unblock(self):
```

