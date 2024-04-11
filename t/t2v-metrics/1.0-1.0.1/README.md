# Comparing `tmp/t2v_metrics-1.0.tar.gz` & `tmp/t2v_metrics-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2v_metrics-1.0.tar", last modified: Mon Apr  1 06:38:58 2024, max compression
+gzip compressed data, was "t2v_metrics-1.0.1.tar", last modified: Thu Apr 11 17:24:53 2024, max compression
```

## Comparing `t2v_metrics-1.0.tar` & `t2v_metrics-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-01 06:38:58.695626 t2v_metrics-1.0/
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)    11357 2023-12-16 12:48:47.000000 t2v_metrics-1.0/LICENSE
--rw-r--r--   0 zhiqiul  (21658) zhiqiul  (21658)     8893 2024-04-01 06:38:58.694626 t2v_metrics-1.0/PKG-INFO
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     7733 2024-04-01 06:38:26.000000 t2v_metrics-1.0/README.md
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     1136 2024-04-01 06:38:46.000000 t2v_metrics-1.0/pyproject.toml
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)       38 2024-04-01 06:38:58.695626 t2v_metrics-1.0/setup.cfg
-drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-01 06:38:58.664626 t2v_metrics-1.0/t2v_metrics/
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      912 2023-12-17 05:53:23.000000 t2v_metrics-1.0/t2v_metrics/__init__.py
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      599 2023-12-16 12:25:05.000000 t2v_metrics-1.0/t2v_metrics/clipscore.py
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      389 2023-12-18 23:55:45.000000 t2v_metrics-1.0/t2v_metrics/constants.py
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      587 2023-12-17 05:21:40.000000 t2v_metrics-1.0/t2v_metrics/itmscore.py
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     3289 2023-12-16 19:25:56.000000 t2v_metrics-1.0/t2v_metrics/score.py
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      593 2023-12-16 12:25:14.000000 t2v_metrics-1.0/t2v_metrics/vqascore.py
-drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-01 06:38:58.693626 t2v_metrics-1.0/t2v_metrics.egg-info/
--rw-r--r--   0 zhiqiul  (21658) zhiqiul  (21658)     8893 2024-04-01 06:38:58.000000 t2v_metrics-1.0/t2v_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      349 2024-04-01 06:38:58.000000 t2v_metrics-1.0/t2v_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)        1 2024-04-01 06:38:58.000000 t2v_metrics-1.0/t2v_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      363 2024-04-01 06:38:58.000000 t2v_metrics-1.0/t2v_metrics.egg-info/requires.txt
--rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)       12 2024-04-01 06:38:58.000000 t2v_metrics-1.0/t2v_metrics.egg-info/top_level.txt
+drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-11 17:24:53.955543 t2v_metrics-1.0.1/
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)    11357 2023-12-16 12:48:47.000000 t2v_metrics-1.0.1/LICENSE
+-rw-r--r--   0 zhiqiul  (21658) zhiqiul  (21658)     9202 2024-04-11 17:24:53.954543 t2v_metrics-1.0.1/PKG-INFO
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     8040 2024-04-09 14:04:22.000000 t2v_metrics-1.0.1/README.md
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     1160 2024-04-11 17:23:13.000000 t2v_metrics-1.0.1/pyproject.toml
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)       38 2024-04-11 17:24:53.955543 t2v_metrics-1.0.1/setup.cfg
+drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-11 17:24:53.933543 t2v_metrics-1.0.1/t2v_metrics/
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      912 2023-12-17 05:53:23.000000 t2v_metrics-1.0.1/t2v_metrics/__init__.py
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      599 2023-12-16 12:25:05.000000 t2v_metrics-1.0.1/t2v_metrics/clipscore.py
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      389 2023-12-18 23:55:45.000000 t2v_metrics-1.0.1/t2v_metrics/constants.py
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      587 2023-12-17 05:21:40.000000 t2v_metrics-1.0.1/t2v_metrics/itmscore.py
+drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-11 17:24:53.942543 t2v_metrics-1.0.1/t2v_metrics/models/
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)        0 2023-12-16 05:55:31.000000 t2v_metrics-1.0.1/t2v_metrics/models/__init__.py
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     1395 2023-12-16 11:45:21.000000 t2v_metrics-1.0.1/t2v_metrics/models/model.py
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)     3289 2023-12-16 19:25:56.000000 t2v_metrics-1.0.1/t2v_metrics/score.py
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      593 2023-12-16 12:25:14.000000 t2v_metrics-1.0.1/t2v_metrics/vqascore.py
+drwxrwxr-x   0 zhiqiul  (21658) zhiqiul  (21658)        0 2024-04-11 17:24:53.953543 t2v_metrics-1.0.1/t2v_metrics.egg-info/
+-rw-r--r--   0 zhiqiul  (21658) zhiqiul  (21658)     9202 2024-04-11 17:24:53.000000 t2v_metrics-1.0.1/t2v_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      408 2024-04-11 17:24:53.000000 t2v_metrics-1.0.1/t2v_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)        1 2024-04-11 17:24:53.000000 t2v_metrics-1.0.1/t2v_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)      363 2024-04-11 17:24:53.000000 t2v_metrics-1.0.1/t2v_metrics.egg-info/requires.txt
+-rw-rw-r--   0 zhiqiul  (21658) zhiqiul  (21658)       12 2024-04-11 17:24:53.000000 t2v_metrics-1.0.1/t2v_metrics.egg-info/top_level.txt
```

### Comparing `t2v_metrics-1.0/LICENSE` & `t2v_metrics-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `t2v_metrics-1.0/PKG-INFO` & `t2v_metrics-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2v_metrics
-Version: 1.0
+Version: 1.0.1
 Summary: Evaluating Text-to-Visual Generation with Image-to-Text Generation.
 Author-email: Zhiqiu Lin <zl279@cornell.edu>
 Project-URL: Home, https://linzhiqiu.github.io/papers/vqascore
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -37,33 +37,34 @@
 ## **VQAScore: Evaluating Text-to-Visual Generation with Image-to-Text Generation [[Project Page]](https://linzhiqiu.github.io/papers/vqascore/)**  
 [Zhiqiu Lin](https://linzhiqiu.github.io/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), Baiqi Li, Jiayao Li, [Xide Xia](https://scholar.google.com/citations?user=FHLTntIAAAAJ&hl=en), [Graham Neubig](https://www.phontron.com/), [Pengchuan Zhang](https://scholar.google.com/citations?user=3VZ_E64AAAAJ&hl=en), [Deva Ramanan](https://www.cs.cmu.edu/~deva/). In [Arxiv](https://linzhiqiu.github.io/papers/vqascore/), 2024.
 
 VQAScore allows researchers to automatically evaluate text-to-image/video/3D models using one-line of Python code!
 
 <img src="images/example.png" width=600> 
 
-VQAScore significantly outperforms prior art (e.g., CLIPScore, TIFA, Davidsonian, VPEval, VIEScore)  on  compositional text prompts and is simpler than prior art relying on proprietary models such as GPT-4Vision. Check out the paper for more details!
+VQAScore significantly outperforms previous metrics such as CLIPScore and PickScore on compositional text prompts, and it is much simpler than prior art (e.g., ImageReward, HPSv2, TIFA, Davidsonian, VPEval, VIEScore) making use of human feedback or proprietary models like ChatGPT and GPT-4Vision. 
 
 ## Quick start
 
 Install the package via:
 ```bash
 git clone https://github.com/linzhiqiu/t2v_metrics
 cd t2v_metrics
 
 conda create -n t2v python=3.10 -y
 conda activate t2v
 conda install pip -y
 
 pip install torch torchvision torchaudio
 pip install git+https://github.com/openai/CLIP.git
-pip install -e .
+pip install -e . # local pip install
 ```
 
 <!-- (not yet implemented) Or simply run `pip install t2v_metrics`.  -->
+Or you can install via `pip install t2v-metrics`.
 
 Now, the following Python code is all you need to compute the VQAScore for image-text alignment (higher scores indicate greater similarity):
 
 ```python
 import t2v_metrics
 clip_flant5_score = t2v_metrics.VQAScore(model='clip-flant5-xxl') # our recommended scoring model
 
@@ -124,15 +125,15 @@
 t2v_metrics.list_all_itmscore_models()
 
 print("CLIPScore models:")
 t2v_metrics.list_all_clipscore_models()
 ```
 
 ### Customizing the question and answer template (for VQAScore)
-The question and answer slightly affect the final score. We provide a simple default template for each model. For example, CLIP-FlanT5 and LLaVA-1.5 use the following template, which can be found at [t2v_metrics/models/vqascore_models/clip_t5_model.py](t2v_metrics/models/vqascore_models/clip_t5_model.py):
+The question and answer slightly affect the final score, as shown in the Appendix of our paper. We provide a simple default template for each model and do not recommend changing it for the sake of reproducibility. However, we do want to point out that the question and answer can be easily modified. For example, CLIP-FlanT5 and LLaVA-1.5 use the following template, which can be found at [t2v_metrics/models/vqascore_models/clip_t5_model.py](t2v_metrics/models/vqascore_models/clip_t5_model.py):
 
 ```python
 # {} will be replaced by the caption
 default_question_template = 'Does this figure show "{}"? Please answer yes or no.'
 default_answer_template = 'Yes'
 ```
 
@@ -161,26 +162,25 @@
 python eval.py --model clip-flant5-xxl # for VQAScore
 python eval.py --model openai:ViT-L-14 # for CLIPScore
 
 # You can optionally specify question/answer template, for example:
 python eval.py --model clip-flant5-xxl --question "Is the figure showing '{}'?" --answer "Yes"
 ```
 
-### Implement New Scoring Metrics
+### Implementing your own scoring metric
 You can easily implement your own scoring metric. For example, if you have a VQA model that you believe is more effective, you can incorporate it into the directory at [t2v_metrics/models/vqascore_models](t2v_metrics/models/vqascore_models/). For guidance, please refer to our example implementations of [LLaVA-1.5](t2v_metrics/models/vqascore_models/llava_model.py) and [InstructBLIP](t2v_metrics/models/vqascore_models/instructblip_model.py) as starting points.
 
 ## Citation
 
 If you find this repository useful for your research, please use the following (TO UPDATE with ArXiv ID).
 
 ```
-@inproceedings{lin2024vqascore,
+@article{lin2024evaluating,
   title={Evaluating Text-to-Visual Generation with Image-to-Text Generation},
-  author={Lin, Zhiqiu and Pathak, Deepak and Li, Baiqi and Li, Jiayao and Xia, Xide and Neubig, Graham, and Zhang, Pengchuan and Ramanan, Deva},
-  eprint={????.?????},
-  archivePrefix={arXiv},
+  author={Lin, Zhiqiu and Pathak, Deepak and Li, Baiqi and Li, Jiayao and Xia, Xide and Neubig, Graham and Zhang, Pengchuan and Ramanan, Deva},
+  journal={arXiv preprint arXiv:2404.01291},
   year={2024}
 }
 ```
 
 ## Acknowledgements
 This repository is inspired from the [Perceptual Metric (LPIPS)](https://github.com/richzhang/PerceptualSimilarity) repository by Richard Zhang for automatic evaluation of image quality.
```

### Comparing `t2v_metrics-1.0/README.md` & `t2v_metrics-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 ## **VQAScore: Evaluating Text-to-Visual Generation with Image-to-Text Generation [[Project Page]](https://linzhiqiu.github.io/papers/vqascore/)**  
 [Zhiqiu Lin](https://linzhiqiu.github.io/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), Baiqi Li, Jiayao Li, [Xide Xia](https://scholar.google.com/citations?user=FHLTntIAAAAJ&hl=en), [Graham Neubig](https://www.phontron.com/), [Pengchuan Zhang](https://scholar.google.com/citations?user=3VZ_E64AAAAJ&hl=en), [Deva Ramanan](https://www.cs.cmu.edu/~deva/). In [Arxiv](https://linzhiqiu.github.io/papers/vqascore/), 2024.
 
 VQAScore allows researchers to automatically evaluate text-to-image/video/3D models using one-line of Python code!
 
 <img src="images/example.png" width=600> 
 
-VQAScore significantly outperforms prior art (e.g., CLIPScore, TIFA, Davidsonian, VPEval, VIEScore)  on  compositional text prompts and is simpler than prior art relying on proprietary models such as GPT-4Vision. Check out the paper for more details!
+VQAScore significantly outperforms previous metrics such as CLIPScore and PickScore on compositional text prompts, and it is much simpler than prior art (e.g., ImageReward, HPSv2, TIFA, Davidsonian, VPEval, VIEScore) making use of human feedback or proprietary models like ChatGPT and GPT-4Vision. 
 
 ## Quick start
 
 Install the package via:
 ```bash
 git clone https://github.com/linzhiqiu/t2v_metrics
 cd t2v_metrics
 
 conda create -n t2v python=3.10 -y
 conda activate t2v
 conda install pip -y
 
 pip install torch torchvision torchaudio
 pip install git+https://github.com/openai/CLIP.git
-pip install -e .
+pip install -e . # local pip install
 ```
 
 <!-- (not yet implemented) Or simply run `pip install t2v_metrics`.  -->
+Or you can install via `pip install t2v-metrics`.
 
 Now, the following Python code is all you need to compute the VQAScore for image-text alignment (higher scores indicate greater similarity):
 
 ```python
 import t2v_metrics
 clip_flant5_score = t2v_metrics.VQAScore(model='clip-flant5-xxl') # our recommended scoring model
 
@@ -88,15 +89,15 @@
 t2v_metrics.list_all_itmscore_models()
 
 print("CLIPScore models:")
 t2v_metrics.list_all_clipscore_models()
 ```
 
 ### Customizing the question and answer template (for VQAScore)
-The question and answer slightly affect the final score. We provide a simple default template for each model. For example, CLIP-FlanT5 and LLaVA-1.5 use the following template, which can be found at [t2v_metrics/models/vqascore_models/clip_t5_model.py](t2v_metrics/models/vqascore_models/clip_t5_model.py):
+The question and answer slightly affect the final score, as shown in the Appendix of our paper. We provide a simple default template for each model and do not recommend changing it for the sake of reproducibility. However, we do want to point out that the question and answer can be easily modified. For example, CLIP-FlanT5 and LLaVA-1.5 use the following template, which can be found at [t2v_metrics/models/vqascore_models/clip_t5_model.py](t2v_metrics/models/vqascore_models/clip_t5_model.py):
 
 ```python
 # {} will be replaced by the caption
 default_question_template = 'Does this figure show "{}"? Please answer yes or no.'
 default_answer_template = 'Yes'
 ```
 
@@ -125,26 +126,25 @@
 python eval.py --model clip-flant5-xxl # for VQAScore
 python eval.py --model openai:ViT-L-14 # for CLIPScore
 
 # You can optionally specify question/answer template, for example:
 python eval.py --model clip-flant5-xxl --question "Is the figure showing '{}'?" --answer "Yes"
 ```
 
-### Implement New Scoring Metrics
+### Implementing your own scoring metric
 You can easily implement your own scoring metric. For example, if you have a VQA model that you believe is more effective, you can incorporate it into the directory at [t2v_metrics/models/vqascore_models](t2v_metrics/models/vqascore_models/). For guidance, please refer to our example implementations of [LLaVA-1.5](t2v_metrics/models/vqascore_models/llava_model.py) and [InstructBLIP](t2v_metrics/models/vqascore_models/instructblip_model.py) as starting points.
 
 ## Citation
 
 If you find this repository useful for your research, please use the following (TO UPDATE with ArXiv ID).
 
 ```
-@inproceedings{lin2024vqascore,
+@article{lin2024evaluating,
   title={Evaluating Text-to-Visual Generation with Image-to-Text Generation},
-  author={Lin, Zhiqiu and Pathak, Deepak and Li, Baiqi and Li, Jiayao and Xia, Xide and Neubig, Graham, and Zhang, Pengchuan and Ramanan, Deva},
-  eprint={????.?????},
-  archivePrefix={arXiv},
+  author={Lin, Zhiqiu and Pathak, Deepak and Li, Baiqi and Li, Jiayao and Xia, Xide and Neubig, Graham and Zhang, Pengchuan and Ramanan, Deva},
+  journal={arXiv preprint arXiv:2404.01291},
   year={2024}
 }
 ```
 
 ## Acknowledgements
 This repository is inspired from the [Perceptual Metric (LPIPS)](https://github.com/richzhang/PerceptualSimilarity) repository by Richard Zhang for automatic evaluation of image quality.
```

### Comparing `t2v_metrics-1.0/pyproject.toml` & `t2v_metrics-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "t2v_metrics"
-version = "1.0"
+version = "1.0.1"
 description = "Evaluating Text-to-Visual Generation with Image-to-Text Generation."
 authors = [
     {name="Zhiqiu Lin", email="zl279@cornell.edu"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -40,11 +40,11 @@
     "pycocoevalcap",
     "image-reward",
     "hpsv2",
     "fire==0.4.0",
 ]
 
 [tool.setuptools]
-packages = ["t2v_metrics"]
+packages = ["t2v_metrics", "t2v_metrics.models"]
 
 [project.urls]
 Home = "https://linzhiqiu.github.io/papers/vqascore"
```

### Comparing `t2v_metrics-1.0/t2v_metrics/__init__.py` & `t2v_metrics-1.0.1/t2v_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `t2v_metrics-1.0/t2v_metrics/clipscore.py` & `t2v_metrics-1.0.1/t2v_metrics/clipscore.py`

 * *Files identical despite different names*

### Comparing `t2v_metrics-1.0/t2v_metrics/itmscore.py` & `t2v_metrics-1.0.1/t2v_metrics/itmscore.py`

 * *Files identical despite different names*

### Comparing `t2v_metrics-1.0/t2v_metrics/score.py` & `t2v_metrics-1.0.1/t2v_metrics/score.py`

 * *Files identical despite different names*

### Comparing `t2v_metrics-1.0/t2v_metrics/vqascore.py` & `t2v_metrics-1.0.1/t2v_metrics/vqascore.py`

 * *Files identical despite different names*

### Comparing `t2v_metrics-1.0/t2v_metrics.egg-info/PKG-INFO` & `t2v_metrics-1.0.1/t2v_metrics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2v_metrics
-Version: 1.0
+Version: 1.0.1
 Summary: Evaluating Text-to-Visual Generation with Image-to-Text Generation.
 Author-email: Zhiqiu Lin <zl279@cornell.edu>
 Project-URL: Home, https://linzhiqiu.github.io/papers/vqascore
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -37,33 +37,34 @@
 ## **VQAScore: Evaluating Text-to-Visual Generation with Image-to-Text Generation [[Project Page]](https://linzhiqiu.github.io/papers/vqascore/)**  
 [Zhiqiu Lin](https://linzhiqiu.github.io/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), Baiqi Li, Jiayao Li, [Xide Xia](https://scholar.google.com/citations?user=FHLTntIAAAAJ&hl=en), [Graham Neubig](https://www.phontron.com/), [Pengchuan Zhang](https://scholar.google.com/citations?user=3VZ_E64AAAAJ&hl=en), [Deva Ramanan](https://www.cs.cmu.edu/~deva/). In [Arxiv](https://linzhiqiu.github.io/papers/vqascore/), 2024.
 
 VQAScore allows researchers to automatically evaluate text-to-image/video/3D models using one-line of Python code!
 
 <img src="images/example.png" width=600> 
 
-VQAScore significantly outperforms prior art (e.g., CLIPScore, TIFA, Davidsonian, VPEval, VIEScore)  on  compositional text prompts and is simpler than prior art relying on proprietary models such as GPT-4Vision. Check out the paper for more details!
+VQAScore significantly outperforms previous metrics such as CLIPScore and PickScore on compositional text prompts, and it is much simpler than prior art (e.g., ImageReward, HPSv2, TIFA, Davidsonian, VPEval, VIEScore) making use of human feedback or proprietary models like ChatGPT and GPT-4Vision. 
 
 ## Quick start
 
 Install the package via:
 ```bash
 git clone https://github.com/linzhiqiu/t2v_metrics
 cd t2v_metrics
 
 conda create -n t2v python=3.10 -y
 conda activate t2v
 conda install pip -y
 
 pip install torch torchvision torchaudio
 pip install git+https://github.com/openai/CLIP.git
-pip install -e .
+pip install -e . # local pip install
 ```
 
 <!-- (not yet implemented) Or simply run `pip install t2v_metrics`.  -->
+Or you can install via `pip install t2v-metrics`.
 
 Now, the following Python code is all you need to compute the VQAScore for image-text alignment (higher scores indicate greater similarity):
 
 ```python
 import t2v_metrics
 clip_flant5_score = t2v_metrics.VQAScore(model='clip-flant5-xxl') # our recommended scoring model
 
@@ -124,15 +125,15 @@
 t2v_metrics.list_all_itmscore_models()
 
 print("CLIPScore models:")
 t2v_metrics.list_all_clipscore_models()
 ```
 
 ### Customizing the question and answer template (for VQAScore)
-The question and answer slightly affect the final score. We provide a simple default template for each model. For example, CLIP-FlanT5 and LLaVA-1.5 use the following template, which can be found at [t2v_metrics/models/vqascore_models/clip_t5_model.py](t2v_metrics/models/vqascore_models/clip_t5_model.py):
+The question and answer slightly affect the final score, as shown in the Appendix of our paper. We provide a simple default template for each model and do not recommend changing it for the sake of reproducibility. However, we do want to point out that the question and answer can be easily modified. For example, CLIP-FlanT5 and LLaVA-1.5 use the following template, which can be found at [t2v_metrics/models/vqascore_models/clip_t5_model.py](t2v_metrics/models/vqascore_models/clip_t5_model.py):
 
 ```python
 # {} will be replaced by the caption
 default_question_template = 'Does this figure show "{}"? Please answer yes or no.'
 default_answer_template = 'Yes'
 ```
 
@@ -161,26 +162,25 @@
 python eval.py --model clip-flant5-xxl # for VQAScore
 python eval.py --model openai:ViT-L-14 # for CLIPScore
 
 # You can optionally specify question/answer template, for example:
 python eval.py --model clip-flant5-xxl --question "Is the figure showing '{}'?" --answer "Yes"
 ```
 
-### Implement New Scoring Metrics
+### Implementing your own scoring metric
 You can easily implement your own scoring metric. For example, if you have a VQA model that you believe is more effective, you can incorporate it into the directory at [t2v_metrics/models/vqascore_models](t2v_metrics/models/vqascore_models/). For guidance, please refer to our example implementations of [LLaVA-1.5](t2v_metrics/models/vqascore_models/llava_model.py) and [InstructBLIP](t2v_metrics/models/vqascore_models/instructblip_model.py) as starting points.
 
 ## Citation
 
 If you find this repository useful for your research, please use the following (TO UPDATE with ArXiv ID).
 
 ```
-@inproceedings{lin2024vqascore,
+@article{lin2024evaluating,
   title={Evaluating Text-to-Visual Generation with Image-to-Text Generation},
-  author={Lin, Zhiqiu and Pathak, Deepak and Li, Baiqi and Li, Jiayao and Xia, Xide and Neubig, Graham, and Zhang, Pengchuan and Ramanan, Deva},
-  eprint={????.?????},
-  archivePrefix={arXiv},
+  author={Lin, Zhiqiu and Pathak, Deepak and Li, Baiqi and Li, Jiayao and Xia, Xide and Neubig, Graham and Zhang, Pengchuan and Ramanan, Deva},
+  journal={arXiv preprint arXiv:2404.01291},
   year={2024}
 }
 ```
 
 ## Acknowledgements
 This repository is inspired from the [Perceptual Metric (LPIPS)](https://github.com/richzhang/PerceptualSimilarity) repository by Richard Zhang for automatic evaluation of image quality.
```

