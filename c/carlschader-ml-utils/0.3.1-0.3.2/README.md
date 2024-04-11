# Comparing `tmp/carlschader_ml_utils-0.3.1.tar.gz` & `tmp/carlschader_ml_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carlschader_ml_utils-0.3.1.tar", last modified: Thu Mar 28 18:27:25 2024, max compression
+gzip compressed data, was "carlschader_ml_utils-0.3.2.tar", last modified: Thu Apr 11 16:22:26 2024, max compression
```

## Comparing `carlschader_ml_utils-0.3.1.tar` & `carlschader_ml_utils-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-28 18:27:25.535802 carlschader_ml_utils-0.3.1/
--rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-03-25 18:47:30.000000 carlschader_ml_utils-0.3.1/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-03-28 18:27:25.535802 carlschader_ml_utils-0.3.1/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 18:48:53.000000 carlschader_ml_utils-0.3.1/README.md
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-28 18:27:25.535802 carlschader_ml_utils-0.3.1/carlschader_ml_utils/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 20:37:15.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4621 2024-03-28 18:27:01.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils/image_utils.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-28 18:27:25.535802 carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-03-28 18:27:25.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      320 2024-03-28 18:27:25.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-03-28 18:27:25.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-03-28 18:27:25.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       26 2024-03-28 18:27:25.000000 carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      872 2024-03-28 18:27:11.000000 carlschader_ml_utils-0.3.1/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-03-28 18:27:25.535802 carlschader_ml_utils-0.3.1/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-11 16:22:26.709083 carlschader_ml_utils-0.3.2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-03-25 18:47:30.000000 carlschader_ml_utils-0.3.2/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-11 16:22:26.709083 carlschader_ml_utils-0.3.2/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 18:48:53.000000 carlschader_ml_utils-0.3.2/README.md
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-11 16:22:26.709083 carlschader_ml_utils-0.3.2/carlschader_ml_utils/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 20:37:15.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4657 2024-04-11 16:20:31.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils/image_utils.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1764 2024-04-02 16:02:55.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils/train.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-11 16:22:26.709083 carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-11 16:22:26.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      350 2024-04-11 16:22:26.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-11 16:22:26.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-11 16:22:26.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       26 2024-04-11 16:22:26.000000 carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      872 2024-04-11 16:20:31.000000 carlschader_ml_utils-0.3.2/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-11 16:22:26.709083 carlschader_ml_utils-0.3.2/setup.cfg
```

### Comparing `carlschader_ml_utils-0.3.1/LICENSE` & `carlschader_ml_utils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carlschader_ml_utils-0.3.1/PKG-INFO` & `carlschader_ml_utils-0.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carlschader_ml_utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of utilities for machine learning projects
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ml-utils
 Project-URL: Issues, https://github.com/carlschader/ml-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `carlschader_ml_utils-0.3.1/carlschader_ml_utils/image_utils.py` & `carlschader_ml_utils-0.3.2/carlschader_ml_utils/image_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         torchvision.transforms.Normalize(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
     ]),
     batch_size=32,
     averages_only=False,
     device=torch.device('cpu'),
     verbose=False,
     ):
-    dataset = ImageFolder(root=data_folder, transform=transform)
+    dataset = ImageFolder(root=data_folder, transform=transform, allow_empty=True)
     data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=False)
     
     shutil.rmtree(save_dir, ignore_errors=True)
     os.mkdir(save_dir)
 
     # get output shape of model by sampling a single image
     sample_image, _ = dataset[0]
@@ -87,15 +87,15 @@
 
 def find_image_folder_normalization(path, crop_size=224, batch_size=64, total_batches=None, device=torch.device('cpu'), verbose=False):
     transform = transforms.Compose([
         transforms.Resize((crop_size, crop_size)),
         transforms.ToTensor(),
     ])
 
-    dataset = datasets.ImageFolder(path, transform=transform)
+    dataset = datasets.ImageFolder(path, transform=transform, allow_empty=True)
     loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=False)
 
     means = torch.zeros(3).to(device)
     pixel_count = 0
     count = 0
 
     print('Calculating means...') if verbose else None
```

### Comparing `carlschader_ml_utils-0.3.1/carlschader_ml_utils.egg-info/PKG-INFO` & `carlschader_ml_utils-0.3.2/carlschader_ml_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carlschader_ml_utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of utilities for machine learning projects
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ml-utils
 Project-URL: Issues, https://github.com/carlschader/ml-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `carlschader_ml_utils-0.3.1/pyproject.toml` & `carlschader_ml_utils-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carlschader_ml_utils"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "A collection of utilities for machine learning projects"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

