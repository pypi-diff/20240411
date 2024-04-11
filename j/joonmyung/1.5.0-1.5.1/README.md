# Comparing `tmp/joonmyung-1.5.0.tar.gz` & `tmp/joonmyung-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joonmyung-1.5.0.tar", last modified: Thu Mar 14 00:36:14 2024, max compression
+gzip compressed data, was "joonmyung-1.5.1.tar", last modified: Thu Apr 11 01:23:18 2024, max compression
```

## Comparing `joonmyung-1.5.0.tar` & `joonmyung-1.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 joonmyung  (1023) joonmyung  (1024)        0 2024-03-14 00:36:14.852160 joonmyung-1.5.0/
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)        0 2023-02-22 17:22:56.000000 joonmyung-1.5.0/LICENSE.txt
--rw-r--r--   0 joonmyung  (1023) joonmyung  (1024)      228 2024-03-14 00:36:14.852160 joonmyung-1.5.0/PKG-INFO
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     2593 2024-02-13 01:56:11.000000 joonmyung-1.5.0/README.md
-drwxrwxr-x   0 joonmyung  (1023) joonmyung  (1024)        0 2024-03-14 00:36:14.848160 joonmyung-1.5.0/joonmyung/
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)       15 2023-02-22 17:22:56.000000 joonmyung-1.5.0/joonmyung/__init__.py
-drwxrwxr-x   0 joonmyung  (1023) joonmyung  (1024)        0 2024-03-14 00:36:14.852160 joonmyung-1.5.0/joonmyung/analysis/
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)      110 2024-02-13 02:56:10.000000 joonmyung-1.5.0/joonmyung/analysis/__init__.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)    11068 2024-02-26 05:23:57.000000 joonmyung-1.5.0/joonmyung/analysis/analysis.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     4726 2024-03-12 06:22:26.000000 joonmyung-1.5.0/joonmyung/analysis/dataset.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)        0 2023-03-01 06:34:05.000000 joonmyung-1.5.0/joonmyung/analysis/hook.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     1217 2023-06-06 06:13:54.000000 joonmyung-1.5.0/joonmyung/analysis/metric.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     1190 2024-02-21 12:53:24.000000 joonmyung-1.5.0/joonmyung/analysis/model.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)      424 2023-06-06 06:36:54.000000 joonmyung-1.5.0/joonmyung/analysis/utils.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     6700 2023-04-03 12:26:27.000000 joonmyung-1.5.0/joonmyung/app.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     1390 2024-02-22 11:08:06.000000 joonmyung-1.5.0/joonmyung/data.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)    14161 2024-02-23 01:44:55.000000 joonmyung-1.5.0/joonmyung/draw.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)       29 2023-04-03 12:26:27.000000 joonmyung-1.5.0/joonmyung/dummy.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     2768 2023-09-08 05:25:20.000000 joonmyung-1.5.0/joonmyung/file.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)      920 2023-02-22 17:22:56.000000 joonmyung-1.5.0/joonmyung/gradcam.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)    11606 2024-03-14 00:35:48.000000 joonmyung-1.5.0/joonmyung/log.py
-drwxrwxr-x   0 joonmyung  (1023) joonmyung  (1024)        0 2024-03-14 00:36:14.852160 joonmyung-1.5.0/joonmyung/meta_data/
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)       41 2023-03-01 06:51:46.000000 joonmyung-1.5.0/joonmyung/meta_data/__init__.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)    45491 2023-02-22 17:22:56.000000 joonmyung-1.5.0/joonmyung/meta_data/label.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     2365 2024-02-23 01:52:00.000000 joonmyung-1.5.0/joonmyung/meta_data/utils.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     4111 2024-03-04 11:43:22.000000 joonmyung-1.5.0/joonmyung/metric.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     3964 2024-02-05 02:36:34.000000 joonmyung-1.5.0/joonmyung/script.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     1487 2023-03-01 13:25:20.000000 joonmyung-1.5.0/joonmyung/status.py
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)     4081 2024-02-13 07:09:14.000000 joonmyung-1.5.0/joonmyung/utils.py
-drwxrwxr-x   0 joonmyung  (1023) joonmyung  (1024)        0 2024-03-14 00:36:14.852160 joonmyung-1.5.0/joonmyung.egg-info/
--rw-r--r--   0 joonmyung  (1023) joonmyung  (1024)      228 2024-03-14 00:36:14.000000 joonmyung-1.5.0/joonmyung.egg-info/PKG-INFO
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)      717 2024-03-14 00:36:14.000000 joonmyung-1.5.0/joonmyung.egg-info/SOURCES.txt
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)        1 2024-03-14 00:36:14.000000 joonmyung-1.5.0/joonmyung.egg-info/dependency_links.txt
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)        1 2024-03-14 00:36:14.000000 joonmyung-1.5.0/joonmyung.egg-info/not-zip-safe
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)       10 2024-03-14 00:36:14.000000 joonmyung-1.5.0/joonmyung.egg-info/top_level.txt
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)       38 2024-03-14 00:36:14.852160 joonmyung-1.5.0/setup.cfg
--rw-rw-r--   0 joonmyung  (1023) joonmyung  (1024)      793 2024-03-14 00:35:59.000000 joonmyung-1.5.0/setup.py
+drwxr-sr-x   0 joonmyung  (1023) mlv       (1001)        0 2024-04-11 01:23:18.612927 joonmyung-1.5.1/
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)        0 2023-02-22 17:22:56.000000 joonmyung-1.5.1/LICENSE.txt
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)      228 2024-04-11 01:23:18.612927 joonmyung-1.5.1/PKG-INFO
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     2593 2024-02-13 01:56:11.000000 joonmyung-1.5.1/README.md
+drwxr-sr-x   0 joonmyung  (1023) mlv       (1001)        0 2024-04-11 01:23:18.612927 joonmyung-1.5.1/joonmyung/
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)       15 2023-02-22 17:22:56.000000 joonmyung-1.5.1/joonmyung/__init__.py
+drwxr-sr-x   0 joonmyung  (1023) mlv       (1001)        0 2024-04-11 01:23:18.612927 joonmyung-1.5.1/joonmyung/analysis/
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)      110 2024-02-13 02:56:10.000000 joonmyung-1.5.1/joonmyung/analysis/__init__.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)    12056 2024-04-09 09:44:53.000000 joonmyung-1.5.1/joonmyung/analysis/analysis.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     4928 2024-04-09 09:30:56.000000 joonmyung-1.5.1/joonmyung/analysis/dataset.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)        0 2023-03-01 06:34:05.000000 joonmyung-1.5.1/joonmyung/analysis/hook.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     1217 2023-06-06 06:13:54.000000 joonmyung-1.5.1/joonmyung/analysis/metric.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     1190 2024-02-21 12:53:24.000000 joonmyung-1.5.1/joonmyung/analysis/model.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)      424 2023-06-06 06:36:54.000000 joonmyung-1.5.1/joonmyung/analysis/utils.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     6700 2023-04-03 12:26:27.000000 joonmyung-1.5.1/joonmyung/app.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     1390 2024-02-22 11:08:06.000000 joonmyung-1.5.1/joonmyung/data.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)    14305 2024-03-14 07:10:42.000000 joonmyung-1.5.1/joonmyung/draw.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)       29 2023-04-03 12:26:27.000000 joonmyung-1.5.1/joonmyung/dummy.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     2768 2023-09-08 05:25:20.000000 joonmyung-1.5.1/joonmyung/file.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)      920 2023-02-22 17:22:56.000000 joonmyung-1.5.1/joonmyung/gradcam.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)    11606 2024-03-14 00:35:48.000000 joonmyung-1.5.1/joonmyung/log.py
+drwxr-sr-x   0 joonmyung  (1023) mlv       (1001)        0 2024-04-11 01:23:18.612927 joonmyung-1.5.1/joonmyung/meta_data/
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)       41 2023-03-01 06:51:46.000000 joonmyung-1.5.1/joonmyung/meta_data/__init__.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)    45491 2023-02-22 17:22:56.000000 joonmyung-1.5.1/joonmyung/meta_data/label.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     2441 2024-03-14 06:54:09.000000 joonmyung-1.5.1/joonmyung/meta_data/utils.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     4095 2024-03-05 03:16:49.000000 joonmyung-1.5.1/joonmyung/metric.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     3979 2024-04-11 01:12:21.000000 joonmyung-1.5.1/joonmyung/script.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     1487 2023-03-01 13:25:20.000000 joonmyung-1.5.1/joonmyung/status.py
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)     4081 2024-02-13 07:09:14.000000 joonmyung-1.5.1/joonmyung/utils.py
+drwxr-sr-x   0 joonmyung  (1023) mlv       (1001)        0 2024-04-11 01:23:18.612927 joonmyung-1.5.1/joonmyung.egg-info/
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)      228 2024-04-11 01:23:18.000000 joonmyung-1.5.1/joonmyung.egg-info/PKG-INFO
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)      717 2024-04-11 01:23:18.000000 joonmyung-1.5.1/joonmyung.egg-info/SOURCES.txt
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)        1 2024-04-11 01:23:18.000000 joonmyung-1.5.1/joonmyung.egg-info/dependency_links.txt
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)        1 2024-04-11 01:23:18.000000 joonmyung-1.5.1/joonmyung.egg-info/not-zip-safe
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)       10 2024-04-11 01:23:18.000000 joonmyung-1.5.1/joonmyung.egg-info/top_level.txt
+-rw-r--r--   0 joonmyung  (1023) mlv       (1001)       38 2024-04-11 01:23:18.612927 joonmyung-1.5.1/setup.cfg
+-rw-rwSr--   0 joonmyung  (1023) mlv       (1001)      794 2024-04-11 01:23:17.000000 joonmyung-1.5.1/setup.py
```

### Comparing `joonmyung-1.5.0/README.md` & `joonmyung-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/analysis/analysis.py` & `joonmyung-1.5.1/joonmyung/analysis/analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-os.environ["CUDA_VISIBLE_DEVICES"] = "4"
+os.environ["CUDA_VISIBLE_DEVICES"] = "1"
 from joonmyung.analysis.dataset import JDataset
 from joonmyung.analysis.model import JModel
 from joonmyung.draw import saliency, overlay, drawImgPlot, drawHeatmap, unNormalize
 from joonmyung.meta_data import data2path
 from joonmyung.data import getTransform
 from joonmyung.metric import targetPred
 from joonmyung.log import AverageMeter
@@ -156,90 +156,102 @@
                         , head_fusion=head_fusion, discard_ratios=discard_ratios, data_from=data_from
                         , ls_rollout=ls_rollout, ls_attentive=ls_attentive, reshape=reshape, device=device)
 
 
 if __name__ == '__main__':
     # Section A. Data
     dataset_name, device, amp_autocast, debug = "imagenet", 'cuda', torch.cuda.amp.autocast, True
-    data_path, _, _ = data2path(dataset_name)
-    data_num, batch_size, bs = [[0, 0], [1, 0], [2, 0], [3, 0], [0, 1], [1, 1], [2, 1], [3, 1]], 16, []
-    view, activate = [False, True, False, False, False], [True, False, False] #
-        # VIEW     : IMG, SALIENCY(M), SALIENCY(D), SALIENCY(S), ATTN. MOVEMENT
+    data_path, num_classes, _, _ = data2path(dataset_name)
+    view, activate = [False, True, False, False, False], [True, False, False]
+        # VIEW     : IMG, SALIENCY:ATTN, SALIENCY:OPENCV, SALIENCY:GRAD, ATTN. MOVEMENT
         # ACTIVATE : ATTN, QKV, HEAD
-    analysis = [2]
-        # [0] : INPUT TYPE, [0 : SAMPLE + POS, 1 : SAMPLE, 2 : POS]
-    if not debug:
-        dataset = JDataset(data_path, dataset_name, device=device)
-        samples, targets, imgs, label_names = dataset.getItems(data_num)
-        loader = dataset.getAllItems(batch_size)
-        num_classes = dataset.num_classes
-    else:
-        transform = getTransform(False, True)
-        img = PIL.Image.open('/hub_data1/joonmyung/data/imagenet/train/n01440764/n01440764_10026.JPEG')
-        samples, targets, label_names = transform(img)[None].to(device), torch.tensor([0]).to(device)[None].to(device), 'tench, Tinca tinca'
-        num_classes = 1000
+    analysis = [0] # [0] : INPUT TYPE, [0 : SAMPLE + POS, 1 : SAMPLE, 2 : POS]
+
+    dataset = JDataset(data_path, dataset_name, device=device)
+    data_idxs = [[c, i] for i in range(1000) for c in range(50)]
+    # data_idxs = [[21, 0], [22, 0], [2, 0], [0, 0], [0, 1], [1, 1], [2, 1], [3, 1]]
 
     # Section B. Model
-    model_number, model_name = 0, "deit_tiny_patch16_224" # deit_tiny_patch16_224, deit_small_patch16_224, deit_base_patch16_224
-    # model_number, model_name = 0, "vit_tiny_patch16_224" # vit_tiny_patch16_224,  vit_small_patch16_224,  vit_base_patch16_224
+    model_number, model_name = 0, "deit_tiny_patch16_224" # deit, vit | tiny, small, base
     # model_number, model_name = 1, "deit_tiny_patch16_224"
 
+    # Section C. Setting
+    ls_rollout, ls_attentive, col = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], 12
+
     modelMaker = JModel(num_classes, device=device)
     model = modelMaker.getModel(model_number, model_name)
     model = Analysis(model, analysis = analysis, activate = activate, device=device)
+    for idx, data_idx in enumerate(data_idxs):
+        print(f"------------------------- [{data_idx[0]}]/[{data_idx[1]}] -------------------------")
 
-
-    samples_ = samples[bs] if bs else samples
-    targets_ = targets[bs] if bs else targets
-    output = model(samples_)
-    if view[0]:
-        drawImgPlot(unNormalize(samples_, "imagenet"))
-
-    if view[1]: # SALIENCY W/ MODEL
-        ls_rollout, ls_attentive, col = [0,1,2,3,4,5,6,7,8,9,10,11], [0,1,2,3,4,5,6,7,8,9,10,11], 12
-        # discard_ratios, v_ratio, head_fusion, data_from = [0.0, 0.4, 0.8], 0.1, "mean", "cls"  # Attention, Gradient
-        discard_ratios, v_ratio, head_fusion, data_from = [0.0], 0.0, "mean", "patch"  # Attention, Gradient
-        rollout, attentive = model.anaSaliency(True, False, output, discard_ratios=discard_ratios,
-                                         ls_attentive = ls_attentive, ls_rollout=ls_rollout,
-                                         head_fusion  = head_fusion, index=targets_, data_from=data_from,
-                                         reshape      = True) # (12(L), 8(B), 14(H), 14(W))
-        print(1)
-        # datas_rollout = overlay(samples_, rollout,   dataset_name)
-        # drawImgPlot(datas_rollout, col=col)
-        # datas_attn    = overlay(samples_, attentive, dataset_name)
-        # drawImgPlot(datas_attn, col=col)
-
-    if view[2]:  # SALIENCY W/ DATA
-        img = np.array(imgs[0])
-
-        saliency = cv2.saliency.StaticSaliencySpectralResidual_create()
-        (success, saliencyMap) = saliency.computeSaliency(img)
-        saliencyMap = (saliencyMap * 255).astype("uint8")
-
-        saliency = cv2.saliency.StaticSaliencyFineGrained_create()
-        (success, saliencyFineMap) = saliency.computeSaliency(img)
-        threshMap = cv2.threshold((saliencyFineMap * 255).astype("uint8"), 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)[1]
-        # plt.imshow(threshMap)
-        # plt.show()
-
-    if view[3]:  # SALIENCY FOR INPUT
-        samples_.requires_grad, model.detach, k = True, False, 3
-        output = model(samples_)
-        attn = torch.stack(model.info["attn"]["f"], dim=1).mean(dim=[2,3])[0,-2]
-        topK = attn[1:].topk(k, -1, True)[1]
-        # a = torch.autograd.grad(attn.sum(), samples, retain_graph=True)[0].sum(dim=1)
-        a = torch.autograd.grad(output[:,3], samples_, retain_graph=True)[0].sum(dim=1)
-        b = F.interpolate(a.unsqueeze(0), scale_factor=0.05, mode='nearest')[0]
-        # drawHeatmap(b)
-        print(1)
-        # to_np(torch.stack([attn[:, :, 0], attn[:, :, 1:].sum(dim=-1)], -1)[0])
-
-    if view[4]: # ATTENTION MOVEMENT (FROM / TO)
-        attn = torch.stack(model.info["attn"]["f"]).mean(dim=2).transpose(0,1) # (8 (B), 12 (L), 197(T_Q), 197(T_K))
-        cls2cls     = attn[:, :, :1, 0].mean(dim=2)              # (8(B), 12(L))
-        patch2cls   = attn[:, :, :1, 1:].mean(dim=2).sum(dim=-1) # (8(B), 12(L))
-        to_np(torch.stack([cls2cls.mean(dim=0), patch2cls.mean(dim=0)]))
-
-        cls2patch   = attn[:, :, 1:, 0].mean(dim=2)
-        patch2patch = attn[:, :, 1:, 1:].mean(dim=2).sum(dim=-1)
-        to_np(torch.stack([cls2patch.mean(dim=0), patch2patch.mean(dim=0)]))
-        print(1)
+        sample, target, label_name = dataset[data_idx[0], data_idx[1]]
+        # sample, _, img, _ = dataset.getItemPath('/hub_data1/joonmyung/data/imagenet/train/n01440764/n01440764_39.JPEG')
+        output = model(sample)
+        if view[0]:
+            drawImgPlot(unNormalize(sample, "imagenet"))
+
+        if view[1]: # SALIENCY W/ MODEL
+            # ls_rollout, ls_attentive, col = [], [0,2,4,6,8,10], 6
+            # discard_ratios, v_ratio, head_fusion, data_from = [0.0, 0.4, 0.8], 0.1, "mean", "cls"
+            discard_ratios, v_ratio, head_fusion, data_from = [0.0], 0.0, "mean", "patch"  # Attention, Gradient
+            rollout, attentive = model.anaSaliency(True, False, output, discard_ratios=discard_ratios,
+                                                   ls_attentive = ls_attentive, ls_rollout=ls_rollout,
+                                                   head_fusion  = head_fusion, index=target, data_from=data_from,
+                                                   reshape      = True) # (12(L), 8(B), 14(H), 14(W))
+            datas_attn    = overlay(sample, attentive, dataset_name)
+            drawImgPlot(datas_attn, col=col)
+
+            discard_ratios, v_ratio, head_fusion, data_from = [0.0], 0.0, "mean", "cls"  # Attention, Gradient
+            rollout, attentive = model.anaSaliency(True, False, output, discard_ratios=discard_ratios,
+                                                   ls_attentive = ls_attentive, ls_rollout=ls_rollout,
+                                                   head_fusion  = head_fusion, index=target, data_from=data_from,
+                                                   reshape      = True) # (12(L), 8(B), 14(H), 14(W))
+            datas_attn = overlay(sample, attentive, dataset_name)
+            drawImgPlot(datas_attn, col=col)
+
+
+            # datas_rollout = overlay(sample, rollout,   dataset_name)
+            # drawImgPlot(datas_rollout, col=col)
+
+            # datas_attn = overlay(sample, attentive, dataset_name)
+            # drawImgPlot(datas_attn, col=col)
+
+            # a = attentive[5]
+            # b = torch.stack([a.clamp(max=a.quantile(1 - v_ratio)) for v_ratio in [0.0, 0.05, 0.1, 0.15, 0.2, 0.25, 0.3, 0.35, 0.4, 0.45, 0.5, 0.55]])
+            # datas_attn    = overlay(sample, b, dataset_name)
+            # drawImgPlot(datas_attn, col=col)
+            # print(1)
+
+        if view[2]:  # SALIENCY W/ DATA
+            img = np.array(dataset[data_idx[0], data_idx[1], 2][0])
+
+            saliency = cv2.saliency.StaticSaliencySpectralResidual_create()
+            (success, saliencyMap) = saliency.computeSaliency(img)
+            saliencyMap = (saliencyMap * 255).astype("uint8")
+
+            saliency = cv2.saliency.StaticSaliencyFineGrained_create()
+            (success, saliencyFineMap) = saliency.computeSaliency(img)
+            threshMap = cv2.threshold((saliencyFineMap * 255).astype("uint8"), 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)[1]
+            # plt.imshow(threshMap)
+            # plt.show()
+
+        if view[3]:  # SALIENCY FOR INPUT
+            sample.requires_grad, model.detach, k = True, False, 3
+            output = model(sample)
+            attn = torch.stack(model.info["attn"]["f"], dim=1).mean(dim=[2,3])[0,-2]
+            topK = attn[1:].topk(k, -1, True)[1]
+            # a = torch.autograd.grad(attn.sum(), samples, retain_graph=True)[0].sum(dim=1)
+            a = torch.autograd.grad(output[:,3], sample, retain_graph=True)[0].sum(dim=1)
+            b = F.interpolate(a.unsqueeze(0), scale_factor=0.05, mode='nearest')[0]
+            # drawHeatmap(b)
+            print(1)
+            # to_np(torch.stack([attn[:, :, 0], attn[:, :, 1:].sum(dim=-1)], -1)[0])
+
+        if view[4]: # ATTENTION MOVEMENT (FROM / TO)
+            attn = torch.stack(model.info["attn"]["f"]).mean(dim=2).transpose(0,1) # (8 (B), 12 (L), 197(T_Q), 197(T_K))
+            cls2cls     = attn[:, :, :1, 0].mean(dim=2)              # (8(B), 12(L))
+            patch2cls   = attn[:, :, :1, 1:].mean(dim=2).sum(dim=-1) # (8(B), 12(L))
+            # PATCH가 받는 정도
+            cls2patch   = attn[:, :, 1:, 0].mean(dim=2)
+            patch2patch = attn[:, :, 1:, 1:].mean(dim=2).sum(dim=-1)
+            # to_np(torch.stack([cls2cls.mean(dim=0), patch2cls.mean(dim=0), cls2patch.mean(dim=0), patch2patch.mean(dim=0)]))
+            print(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `joonmyung-1.5.0/joonmyung/analysis/metric.py` & `joonmyung-1.5.1/joonmyung/analysis/metric.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/analysis/model.py` & `joonmyung-1.5.1/joonmyung/analysis/model.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/app.py` & `joonmyung-1.5.1/joonmyung/app.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/data.py` & `joonmyung-1.5.1/joonmyung/data.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/draw.py` & `joonmyung-1.5.1/joonmyung/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,16 +208,18 @@
         rollouts = torch.stack(rollouts, dim=0)
         rollouts = rollouts[:, :, 1:]
 
         if reshape:
             rollouts = rollouts.reshape(-1, B, H, W) # L, B, H, W
 
     if ls_attentive:
+        # attentive = saliencys[ls_attentive, :, 0] \
+        #         if data_from == "cls" else saliencys[ls_attentive, :, 1:].mean(dim=2) # (L, B, T)
         attentive = saliencys[ls_attentive, :, 0] \
-                if data_from == "cls" else saliencys[ls_attentive, :, 1:].mean(dim=2) # (L, B, T)
+            if data_from == "cls" else saliencys[ls_attentive].mean(dim=2)  # (L, B, T)
         attentive = attentive[:, :, 1:]
         if reshape:
             attentive = attentive.reshape(-1, B, H, W)
 
     return rollouts, attentive
```

### Comparing `joonmyung-1.5.0/joonmyung/file.py` & `joonmyung-1.5.1/joonmyung/file.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/gradcam.py` & `joonmyung-1.5.1/joonmyung/gradcam.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/log.py` & `joonmyung-1.5.1/joonmyung/log.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/meta_data/label.py` & `joonmyung-1.5.1/joonmyung/meta_data/label.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/meta_data/utils.py` & `joonmyung-1.5.1/joonmyung/meta_data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,21 @@
         data_path  = f"/scratch/{getpass.getuser()}/data"
         output_dir = f"/scratch/{getpass.getuser()}/result"
     else:
         raise ValueError
 
     if dataset in ["imagenet", "IMNET"]:
         data_path = os.path.join(data_path, "imagenet") if "kakao" not in server else os.path.join(data_path, "imagenet-pytorch")
+        num_classes = 1000
+    else:
+        raise ValueError
+
     output_dir    = os.path.join(output_dir, conference, wandb_version, wandb_name)
 
-    return data_path, output_dir, server
+    return data_path, num_classes, output_dir, server
 
 def get_label(key, d_name ="imagenet"):
     d_name = d_name.lower()
     if d_name in ["imagenet", "IMNET"] :
         return imnet_label[key]
     elif d_name in ["cifar10", "cifar100"]:
         return cifar_label[key]
```

### Comparing `joonmyung-1.5.0/joonmyung/metric.py` & `joonmyung-1.5.1/joonmyung/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fvcore.nn import FlopCountAnalysis, flop_count_table, flop_count_str
+from fvcore.nn import FlopCountAnalysis, flop_count_table
 from torchprofile import profile_macs
 from typing import Tuple
 from thop import profile
 from tqdm import tqdm
 import torch
 import time
```

### Comparing `joonmyung-1.5.0/joonmyung/script.py` & `joonmyung-1.5.1/joonmyung/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from joonmyung.utils import time2str
 from tqdm import tqdm
 import subprocess
 import time
 import pynvml
+import datetime
 
 class GPU_Worker():
     def __init__(self, gpus:list, waitTimeInit = 30, waitTime = 60, count = 0,
                  checkType:int = 0, utilRatio:int = 50, need_gpu=1, max_run_num = 8, p = True):
         self.activate  = False
 
         self.gpus      = [int(gpu) for gpu in gpus]
@@ -65,15 +66,15 @@
         self.availGPUs = availGPUs
         if self.p: print("Activate GPUS : ", self.availGPUs)
 
     def getGPU(self):
         if len(self.availGPUs) < self.need_gpu: self.setGPU()
         gpus, self.availGPUs = self.availGPUs[:self.need_gpu], self.availGPUs[self.need_gpu:]
 
-        return ', '.join(map(str, gpus))
+        return ','.join(map(str, gpus))
 
 
     def check_process(self):
         endGPUs = []
         for gpu, process in self.runGPUs.items():
             if process.poll() is not None:
                 endGPUs.append(gpu)
```

### Comparing `joonmyung-1.5.0/joonmyung/status.py` & `joonmyung-1.5.1/joonmyung/status.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung/utils.py` & `joonmyung-1.5.1/joonmyung/utils.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/joonmyung.egg-info/SOURCES.txt` & `joonmyung-1.5.1/joonmyung.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joonmyung-1.5.0/setup.py` & `joonmyung-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import find_packages
 
 setuptools.setup(
     name="joonmyung",
-    version="1.5.0",
+    version="1.5.1",
     author="JoonMyung Choi",
     author_email="pizard@korea.ac.kr",
     description="JoonMyung's Library",
     url="https://github.com/pizard/JoonMyung.git",
     license="MIT",
     packages=find_packages(exclude=["playground",
                                     "playground.*",
@@ -23,7 +23,8 @@
 # git add .
 # git commit
 # git push
 # rm -rf ./*.egg-info ./dist/*
 
 # python setup.py sdist; python -m twine upload dist/*
 # ID:JoonmyungChoi
+
```

