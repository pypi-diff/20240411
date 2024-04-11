# Comparing `tmp/sharemyai_utils-0.1.7.tar.gz` & `tmp/sharemyai_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharemyai_utils-0.1.7.tar", last modified: Sat Mar 30 19:22:08 2024, max compression
+gzip compressed data, was "sharemyai_utils-0.1.8.tar", last modified: Thu Apr 11 00:08:11 2024, max compression
```

## Comparing `sharemyai_utils-0.1.7.tar` & `sharemyai_utils-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:08.986938 sharemyai_utils-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-30 19:22:08.986938 sharemyai_utils-0.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:08.982938 sharemyai_utils-0.1.7/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/cli/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:22:08.986938 sharemyai_utils-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:08.982938 sharemyai_utils-0.1.7/sharemyai_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:08.982938 sharemyai_utils-0.1.7/sharemyai_pluginsv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_pluginsv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:08.982938 sharemyai_utils-0.1.7/sharemyai_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_utils/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-03-30 19:22:04.000000 sharemyai_utils-0.1.7/sharemyai_utils/videos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:22:08.986938 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-30 19:22:08.000000 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-30 19:22:08.000000 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 19:22:08.000000 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:22:08.000000 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-30 19:22:08.000000 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 19:22:08.000000 sharemyai_utils-0.1.7/sharemyai_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:08:11.638907 sharemyai_utils-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-11 00:08:11.638907 sharemyai_utils-0.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:08:11.634907 sharemyai_utils-0.1.8/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/cli/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:08:11.638907 sharemyai_utils-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:08:11.634907 sharemyai_utils-0.1.8/sharemyai_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:08:11.634907 sharemyai_utils-0.1.8/sharemyai_pluginsv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_pluginsv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:08:11.638907 sharemyai_utils-0.1.8/sharemyai_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_utils/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-11 00:07:58.000000 sharemyai_utils-0.1.8/sharemyai_utils/videos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:08:11.638907 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-11 00:08:11.000000 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 00:08:11.000000 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:08:11.000000 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:08:11.000000 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 00:08:11.000000 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 00:08:11.000000 sharemyai_utils-0.1.8/sharemyai_utils.egg-info/top_level.txt
```

### Comparing `sharemyai_utils-0.1.7/PKG-INFO` & `sharemyai_utils-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharemyai_utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reusable utils for sharemyai plugins
 Home-page: http://github.com/catswithkeyboards
 Author: Cats with Keyboards
 Author-email: tech@catswithkeyboards.com
 Keywords: sharemyai utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `sharemyai_utils-0.1.7/cli/cli.py` & `sharemyai_utils-0.1.8/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/cli/fingerprint.py` & `sharemyai_utils-0.1.8/cli/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/cli/lib.py` & `sharemyai_utils-0.1.8/cli/lib.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/setup.py` & `sharemyai_utils-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/sharemyai_utils/defaults.py` & `sharemyai_utils-0.1.8/sharemyai_utils/defaults.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/sharemyai_utils/images.py` & `sharemyai_utils-0.1.8/sharemyai_utils/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
                     "prompt": params.get('prompt'),
                     "negative_prompt": params.get('negative_prompt'),
                     "num_images_per_prompt": params.get('batch_size', 1),
                     "num_inference_steps": params.get('inference_steps', 40),
                     "guidance_scale": params.get('guidance_scale', 5.0),
                     "height": params.get('height', 512),
                     "width": params.get('width', 512),
+                    "eta": params.get('eta', 0.3),
                     "callback_on_step_end": callback
                 }
                 if image is not None:
                     generation_args.update({"image": image, "strength": params.get('strength', 1.0)})
                 result = forward_pass(pipe, **generation_args) if forward_pass else pipe(**generation_args)
             except Exception as e:
                 ws.send(json.dumps({'error': str(e)}))
```

### Comparing `sharemyai_utils-0.1.7/sharemyai_utils/utils.py` & `sharemyai_utils-0.1.8/sharemyai_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/sharemyai_utils/videos.py` & `sharemyai_utils-0.1.8/sharemyai_utils/videos.py`

 * *Files identical despite different names*

### Comparing `sharemyai_utils-0.1.7/sharemyai_utils.egg-info/PKG-INFO` & `sharemyai_utils-0.1.8/sharemyai_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharemyai_utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reusable utils for sharemyai plugins
 Home-page: http://github.com/catswithkeyboards
 Author: Cats with Keyboards
 Author-email: tech@catswithkeyboards.com
 Keywords: sharemyai utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```
