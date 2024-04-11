# Comparing `tmp/bio-image-unet-0.6.1.tar.gz` & `tmp/bio_image_unet-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-image-unet-0.6.1.tar", max compression
+gzip compressed data, was "bio_image_unet-1.0.0a1.tar", max compression
```

## Comparing `bio-image-unet-0.6.1.tar` & `bio_image_unet-1.0.0a1.tar`

### file list

```diff
@@ -1,41 +1,39 @@
--rw-r--r--   0        0        0     1072 2022-06-27 10:34:59.772125 bio-image-unet-0.6.1/LICENSE
--rw-r--r--   0        0        0      659 2023-05-10 12:48:03.179904 bio-image-unet-0.6.1/README.md
--rw-r--r--   0        0        0     6148 2022-11-11 16:07:45.185829 bio-image-unet-0.6.1/biu/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-14 12:07:49.348357 bio-image-unet-0.6.1/biu/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 11:52:01.620433 bio-image-unet-0.6.1/biu/lstm_unet/__init__.py
--rw-r--r--   0        0        0     9931 2023-10-26 11:52:01.639505 bio-image-unet-0.6.1/biu/lstm_unet/models/lstm_pytorch.py
--rw-r--r--   0        0        0     8857 2023-10-26 11:52:01.634842 bio-image-unet-0.6.1/biu/lstm_unet/models/lstm_unet.py
--rw-r--r--   0        0        0       32 2022-06-27 10:34:59.772305 bio-image-unet-0.6.1/biu/progress/__init__.py
--rw-r--r--   0        0        0      196 2022-06-27 10:34:59.772393 bio-image-unet-0.6.1/biu/progress/note.txt
--rw-r--r--   0        0        0     5969 2022-11-10 16:09:23.098804 bio-image-unet-0.6.1/biu/progress/progressnotifier.py
--rw-r--r--   0        0        0     6148 2022-11-11 15:52:42.902284 bio-image-unet-0.6.1/biu/siam_unet/.DS_Store
--rw-r--r--   0        0        0      600 2022-06-27 14:38:00.834425 bio-image-unet-0.6.1/biu/siam_unet/__init__.py
--rw-r--r--   0        0        0    13709 2022-09-14 12:28:05.578919 bio-image-unet-0.6.1/biu/siam_unet/data.py
--rw-r--r--   0        0        0      156 2022-06-27 10:34:59.773322 bio-image-unet-0.6.1/biu/siam_unet/helpers/__cpu_count__.py
--rw-r--r--   0        0        0      656 2022-06-27 10:34:59.773399 bio-image-unet-0.6.1/biu/siam_unet/helpers/__md5sum__.py
--rw-r--r--   0        0        0     1318 2022-06-27 10:34:59.773503 bio-image-unet-0.6.1/biu/siam_unet/helpers/average_tifs.py
--rw-r--r--   0        0        0     1745 2022-06-27 10:34:59.773598 bio-image-unet-0.6.1/biu/siam_unet/helpers/create_pixel_value_histogram.py
--rw-r--r--   0        0        0      257 2022-06-27 10:34:59.773681 bio-image-unet-0.6.1/biu/siam_unet/helpers/cuda_test.py
--rw-r--r--   0        0        0     1397 2022-06-27 10:34:59.773959 bio-image-unet-0.6.1/biu/siam_unet/helpers/extract_frame_of_movie.py
--rw-r--r--   0        0        0     4669 2022-06-27 10:34:59.774141 bio-image-unet-0.6.1/biu/siam_unet/helpers/find_frame_of_image.py
--rw-r--r--   0        0        0      699 2022-06-27 10:34:59.774260 bio-image-unet-0.6.1/biu/siam_unet/helpers/generate_plain_image.py
--rw-r--r--   0        0        0     5044 2022-09-14 12:28:05.579071 bio-image-unet-0.6.1/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py
--rw-r--r--   0        0        0     1442 2022-06-27 10:34:59.774530 bio-image-unet-0.6.1/biu/siam_unet/helpers/low_mem_tif_utils.py
--rw-r--r--   0        0        0     1280 2022-06-27 10:34:59.774638 bio-image-unet-0.6.1/biu/siam_unet/helpers/threshold_images.py
--rw-r--r--   0        0        0     3196 2022-06-27 10:34:59.774817 bio-image-unet-0.6.1/biu/siam_unet/helpers/tif_to_mp4.py
--rw-r--r--   0        0        0     3914 2022-06-27 10:34:59.774949 bio-image-unet-0.6.1/biu/siam_unet/helpers/util.py
--rw-r--r--   0        0        0     3611 2022-09-14 12:28:05.579199 bio-image-unet-0.6.1/biu/siam_unet/losses.py
--rw-r--r--   0        0        0    11106 2023-05-10 12:48:03.180154 bio-image-unet-0.6.1/biu/siam_unet/predict.py
--rw-r--r--   0        0        0     5276 2022-09-14 12:28:05.579474 bio-image-unet-0.6.1/biu/siam_unet/siam_unet.py
--rw-r--r--   0        0        0     7967 2022-11-10 16:09:23.099636 bio-image-unet-0.6.1/biu/siam_unet/train.py
--rw-r--r--   0        0        0      340 2022-09-14 12:28:05.579720 bio-image-unet-0.6.1/biu/unet/__init__.py
--rw-r--r--   0        0        0     3456 2022-09-14 12:28:05.579805 bio-image-unet-0.6.1/biu/unet/baby_unet.py
--rw-r--r--   0        0        0    11482 2022-06-27 10:34:59.776449 bio-image-unet-0.6.1/biu/unet/data.py
--rw-r--r--   0        0        0     3068 2022-06-27 10:34:59.776569 bio-image-unet-0.6.1/biu/unet/losses.py
--rw-r--r--   0        0        0    11291 2023-05-10 12:48:03.180490 bio-image-unet-0.6.1/biu/unet/predict.py
--rw-r--r--   0        0        0     7705 2022-11-10 16:09:23.100108 bio-image-unet-0.6.1/biu/unet/train.py
--rw-r--r--   0        0        0     4039 2022-06-27 11:16:15.785010 bio-image-unet-0.6.1/biu/unet/unet.py
--rw-r--r--   0        0        0      859 2023-11-02 12:18:17.262996 bio-image-unet-0.6.1/biu/unet/utils.py
--rw-r--r--   0        0        0      681 2023-11-02 12:24:51.257895 bio-image-unet-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1648 2023-11-02 12:24:57.092654 bio-image-unet-0.6.1/setup.py
--rw-r--r--   0        0        0     1475 2023-11-02 12:24:57.092844 bio-image-unet-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-10 18:36:38.078294 bio_image_unet-1.0.0a1/biu/__init__.py
+-rw-r--r--   0        0        0       33 2021-09-27 08:49:49.234107 bio_image_unet-1.0.0a1/biu/progress/__init__.py
+-rw-r--r--   0        0        0      200 2021-09-28 08:12:49.748674 bio_image_unet-1.0.0a1/biu/progress/note.txt
+-rw-r--r--   0        0        0     6106 2023-04-20 07:59:32.418013 bio_image_unet-1.0.0a1/biu/progress/progressnotifier.py
+-rw-r--r--   0        0        0      627 2024-04-10 18:36:47.515504 bio_image_unet-1.0.0a1/biu/siam_unet/__init__.py
+-rw-r--r--   0        0        0    14029 2024-04-10 18:49:07.846468 bio_image_unet-1.0.0a1/biu/siam_unet/data.py
+-rw-r--r--   0        0        0      163 2021-09-27 08:49:49.247073 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/__cpu_count__.py
+-rw-r--r--   0        0        0      679 2024-04-11 09:40:15.397614 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/__md5sum__.py
+-rw-r--r--   0        0        0     1360 2021-09-27 08:49:49.250065 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/average_tifs.py
+-rw-r--r--   0        0        0     1790 2021-09-27 16:04:41.509245 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/create_pixel_value_histogram.py
+-rw-r--r--   0        0        0      269 2021-09-27 08:49:49.253057 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/cuda_test.py
+-rw-r--r--   0        0        0     1438 2021-09-27 08:49:49.256048 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/extract_frame_of_movie.py
+-rw-r--r--   0        0        0     4761 2021-09-27 08:49:49.257046 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/find_frame_of_image.py
+-rw-r--r--   0        0        0      717 2021-09-27 08:49:49.258043 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/generate_plain_image.py
+-rw-r--r--   0        0        0     5170 2022-06-09 07:58:44.702035 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py
+-rw-r--r--   0        0        0     1487 2021-09-27 08:49:49.261035 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/low_mem_tif_utils.py
+-rw-r--r--   0        0        0     1316 2021-09-27 08:49:49.262033 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/threshold_images.py
+-rw-r--r--   0        0        0     3269 2021-09-27 16:04:36.182184 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/tif_to_mp4.py
+-rw-r--r--   0        0        0     4017 2021-09-27 16:04:48.533471 bio_image_unet-1.0.0a1/biu/siam_unet/helpers/util.py
+-rw-r--r--   0        0        0     3726 2022-06-09 07:58:44.702035 bio_image_unet-1.0.0a1/biu/siam_unet/losses.py
+-rw-r--r--   0        0        0    11132 2024-04-10 19:13:07.466796 bio_image_unet-1.0.0a1/biu/siam_unet/predict.py
+-rw-r--r--   0        0        0     5676 2024-04-10 19:06:03.549330 bio_image_unet-1.0.0a1/biu/siam_unet/siam_unet.py
+-rw-r--r--   0        0        0     8016 2024-04-10 19:13:07.474060 bio_image_unet-1.0.0a1/biu/siam_unet/train.py
+-rw-r--r--   0        0        0      341 2024-04-10 18:37:10.871074 bio_image_unet-1.0.0a1/biu/unet/__init__.py
+-rw-r--r--   0        0        0     7344 2024-04-08 16:06:08.358464 bio_image_unet-1.0.0a1/biu/unet/attention_unet.py
+-rw-r--r--   0        0        0     3548 2022-06-09 07:58:44.710015 bio_image_unet-1.0.0a1/biu/unet/baby_unet.py
+-rw-r--r--   0        0        0    12367 2024-04-10 07:56:06.705772 bio_image_unet-1.0.0a1/biu/unet/data.py
+-rw-r--r--   0        0        0     2960 2024-04-10 08:17:56.464512 bio_image_unet-1.0.0a1/biu/unet/losses.py
+-rw-r--r--   0        0        0     9569 2024-04-10 18:45:02.920047 bio_image_unet-1.0.0a1/biu/unet/predict.py
+-rw-r--r--   0        0        0     9150 2024-04-10 18:45:02.913943 bio_image_unet-1.0.0a1/biu/unet/train.py
+-rw-r--r--   0        0        0     4401 2024-04-10 18:40:49.654375 bio_image_unet-1.0.0a1/biu/unet/unet.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:45:37.802148 bio_image_unet-1.0.0a1/biu/unet/utils.py
+-rw-r--r--   0        0        0       22 2024-04-10 19:46:28.006248 bio_image_unet-1.0.0a1/biu/utils/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-10 19:13:07.499413 bio_image_unet-1.0.0a1/biu/utils/test.py
+-rw-r--r--   0        0        0     2347 2024-04-10 19:55:09.496216 bio_image_unet-1.0.0a1/biu/utils/utils.py
+-rw-r--r--   0        0        0     1093 2021-09-27 08:49:49.231116 bio_image_unet-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0      630 2024-04-11 11:22:10.002961 bio_image_unet-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      679 2023-10-24 12:59:58.989010 bio_image_unet-1.0.0a1/README.md
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 bio_image_unet-1.0.0a1/PKG-INFO
```

### Comparing `bio-image-unet-0.6.1/LICENSE` & `bio_image_unet-1.0.0a1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Daniel Härtter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Daniel Härtter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `bio-image-unet-0.6.1/README.md` & `bio_image_unet-1.0.0a1/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Bio Image U-Net
-
-Implementations of U-Net and Siam U-Net for biological image segmentation
-
-### Authors
-[Daniel Härtter](daniel.haertter@duke.edu) (Duke University, University of Göttingen) \
-[Yuxi Long](longyuxi@live.com) (Duke University) \
-Andreas Primeßnig
-
-### Installation
-Install with ``pip install git+https://github.com/danihae/bio-image-unet``
-
-
-### Usage example
-[iPython Notebook for getting started with U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_unet.ipynb) \
-[iPython Notebook for getting started with Siam U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_siam_unet.ipynb)
-
-### Documentation
-
-TBD
+# Bio Image U-Net
+
+Implementations of U-Net and Siam U-Net for biological image segmentation
+
+### Authors
+[Daniel Härtter](daniel.haertter@duke.edu) (Duke University, University of Göttingen) \
+[Yuxi Long](longyuxi@live.com) (Duke University) \
+Andreas Primeßnig
+
+### Installation
+Install with ``pip install git+https://github.com/danihae/bio-image-unet``
+
+
+### Usage example
+[iPython Notebook for getting started with U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_unet.ipynb) \
+[iPython Notebook for getting started with Siam U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_siam_unet.ipynb)
+
+### Documentation
+
+TBD
```

### Comparing `bio-image-unet-0.6.1/biu/progress/progressnotifier.py` & `bio_image_unet-1.0.0a1/biu/progress/progressnotifier.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import math
-import time
-from tqdm import tqdm as tqdm
-
-"""
-Build a super dumb iterator wrapper which then returns a progress, this should be kinda splitted
-first we need an object which remains alive the whole time where the logic and the variables are set to know
-where the progress should be displayed (in our case we set in the gui, that we want the progress bar to be updated)
-
-The second part is the iterator which only needs to be alive during "work"
-
-thats how an iterator is made: https://treyhunner.com/2018/06/how-to-make-an-iterator-in-python/
-
-
-
-this should probably be in an extra package since tqdm is used in the unet_pytorch package and we should not create
-circular dependencies between the packages
-
-
-the persistent class could have a private class which is the iterator and a method for creating the iterator
-
-
-"""
-
-
-class ProgressNotifier:
-
-    def __init__(self):
-        self.__task_progress = None
-        self.__task_progress_details = None
-        self.__use_tqdm = False
-
-    @staticmethod
-    def progress_notifier_tqdm():
-        # should create a progress-notifier object prepared for using tqdm as output
-        notifier = ProgressNotifier()
-        notifier.__use_tqdm = True
-        return notifier
-
-    @staticmethod
-    def silent_notifier():
-        """
-        returns a progress notifier that is silent (no progress notifications)
-        used for the case a method requires a progress notifier but we do not want to show anything
-        """
-        return ProgressNotifier()
-
-    def iterator(self, iterateable):
-        # check if it is iterable
-        try:
-            iterator = iter(iterateable)
-            if self.__use_tqdm:
-                return tqdm(iterateable)
-            return self.__IteratorWrapper(iterateable, self.__task_progress, self.__task_progress_details)
-        except TypeError:
-            raise TypeError("object is not possible to iterate")
-
-    def set_progress_report(self, task):
-        # check if task meets the requirements
-        try:
-            task(0)
-            self.__task_progress = task
-        except:
-            raise Exception('The given variable is not a function with 1 numeric parameter (or similar constructs)')
-        # sets the task that should be called on progress change
-        # task should be a method or lambda that takes a number as input
-
-    def set_progress_detail(self, task):
-        # check if task meets the requirements
-        try:
-            task(0, 0, 0, 0, 0, 0)
-            self.__task_progress_details = task
-        except:
-            raise Exception('The given variable is not a function with 6 numeric parameters (or similar constructs)')
-
-        # sets the task that should be called on progress change
-        # it gives details about the progress (like tqdm does), ETA, iterations per second and so on
-        # this var doesn't have to be set
-
-    class __IteratorWrapper:
-        # this is a class variable (in java like static)
-        timeMultiplier = 1000  # time values in milli seconds
-
-        def __init__(self, iterable, task_progress, task_progress_details=None):
-            self.__total = None
-            self.__time = None  # time used until "now", now is the current "next" call
-            self.__eta = None  # calculated value of how long will it take
-
-            self.__iterable = iterable
-            self.__iterator = iter(iterable)
-            self.__task_progress = task_progress
-            self.__task_progress_details = task_progress_details
-            self.__time_start = int(round(time.time() * self.timeMultiplier))
-            self.__current = 0  # current count of iterations
-            # init total iterations number if possible
-            if iterable is not None:
-                try:
-                    self.__total = len(iterable)
-                except (TypeError, AttributeError):
-                    self.__total = None
-            if task_progress_details is not None:
-                task_progress_details(0, 0, 0, 0, 0, 0)
-
-        def __iter__(self):
-            return self
-
-        def __next__(self):
-            self.__current += 1
-            self.__time = int(round(time.time() * self.timeMultiplier))
-            # eta is an approximation time until now divided by current and multiplied by total,
-            # only if total is not None
-            if self.__total is not None:
-                self.__eta = ((self.__time - self.__time_start) / self.__current) * self.__total
-
-            # report progress and return next element
-            if self.__task_progress is not None:
-                if self.__total is not None:  # if total is not None the current progress is reported
-                    self.__task_progress(self.__current / self.__total)
-                else:  # otherwise the number of iterations is reported
-                    self.__task_progress(self.__current)
-
-            # todo: the progress_details should update in an extra thread each second and the duration should be a timer in there
-            # since there could be very slow iterations taking a while and with extra thread and duration as timer
-            # the user "notices" progress
-            if self.__task_progress_details is not None and self.__eta is not None:
-                hh_eta = math.floor(self.__eta / (self.timeMultiplier * 3600))
-                mm_eta = math.floor(self.__eta / (self.timeMultiplier * 60) - hh_eta * 60)
-                ss_eta = math.floor((self.__eta / self.timeMultiplier) - (hh_eta * 3600 + mm_eta * 60))
-
-                duration = (self.__time - self.__time_start) / self.timeMultiplier
-                hh_current = math.floor(duration / 3600)
-                mm_current = math.floor(duration / 60) - hh_current * 60
-                ss_current = math.floor(duration) - (hh_current * 3600 + mm_current * 60)
-
-                self.__task_progress_details(hh_current, mm_current, ss_current, hh_eta, mm_eta, ss_eta)
-
-            return self.__iterator.__next__()
+import math
+import time
+from tqdm import tqdm as tqdm
+
+"""
+Build a super dumb iterator wrapper which then returns a progress, this should be kinda splitted
+first we need an object which remains alive the whole time where the logic and the variables are set to know
+where the progress should be displayed (in our case we set in the gui, that we want the progress bar to be updated)
+
+The second part is the iterator which only needs to be alive during "work"
+
+thats how an iterator is made: https://treyhunner.com/2018/06/how-to-make-an-iterator-in-python/
+
+
+
+this should probably be in an extra package since tqdm is used in the unet_pytorch package and we should not create
+circular dependencies between the packages
+
+
+the persistent class could have a private class which is the iterator and a method for creating the iterator
+
+
+"""
+
+
+class ProgressNotifier:
+
+    def __init__(self):
+        self.__task_progress = None
+        self.__task_progress_details = None
+        self.__use_tqdm = False
+
+    @staticmethod
+    def progress_notifier_tqdm():
+        # should create a progress-notifier object prepared for using tqdm as output
+        notifier = ProgressNotifier()
+        notifier.__use_tqdm = True
+        return notifier
+
+    @staticmethod
+    def silent_notifier():
+        """
+        returns a progress notifier that is silent (no progress notifications)
+        used for the case a method requires a progress notifier but we do not want to show anything
+        """
+        return ProgressNotifier()
+
+    def iterator(self, iterateable):
+        # check if it is iterable
+        try:
+            iterator = iter(iterateable)
+            if self.__use_tqdm:
+                return tqdm(iterateable)
+            return self.__IteratorWrapper(iterateable, self.__task_progress, self.__task_progress_details)
+        except TypeError:
+            raise TypeError("object is not possible to iterate")
+
+    def set_progress_report(self, task):
+        # check if task meets the requirements
+        try:
+            task(0)
+            self.__task_progress = task
+        except:
+            raise Exception('The given variable is not a function with 1 numeric parameter (or similar constructs)')
+        # sets the task that should be called on progress change
+        # task should be a method or lambda that takes a number as input
+
+    def set_progress_detail(self, task):
+        # check if task meets the requirements
+        try:
+            task(0, 0, 0, 0, 0, 0)
+            self.__task_progress_details = task
+        except:
+            raise Exception('The given variable is not a function with 6 numeric parameters (or similar constructs)')
+
+        # sets the task that should be called on progress change
+        # it gives details about the progress (like tqdm does), ETA, iterations per second and so on
+        # this var doesn't have to be set
+
+    class __IteratorWrapper:
+        # this is a class variable (in java like static)
+        timeMultiplier = 1000  # time values in milli seconds
+
+        def __init__(self, iterable, task_progress, task_progress_details=None):
+            self.__total = None
+            self.__time = None  # time used until "now", now is the current "next" call
+            self.__eta = None  # calculated value of how long will it take
+
+            self.__iterable = iterable
+            self.__iterator = iter(iterable)
+            self.__task_progress = task_progress
+            self.__task_progress_details = task_progress_details
+            self.__time_start = int(round(time.time() * self.timeMultiplier))
+            self.__current = 0  # current count of iterations
+            # init total iterations number if possible
+            if iterable is not None:
+                try:
+                    self.__total = len(iterable)
+                except (TypeError, AttributeError):
+                    self.__total = None
+            if task_progress_details is not None:
+                task_progress_details(0, 0, 0, 0, 0, 0)
+
+        def __iter__(self):
+            return self
+
+        def __next__(self):
+            self.__current += 1
+            self.__time = int(round(time.time() * self.timeMultiplier))
+            # eta is an approximation time until now divided by current and multiplied by total,
+            # only if total is not None
+            if self.__total is not None:
+                self.__eta = ((self.__time - self.__time_start) / self.__current) * self.__total
+
+            # report progress and return next element
+            if self.__task_progress is not None:
+                if self.__total is not None:  # if total is not None the current progress is reported
+                    self.__task_progress(self.__current / self.__total)
+                else:  # otherwise the number of iterations is reported
+                    self.__task_progress(self.__current)
+
+            # todo: the progress_details should update in an extra thread each second and the duration should be a timer in there
+            # since there could be very slow iterations taking a while and with extra thread and duration as timer
+            # the user "notices" progress
+            if self.__task_progress_details is not None and self.__eta is not None:
+                hh_eta = math.floor(self.__eta / (self.timeMultiplier * 3600))
+                mm_eta = math.floor(self.__eta / (self.timeMultiplier * 60) - hh_eta * 60)
+                ss_eta = math.floor((self.__eta / self.timeMultiplier) - (hh_eta * 3600 + mm_eta * 60))
+
+                duration = (self.__time - self.__time_start) / self.timeMultiplier
+                hh_current = math.floor(duration / 3600)
+                mm_current = math.floor(duration / 60) - hh_current * 60
+                ss_current = math.floor(duration) - (hh_current * 3600 + mm_current * 60)
+
+                self.__task_progress_details(hh_current, mm_current, ss_current, hh_eta, mm_eta, ss_eta)
+
+            return self.__iterator.__next__()
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/__init__.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-try:
-    import torch
-except ImportError:
-    raise ImportError('Torch is not installed. Please install through https://pytorch.org/get-started/locally/')
-
-# check if torch version >= 1.9.0
-from packaging import version
-if not version.parse(torch.__version__) >= version.parse('1.9.0'):
-    raise ImportError(f'This package requires torch >=1.9.0 to run. You have version {torch.__version__}.Please install through https://pytorch.org/get-started/locally/')
-
-from .data import DataProcess
-from .losses import *
-from .predict import Predict
-from .siam_unet import Siam_UNet
-from .train import Trainer
+try:
+    import torch
+except ImportError:
+    raise ImportError('Torch is not installed. Please install through https://pytorch.org/get-started/locally/')
+
+# check if torch version >= 1.9.0
+from packaging import version
+
+if not version.parse(torch.__version__) >= version.parse('1.9.0'):
+    raise ImportError(
+        f'This package requires torch >=1.9.0 to run. You have version {torch.__version__}.Please install through https://pytorch.org/get-started/locally/')
+
+from .data import DataProcess
+from .losses import *
+from .predict import Predict
+from .siam_unet import Siam_UNet
+from .train import Trainer
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/data.py` & `bio_image_unet-1.0.0a1/biu/unet/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,290 +1,265 @@
-import glob
-import os
-import shutil
-
-import numpy as np
-import tifffile
-import torch
-from albumentations import (
-    ShiftScaleRotate, GaussNoise,
-    RandomBrightnessContrast, Compose, RandomRotate90)
-from skimage import morphology, transform
-from torch.utils.data import Dataset
-
-
-class DataProcess(Dataset):
-    def __init__(self, source_dir, dim_out=(256, 256), aug_factor=10, data_path='../data/', threshold_masks=50,
-                 dilate_mask=0, dilate_kernel='disk', val_split=0.2, invert_masks=False, skeletonize=False, create=True,
-                 clip_threshold=(0.2, 99.8), shiftscalerotate=(0, 0, 0), noise_amp=10, brightness_contrast=(0.25, 0.25),
-                 rescale=None):
-        """
-        Create training data object for network training
-
-        1) Create folder structure for training data
-        2) Move and preprocess training images
-        3) Split input images into tiles
-        4) Augment training data
-        5) Create object of PyTorch Dataset class for training
-
-        Parameters
-        ----------
-        source_dir : Tuple[str, str]
-            Path of training data [images, labels]. Images need to be tif files.
-        dim_out : Tuple[int, int]
-            Resize dimensions of images for training
-        aug_factor : int
-            Factor of image augmentation
-        data_path : str
-            Base path of directories for training data
-        threshold_masks : int
-            Threshold to binarize masks [0-255]
-        dilate_mask
-            Radius of binary erosion/dilation of masks [-2, -1, 0, 1, 2]
-        dilate_kernel : str
-            Dilation kernel ('disk' or 'square')
-        val_split : float
-            Validation split for training
-        invert_masks : bool
-            If True, greyscale binary labels is inverted
-        skeletonize : bool
-            If True, binary labels are skeletonized
-        create : bool, optional
-            If False, existing data set in data_path is used
-        clip_threshold : Tuple[float, float]
-            Clip thresholds for intensity normalization of images
-        shiftscalerotate : [float, float, float]
-            Shift, scale and rotate image during augmentation
-        noise_amp : float
-            Amplitude of Gaussian noise for image augmentation
-        brightness_contrast : Tuple[float, float]
-            Adapt brightness and contrast of images during augmentation
-        rescale : float, optional
-            Rescale all images and labels by factor rescale
-        """
-        self.source_dir = source_dir
-        self.create = create
-        self.data_path = data_path
-        self.dim_out = dim_out
-        self.threshold_masks = threshold_masks
-        self.skeletonize = skeletonize
-        self.invert_masks = invert_masks
-        self.clip_threshold = clip_threshold
-        self.aug_factor = aug_factor
-        self.shiftscalerotate = shiftscalerotate
-        self.brightness_contrast = brightness_contrast
-        self.noise_amp = noise_amp
-        self.rescale = rescale
-        self.dilate_mask = dilate_mask
-        self.dilate_kernel = dilate_kernel
-        self.val_split = val_split
-        self.mode = 'train'
-
-        self.__make_dirs()
-
-        if create:
-            self.__move_and_edit()
-            self.__merge_images()
-            self.__split()
-            if self.aug_factor is not None:
-                self.__augment()
-
-    def __make_dirs(self):
-        self.image_path = self.data_path + '/image/'
-        self.prev_image_path = self.data_path + '/prev_image/'
-        self.mask_path = self.data_path + '/mask/'
-        self.merge_path = self.data_path + '/merge/'
-        self.split_merge_path = self.data_path + '/split/merge/'
-        self.split_image_path = self.data_path + '/split/image/'
-        self.split_prev_image_path = self.data_path + '/split/prev_image/'
-        self.split_mask_path = self.data_path + '/split/mask/'
-        self.aug_image_path = self.data_path + '/augmentation/aug_image/'
-        self.aug_mask_path = self.data_path + '/augmentation/aug_mask/'
-        self.aug_prev_image_path = self.data_path + '/augmentation/aug_prev_image/'
-
-        # delete old files
-        if self.create:
-            try:
-                shutil.rmtree(self.data_path)
-            except:
-                pass
-        # make folders
-        os.makedirs(self.image_path, exist_ok=True)
-        os.makedirs(self.mask_path, exist_ok=True)
-        os.makedirs(self.merge_path, exist_ok=True)
-        os.makedirs(self.split_merge_path, exist_ok=True)
-        os.makedirs(self.split_image_path, exist_ok=True)
-        os.makedirs(self.split_mask_path, exist_ok=True)
-        os.makedirs(self.aug_image_path, exist_ok=True)
-        os.makedirs(self.aug_mask_path, exist_ok=True)
-        os.makedirs(self.aug_prev_image_path, exist_ok=True)
-        os.makedirs(self.prev_image_path, exist_ok=True)
-        os.makedirs(self.split_prev_image_path, exist_ok=True)
-
-    def __move_and_edit(self):
-        # create image data
-        files_image = glob.glob(self.source_dir[0] + '*')
-        for file_i in files_image:
-            img_i = tifffile.imread(file_i)
-            # clip and normalize (0,255)
-            img_i_nan = np.copy(img_i).astype('float32')
-            img_i_nan[img_i == 0] = np.nan
-            img_i = np.clip(img_i, a_min=np.nanpercentile(img_i_nan, self.clip_threshold[0]),
-                            a_max=np.percentile(img_i_nan, self.clip_threshold[1]))
-            img_i = img_i - np.min(img_i)
-            img_i = img_i / np.max(img_i) * 255
-            img_i[np.isnan(img_i_nan)] = 0
-            if self.rescale is not None:
-                img_i = transform.rescale(img_i, self.rescale)
-            img_i = img_i.astype('uint8')
-            save_i = os.path.splitext(os.path.basename(file_i))[0]
-            save_i = save_i.replace(' ', '_')
-            # split the input image into two
-            # if the previous image and currently image are concatenated horizontally
-            if len(img_i.shape) == 2:
-                img_width = int(img_i.shape[1] / 2)
-                prev_img = img_i[:, :img_width]
-                infer_img = img_i[:, img_width:]
-            # if the previous image image is stacked as another layer
-            elif len(img_i.shape) == 3:
-                prev_img = img_i[0]
-                infer_img = img_i[1]
-            else:
-                raise ValueError('Unknown data structure of input images.')
-            tifffile.imsave(self.prev_image_path + save_i + '.tif', prev_img)
-            tifffile.imsave(self.image_path + save_i + '.tif', infer_img)
-
-        # create masks
-        files_mask = glob.glob(self.source_dir[1] + '*')
-        print('%s files found' % len(files_mask))
-        for file_i in files_mask:
-            mask_i = tifffile.imread(file_i)
-            if self.rescale is not None:
-                mask_i = transform.rescale(mask_i, self.rescale)
-            if self.invert_masks:
-                mask_i = 255 - mask_i
-            if self.threshold_masks is not None:
-                mask_i[mask_i >= self.threshold_masks] = 255
-                mask_i[mask_i < self.threshold_masks] = 0
-            if self.skeletonize:
-                mask_i[mask_i > 1] = 1
-                mask_i = morphology.skeletonize(mask_i) * 255
-            if self.dilate_kernel == 'disk':
-                kernel = morphology.disk
-            elif self.dilate_kernel == 'square':
-                kernel = morphology.square
-            else:
-                raise ValueError(f'Dilate kernel {self.dilate_kernel} unknown!')
-            if self.dilate_mask > 0:
-                mask_i = morphology.dilation(mask_i, kernel(self.dilate_mask))
-            elif self.dilate_mask < 0:
-                mask_i = morphology.erosion(mask_i, kernel(-self.dilate_mask))
-            mask_i = mask_i.astype('uint8')
-            save_i = os.path.splitext(os.path.basename(file_i))[0]
-            save_i = save_i.replace(' ', '_')
-            tifffile.imwrite(self.mask_path + save_i + '.tif', mask_i)
-
-    def __merge_images(self):
-        self.mask_files = glob.glob(self.data_path + '/mask/*.tif')
-        self.image_files = glob.glob(self.data_path + '/image/*.tif')
-        self.prev_image_files = glob.glob(self.data_path + '/prev_image/*.tif')
-
-        if len(self.mask_files) != len(self.image_files):
-            raise ValueError('Number of ground truth does not match number of image stacks')
-
-        for i, file_i in enumerate(self.mask_files):
-            basename_i = os.path.basename(file_i)
-            mask_i = tifffile.imread(self.data_path + '/mask/' + basename_i)
-            image_i = tifffile.imread(self.data_path + '/image/' + basename_i)
-            prev_image_i = tifffile.imread(self.data_path + '/prev_image/' + basename_i)
-            merge = np.zeros((mask_i.shape[0], mask_i.shape[1], 3))
-            merge[:, :, 0] = mask_i
-            merge[:, :, 1] = image_i
-            merge[:, :, 2] = prev_image_i
-            merge = merge.astype('uint8')
-            tifffile.imsave(self.merge_path + str(i) + '.tif', merge)
-
-    def __split(self):
-        self.merges = glob.glob(self.merge_path + '*.tif')
-        n = 0
-        for i in range(len(self.merges)):
-            merge = tifffile.imread(self.merge_path + str(i) + '.tif')
-            dim_in = merge.shape
-            # padding if dim_in < dim_out
-            x_gap = max(0, self.dim_out[0] - dim_in[0])
-            y_gap = max(0, self.dim_out[1] - dim_in[1])
-            merge = np.pad(merge, ((0, x_gap), (0, y_gap), (0, 0)), 'reflect')
-            # number of patches in x and y
-            dim_in = merge.shape
-            N_x = int(np.ceil(dim_in[0] / self.dim_out[0]))
-            N_y = int(np.ceil(dim_in[1] / self.dim_out[1]))
-            # starting indices of patches
-            X_start = np.linspace(0, dim_in[0] - self.dim_out[0], N_x).astype('int16')
-            Y_start = np.linspace(0, dim_in[1] - self.dim_out[1], N_y).astype('int16')
-            for j in range(N_x):
-                for k in range(N_y):
-                    patch_ij = merge[X_start[j]:X_start[j] + self.dim_out[0], Y_start[k]:Y_start[k] + self.dim_out[1],
-                               :]
-                    mask_ij = patch_ij[:, :, 0]
-                    image_ij = patch_ij[:, :, 1]
-                    prev_image_ij = patch_ij[:, :, 2]
-                    tifffile.imsave(self.split_merge_path + f'{n}.tif', patch_ij)
-                    tifffile.imsave(self.split_mask_path + f'{n}.tif', mask_ij)
-                    tifffile.imsave(self.split_image_path + f'{n}.tif', image_ij)
-                    tifffile.imsave(self.split_prev_image_path + f'{n}.tif', prev_image_ij)
-                    n += 1
-
-    def __augment(self, p=0.8):
-        aug_pipeline = Compose([
-            RandomRotate90(p=1.0),
-            ShiftScaleRotate(self.shiftscalerotate[0], self.shiftscalerotate[1], self.shiftscalerotate[2]),
-            GaussNoise(var_limit=(self.noise_amp, self.noise_amp), p=0.3),
-            RandomBrightnessContrast(brightness_limit=self.brightness_contrast[0],
-                                     contrast_limit=self.brightness_contrast[1], p=0.5),
-        ],
-            p=p)
-
-        patches_image = glob.glob(self.split_image_path + '*.tif')
-        patches_mask = glob.glob(self.split_mask_path + '*.tif')
-        patches_prev_image = glob.glob(self.split_prev_image_path + '*.tif')
-        n_patches = len(patches_image)
-        k = 0
-        for i in range(n_patches):
-            image_i = tifffile.imread(patches_image[i])
-            mask_i = tifffile.imread(patches_mask[i])
-            prev_image_i = tifffile.imread(patches_prev_image[i])
-            data_i = {'image': np.dstack([image_i, prev_image_i]), 'mask': mask_i}
-            data_aug_i = np.asarray([aug_pipeline(**data_i) for _ in range(self.aug_factor)])
-            imgs_aug_i = np.asarray([data_aug_i[j]['image'][:, :, 0] for j in range(self.aug_factor)])
-            masks_aug_i = np.asarray([data_aug_i[j]['mask'] for j in range(self.aug_factor)])
-            prev_image_aug_i = np.asarray([data_aug_i[j]['image'][:, :, 1] for j in range(self.aug_factor)])
-
-            for j in range(self.aug_factor):
-                tifffile.imsave(self.aug_image_path + f'{k}.tif', imgs_aug_i[j])
-                tifffile.imsave(self.aug_mask_path + f'{k}.tif', masks_aug_i[j])
-                tifffile.imsave(self.aug_prev_image_path + f'{k}.tif', prev_image_aug_i[j])
-                k += 1
-        print(f'Number of training images: {k}', )
-
-    def __len__(self):
-        if self.aug_factor is not None:
-            return len(os.listdir(self.aug_image_path))
-        else:
-            return len(os.listdir(self.split_image_path))
-
-    def __getitem__(self, idx):
-        imgname = str(idx) + '.tif'
-        midname = os.path.basename(imgname)
-        if self.aug_factor is not None:
-            image_0 = tifffile.imread(self.aug_image_path + midname).astype('float32') / 255
-            mask_0 = tifffile.imread(self.aug_mask_path + midname).astype('float32') / 255
-            prev_image_0 = tifffile.imread(self.aug_prev_image_path + midname).astype('float32') / 255
-        else:
-            image_0 = tifffile.imread(self.split_image_path + midname).astype('float32') / 255
-            mask_0 = tifffile.imread(self.split_image_path + midname).astype('float32') / 255
-            prev_image_0 = tifffile.imread(self.split_prev_image_path + midname).astype('float32') / 255
-        image = torch.from_numpy(image_0)
-        mask = torch.from_numpy(mask_0)
-        prev_image = torch.from_numpy(prev_image_0)
-        del image_0, mask_0, prev_image_0
-        sample = {'image': image, 'mask': mask, 'prev_image': prev_image}
-        return sample
+import glob
+import os
+import shutil
+from skimage import morphology
+from albumentations import (
+    ShiftScaleRotate, GaussNoise,
+    RandomBrightnessContrast, Flip, Compose, RandomRotate90)
+
+import numpy as np
+import tifffile
+import torch
+from torch.utils.data import Dataset
+
+
+class DataProcess(Dataset):
+    """Class for training data generation (processing, splitting, augmentation)"""
+
+    def __init__(self, source_dir, dim_out=(256, 256), aug_factor=10, data_path='../data/', in_channels=1,
+                 out_channels=1, dilate_mask=0, dilate_kernel='disk', add_tile=0,
+                 val_split=0.2, invert=False, skeletonize=False, clip_threshold=(0.2, 99.8), shiftscalerotate=(0, 0, 0),
+                 noise_amp=10, brightness_contrast=(0.25, 0.25), rescale=None, create=True):
+        """
+        Create training data object for network training
+
+        1) Create folder structure for training data
+        2) Move and preprocess training images
+        3) Split input images into tiles
+        4) Augment training data
+        5) Create object of PyTorch Dataset class for training
+
+        Parameters
+        ----------
+        source_dir : Tuple[str, str]
+            Path of training data [images, labels]. Images need to be tif files.
+        dim_out : Tuple[int, int]
+            Resize dimensions of images for training
+        aug_factor : int
+            Factor of image augmentation
+        data_path : str
+            Base path of temporary directories for training data
+        in_channels : int
+            Number of input channels of training data
+        out_channels : int
+            Number of output channels of training data
+        dilate_mask
+            Radius of binary dilation of masks [-2, -1, 0, 1, 2]
+        dilate_kernel : str
+            Dilation kernel ('disk' or 'square')
+        add_tile : int
+            Add additional tile for splitting images into tiles with more overlapping tiles
+        val_split : float
+            Validation split for training
+        invert : bool
+            If True, greyscale binary labels is inverted
+        skeletonize : bool
+            If True, binary labels are skeletonized
+        clip_threshold : Tuple[float, float]
+            Clip thresholds for intensity normalization of images
+        shiftscalerotate : [float, float, float]
+            Shift, scale and rotate image during augmentation
+        noise_amp : float
+            Amplitude of Gaussian noise for image augmentation
+        brightness_contrast : Tuple[float, float]
+            Adapt brightness and contrast of images during augmentation
+        rescale : float, optional
+            Rescale all images and labels by factor rescale
+        create : bool, optional
+            If False, existing data set in data_path is used
+        """
+        self.source_dir = source_dir
+        self.create = create
+        self.data_path = data_path
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.dim_out = dim_out
+        self.skeletonize = skeletonize
+        self.invert = invert
+        self.clip_threshold = clip_threshold
+        self.add_tile = add_tile
+        self.aug_factor = aug_factor
+        self.shiftscalerotate = shiftscalerotate
+        self.brightness_contrast = brightness_contrast
+        self.noise_amp = noise_amp
+        self.dilate_mask = dilate_mask
+        self.dilate_kernel = dilate_kernel
+        self.val_split = val_split
+        self.mode = 'train'
+
+        self.__make_dirs()
+        if create:
+            self.__move_and_edit()
+            self.__merge_images()
+            self.__split()
+            if self.aug_factor is not None:
+                self.__augment()
+
+    def __make_dirs(self):
+        self.image_path = self.data_path + '/image/'
+        self.mask_path = self.data_path + '/mask/'
+        self.merge_path = self.data_path + '/merge/'
+        self.split_merge_path = self.data_path + '/split/merge/'
+        self.split_image_path = self.data_path + '/split/image/'
+        self.split_mask_path = self.data_path + '/split/mask/'
+        self.aug_image_path = self.data_path + '/augmentation/aug_image/'
+        self.aug_mask_path = self.data_path + '/augmentation/aug_mask/'
+
+        # delete old files
+        if self.create:
+            try:
+                shutil.rmtree(self.data_path)
+            except:
+                pass
+        # make folders
+        os.makedirs(self.image_path, exist_ok=True)
+        os.makedirs(self.mask_path, exist_ok=True)
+        os.makedirs(self.merge_path, exist_ok=True)
+        os.makedirs(self.split_merge_path, exist_ok=True)
+        os.makedirs(self.split_image_path, exist_ok=True)
+        os.makedirs(self.split_mask_path, exist_ok=True)
+        os.makedirs(self.aug_image_path, exist_ok=True)
+        os.makedirs(self.aug_mask_path, exist_ok=True)
+
+    def __move_and_edit(self):
+        # create image data
+        files_image = glob.glob(self.source_dir[0] + '*')
+        for file_i in files_image:
+            img_i = tifffile.imread(file_i).astype(np.float32)
+            # clip and normalize (0,255)
+            img_i = np.clip(img_i, a_min=np.nanpercentile(img_i, self.clip_threshold[0]),
+                            a_max=np.percentile(img_i, self.clip_threshold[1]))
+            img_i = (img_i - np.nanmin(img_i)) / (np.nanmax(img_i) - np.nanmin(img_i)) * 255
+            img_i = img_i.astype('uint8')
+            save_i = os.path.splitext(os.path.basename(file_i))[0]
+            save_i = save_i.replace(' ', '_')
+            if len(img_i.shape) == 2:
+                img_i = np.expand_dims(img_i, 0)
+            tifffile.imwrite(self.image_path + save_i + '.tif', img_i)
+        # create masks
+        files_mask = glob.glob(self.source_dir[1] + '*')
+        print('%s files found' % len(files_mask))
+        for file_i in files_mask:
+            mask_i = tifffile.imread(file_i)
+            if len(mask_i.shape) == 2:
+                mask_i = np.expand_dims(mask_i, 0)
+            for j, ch_j in enumerate(mask_i):  # iterate channels
+                if self.skeletonize:
+                    ch_j[ch_j > 1] = 1
+                    ch_j = 1 - ch_j
+                    ch_j = morphology.skeletonize(ch_j)
+                    ch_j = 255 * (1 - ch_j)
+                if self.dilate_kernel == 'disk':
+                    kernel = morphology.disk
+                elif self.dilate_kernel == 'square':
+                    kernel = morphology.square
+                else:
+                    raise ValueError(f'Dilate kernel {self.dilate_kernel} unknown!')
+                if self.dilate_mask > 0 and self.dilate_mask:
+                    ch_j = morphology.erosion(ch_j, kernel(self.dilate_mask))
+                elif self.dilate_mask < 0:
+                    ch_j = morphology.dilation(ch_j, kernel(-self.dilate_mask))
+                if self.invert:
+                    ch_j = 255 - ch_j
+                mask_i[j] = ch_j
+            mask_i = mask_i.astype('uint8')
+            save_i = os.path.splitext(os.path.basename(file_i))[0]
+            save_i = save_i.replace(' ', '_')
+            tifffile.imwrite(self.mask_path + save_i + '.tif', mask_i.astype('int8'))
+
+    def __merge_images(self):
+        self.mask_files = glob.glob(self.data_path + '/mask/*.tif')
+        self.image_files = glob.glob(self.data_path + '/image/*.tif')
+
+        if len(self.mask_files) != len(self.image_files):
+            raise ValueError('Number of ground truth does not match number of image stacks')
+
+        for i, file_i in enumerate(self.mask_files):
+            basename_i = os.path.basename(file_i)
+            mask_i = tifffile.imread(self.data_path + '/mask/' + basename_i)
+            img_i = tifffile.imread(self.data_path + '/image/' + basename_i)
+            merge = np.zeros((mask_i.shape[1], mask_i.shape[2], mask_i.shape[0]+img_i.shape[0]))
+            merge[:, :, :mask_i.shape[0]] = np.moveaxis(mask_i, 0, 2)
+            merge[:, :, mask_i.shape[0]:] = np.moveaxis(img_i, 0, 2)
+            merge = merge.astype('uint8')
+            tifffile.imwrite(self.merge_path + str(i) + '.tif', merge)
+
+    def __split(self):
+        self.merges = glob.glob(self.merge_path + '*.tif')
+        n = 0
+        for i in range(len(self.merges)):
+            merge = tifffile.imread(self.merge_path + str(i) + '.tif')
+            dim_in = merge.shape
+            # padding if dim_in < dim_out
+            x_gap = max(0, self.dim_out[0] - dim_in[0])
+            y_gap = max(0, self.dim_out[1] - dim_in[1])
+            merge = np.pad(merge, ((0, x_gap), (0, y_gap), (0, 0)), 'reflect')
+            # number of patches in x and y
+            dim_in = merge.shape
+            N_x = int(np.ceil(dim_in[0] / self.dim_out[0]))
+            N_y = int(np.ceil(dim_in[1] / self.dim_out[1]))
+            N_x += self.add_tile if N_x > 1 else 0
+            N_y += self.add_tile if N_y > 1 else 0
+            # starting indices of patches
+            X_start = np.linspace(0, dim_in[0] - self.dim_out[0], N_x).astype('int16')
+            Y_start = np.linspace(0, dim_in[1] - self.dim_out[1], N_y).astype('int16')
+            for j in range(N_x):
+                for k in range(N_y):
+                    patch_ij = merge[X_start[j]:X_start[j] + self.dim_out[0], Y_start[k]:Y_start[k] + self.dim_out[1],
+                               :]
+                    mask_ij = patch_ij[:, :, :self.out_channels]
+                    image_ij = patch_ij[:, :, self.out_channels:]
+                    tifffile.imwrite(self.split_merge_path + f'{n}.tif', patch_ij)
+                    tifffile.imwrite(self.split_mask_path + f'{n}.tif', mask_ij)
+                    tifffile.imwrite(self.split_image_path + f'{n}.tif', image_ij)
+                    n += 1
+
+    def __augment(self, p=0.8):
+        aug_pipeline = Compose(transforms=[
+            Flip(),
+            RandomRotate90(p=1.0),
+            ShiftScaleRotate(self.shiftscalerotate[0], self.shiftscalerotate[1], self.shiftscalerotate[2]),
+            GaussNoise(var_limit=(self.noise_amp, self.noise_amp), p=0.3),
+            RandomBrightnessContrast(brightness_limit=self.brightness_contrast[0],
+                                     contrast_limit=self.brightness_contrast[1], p=0.5),
+        ],
+            p=p)
+
+        patches_image = glob.glob(self.split_image_path + '*.tif')
+        patches_mask = glob.glob(self.split_mask_path + '*.tif')
+        n_patches = len(patches_image)
+        k = 0
+        for i in range(n_patches):
+            image_i = tifffile.imread(patches_image[i])
+            mask_i = tifffile.imread(patches_mask[i])
+
+            data_i = {'image': image_i, 'mask': mask_i}
+            data_aug_i = np.asarray([aug_pipeline(**data_i) for _ in range(self.aug_factor)])
+            imgs_aug_i = np.asarray([data_aug_i[j]['image'] for j in range(self.aug_factor)])
+            masks_aug_i = np.asarray([data_aug_i[j]['mask'] for j in range(self.aug_factor)])
+
+            for j in range(self.aug_factor):
+                tifffile.imwrite(self.aug_image_path + f'{k}.tif', imgs_aug_i[j])
+                tifffile.imwrite(self.aug_mask_path + f'{k}.tif', np.moveaxis(masks_aug_i[j], 2, 0))
+                k += 1
+        print(f'Number of training images: {k}')
+
+    def __len__(self):
+        if self.aug_factor is not None:
+            return len(os.listdir(self.aug_image_path))
+        else:
+            return len(os.listdir(self.split_image_path))
+
+    def __getitem__(self, idx):
+        imgname = str(idx) + '.tif'
+        midname = os.path.basename(imgname)
+        if self.aug_factor is not None:
+            image_0 = tifffile.imread(self.aug_image_path + midname).astype('float32') / 255
+            mask_0 = tifffile.imread(self.aug_mask_path + midname).astype('float32') / 255
+        else:
+            image_0 = tifffile.imread(self.split_image_path + midname).astype('float32') / 255
+            mask_0 = tifffile.imread(self.split_image_path + midname).astype('float32') / 255
+        image = torch.from_numpy(image_0)
+        mask = torch.from_numpy(mask_0)
+        del image_0, mask_0
+        sample = {'image': image, 'mask': mask}
+        return sample
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/__md5sum__.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/__md5sum__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import os
-import subprocess
-
-try:
-    subprocess.call(["md5sum", "--help"], stdout=subprocess.DEVNULL)
-except FileNotFoundError:
-	raise Exception # md5sum not found. Are you using Linux?
-
-def md5sum(filename):
-	"""
-		returns the md5sum of a file, along with its filename, e.g.:
-		0df61fe4ddf4455ba4d4e3c15abfabe2  predict_draft.py
-	"""
-	return os.popen(f'md5sum \'{filename}\'').read().split(' ')[0]
-
-def md5sum_folder(folder_name):
-	"""
-		returns the md5sum of a file using the command `tar -cf - {folder_name} | md5sum`
-	"""
-	
-	return os.popen(f'tar -cf - \'{folder_name}\' | md5sum').read()
-
-if __name__ == '__main__':
+import os
+import subprocess
+
+try:
+    subprocess.call(["md5sum", "--help"], stdout=subprocess.DEVNULL)
+except FileNotFoundError:
+	raise Exception # md5sum not found. Are you using Linux?
+
+def md5sum(filename):
+	"""
+		returns the md5sum of a file, along with its filename, e.g.:
+		0df61fe4ddf4455ba4d4e3c15abfabe2  predict_draft.py
+	"""
+	return os.popen(f'md5sum \'{filename}\'').read().split(' ')[0]
+
+def md5sum_folder(folder_name):
+	"""
+		returns the md5sum of a file using the command `tar -cf - {folder_name} | md5sum`
+	"""
+	
+	return os.popen(f'tar -cf - \'{folder_name}\' | md5sum').read()
+
+if __name__ == '__main__':
 	print(md5sum('predict_draft.py'))
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/create_pixel_value_histogram.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/create_pixel_value_histogram.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import cv2
-import numpy as np
-import matplotlib.pyplot as plt
-import math
-
-def create_pixel_value_histogram(input_tifs, frames_per_hist=100, bin_width=8):
-	"""Creates a histogram for the pixel values in a tif file
-
-	Args:
-		input_tifs (str path to .tif files): input
-		frames_per_hist (int, optional): number of frames to plot a histogram. Defaults to 100.
-		bin_width (int, optional): bin width on the outpuut tif plot. Should be set to a value divisible by 256. Defaults to 8.
-
-	Raises:
-		IOError: An IOError is raised when the input tif file cannot be found
-	"""
-	retval, imgs = cv2.imreadmulti(input_tifs[0])
-	fig, axs = plt.subplots(math.ceil(len(imgs)/frames_per_hist), len(input_tifs), figsize=(5, 20))
-	fig.suptitle([input_tif.split('/')[-1] for input_tif in input_tifs])
-	for input_tif_idx, input_tif in enumerate(input_tifs):
-		if input_tif_idx != 0:
-			retval, imgs = cv2.imreadmulti(input_tif)
-		if not retval:
-			print(f'Error: {input_tif} not found.')
-			raise IOError   # tiff file not found		
-		axis_idx = 0
-		for idx, img in enumerate(imgs):
-			if idx % frames_per_hist == 0:
-				img_val = img.flatten()
-				axs[axis_idx, input_tif_idx].hist(img_val, bins=range(0, 256, bin_width))
-				axs[axis_idx, input_tif_idx].set(title=f'frame={idx}')
-				axs[axis_idx, input_tif_idx].set_xlim([0, 255])
-				axs[axis_idx, input_tif_idx].set_yscale('log')
-				axis_idx += 1
-	plt.show()
-
-
-def main():
-	# tif_name = constants.TIFS_NAMES[3]
-	# create_pixel_value_histogram([f"/home/longyuxi/Documents/mount/predicted_out/old_self_model_predictions/predicted_{tif_name}_with_cosh_dice.tif", f"/home/longyuxi/Documents/mount/predicted_out/predicted_newly_drawn_{tif_name}_epoch_500.tif"], bin_width=2)
-	pass
-
-
-
-if __name__ == '__main__':
+import cv2
+import numpy as np
+import matplotlib.pyplot as plt
+import math
+
+def create_pixel_value_histogram(input_tifs, frames_per_hist=100, bin_width=8):
+	"""Creates a histogram for the pixel values in a tif file
+
+	Args:
+		input_tifs (str path to .tif files): input
+		frames_per_hist (int, optional): number of frames to plot a histogram. Defaults to 100.
+		bin_width (int, optional): bin width on the outpuut tif plot. Should be set to a value divisible by 256. Defaults to 8.
+
+	Raises:
+		IOError: An IOError is raised when the input tif file cannot be found
+	"""
+	retval, imgs = cv2.imreadmulti(input_tifs[0])
+	fig, axs = plt.subplots(math.ceil(len(imgs)/frames_per_hist), len(input_tifs), figsize=(5, 20))
+	fig.suptitle([input_tif.split('/')[-1] for input_tif in input_tifs])
+	for input_tif_idx, input_tif in enumerate(input_tifs):
+		if input_tif_idx != 0:
+			retval, imgs = cv2.imreadmulti(input_tif)
+		if not retval:
+			print(f'Error: {input_tif} not found.')
+			raise IOError   # tiff file not found		
+		axis_idx = 0
+		for idx, img in enumerate(imgs):
+			if idx % frames_per_hist == 0:
+				img_val = img.flatten()
+				axs[axis_idx, input_tif_idx].hist(img_val, bins=range(0, 256, bin_width))
+				axs[axis_idx, input_tif_idx].set(title=f'frame={idx}')
+				axs[axis_idx, input_tif_idx].set_xlim([0, 255])
+				axs[axis_idx, input_tif_idx].set_yscale('log')
+				axis_idx += 1
+	plt.show()
+
+
+def main():
+	# tif_name = constants.TIFS_NAMES[3]
+	# create_pixel_value_histogram([f"/home/longyuxi/Documents/mount/predicted_out/old_self_model_predictions/predicted_{tif_name}_with_cosh_dice.tif", f"/home/longyuxi/Documents/mount/predicted_out/predicted_newly_drawn_{tif_name}_epoch_500.tif"], bin_width=2)
+	pass
+
+
+
+if __name__ == '__main__':
 	main()
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/extract_frame_of_movie.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/extract_frame_of_movie.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import cv2 # type: ignore
-import numpy as np
-
-def extract_frame_of_movie(tiff_movie, frame_number, output_file):
-	"""Extract a certain frame of tiff_movie, and write it into a separate file. Used for testing find_frame_of_image
-
-	Args:
-		tiff_movie (str): path to input
-		frame_number (int): which frame to extract
-
-	Raises:
-		IOError: raised when tiff file cannot be found
-	"""
-	retval, imgs = cv2.imreadmulti(tiff_movie)
-	if not retval:
-		print(f'Error: {tiff_movie} not found.')
-		raise IOError   # tiff file not found
-	output = imgs[frame_number]
-	print(output.shape)
-	cv2.imwrite(filename=output_file, img=output, )
-
-def extract_frames_of_movie(tiff_movie, frame_number, output_file):
-	"""Extract up to a certain frame of tiff_movie, and write it into a separate file. Used for testing find_frame_of_image
-
-	Args:
-		tiff_movie (str): path to input
-		frame_number (int): up to which frame to extract
-
-	Raises:
-		IOError: raised when tiff file cannot be found
-	"""
-	retval, imgs = cv2.imreadmulti(tiff_movie)
-	if not retval:
-		print(f'Error: {tiff_movie} not found.')
-		raise IOError   # tiff file not found
-	output = imgs[:frame_number]
-	cv2.imwritemulti(filename=output_file, img=output, )
-
-
-if __name__ == '__main__':
-	# extract_frames_of_movie(f'{constants.LOCAL_MOVIE_DIR}/{constants.TIFS_NAMES[1]}.tif', 10, f'{constants.LOCAL_OUT_DIR}/{constants.TIFS_NAMES[1]}_up_to_frame_10.tif')
+import cv2 # type: ignore
+import numpy as np
+
+def extract_frame_of_movie(tiff_movie, frame_number, output_file):
+	"""Extract a certain frame of tiff_movie, and write it into a separate file. Used for testing find_frame_of_image
+
+	Args:
+		tiff_movie (str): path to input
+		frame_number (int): which frame to extract
+
+	Raises:
+		IOError: raised when tiff file cannot be found
+	"""
+	retval, imgs = cv2.imreadmulti(tiff_movie)
+	if not retval:
+		print(f'Error: {tiff_movie} not found.')
+		raise IOError   # tiff file not found
+	output = imgs[frame_number]
+	print(output.shape)
+	cv2.imwrite(filename=output_file, img=output, )
+
+def extract_frames_of_movie(tiff_movie, frame_number, output_file):
+	"""Extract up to a certain frame of tiff_movie, and write it into a separate file. Used for testing find_frame_of_image
+
+	Args:
+		tiff_movie (str): path to input
+		frame_number (int): up to which frame to extract
+
+	Raises:
+		IOError: raised when tiff file cannot be found
+	"""
+	retval, imgs = cv2.imreadmulti(tiff_movie)
+	if not retval:
+		print(f'Error: {tiff_movie} not found.')
+		raise IOError   # tiff file not found
+	output = imgs[:frame_number]
+	cv2.imwritemulti(filename=output_file, img=output, )
+
+
+if __name__ == '__main__':
+	# extract_frames_of_movie(f'{constants.LOCAL_MOVIE_DIR}/{constants.TIFS_NAMES[1]}.tif', 10, f'{constants.LOCAL_OUT_DIR}/{constants.TIFS_NAMES[1]}_up_to_frame_10.tif')
 	pass
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/find_frame_of_image.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/find_frame_of_image.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import cv2 # type: ignore
-import numpy as np
-import time
-import tifffile
-from tifffile import TiffFile
-import os
-
-def find_frame_of_image(query_image, search_space=[], save_machine_readable_output=True, machine_readable_output_filename='search_result_mr.txt'):
-    """Finds the frame number of query_image within search_space. 
-    
-    This function will move on to the next candidate in search_space if the dimensions of query_image doesn't match a certain candidate. If the dimensions of query_image and candidate match, this function first attempts to find an exact match, but resorts to finding frame with the least mean squared error (MSE) if no exact match is found.
-
-    If save_machine_readable_output is set to True, this function will write a tab-separated file containing the names (not absolute paths) of the query image (label), the candidate image with the best match, and the frame number (0-indexed) that has the best match.
-
-    This function is best used with the function utilize_search_result.generate_siam_unet_input_imgs().
-
-    Args:
-        query_image (str): path to query tiff image, must be single frame
-        search_space (list of str, optional): The list of images over which to search query_image. Defaults to constants.TIFS_NAMES.
-    """
-
-    query = cv2.imread(query_image, cv2.IMREAD_GRAYSCALE)
-    for candidate in search_space:
-        tif_key = TiffFile(candidate)
-        # tif_len = len(tif_key.pages)
-
-        # check if dimensions are the same
-        if not tif_key.pages[0].shape == query.shape:
-            print(f'Shape of query {query.shape} differs with shape of {candidate} {tif_key.pages[0].shape}')
-            continue
-
-        # if yes, progress
-        mses = []
-        frame_nbr = 0
-        imgs = frame_generator(candidate)
-        for img in imgs:
-            # print(frame_nbr)
-            if np.array_equal(img, query):
-                print(f"\n\n!!!!Found exact match in frame {frame_nbr} of {candidate}.\n\n")
-                continue
-            mses.append(mse(query, img))
-            frame_nbr += 1
-        
-        # if there is not an exact match, resort to the best MSE solution
-        print(f'No exact match was found in {candidate}. The closest matching frame was {mses.index(min(mses))} with MSE of {min(mses)}')
-
-
-        if save_machine_readable_output:
-            # save information directly if:
-            #   1. frame numbers match
-            #   2. MSE < 1000
-            if mses.index(min(mses)) == int(os.path.basename(query_image).split(".")[0]):
-                if min(mses) < 1000:
-                    with open(machine_readable_output_filename, 'a') as o:
-                        o.write(f'{os.path.basename(query_image)}\t{os.path.basename(candidate)}\t{mses.index(min(mses))}\n')
-
-def frame_generator(tiff_movie):
-    """Returns a generator for each individual frame of the movie. Should function in the same way as imgs in the expression "for img in imgs".
-
-    Args:
-        tiff_movie (str): path to tiff movie
-    """
-    tif_key = tifffile.TiffFile(tiff_movie)
-    tif_len = len(tif_key.pages)
-    for i in range(tif_len):
-        yield tifffile.imread(tiff_movie, key=i)
-
-def mse(imageA, imageB):
-    # the 'Mean Squared Error' between the two images is the
-    # sum of the squared difference between the two images;
-    # NOTE: the two images must have the same dimension
-    err = np.sum((imageA.astype("float") - imageB.astype("float")) ** 2)
-    err /= float(imageA.shape[0] * imageA.shape[1])
-    
-    # return the MSE, the lower the error, the more "similar"
-    # the two images are
-    return err
-
-
-if __name__ == '__main__':
-    # find_frame_of_image(f'{constants.LOCAL_OUT_DIR}/21B25_shgGFP_kin_1_Pos0_frame_10.tif', [f'{constants.LOCAL_MOVIE_DIR}/{constants.TIFS_NAMES[1]}.tif'])
-
-    # the missing search space was 21D16_shgGFPkin_Pos7.tif
-
-
-    # # successful at finding the location to the amnioserosa images
-    # file_names = ['105.tif','111.tif','120.tif','121.tif','146.tif','165.tif','166.tif','167.tif','1.tif','212.tif','224.tif','231.tif','253.tif','268.tif','2.tif','305.tif','314.tif','328.tif','331.tif','335.tif','369.tif','372.tif','3.tif','413.tif','439.tif','480.tif','496.tif','502.tif','510.tif','522.tif','5.tif','625.tif','646.tif','681.tif','69.tif','700.tif','707.tif','732.tif','778.tif','792.tif','7.tif','822.tif','837.tif','83.tif','840.tif']
-
-    # # file_names = ['105.tif']
-    # for file_name in file_names:
-    #     print(file_name)
-    #     find_frame_of_image(f'{constants.RAZER_LOCAL_BASE_DIR}/training_data/training_data/yokogawa/amnioserosa/image/{file_name}', search_space=constants.RAZER_LARGE_SEARCH_SPACE)
+import cv2 # type: ignore
+import numpy as np
+import time
+import tifffile
+from tifffile import TiffFile
+import os
+
+def find_frame_of_image(query_image, search_space=[], save_machine_readable_output=True, machine_readable_output_filename='search_result_mr.txt'):
+    """Finds the frame number of query_image within search_space. 
+    
+    This function will move on to the next candidate in search_space if the dimensions of query_image doesn't match a certain candidate. If the dimensions of query_image and candidate match, this function first attempts to find an exact match, but resorts to finding frame with the least mean squared error (MSE) if no exact match is found.
+
+    If save_machine_readable_output is set to True, this function will write a tab-separated file containing the names (not absolute paths) of the query image (label), the candidate image with the best match, and the frame number (0-indexed) that has the best match.
+
+    This function is best used with the function utilize_search_result.generate_siam_unet_input_imgs().
+
+    Args:
+        query_image (str): path to query tiff image, must be single frame
+        search_space (list of str, optional): The list of images over which to search query_image. Defaults to constants.TIFS_NAMES.
+    """
+
+    query = cv2.imread(query_image, cv2.IMREAD_GRAYSCALE)
+    for candidate in search_space:
+        tif_key = TiffFile(candidate)
+        # tif_len = len(tif_key.pages)
+
+        # check if dimensions are the same
+        if not tif_key.pages[0].shape == query.shape:
+            print(f'Shape of query {query.shape} differs with shape of {candidate} {tif_key.pages[0].shape}')
+            continue
+
+        # if yes, progress
+        mses = []
+        frame_nbr = 0
+        imgs = frame_generator(candidate)
+        for img in imgs:
+            # print(frame_nbr)
+            if np.array_equal(img, query):
+                print(f"\n\n!!!!Found exact match in frame {frame_nbr} of {candidate}.\n\n")
+                continue
+            mses.append(mse(query, img))
+            frame_nbr += 1
+        
+        # if there is not an exact match, resort to the best MSE solution
+        print(f'No exact match was found in {candidate}. The closest matching frame was {mses.index(min(mses))} with MSE of {min(mses)}')
+
+
+        if save_machine_readable_output:
+            # save information directly if:
+            #   1. frame numbers match
+            #   2. MSE < 1000
+            if mses.index(min(mses)) == int(os.path.basename(query_image).split(".")[0]):
+                if min(mses) < 1000:
+                    with open(machine_readable_output_filename, 'a') as o:
+                        o.write(f'{os.path.basename(query_image)}\t{os.path.basename(candidate)}\t{mses.index(min(mses))}\n')
+
+def frame_generator(tiff_movie):
+    """Returns a generator for each individual frame of the movie. Should function in the same way as imgs in the expression "for img in imgs".
+
+    Args:
+        tiff_movie (str): path to tiff movie
+    """
+    tif_key = tifffile.TiffFile(tiff_movie)
+    tif_len = len(tif_key.pages)
+    for i in range(tif_len):
+        yield tifffile.imread(tiff_movie, key=i)
+
+def mse(imageA, imageB):
+    # the 'Mean Squared Error' between the two images is the
+    # sum of the squared difference between the two images;
+    # NOTE: the two images must have the same dimension
+    err = np.sum((imageA.astype("float") - imageB.astype("float")) ** 2)
+    err /= float(imageA.shape[0] * imageA.shape[1])
+    
+    # return the MSE, the lower the error, the more "similar"
+    # the two images are
+    return err
+
+
+if __name__ == '__main__':
+    # find_frame_of_image(f'{constants.LOCAL_OUT_DIR}/21B25_shgGFP_kin_1_Pos0_frame_10.tif', [f'{constants.LOCAL_MOVIE_DIR}/{constants.TIFS_NAMES[1]}.tif'])
+
+    # the missing search space was 21D16_shgGFPkin_Pos7.tif
+
+
+    # # successful at finding the location to the amnioserosa images
+    # file_names = ['105.tif','111.tif','120.tif','121.tif','146.tif','165.tif','166.tif','167.tif','1.tif','212.tif','224.tif','231.tif','253.tif','268.tif','2.tif','305.tif','314.tif','328.tif','331.tif','335.tif','369.tif','372.tif','3.tif','413.tif','439.tif','480.tif','496.tif','502.tif','510.tif','522.tif','5.tif','625.tif','646.tif','681.tif','69.tif','700.tif','707.tif','732.tif','778.tif','792.tif','7.tif','822.tif','837.tif','83.tif','840.tif']
+
+    # # file_names = ['105.tif']
+    # for file_name in file_names:
+    #     print(file_name)
+    #     find_frame_of_image(f'{constants.RAZER_LOCAL_BASE_DIR}/training_data/training_data/yokogawa/amnioserosa/image/{file_name}', search_space=constants.RAZER_LARGE_SEARCH_SPACE)
     pass
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/generate_plain_image.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/generate_plain_image.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import cv2
-import os
-os.nice(20)
-import subprocess
-import numpy as np
-
-def generate_plain_image(pixel_value=255, shape=(1000, 500), outfile_name="val_255.png"):
-	"""Generates a plain image. Useful for figuring out whether a pixel value of 255 means white or 0 means white. (Hint: 255 is whie in png files)
-
-	Args:
-		pixel_value (int, optional): the pixel value to generate. Defaults to 255.
-		shape (tuple, optional): size of image. Defaults to (1000, 500).
-		outfile_name (str, optional): where to save the file. Defaults to "val_255.png".
-	"""
-	out = (np.ones(shape) * pixel_value).astype(np.uint8)
-	cv2.imwrite(filename=outfile_name, img=out, )
-
-if __name__ == '__main__':
+import cv2
+import os
+os.nice(20)
+import subprocess
+import numpy as np
+
+def generate_plain_image(pixel_value=255, shape=(1000, 500), outfile_name="val_255.png"):
+	"""Generates a plain image. Useful for figuring out whether a pixel value of 255 means white or 0 means white. (Hint: 255 is whie in png files)
+
+	Args:
+		pixel_value (int, optional): the pixel value to generate. Defaults to 255.
+		shape (tuple, optional): size of image. Defaults to (1000, 500).
+		outfile_name (str, optional): where to save the file. Defaults to "val_255.png".
+	"""
+	out = (np.ones(shape) * pixel_value).astype(np.uint8)
+	cv2.imwrite(filename=outfile_name, img=out, )
+
+if __name__ == '__main__':
 	generate_plain_image()
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import cv2
-import numpy as np
-import tifffile
-import os
-import glob
-from scipy.ndimage import geometric_transform
-import tifffile
-import glob
-import numpy as np
-import matplotlib.pyplot as plt
-
-
-def generate_coupled_image(movie, frame, output):
-    """
-    Generates an image from the previous frame of the given frame and the given frame of the given movie. Should be used as input to Siam_UNet. The output image is a tiff file with the files like this, with the output image of twice the width of the input.
-    [    Previous   |     Frame to be    ]
-    [     Frame     |   Inferred From    ]
-
-    Note on arg: 
-        frame (int): 0-indexed
-    """
-
-    curr_frame = tifffile.imread(movie, key=frame)
-    if frame == 0:
-        prev_frame = tifffile.imread(movie, key=(frame + 1))
-    else:
-        prev_frame = tifffile.imread(movie, key=(frame - 1))
-
-    if curr_frame is None:
-        print(f'Error: {movie} not found.')
-        raise IOError  # tiff file not found
-
-    out = np.concatenate((prev_frame, curr_frame), axis=1).astype(np.uint8)
-    cv2.imwrite(filename=output, img=out, )
-
-
-def generate_coupled_image_from_self(img, out_img, noise_amp=10):
-    """
-        Generates an input image for siam by concatenating an image with a transformed version of itself 
-    """
-
-    def __synthesize_prev_img(in_img, noise_amp=10):
-        """Synthesizes previous frame by transforming the input image
-
-        Args:
-            in_img (str): input image path
-            noise_amp (int, optional): Defaults to 10.
-
-        Returns:
-            2-D ndarray: the synthesized previous image
-        """
-        data = tifffile.imread(in_img)
-        image = data
-        modes_x, modes_y = 10, 4
-        amp = 1
-        amps_x, amps_y = np.random.random_sample(modes_x) * amp, np.random.random_sample(modes_y) * amp
-
-        def func(xy):
-            return (xy[0] + np.sum(amps_y * np.sin(modes_y * 2 * np.pi * xy[0] / image.shape[0])),
-                    xy[1] + np.sum(amps_x * np.sin(modes_x * 2 * np.pi * xy[1] / image.shape[1])))
-
-        out = geometric_transform(image, func)
-        noise = np.random.normal(0, noise_amp, size=image.shape)
-        out = out + noise
-        out[out < 0] = 0
-        out[out > 255] = 255
-
-        return out
-
-    curr_frame = tifffile.imread(img)
-    synthesized_previous_frame = __synthesize_prev_img(img, noise_amp)
-
-    if curr_frame is None:
-        raise IOError  # tiff file not found
-
-    out = np.concatenate((synthesized_previous_frame, curr_frame), axis=1).astype(np.uint8)
-    cv2.imwrite(filename=out_img, img=out, )
-
-
-def utilize_search_result(search_result_mr_txt, movie_path_prefix, labels_path_prefix, output_folder):
-    """Parses search results obtained from find_frame_of_image.find_frame_of_image()'s machine readable output and pass them to generate_coupled_image() to create training data for Siam_UNet. 
-
-    This function outputs two folders under output_folder: image and label. All the output will have a suffix of .tif, and thyey will have the same names as the names of input labels. The output in the image directory will be the current frame concatenated with the previous frame, while the label directory will contain the corresponding labels, directly copied from the input labels directory. Visually, the directory structure at output:
-
-    output_folder
-    |
-    |----image
-    |       |-----concatenated images
-    |
-    |
-    |----label
-    |       |-----labels copied from the input labels directory
-
-    Args:
-        search_result_mr_txt (str): path to the machine readable output
-        movie_path_prefix, labels_path_prefix (str): prefixes to name of each movie in the search result file, respectively
-        output_folder (str): path to the output folder. See above.
-    """
-
-    image_output_folder = output_folder + '/image/'
-    label_output_folder = output_folder + '/label/'
-
-    # make output folder if it does not exist
-    os.system(f'mkdir -p \'{output_folder}\'')
-    # recreate image and label output folders
-    os.system(f'rm -rf \'{image_output_folder}\'')
-    os.system(f'rm -rf \'{label_output_folder}\'')
-    os.system(f'mkdir -p \'{image_output_folder}\'')
-    os.system(f'mkdir -p \'{label_output_folder}\'')
-
-    with open(search_result_mr_txt) as sr:
-        lines = sr.readlines()
-        for line in lines:
-            label_path = labels_path_prefix + '/' + line.split('\t')[0]
-            image_path = movie_path_prefix + '/' + line.split('\t')[1]
-            output_image_path = image_output_folder + line.split('\t')[0]
-            frame_number = int(line.split('\t')[2])
-            # copy label to label folder
-            os.system(f'cp \'{label_path}\' \'{label_output_folder}\'')
-            # create concatenated image in image_folder
-            generate_coupled_image(image_path, frame=frame_number, output=output_image_path)
-
-    for file in glob.glob(f'{label_output_folder}/*.tif'):
-        i = cv2.imread(file)
-        fo = cv2.cvtColor(i, cv2.COLOR_RGB2GRAY)
-        os.remove(file)
+import cv2
+import numpy as np
+import tifffile
+import os
+import glob
+from scipy.ndimage import geometric_transform
+import tifffile
+import glob
+import numpy as np
+import matplotlib.pyplot as plt
+
+
+def generate_coupled_image(movie, frame, output):
+    """
+    Generates an image from the previous frame of the given frame and the given frame of the given movie. Should be used as input to Siam_UNet. The output image is a tiff file with the files like this, with the output image of twice the width of the input.
+    [    Previous   |     Frame to be    ]
+    [     Frame     |   Inferred From    ]
+
+    Note on arg: 
+        frame (int): 0-indexed
+    """
+
+    curr_frame = tifffile.imread(movie, key=frame)
+    if frame == 0:
+        prev_frame = tifffile.imread(movie, key=(frame + 1))
+    else:
+        prev_frame = tifffile.imread(movie, key=(frame - 1))
+
+    if curr_frame is None:
+        print(f'Error: {movie} not found.')
+        raise IOError  # tiff file not found
+
+    out = np.concatenate((prev_frame, curr_frame), axis=1).astype(np.uint8)
+    cv2.imwrite(filename=output, img=out, )
+
+
+def generate_coupled_image_from_self(img, out_img, noise_amp=10):
+    """
+        Generates an input image for siam by concatenating an image with a transformed version of itself 
+    """
+
+    def __synthesize_prev_img(in_img, noise_amp=10):
+        """Synthesizes previous frame by transforming the input image
+
+        Args:
+            in_img (str): input image path
+            noise_amp (int, optional): Defaults to 10.
+
+        Returns:
+            2-D ndarray: the synthesized previous image
+        """
+        data = tifffile.imread(in_img)
+        image = data
+        modes_x, modes_y = 10, 4
+        amp = 1
+        amps_x, amps_y = np.random.random_sample(modes_x) * amp, np.random.random_sample(modes_y) * amp
+
+        def func(xy):
+            return (xy[0] + np.sum(amps_y * np.sin(modes_y * 2 * np.pi * xy[0] / image.shape[0])),
+                    xy[1] + np.sum(amps_x * np.sin(modes_x * 2 * np.pi * xy[1] / image.shape[1])))
+
+        out = geometric_transform(image, func)
+        noise = np.random.normal(0, noise_amp, size=image.shape)
+        out = out + noise
+        out[out < 0] = 0
+        out[out > 255] = 255
+
+        return out
+
+    curr_frame = tifffile.imread(img)
+    synthesized_previous_frame = __synthesize_prev_img(img, noise_amp)
+
+    if curr_frame is None:
+        raise IOError  # tiff file not found
+
+    out = np.concatenate((synthesized_previous_frame, curr_frame), axis=1).astype(np.uint8)
+    cv2.imwrite(filename=out_img, img=out, )
+
+
+def utilize_search_result(search_result_mr_txt, movie_path_prefix, labels_path_prefix, output_folder):
+    """Parses search results obtained from find_frame_of_image.find_frame_of_image()'s machine readable output and pass them to generate_coupled_image() to create training data for Siam_UNet. 
+
+    This function outputs two folders under output_folder: image and label. All the output will have a suffix of .tif, and thyey will have the same names as the names of input labels. The output in the image directory will be the current frame concatenated with the previous frame, while the label directory will contain the corresponding labels, directly copied from the input labels directory. Visually, the directory structure at output:
+
+    output_folder
+    |
+    |----image
+    |       |-----concatenated images
+    |
+    |
+    |----label
+    |       |-----labels copied from the input labels directory
+
+    Args:
+        search_result_mr_txt (str): path to the machine readable output
+        movie_path_prefix, labels_path_prefix (str): prefixes to name of each movie in the search result file, respectively
+        output_folder (str): path to the output folder. See above.
+    """
+
+    image_output_folder = output_folder + '/image/'
+    label_output_folder = output_folder + '/label/'
+
+    # make output folder if it does not exist
+    os.system(f'mkdir -p \'{output_folder}\'')
+    # recreate image and label output folders
+    os.system(f'rm -rf \'{image_output_folder}\'')
+    os.system(f'rm -rf \'{label_output_folder}\'')
+    os.system(f'mkdir -p \'{image_output_folder}\'')
+    os.system(f'mkdir -p \'{label_output_folder}\'')
+
+    with open(search_result_mr_txt) as sr:
+        lines = sr.readlines()
+        for line in lines:
+            label_path = labels_path_prefix + '/' + line.split('\t')[0]
+            image_path = movie_path_prefix + '/' + line.split('\t')[1]
+            output_image_path = image_output_folder + line.split('\t')[0]
+            frame_number = int(line.split('\t')[2])
+            # copy label to label folder
+            os.system(f'cp \'{label_path}\' \'{label_output_folder}\'')
+            # create concatenated image in image_folder
+            generate_coupled_image(image_path, frame=frame_number, output=output_image_path)
+
+    for file in glob.glob(f'{label_output_folder}/*.tif'):
+        i = cv2.imread(file)
+        fo = cv2.cvtColor(i, cv2.COLOR_RGB2GRAY)
+        os.remove(file)
         cv2.imwrite(file, fo)
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/threshold_images.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/threshold_images.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import cv2
-from os import listdir
-from os.path import isfile, join
-import numpy as np
-
-def threshold_images(in_path, out_path):
-    """
-    Performs the threshold function on all the images in the folder `in_path` and outputs them in `out_path`
-    Params:
-        in_path: folder of source images
-        out_path: folder to place images
-    """
-
-    files = [f for f in listdir(in_path) if isfile(join(in_path, f))]
-    for f in files:
-        img = np.array(cv2.imread(join(in_path, f), cv2.IMREAD_GRAYSCALE))
-        out_img = ((img >= 150) * np.ones(img.shape) * 255 ).astype(np.uint8)
-        cv2.imwrite(filename=join(out_path, f), img=out_img, )
-
-def invert_images(in_path, out_path):
-    """
-    Performs the invert function on all the images in the folder `in_path` and outputs them in `out_path`
-    Params:
-        in_path: folder of source images
-        out_path: folder to place images
-    """
-
-    files = [f for f in listdir(in_path) if isfile(join(in_path, f))]
-    for f in files:
-        img = np.array(cv2.imread(join(in_path, f), cv2.IMREAD_GRAYSCALE))
-        img = (np.ones(img.shape) * 255 - img).astype(np.uint8)
-        cv2.imwrite(filename=join(out_path, f), img=img, )
-
-
-if __name__ == '__main__':
-    # threshold all the images I have drawn 
+import cv2
+from os import listdir
+from os.path import isfile, join
+import numpy as np
+
+def threshold_images(in_path, out_path):
+    """
+    Performs the threshold function on all the images in the folder `in_path` and outputs them in `out_path`
+    Params:
+        in_path: folder of source images
+        out_path: folder to place images
+    """
+
+    files = [f for f in listdir(in_path) if isfile(join(in_path, f))]
+    for f in files:
+        img = np.array(cv2.imread(join(in_path, f), cv2.IMREAD_GRAYSCALE))
+        out_img = ((img >= 150) * np.ones(img.shape) * 255 ).astype(np.uint8)
+        cv2.imwrite(filename=join(out_path, f), img=out_img, )
+
+def invert_images(in_path, out_path):
+    """
+    Performs the invert function on all the images in the folder `in_path` and outputs them in `out_path`
+    Params:
+        in_path: folder of source images
+        out_path: folder to place images
+    """
+
+    files = [f for f in listdir(in_path) if isfile(join(in_path, f))]
+    for f in files:
+        img = np.array(cv2.imread(join(in_path, f), cv2.IMREAD_GRAYSCALE))
+        img = (np.ones(img.shape) * 255 - img).astype(np.uint8)
+        cv2.imwrite(filename=join(out_path, f), img=img, )
+
+
+if __name__ == '__main__':
+    # threshold all the images I have drawn 
     pass
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/helpers/tif_to_mp4.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/helpers/tif_to_mp4.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import cv2
-import os
-os.nice(20)
-import subprocess
-import numpy as np
-import tifffile
-from skimage import morphology
-
-import platform
-if platform.system() != 'Linux':
-    raise Exception  # this script is designed to use Linux bash commands. Please use Linux
-
-try:
-    subprocess.run(["ffmpeg"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-except:
-    raise Exception   # ffmpeg not detected. Please install ffmpeg
-
-
-def convert_to_mp4(tiff_movie, output_file="out.mp4", fps=30, perform_threshold=False, threshold_val=250, invert=False, normalize_to_0_255=True, closing=False, close_thresh=10):
-    """
-    Converts tiff_movie to an mp4 movie
-
-    params:
-        tiff_movie: file name for input
-        fps: number of frames per second in the output
-        perform_threshold: whether we want the images to be thresholded (i.e. the pixels to be aligned to either white or black), 0 is black, 255 is white
-        threshold_val: the value at which thresholding is done. pixel_val = 255 if pixel_val >= threshold_val else 0
-        normalize_to_0_255: scales each individual image to the full range of (0, 255).
-    """
-
-    imgs = frame_generator(tiff_movie)
-    temp_dir = f'temp_{tiff_movie.split("/")[-1]}'
-    os.system(f"mkdir -p \'{temp_dir}\'")
-
-    ct = 0
-    for img in imgs:
-        if invert:
-            img = np.ones(img.shape) * 255 - img
-        if perform_threshold:
-            img = ((img >= threshold_val) * np.ones(img.shape) * 255 ).astype(np.uint8)
-        if normalize_to_0_255:
-            img = img.astype(np.double)
-            img = (img - np.min(img))/(np.max(img) - np.min(img)) * 255
-            img = img.astype(np.uint8)
-        if closing:
-            img = morphology.opening(img, selem=morphology.star(close_thresh))
-        name = str(ct).zfill(5)
-        cv2.imwrite(f"{temp_dir}/{name}.png", img, [cv2.IMWRITE_PNG_COMPRESSION, 0])
-        ct += 1
-
-    # convert to mp4
-    # -crf 17 is visually "lossless" as mentioned in https://trac.ffmpeg.org/wiki/Encode/H.264
-    ffmpeg_command = f'ffmpeg -y -r {fps} -i \'{temp_dir}/%5d.png\' -c:v libx264 -crf 17 -pix_fmt yuv420p \'{output_file}\''
-
-    # execution and cleanup
-    print('Executing ' + ffmpeg_command)
-    os.system(f'{ffmpeg_command} ; rm -rf \'{temp_dir}\'')
-
-def frame_generator(tiff_movie):
-    """Returns a generator for each individual frame of the movie. Should function in the same way as imgs.
-
-    Args:
-        tiff_movie (str): path to tiff movie
-    """
-    tif_key = tifffile.TiffFile(tiff_movie)
-    tif_len = len(tif_key.pages)
-    for i in range(tif_len):
-        yield tifffile.imread(tiff_movie, key=i)
-
-
-if __name__ == '__main__':
-    # convert_to_mp4('/media/longyuxi/H is for HUGE/docmount backup/unet_pytorch/training_data/test_data/new_microscope/21B11-shgGFP-kin-18-bro4.tif', output_file='/media/longyuxi/H is for HUGE/docmount backup/predicted_out/siam_bce_predicted_lowmem_21B11-shgGFP-kin-18-bro4.mp4', normalize_to_0_255=True)
-    convert_to_mp4('/media/longyuxi/H is for HUGE/docmount backup/predicted_out/minitest.tif', output_file='/media/longyuxi/H is for HUGE/docmount backup/predicted_out/minitest_closing.mp4', normalize_to_0_255=True, closing=True)
+import cv2
+import os
+os.nice(20)
+import subprocess
+import numpy as np
+import tifffile
+from skimage import morphology
+
+import platform
+if platform.system() != 'Linux':
+    raise Exception  # this script is designed to use Linux bash commands. Please use Linux
+
+try:
+    subprocess.run(["ffmpeg"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+except:
+    raise Exception   # ffmpeg not detected. Please install ffmpeg
+
+
+def convert_to_mp4(tiff_movie, output_file="out.mp4", fps=30, perform_threshold=False, threshold_val=250, invert=False, normalize_to_0_255=True, closing=False, close_thresh=10):
+    """
+    Converts tiff_movie to an mp4 movie
+
+    params:
+        tiff_movie: file name for input
+        fps: number of frames per second in the output
+        perform_threshold: whether we want the images to be thresholded (i.e. the pixels to be aligned to either white or black), 0 is black, 255 is white
+        threshold_val: the value at which thresholding is done. pixel_val = 255 if pixel_val >= threshold_val else 0
+        normalize_to_0_255: scales each individual image to the full range of (0, 255).
+    """
+
+    imgs = frame_generator(tiff_movie)
+    temp_dir = f'temp_{tiff_movie.split("/")[-1]}'
+    os.system(f"mkdir -p \'{temp_dir}\'")
+
+    ct = 0
+    for img in imgs:
+        if invert:
+            img = np.ones(img.shape) * 255 - img
+        if perform_threshold:
+            img = ((img >= threshold_val) * np.ones(img.shape) * 255 ).astype(np.uint8)
+        if normalize_to_0_255:
+            img = img.astype(np.double)
+            img = (img - np.min(img))/(np.max(img) - np.min(img)) * 255
+            img = img.astype(np.uint8)
+        if closing:
+            img = morphology.opening(img, selem=morphology.star(close_thresh))
+        name = str(ct).zfill(5)
+        cv2.imwrite(f"{temp_dir}/{name}.png", img, [cv2.IMWRITE_PNG_COMPRESSION, 0])
+        ct += 1
+
+    # convert to mp4
+    # -crf 17 is visually "lossless" as mentioned in https://trac.ffmpeg.org/wiki/Encode/H.264
+    ffmpeg_command = f'ffmpeg -y -r {fps} -i \'{temp_dir}/%5d.png\' -c:v libx264 -crf 17 -pix_fmt yuv420p \'{output_file}\''
+
+    # execution and cleanup
+    print('Executing ' + ffmpeg_command)
+    os.system(f'{ffmpeg_command} ; rm -rf \'{temp_dir}\'')
+
+def frame_generator(tiff_movie):
+    """Returns a generator for each individual frame of the movie. Should function in the same way as imgs.
+
+    Args:
+        tiff_movie (str): path to tiff movie
+    """
+    tif_key = tifffile.TiffFile(tiff_movie)
+    tif_len = len(tif_key.pages)
+    for i in range(tif_len):
+        yield tifffile.imread(tiff_movie, key=i)
+
+
+if __name__ == '__main__':
+    # convert_to_mp4('/media/longyuxi/H is for HUGE/docmount backup/unet_pytorch/training_data/test_data/new_microscope/21B11-shgGFP-kin-18-bro4.tif', output_file='/media/longyuxi/H is for HUGE/docmount backup/predicted_out/siam_bce_predicted_lowmem_21B11-shgGFP-kin-18-bro4.mp4', normalize_to_0_255=True)
+    convert_to_mp4('/media/longyuxi/H is for HUGE/docmount backup/predicted_out/minitest.tif', output_file='/media/longyuxi/H is for HUGE/docmount backup/predicted_out/minitest_closing.mp4', normalize_to_0_255=True, closing=True)
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/losses.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/losses.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import torch
-from torch import nn as nn
-
-
-# adapted from https://github.com/achaiah/pywick/blob/master/pywick/losses.py
-class BCEDiceLoss(nn.Module):
-    def __init__(self, alpha, beta):
-        super(BCEDiceLoss, self).__init__()
-        self.bce = BCELoss2d()
-        self.dice = SoftDiceLoss()
-        self.alpha = alpha
-        self.beta = beta
-
-    def forward(self, logits, targets):
-        return self.alpha * self.bce(logits, targets) + self.beta * self.dice(logits, targets)
-
-
-class logcoshDiceLoss(nn.Module):
-    def __init__(self):
-        super(logcoshDiceLoss, self).__init__()
-        self.dice = SoftDiceLoss()
-
-    def forward(self, logits, targets):
-        x = self.dice(logits, targets)
-        return torch.log((torch.exp(x) + torch.exp(-x)) / 2)
-
-
-class BCELoss2d(nn.Module):
-    def __init__(self, weight=None, size_average=True, **kwargs):
-        super(BCELoss2d, self).__init__()
-        self.bce_loss = nn.BCELoss(weight, size_average)
-
-    def forward(self, logits, targets):
-        probs = torch.sigmoid(logits)
-        probs_flat = probs.view(-1)
-        targets_flat = targets.view(-1)
-        return self.bce_loss(probs_flat, targets_flat)
-
-
-class weightedBCELoss(nn.Module):
-    def __init__(self, alpha=1, beta=0.1):
-        super(weightedBCELoss, self).__init__()
-        self.bce = nn.BCELoss(reduce=False)
-        self.alpha, self.beta = alpha, beta
-
-    def forward(self, logits, targets):
-        probs = torch.sigmoid(logits)
-        # compute weights
-        weights = torch.clone(targets)
-        weights[targets >= 0.5] = self.alpha
-        weights[targets < 0.5] = self.beta
-        # compute loss
-        loss = torch.mean(self.bce(probs, targets) * weights)
-        return loss
-
-
-class SoftDiceLoss(nn.Module):
-    def __init__(self, smooth=1.0):
-        super(SoftDiceLoss, self).__init__()
-        self.smooth = smooth
-
-    def forward(self, logits, targets):
-        num = targets.size(0)
-        probs = torch.sigmoid(logits)
-        m1 = probs.view(num, -1)
-        m2 = targets.view(num, -1)
-        intersection = (m1 * m2)
-
-        score = 2. * (intersection.sum(1) + self.smooth) / (m1.sum(1) + m2.sum(1) + self.smooth)
-        score = 1 - score.sum() / num
-        return score
-
-
-class TverskyLoss(nn.Module):
-    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
-        super(TverskyLoss, self).__init__()
-        self.alpha = alpha
-        self.beta = beta
-        self.smooth = smooth
-
-    def forward(self, inputs, targets):
-        inputs = torch.sigmoid(inputs)
-        inputs = inputs.view(-1)
-        targets = targets.view(-1)
-
-        # True Positives, False Positives & False Negatives
-        TP = (inputs * targets).sum()
-        FP = ((1 - targets) * inputs).sum()
-        FN = (targets * (1 - inputs)).sum()
-
-        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
-
-        return 1 - Tversky
-
-
-class logcoshTverskyLoss(nn.Module):
-    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
-        super(logcoshTverskyLoss, self).__init__()
-        self.alpha = alpha
-        self.beta = beta
-        self.smooth = smooth
-
-    def forward(self, inputs, targets):
-        inputs = torch.sigmoid(inputs)
-        inputs = inputs.view(-1)
-        targets = targets.view(-1)
-
-        # True Positives, False Positives & False Negatives
-        TP = (inputs * targets).sum()
-        FP = ((1 - targets) * inputs).sum()
-        FN = (targets * (1 - inputs)).sum()
-
-        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
-
-        return torch.log(torch.cosh(1 - Tversky))
+import torch
+from torch import nn as nn
+
+
+# adapted from https://github.com/achaiah/pywick/blob/master/pywick/losses.py
+class BCEDiceLoss(nn.Module):
+    def __init__(self, alpha, beta):
+        super(BCEDiceLoss, self).__init__()
+        self.bce = BCELoss2d()
+        self.dice = SoftDiceLoss()
+        self.alpha = alpha
+        self.beta = beta
+
+    def forward(self, logits, targets):
+        return self.alpha * self.bce(logits, targets) + self.beta * self.dice(logits, targets)
+
+
+class logcoshDiceLoss(nn.Module):
+    def __init__(self):
+        super(logcoshDiceLoss, self).__init__()
+        self.dice = SoftDiceLoss()
+
+    def forward(self, logits, targets):
+        x = self.dice(logits, targets)
+        return torch.log((torch.exp(x) + torch.exp(-x)) / 2)
+
+
+class BCELoss2d(nn.Module):
+    def __init__(self, weight=None, size_average=True, **kwargs):
+        super(BCELoss2d, self).__init__()
+        self.bce_loss = nn.BCELoss(weight, size_average)
+
+    def forward(self, logits, targets):
+        probs = torch.sigmoid(logits)
+        probs_flat = probs.view(-1)
+        targets_flat = targets.view(-1)
+        return self.bce_loss(probs_flat, targets_flat)
+
+
+class weightedBCELoss(nn.Module):
+    def __init__(self, alpha=1, beta=0.1):
+        super(weightedBCELoss, self).__init__()
+        self.bce = nn.BCELoss(reduce=False)
+        self.alpha, self.beta = alpha, beta
+
+    def forward(self, logits, targets):
+        probs = torch.sigmoid(logits)
+        # compute weights
+        weights = torch.clone(targets)
+        weights[targets >= 0.5] = self.alpha
+        weights[targets < 0.5] = self.beta
+        # compute loss
+        loss = torch.mean(self.bce(probs, targets) * weights)
+        return loss
+
+
+class SoftDiceLoss(nn.Module):
+    def __init__(self, smooth=1.0):
+        super(SoftDiceLoss, self).__init__()
+        self.smooth = smooth
+
+    def forward(self, logits, targets):
+        num = targets.size(0)
+        probs = torch.sigmoid(logits)
+        m1 = probs.view(num, -1)
+        m2 = targets.view(num, -1)
+        intersection = (m1 * m2)
+
+        score = 2. * (intersection.sum(1) + self.smooth) / (m1.sum(1) + m2.sum(1) + self.smooth)
+        score = 1 - score.sum() / num
+        return score
+
+
+class TverskyLoss(nn.Module):
+    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
+        super(TverskyLoss, self).__init__()
+        self.alpha = alpha
+        self.beta = beta
+        self.smooth = smooth
+
+    def forward(self, inputs, targets):
+        inputs = torch.sigmoid(inputs)
+        inputs = inputs.view(-1)
+        targets = targets.view(-1)
+
+        # True Positives, False Positives & False Negatives
+        TP = (inputs * targets).sum()
+        FP = ((1 - targets) * inputs).sum()
+        FN = (targets * (1 - inputs)).sum()
+
+        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
+
+        return 1 - Tversky
+
+
+class logcoshTverskyLoss(nn.Module):
+    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
+        super(logcoshTverskyLoss, self).__init__()
+        self.alpha = alpha
+        self.beta = beta
+        self.smooth = smooth
+
+    def forward(self, inputs, targets):
+        inputs = torch.sigmoid(inputs)
+        inputs = inputs.view(-1)
+        targets = targets.view(-1)
+
+        # True Positives, False Positives & False Negatives
+        TP = (inputs * targets).sum()
+        FP = ((1 - targets) * inputs).sum()
+        FN = (targets * (1 - inputs)).sum()
+
+        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
+
+        return torch.log(torch.cosh(1 - Tversky))
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/predict.py` & `bio_image_unet-1.0.0a1/biu/siam_unet/predict.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,240 +1,233 @@
-import os
-
-import numpy as np
-import tifffile
-import torch
-from tifffile.tifffile import TiffFile
-from tqdm import tqdm as tqdm
-from biu.progress import ProgressNotifier
-
-from .siam_unet import Siam_UNet
-
-# select device
-if torch.has_cuda:
-    device = torch.device('cuda:0')
-elif hasattr(torch, 'has_mps'):  # only for apple m1/m2/...
-    if torch.has_mps:
-        device = torch.device('mps')
-    else:
-        device = torch.device('cpu')
-else:
-    device = torch.device('cpu')
-
-
-class Predict:
-    """
-    Class for prediction of tif-movies.
-    1) Loading file and preprocess (normalization)
-    2) Resizing of images into patches with resize_dim
-    3) Prediction with U-Net
-    4) Stitching of predicted patches and averaging of overlapping regions
-    """
-
-    def __init__(self, tif_file, result_name, model_params, resize_dim=(512, 512), invert=False,
-                 normalization_mode='single', clip_threshold=(0.0, 99.98), add_tile=0, normalize_result=False,
-                 progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
-        """
-        Predicts a tif movie
-
-        Parameters
-        ----------
-        tif_file : str
-            Path to input tif stack
-        result_name : str
-            Path of result file
-        tif_file : str
-            path of tif file
-        result_name : str
-            path for result
-        model_params : str
-            path of u-net parameters (.pth file)
-        resize_dim
-            Image dimensions for resizing for prediction. If resize_dim=None, the image will not be resized but
-            the whole image will be processed by the convolution layers.
-        invert : bool
-            Invert greyscale of image(s) before prediction
-        normalization_mode : str
-            Mode for intensity normalization for 3D stacks prior to prediction ('single': each image individually,
-            'all': based on histogram of full stack, 'first': based on histogram of first image in stack)
-        clip_threshold : Tuple[float, float]
-            Clip threshold for image intensity before prediction
-        add_tile : int, optional
-            Add additional tiles for splitting large images to increase overlap
-        normalize_result : bool
-            If True, results are normalized to [0, 255]
-        progress_notifier:
-            Wrapper to show tqdm progress notifier in gui
-        """
-        self.tif_file = tif_file
-        self.add_tile = add_tile
-        self.invert = invert
-        self.normalization_mode = normalization_mode
-        self.clip_threshold = clip_threshold
-        self.result_name = result_name
-        self.normalize_result = normalize_result  # todo to be implemented for Siam-U-Net?
-
-        # load model
-        self.model_params = torch.load(model_params, map_location=device)
-        self.model = Siam_UNet(n_filter=self.model_params['n_filter'], mode=self.model_params['mode']).to(device)
-        self.model.load_state_dict(self.model_params['state_dict'])
-        self.model.eval()
-
-        # split data into groups of two images
-        tif_key = TiffFile(self.tif_file)
-        self.tif_len = len(tif_key.pages)
-        self.imgs_shape = [self.tif_len, tif_key.pages[0].shape[0], tif_key.pages[0].shape[1]]
-        if resize_dim is not None:
-            self.resize_dim = resize_dim
-        else:
-            self.resize_dim = (self.imgs_shape[1], self.imgs_shape[2])
-
-        # create temp folder
-        temp_dir = f'temp_{self.tif_file.split("/")[-1]}'
-
-        # taken from split()
-        # number of patches in x and y
-        self.N_x = int(np.ceil(self.imgs_shape[1] / self.resize_dim[0])) + self.add_tile
-        self.N_y = int(np.ceil(self.imgs_shape[2] / self.resize_dim[1])) + self.add_tile
-        self.N_per_img = self.N_x * self.N_y
-        self.N = self.N_x * self.N_y  # total number of patches
-
-        self.progress_notifier = progress_notifier
-
-        # predict each pair, and save the output of each one as a separate image
-        os.makedirs(temp_dir, exist_ok=True)
-        print('Predicting data ...')
-        with tifffile.TiffWriter(self.result_name, bigtiff=False) as tif:
-            for i, _ in enumerate(self.progress_notifier.iterator(range(self.tif_len))):
-                if i == 0:
-                    if self.tif_len == 1:
-                        prev_img = tifffile.imread(self.tif_file, key=0)
-                    else:
-                        prev_img = tifffile.imread(self.tif_file, key=1)
-                else:
-                    prev_img = current_img
-                current_img = tifffile.imread(self.tif_file, key=i)
-
-                img_stack = np.array([prev_img, current_img])
-                img_stack = self.__preprocess(img_stack)
-                patches = self.__split(img_stack)
-                print(f'Patches shape:{patches.shape}') if i == 0 else None
-                result_patches = self.__predict(patches)
-                imgs_result = self.__stitch(result_patches)
-                tif.write(imgs_result, contiguous=True)
-
-    def __preprocess(self, imgs):
-        if len(imgs.shape) == 3:
-            if self.normalization_mode == 'single':
-                for i, img in enumerate(imgs):
-                    img = np.clip(img, a_min=np.nanpercentile(img, self.clip_threshold[0]),
-                                  a_max=np.percentile(img, self.clip_threshold[1]))
-                    img = img - np.min(img)
-                    img = img / np.max(img) * 255
-                    if self.invert:
-                        img = 255 - img
-                    imgs[i] = img
-            elif self.normalization_mode == 'first':
-                clip_threshold = (np.nanpercentile(imgs[0], self.clip_threshold[0]),
-                                  np.percentile(imgs[0], self.clip_threshold[1]))
-                imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
-                imgs = imgs - np.min(imgs)
-                imgs = imgs / np.max(imgs) * 255
-                if self.invert:
-                    imgs = 255 - imgs
-            elif self.normalization_mode == 'all':
-                clip_threshold = (np.nanpercentile(imgs, self.clip_threshold[0]),
-                                  np.percentile(imgs, self.clip_threshold[1]))
-                imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
-                imgs = imgs - np.min(imgs)
-                imgs = imgs / np.max(imgs) * 255
-                if self.invert:
-                    imgs = 255 - imgs
-            else:
-                raise ValueError(f'normalization_mode {self.normalization_mode} not valid!')
-        if len(imgs.shape) == 2:
-            imgs = np.clip(imgs, a_min=np.nanpercentile(imgs, self.clip_threshold[0]),
-                           a_max=np.percentile(imgs, self.clip_threshold[1]))
-            imgs = imgs - np.min(imgs)
-            imgs = imgs / np.max(imgs) * 255
-            if self.invert:
-                imgs = 255 - imgs
-        imgs = imgs.astype('uint8')
-        return imgs
-
-    def __split(self, imgs):
-        # define array for prediction
-        patches = np.zeros((self.N, 2, self.resize_dim[0], self.resize_dim[1]), dtype='uint8')
-
-        # zero padding of image if imgs_shape < resize_dim
-        if self.imgs_shape[0] > 1:
-            if self.imgs_shape[1] < self.resize_dim[0]:  # for x
-                imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)),
-                              'constant')
-            if self.imgs_shape[2] < self.resize_dim[1]:  # for y
-                imgs = np.pad(imgs, ((0, 0), (0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])),
-                              'constant')
-        elif self.imgs_shape[0] == 1:
-            if self.imgs_shape[1] < self.resize_dim[0]:  # for x
-                imgs = np.pad(imgs, ((0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)), 'constant')
-            if self.imgs_shape[2] < self.resize_dim[1]:  # for y
-                imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])), 'constant')
-
-        # starting indices of patches
-        self.X_start = np.linspace(0, self.imgs_shape[1] - self.resize_dim[0], self.N_x).astype('uint16')
-        self.Y_start = np.linspace(0, self.imgs_shape[2] - self.resize_dim[1], self.N_y).astype('uint16')
-
-        # split in resize_dim
-        n = 0
-
-        i = 1
-        for j in range(self.N_x):
-            for k in range(self.N_y):
-                patches[n, 0, :, :] = imgs[i][self.X_start[j]:self.X_start[j] + self.resize_dim[0],
-                                      self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
-                patches[n, 1, :, :] = imgs[i - 1][self.X_start[j]:self.X_start[j] + self.resize_dim[0],
-                                      self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
-                n += 1
-        return patches
-
-    def __predict(self, patches):
-        result_patches = np.zeros((patches.shape[0], 1, patches.shape[2], patches.shape[3]), dtype='uint8')
-        with torch.no_grad():
-            for i, patch_i in enumerate(patches):
-                image_patch_i = patch_i[0, :, :]
-                prev_image_patch_i = patch_i[1, :, :]
-
-                image_patch_i = torch.from_numpy(image_patch_i.astype('float32') / 255).to(device).view(
-                    (1, 1, self.resize_dim[0], self.resize_dim[1]))
-                prev_image_patch_i = torch.from_numpy(prev_image_patch_i.astype('float32') / 255).to(device).view(
-                    (1, 1, self.resize_dim[0], self.resize_dim[1]))
-
-                res_i = self.model(image_patch_i, prev_image_patch_i)[0].view(
-                    (1, self.resize_dim[0], self.resize_dim[1])).cpu().numpy() * 255
-                result_patches[i] = res_i.astype('uint8')
-                del patch_i, res_i
-        return result_patches
-
-    def __stitch(self, result_patches):
-        dtype = result_patches.dtype
-        i = 0
-        if self.imgs_shape[0] > 1:  # if stack
-            stack_result_i = np.zeros((self.N_per_img, np.max((self.resize_dim[0], self.imgs_shape[1])),
-                                       np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype=dtype) * np.nan
-        elif self.imgs_shape[0] == 1:  # if only one image
-            stack_result_i = np.zeros((self.N_per_img, np.max((self.resize_dim[0], self.imgs_shape[1])),
-                                       np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype=dtype) * np.nan
-        else:
-            raise ValueError('Wrong data format!')
-        n = 0
-        for j in range(self.N_x):
-            for k in range(self.N_y):
-                stack_result_i[n, self.X_start[j]:self.X_start[j] + self.resize_dim[0],
-                self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]] = result_patches[i * self.N_per_img + n, 0, :, :]
-                n += 1
-        # average overlapping regions
-        imgs_result = np.nanmean(stack_result_i, axis=0).astype(dtype)
-
-        # change to input size (if zero padding)
-        imgs_result = imgs_result[:self.imgs_shape[1], :self.imgs_shape[2]]
-
-        return imgs_result
+import os
+
+import numpy as np
+import tifffile
+import torch
+from tifffile.tifffile import TiffFile
+from tqdm import tqdm as tqdm
+from biu.progress import ProgressNotifier
+
+from .siam_unet import Siam_UNet
+from ..utils import get_device
+
+# select device
+device = get_device()
+
+
+class Predict:
+    """
+    Class for prediction of tif-movies.
+    1) Loading file and preprocess (normalization)
+    2) Resizing of images into patches with resize_dim
+    3) Prediction with U-Net
+    4) Stitching of predicted patches and averaging of overlapping regions
+    """
+
+    def __init__(self, tif_file, result_name, model_params, resize_dim=(512, 512), invert=False,
+                 normalization_mode='single', clip_threshold=(0.0, 99.98), add_tile=0, normalize_result=False,
+                 progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
+        """
+        Predicts a tif movie
+
+        Parameters
+        ----------
+        tif_file : str
+            Path to input tif stack
+        result_name : str
+            Path of result file
+        tif_file : str
+            path of tif file
+        result_name : str
+            path for result
+        model_params : str
+            path of u-net parameters (.pth file)
+        resize_dim
+            Image dimensions for resizing for prediction. If resize_dim=None, the image will not be resized but
+            the whole image will be processed by the convolution layers.
+        invert : bool
+            Invert greyscale of image(s) before prediction
+        normalization_mode : str
+            Mode for intensity normalization for 3D stacks prior to prediction ('single': each image individually,
+            'all': based on histogram of full stack, 'first': based on histogram of first image in stack)
+        clip_threshold : Tuple[float, float]
+            Clip threshold for image intensity before prediction
+        add_tile : int, optional
+            Add additional tiles for splitting large images to increase overlap
+        normalize_result : bool
+            If True, results are normalized to [0, 255]
+        progress_notifier:
+            Wrapper to show tqdm progress notifier in gui
+        """
+        self.tif_file = tif_file
+        self.add_tile = add_tile
+        self.invert = invert
+        self.normalization_mode = normalization_mode
+        self.clip_threshold = clip_threshold
+        self.result_name = result_name
+        self.normalize_result = normalize_result  # todo to be implemented for Siam-U-Net?
+
+        # load model
+        self.model_params = torch.load(model_params, map_location=device)
+        self.model = Siam_UNet(n_filter=self.model_params['n_filter'], mode=self.model_params['mode']).to(device)
+        self.model.load_state_dict(self.model_params['state_dict'])
+        self.model.eval()
+
+        # split data into groups of two images
+        tif_key = TiffFile(self.tif_file)
+        self.tif_len = len(tif_key.pages)
+        self.imgs_shape = [self.tif_len, tif_key.pages[0].shape[0], tif_key.pages[0].shape[1]]
+        if resize_dim is not None:
+            self.resize_dim = resize_dim
+        else:
+            self.resize_dim = (self.imgs_shape[1], self.imgs_shape[2])
+
+        # create temp folder
+        temp_dir = f'temp_{self.tif_file.split("/")[-1]}'
+
+        # taken from split()
+        # number of patches in x and y
+        self.N_x = int(np.ceil(self.imgs_shape[1] / self.resize_dim[0])) + self.add_tile
+        self.N_y = int(np.ceil(self.imgs_shape[2] / self.resize_dim[1])) + self.add_tile
+        self.N_per_img = self.N_x * self.N_y
+        self.N = self.N_x * self.N_y  # total number of patches
+
+        self.progress_notifier = progress_notifier
+
+        # predict each pair, and save the output of each one as a separate image
+        os.makedirs(temp_dir, exist_ok=True)
+        print('Predicting data ...')
+        with tifffile.TiffWriter(self.result_name, bigtiff=False) as tif:
+            for i, _ in enumerate(self.progress_notifier.iterator(range(self.tif_len))):
+                if i == 0:
+                    if self.tif_len == 1:
+                        prev_img = tifffile.imread(self.tif_file, key=0)
+                    else:
+                        prev_img = tifffile.imread(self.tif_file, key=1)
+                else:
+                    prev_img = current_img
+                current_img = tifffile.imread(self.tif_file, key=i)
+
+                img_stack = np.array([prev_img, current_img])
+                img_stack = self.__preprocess(img_stack)
+                patches = self.__split(img_stack)
+                print(f'Patches shape:{patches.shape}') if i == 0 else None
+                result_patches = self.__predict(patches)
+                imgs_result = self.__stitch(result_patches)
+                tif.write(imgs_result, contiguous=True)
+
+    def __preprocess(self, imgs):
+        if len(imgs.shape) == 3:
+            if self.normalization_mode == 'single':
+                for i, img in enumerate(imgs):
+                    img = np.clip(img, a_min=np.nanpercentile(img, self.clip_threshold[0]),
+                                  a_max=np.percentile(img, self.clip_threshold[1]))
+                    img = img - np.min(img)
+                    img = img / np.max(img) * 255
+                    if self.invert:
+                        img = 255 - img
+                    imgs[i] = img
+            elif self.normalization_mode == 'first':
+                clip_threshold = (np.nanpercentile(imgs[0], self.clip_threshold[0]),
+                                  np.percentile(imgs[0], self.clip_threshold[1]))
+                imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
+                imgs = imgs - np.min(imgs)
+                imgs = imgs / np.max(imgs) * 255
+                if self.invert:
+                    imgs = 255 - imgs
+            elif self.normalization_mode == 'all':
+                clip_threshold = (np.nanpercentile(imgs, self.clip_threshold[0]),
+                                  np.percentile(imgs, self.clip_threshold[1]))
+                imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
+                imgs = imgs - np.min(imgs)
+                imgs = imgs / np.max(imgs) * 255
+                if self.invert:
+                    imgs = 255 - imgs
+            else:
+                raise ValueError(f'normalization_mode {self.normalization_mode} not valid!')
+        if len(imgs.shape) == 2:
+            imgs = np.clip(imgs, a_min=np.nanpercentile(imgs, self.clip_threshold[0]),
+                           a_max=np.percentile(imgs, self.clip_threshold[1]))
+            imgs = imgs - np.min(imgs)
+            imgs = imgs / np.max(imgs) * 255
+            if self.invert:
+                imgs = 255 - imgs
+        imgs = imgs.astype('uint8')
+        return imgs
+
+    def __split(self, imgs):
+        # define array for prediction
+        patches = np.zeros((self.N, 2, self.resize_dim[0], self.resize_dim[1]), dtype='uint8')
+
+        # zero padding of image if imgs_shape < resize_dim
+        if self.imgs_shape[0] > 1:
+            if self.imgs_shape[1] < self.resize_dim[0]:  # for x
+                imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)),
+                              'constant')
+            if self.imgs_shape[2] < self.resize_dim[1]:  # for y
+                imgs = np.pad(imgs, ((0, 0), (0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])),
+                              'constant')
+        elif self.imgs_shape[0] == 1:
+            if self.imgs_shape[1] < self.resize_dim[0]:  # for x
+                imgs = np.pad(imgs, ((0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)), 'constant')
+            if self.imgs_shape[2] < self.resize_dim[1]:  # for y
+                imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])), 'constant')
+
+        # starting indices of patches
+        self.X_start = np.linspace(0, self.imgs_shape[1] - self.resize_dim[0], self.N_x).astype('uint16')
+        self.Y_start = np.linspace(0, self.imgs_shape[2] - self.resize_dim[1], self.N_y).astype('uint16')
+
+        # split in resize_dim
+        n = 0
+
+        i = 1
+        for j in range(self.N_x):
+            for k in range(self.N_y):
+                patches[n, 0, :, :] = imgs[i][self.X_start[j]:self.X_start[j] + self.resize_dim[0],
+                                      self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
+                patches[n, 1, :, :] = imgs[i - 1][self.X_start[j]:self.X_start[j] + self.resize_dim[0],
+                                      self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
+                n += 1
+        return patches
+
+    def __predict(self, patches):
+        result_patches = np.zeros((patches.shape[0], 1, patches.shape[2], patches.shape[3]), dtype='uint8')
+        with torch.no_grad():
+            for i, patch_i in enumerate(patches):
+                image_patch_i = patch_i[0, :, :]
+                prev_image_patch_i = patch_i[1, :, :]
+
+                image_patch_i = torch.from_numpy(image_patch_i.astype('float32') / 255).to(device).view(
+                    (1, 1, self.resize_dim[0], self.resize_dim[1]))
+                prev_image_patch_i = torch.from_numpy(prev_image_patch_i.astype('float32') / 255).to(device).view(
+                    (1, 1, self.resize_dim[0], self.resize_dim[1]))
+
+                res_i = self.model(image_patch_i, prev_image_patch_i)[0].view(
+                    (1, self.resize_dim[0], self.resize_dim[1])).cpu().numpy() * 255
+                result_patches[i] = res_i.astype('uint8')
+                del patch_i, res_i
+        return result_patches
+
+    def __stitch(self, result_patches):
+        dtype = result_patches.dtype
+        i = 0
+        if self.imgs_shape[0] > 1:  # if stack
+            stack_result_i = np.zeros((self.N_per_img, np.max((self.resize_dim[0], self.imgs_shape[1])),
+                                       np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype=dtype) * np.nan
+        elif self.imgs_shape[0] == 1:  # if only one image
+            stack_result_i = np.zeros((self.N_per_img, np.max((self.resize_dim[0], self.imgs_shape[1])),
+                                       np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype=dtype) * np.nan
+        else:
+            raise ValueError('Wrong data format!')
+        n = 0
+        for j in range(self.N_x):
+            for k in range(self.N_y):
+                stack_result_i[n, self.X_start[j]:self.X_start[j] + self.resize_dim[0],
+                self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]] = result_patches[i * self.N_per_img + n, 0, :, :]
+                n += 1
+        # average overlapping regions
+        imgs_result = np.nanmean(stack_result_i, axis=0).astype(dtype)
+
+        # change to input size (if zero padding)
+        imgs_result = imgs_result[:self.imgs_shape[1], :self.imgs_shape[2]]
+
+        return imgs_result
```

### Comparing `bio-image-unet-0.6.1/biu/siam_unet/train.py` & `bio_image_unet-1.0.0a1/biu/unet/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,191 @@
-import glob
-import os
-
-import torch
-import torch.optim as optim
-from barbar import Bar
-from biu.siam_unet import BCEDiceLoss
-from torch.utils.data import DataLoader, random_split
-
-from . import logcoshTverskyLoss, TverskyLoss, weightedBCELoss
-from .predict import Predict
-from .siam_unet import Siam_UNet
-
-# select device
-if torch.has_cuda:
-    device = torch.device('cuda:0')
-elif hasattr(torch, 'has_mps'):  # only for apple m1/m2/...
-    if torch.has_mps:
-        device = torch.device('mps')
-    else:
-        device = torch.device('cpu')
-else:
-    device = torch.device('cpu')
-
-
-class Trainer:
-    def __init__(self, dataset, num_epochs, batch_size=4, lr=1e-3, n_filter=32, mode='max', val_split=0.2,
-                 save_dir='./', save_name='model.pth', save_iter=False, loss_function='BCEDice',
-                 loss_params=(1, 1), load_weights=None):
-        """
-        Class for training of neural network. Creates trainer object, training is started with .start().
-
-        Parameters
-        ----------
-        dataset
-            Training data, object of PyTorch Dataset class
-        num_epochs : int
-            Number of training epochs
-        batch_size : int
-            Batch size for training
-        lr : float
-            Learning rate
-        n_filter : int
-            Number of convolutional filters in first layer
-        mode : str
-            Mode to combine low-level features of T-1 and T ('max' or 'corr')
-        val_split : float
-            Validation split
-        save_dir : str
-            Path of directory to save trained networks
-        save_name : str
-            Base name for saving trained networks
-        save_iter : bool
-            If True, network state is save after each epoch
-        load_weights : str, optional
-            If not None, network state is loaded before training
-        loss_function : str
-            Loss function ('BCEDice', 'Tversky' or 'logcoshTversky')
-        loss_params : Tuple[float, float]
-            Parameter of loss function, depends on chosen loss function
-        """
-
-        self.model = Siam_UNet(n_filter=n_filter, mode=mode).to(device)
-
-        self.data = dataset
-        self.num_epochs = num_epochs
-        self.batch_size = batch_size
-        self.lr = lr
-        self.n_filter = n_filter
-        self.mode = mode
-        self.best_loss = torch.tensor(float('inf'))
-        self.save_iter = save_iter
-        self.loss_function = loss_function
-        self.loss_params = loss_params
-        # split training and validation data
-        num_val = int(len(dataset) * val_split)
-        num_train = len(dataset) - num_val
-        self.dim = dataset.dim_out
-        train_data, val_data = random_split(dataset, [num_train, num_val])
-        self.train_loader = DataLoader(train_data, batch_size=self.batch_size, pin_memory=True, drop_last=True)
-        self.val_loader = DataLoader(val_data, batch_size=self.batch_size, pin_memory=True, drop_last=True)
-        if loss_function == 'BCEDice':
-            self.criterion = BCEDiceLoss(loss_params[0], loss_params[1])
-        elif loss_function == 'Tversky':
-            self.criterion = TverskyLoss(loss_params[0], loss_params[1])
-        elif loss_function == 'logcoshTversky':
-            self.criterion = logcoshTverskyLoss(loss_params[0], loss_params[1])
-        elif loss_function == 'weightedBCELoss':
-            self.criterion = weightedBCELoss(loss_params[0], loss_params[1])
-        else:
-            raise ValueError(f'Loss function "{loss_function}" not defined!')
-        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=self.lr)
-        self.scheduler = optim.lr_scheduler.ReduceLROnPlateau(self.optimizer, 'min', patience=4, factor=0.1)
-        self.save_dir = save_dir
-        os.makedirs(self.save_dir, exist_ok=True)
-        self.save_name = save_name
-
-        if load_weights is not None:
-            self.state = torch.load(load_weights)
-            self.model.load_state_dict(self.state['state_dict'])
-
-    def iterate(self, epoch, mode):
-        if mode == 'train':
-            print('\nStarting training epoch %s ...' % epoch)
-            for i, batch_i in enumerate(Bar(self.train_loader)):
-                x_i = batch_i['image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                prev_x_i = batch_i['prev_image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                y_i = batch_i['mask'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                # Forward pass: Compute predicted y by passing x to the model
-                y_pred, y_logits = self.model(x_i, prev_x_i)
-                # Compute loss
-                loss = self.criterion(y_logits, y_i)
-                # Zero gradients, perform a backward pass, and update the weights.
-                self.optimizer.zero_grad()
-                loss.backward()
-                self.optimizer.step()
-
-        elif mode == 'val':
-            loss_list = []
-            print('\nStarting validation epoch %s ...' % epoch)
-            with torch.no_grad():
-                for i, batch_i in enumerate(Bar(self.val_loader)):
-                    x_i = batch_i['image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                    prev_x_i = batch_i['prev_image'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                    y_i = batch_i['mask'].view(self.batch_size, 1, self.dim[0], self.dim[1]).to(device)
-                    # Forward pass: Compute predicted y by passing x to the model
-                    y_pred, y_logits = self.model(x_i, prev_x_i)
-                    # Compute loss
-                    loss = self.criterion(y_logits, y_i)
-                    loss_list.append(loss.detach())
-            val_loss = torch.stack(loss_list).mean()
-            return val_loss
-
-        torch.cuda.empty_cache()
-
-    def start(self, test_data_path=None, result_path=None, test_resize_dim=(512, 512)):
-        for epoch in range(self.num_epochs):
-            self.iterate(epoch, 'train')
-            self.state = {
-                'epoch': epoch,
-                'best_loss': self.best_loss,
-                'state_dict': self.model.state_dict(),
-                'optimizer': self.optimizer.state_dict(),
-                'lr': self.lr,
-                'loss': self.loss_function,
-                'loss_params': self.loss_params,
-                'n_filter': self.n_filter,
-                'mode': self.mode,
-                'augmentation': self.data.aug_factor,
-                'clip_threshold': self.data.clip_threshold,
-                'noise_amp': self.data.noise_amp,
-                'brightness_contrast': self.data.brightness_contrast,
-                'shiftscalerotate': self.data.shiftscalerotate,
-            }
-            with torch.no_grad():
-                val_loss = self.iterate(epoch, 'val')
-                self.scheduler.step(val_loss)
-            if val_loss < self.best_loss:
-                print(f'\nEpoch {epoch}: Validation loss improved from {round(self.best_loss.item(), 5)} to '
-                      f'{round(val_loss.item(), 5)} - saving model state')
-                self.state['best_loss'] = self.best_loss = val_loss
-                torch.save(self.state, self.save_dir + '/' + self.save_name)
-            else:
-                print(f'\nEpoch {epoch}: Validation loss did not improve from {round(self.best_loss.item(), 5)}')
-            if self.save_iter:
-                torch.save(self.state, self.save_dir + '/' + f'model_epoch_{epoch}.pth')
-
-            if test_data_path is not None:
-                os.makedirs(result_path, exist_ok=True)
-                files = glob.glob(test_data_path + '*.tif')
-                for i, file in enumerate(files):
-                    Predict(file, result_path + os.path.basename(file) + f'epoch_{epoch}.tif',
-                            self.save_dir + '/' + f'model_epoch_{epoch}.pth', resize_dim=test_resize_dim,
-                            invert=False)
+import glob
+import os
+
+import tifffile
+import torch.optim as optim
+from torch.utils.data import DataLoader, random_split
+from tqdm import tqdm
+
+from .losses import *
+from .predict import Predict
+from .unet import Unet
+from ..utils import init_weights, get_device
+
+# get device
+device = get_device()
+
+
+class Trainer:
+    def __init__(self, dataset, num_epochs, network=Unet, batch_size=4, lr=1e-3, in_channels=1, out_channels=1,
+                 channel_weights=None, n_filter=64, dilation=1, val_split=0.2, save_dir='./', save_name='model.pth',
+                 save_iter=False, load_weights=False, loss_function='BCEDice', loss_params=(0.5, 0.5)):
+        """
+        Class for training of neural network. Creates trainer object, training is started with .start().
+
+        Parameters
+        ----------
+        dataset
+            Training data, object of PyTorch Dataset class
+        num_epochs : int
+            Number of training epochs
+        network
+            Network class (Default Unet)
+        batch_size : int
+            Batch size for training
+        lr : float
+            Learning rate
+        in_channels : int
+            Number of input channels
+        out_channels : int
+            Number of output channels
+        channel_weights : list
+            List of loss weights for each channel
+        n_filter : int
+            Number of convolutional filters in first layer
+        val_split : float
+            Validation split
+        save_dir : str
+            Path of directory to save trained networks
+        save_name : str
+            Base name for saving trained networks
+        save_iter : bool
+            If True, network state is save after each epoch
+        load_weights : str, optional
+            If not None, network state is loaded before training
+        loss_function : str
+            Loss function ('BCEDice', 'Tversky' or 'logcoshTversky')
+        loss_params : Tuple[float, float]
+            Parameter of loss function, depends on chosen loss function
+        """
+        self.network = network
+        self.model = network(n_filter=n_filter, in_channels=in_channels, out_channels=out_channels,
+                             dilation=dilation).to(device)
+        self.model.apply(init_weights)
+        self.data = dataset
+        self.num_epochs = num_epochs
+        self.batch_size = batch_size
+        self.lr = lr
+        self.best_loss = torch.tensor(float('inf'))
+        self.save_iter = save_iter
+        self.loss_function = loss_function
+        self.loss_params = loss_params
+        self.n_filter = n_filter
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        if channel_weights is None:
+            self.channel_weights = torch.ones(out_channels)
+        else:
+            self.channel_weights = torch.tensor(channel_weights)
+
+        # split training and validation data
+        num_val = int(len(dataset) * val_split)
+        num_train = len(dataset) - num_val
+        self.dim = dataset.dim_out
+        train_data, val_data = random_split(dataset, [num_train, num_val])
+        self.train_loader = DataLoader(train_data, batch_size=self.batch_size, pin_memory=True, drop_last=True)
+        self.val_loader = DataLoader(val_data, batch_size=self.batch_size, pin_memory=True, drop_last=True)
+        if loss_function == 'BCEDice':
+            self.criterion = BCEDiceLoss(loss_params[0], loss_params[1])
+        elif loss_function == 'Tversky':
+            self.criterion = TverskyLoss(loss_params[0], loss_params[1])
+        elif loss_function == 'logcoshTversky':
+            self.criterion = logcoshTverskyLoss(loss_params[0], loss_params[1])
+        else:
+            raise ValueError(f'Loss "{loss_function}" not defined!')
+        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=self.lr)
+        self.scheduler = optim.lr_scheduler.ReduceLROnPlateau(self.optimizer, mode='min', patience=4, factor=0.1)
+        self.save_dir = save_dir
+        os.makedirs(self.save_dir, exist_ok=True)
+        self.save_name = save_name
+        self.params = {'optimizer': self.optimizer.state_dict(),
+                       'lr': self.lr,
+                       'loss_function': self.loss_function,
+                       'loss_params': self.loss_params,
+                       'n_filter': self.n_filter,
+                       'dilation': dilation, 'batch_size': self.batch_size,
+                       'augmentation': self.data.aug_factor,
+                       'clip_threshold': self.data.clip_threshold,
+                       'noise_amp': self.data.noise_amp,
+                       'brightness_contrast': self.data.brightness_contrast,
+                       'shiftscalerotate': self.data.shiftscalerotate,
+                       'in_channels': in_channels, 'out_channels': out_channels}
+        if load_weights:
+            self.state = torch.load(self.save_dir + '/' + self.save_name)
+            self.model.load_state_dict(self.state['state_dict'])
+
+    def __iterate(self, epoch, mode):
+        if mode == 'train':
+            print('\nStarting training epoch %s ...' % epoch)
+            for i, batch_i in tqdm(enumerate(self.train_loader), total=len(self.train_loader), unit='batch'):
+                x_i = batch_i['image'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1]).to(device)
+                y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[0]).to(device)
+                # Forward pass: Compute predicted y by passing x to the model
+                y_pred, y_logits = self.model(x_i)
+
+                # Compute loss
+                loss = sum([self.criterion(y_logits[ch], y_i[ch]) * self.channel_weights[j] for j, ch in
+                            enumerate(range(self.out_channels))]) / sum(self.channel_weights)
+
+                # Zero gradients, perform a backward pass, and update the weights.
+                self.optimizer.zero_grad()
+                loss.backward()
+                self.optimizer.step()
+
+        elif mode == 'val':
+            loss_list = []
+            print('\nStarting validation epoch %s ...' % epoch)
+            with torch.no_grad():
+                for i, batch_i in tqdm(enumerate(self.val_loader), total=len(self.val_loader), unit='batch'):
+                    x_i = batch_i['image'].view(self.batch_size, self.in_channels, self.dim[0], self.dim[1]).to(device)
+                    y_i = batch_i['mask'].view(self.batch_size, self.out_channels, self.dim[0], self.dim[1]).to(device)
+                    # Forward pass: Compute predicted y by passing x to the model
+                    y_pred, y_logits = self.model(x_i)
+                    # Compute loss
+                    loss = sum([self.criterion(y_logits[ch], y_i[ch]) * self.channel_weights[j] for j, ch in
+                                enumerate(range(self.out_channels))]) / sum(self.channel_weights)
+                loss_list.append(loss.detach())
+            val_loss = torch.stack(loss_list).mean()
+            return val_loss
+
+        torch.cuda.empty_cache()
+
+    def start(self, test_data_path=None, result_path=None, test_resize_dim=(512, 512)):
+        """
+        Start network training. Optional: predict small test sample after each epoch.
+
+        Parameters
+        ----------
+        test_data_path : str
+            Path of folder with test tif files
+        result_path : str
+            Path for saving prediction results of test data
+        test_resize_dim: tuple
+            Resize dimensions for prediction of test movies
+        """
+        for epoch in range(self.num_epochs):
+            self.__iterate(epoch, 'train')
+            self.state = {
+                'epoch': epoch,
+                'best_loss': self.best_loss,
+                'state_dict': self.model.state_dict()}
+            self.state.update(self.params)
+            with torch.no_grad():
+                val_loss = self.__iterate(epoch, 'val')
+                self.scheduler.step(val_loss)
+            if val_loss < self.best_loss:
+                print('\nValidation loss improved from %s to %s - saving model state' % (
+                    round(self.best_loss.item(), 5), round(val_loss.item(), 5)))
+                self.state['best_loss'] = self.best_loss = val_loss
+                torch.save(self.state, self.save_dir + '/' + self.save_name)
+            if self.save_iter:
+                torch.save(self.state, self.save_dir + '/' + f'model_epoch_{epoch}.pth')
+
+            if test_data_path is not None:
+                print('\nPredicting test data...')
+                files = glob.glob(test_data_path + '*.tif')
+                for i, file in enumerate(files):
+                    img = tifffile.imread(file)
+                    Predict(img, result_path + os.path.basename(file) + f'epoch_{epoch}.tif',
+                            self.save_dir + '/' + f'model_epoch_{epoch}.pth', self.network, resize_dim=test_resize_dim,
+                            invert=False, progress_bar=False)
+
```

### Comparing `bio-image-unet-0.6.1/biu/unet/baby_unet.py` & `bio_image_unet-1.0.0a1/biu/unet/baby_unet.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import torch
-from torch import nn
-
-
-class BabyUnet(nn.Module):
-    def __init__(self, n_filter=4):
-        """
-        Neural network for semantic image segmentation U-Net (PyTorch), with only three max-pooling layers
-        Reference:  Falk, T. et al. U-Net: deep learning for cell counting, detection, and morphometry. Nat Methods 16,
-        67–70 (2019).
-
-        Parameters
-        ----------
-        n_filter : int
-            Number of convolutional filters (commonly 2**n)
-        """
-        super().__init__()
-        # encode
-        self.encode1 = self.conv(1, n_filter)
-        self.encode2 = self.conv(n_filter, n_filter)
-        self.maxpool1 = nn.MaxPool2d(kernel_size=2, stride=2)
-        self.encode3 = self.conv(n_filter, 2 * n_filter)
-        self.encode4 = self.conv(2 * n_filter, 2 * n_filter)
-        self.maxpool2 = nn.MaxPool2d(kernel_size=2, stride=2)
-        self.encode5 = self.conv(2 * n_filter, 4 * n_filter)
-        self.encode6 = self.conv(4 * n_filter, 4 * n_filter)
-        self.maxpool3 = nn.MaxPool2d(kernel_size=2, stride=2)
-
-        # middle
-        self.middle_conv1 = self.conv(4 * n_filter, 8 * n_filter)
-        self.middle_conv2 = self.conv(8 * n_filter, 8 * n_filter, dropout=0.5)
-
-        # decode
-        self.up1 = nn.ConvTranspose2d(8 * n_filter, 4 * n_filter, kernel_size=2, stride=2)
-        self.decode1 = self.conv(8 * n_filter, 4 * n_filter)
-        self.decode2 = self.conv(4 * n_filter, 4 * n_filter)
-        self.up2 = nn.ConvTranspose2d(4 * n_filter, 2 * n_filter, kernel_size=2, stride=2)
-        self.decode3 = self.conv(4 * n_filter, 2 * n_filter)
-        self.decode4 = self.conv(2 * n_filter, 2 * n_filter)
-        self.up3 = nn.ConvTranspose2d(2 * n_filter, 1 * n_filter, kernel_size=2, stride=2)
-        self.decode5 = self.conv(2 * n_filter, 1 * n_filter)
-        self.decode6 = self.conv(1 * n_filter, 1 * n_filter)
-        self.decode7 = self.conv(1 * n_filter, 1)
-        self.final = nn.Sequential(
-            nn.Conv2d(1, 1, kernel_size=1, padding=0),
-        )
-
-    def conv(self, in_channels, out_channels, kernel_size=3, dropout=0.0):
-        block = nn.Sequential(
-            nn.Conv2d(kernel_size=kernel_size, in_channels=in_channels, out_channels=out_channels, padding=1),
-            nn.BatchNorm2d(out_channels),
-            nn.ReLU(),
-            nn.Dropout2d(dropout)
-        )
-        return block
-
-    def concat(self, x1, x2):
-        if x1.shape == x2.shape:
-            return torch.cat((x1, x2), 1)
-        else:
-            print(x1.shape, x2.shape)
-            raise ValueError('concatenation failed: wrong dimensions')
-
-    def forward(self, x):
-        e1 = self.encode1(x)
-        e2 = self.encode2(e1)
-        m1 = self.maxpool1(e2)
-        e3 = self.encode3(m1)
-        e4 = self.encode4(e3)
-        m2 = self.maxpool2(e4)
-        e5 = self.encode5(m2)
-        e6 = self.encode6(e5)
-        m3 = self.maxpool3(e6)
-
-        mid1 = self.middle_conv1(m3)
-        mid2 = self.middle_conv2(mid1)
-
-        u1 = self.up1(mid2)
-        c1 = self.concat(u1, e5)
-        d1 = self.decode1(c1)
-        d2 = self.decode2(d1)
-        u2 = self.up2(d2)
-        c2 = self.concat(u2, e3)
-        d3 = self.decode3(c2)
-        d4 = self.decode4(d3)
-        u3 = self.up3(d4)
-        c3 = self.concat(u3, e1)
-        d5 = self.decode5(c3)
-        d6 = self.decode6(d5)
-        d9 = self.decode7(d6)
-        logits = self.final(d9)
-        return torch.sigmoid(logits), logits
+import torch
+from torch import nn
+
+
+class BabyUnet(nn.Module):
+    def __init__(self, n_filter=4):
+        """
+        Neural network for semantic image segmentation U-Net (PyTorch), with only three max-pooling layers
+        Reference:  Falk, T. et al. U-Net: deep learning for cell counting, detection, and morphometry. Nat Methods 16,
+        67–70 (2019).
+
+        Parameters
+        ----------
+        n_filter : int
+            Number of convolutional filters (commonly 2**n)
+        """
+        super().__init__()
+        # encode
+        self.encode1 = self.conv(1, n_filter)
+        self.encode2 = self.conv(n_filter, n_filter)
+        self.maxpool1 = nn.MaxPool2d(kernel_size=2, stride=2)
+        self.encode3 = self.conv(n_filter, 2 * n_filter)
+        self.encode4 = self.conv(2 * n_filter, 2 * n_filter)
+        self.maxpool2 = nn.MaxPool2d(kernel_size=2, stride=2)
+        self.encode5 = self.conv(2 * n_filter, 4 * n_filter)
+        self.encode6 = self.conv(4 * n_filter, 4 * n_filter)
+        self.maxpool3 = nn.MaxPool2d(kernel_size=2, stride=2)
+
+        # middle
+        self.middle_conv1 = self.conv(4 * n_filter, 8 * n_filter)
+        self.middle_conv2 = self.conv(8 * n_filter, 8 * n_filter, dropout=0.5)
+
+        # decode
+        self.up1 = nn.ConvTranspose2d(8 * n_filter, 4 * n_filter, kernel_size=2, stride=2)
+        self.decode1 = self.conv(8 * n_filter, 4 * n_filter)
+        self.decode2 = self.conv(4 * n_filter, 4 * n_filter)
+        self.up2 = nn.ConvTranspose2d(4 * n_filter, 2 * n_filter, kernel_size=2, stride=2)
+        self.decode3 = self.conv(4 * n_filter, 2 * n_filter)
+        self.decode4 = self.conv(2 * n_filter, 2 * n_filter)
+        self.up3 = nn.ConvTranspose2d(2 * n_filter, 1 * n_filter, kernel_size=2, stride=2)
+        self.decode5 = self.conv(2 * n_filter, 1 * n_filter)
+        self.decode6 = self.conv(1 * n_filter, 1 * n_filter)
+        self.decode7 = self.conv(1 * n_filter, 1)
+        self.final = nn.Sequential(
+            nn.Conv2d(1, 1, kernel_size=1, padding=0),
+        )
+
+    def conv(self, in_channels, out_channels, kernel_size=3, dropout=0.0):
+        block = nn.Sequential(
+            nn.Conv2d(kernel_size=kernel_size, in_channels=in_channels, out_channels=out_channels, padding=1),
+            nn.BatchNorm2d(out_channels),
+            nn.ReLU(),
+            nn.Dropout2d(dropout)
+        )
+        return block
+
+    def concat(self, x1, x2):
+        if x1.shape == x2.shape:
+            return torch.cat((x1, x2), 1)
+        else:
+            print(x1.shape, x2.shape)
+            raise ValueError('concatenation failed: wrong dimensions')
+
+    def forward(self, x):
+        e1 = self.encode1(x)
+        e2 = self.encode2(e1)
+        m1 = self.maxpool1(e2)
+        e3 = self.encode3(m1)
+        e4 = self.encode4(e3)
+        m2 = self.maxpool2(e4)
+        e5 = self.encode5(m2)
+        e6 = self.encode6(e5)
+        m3 = self.maxpool3(e6)
+
+        mid1 = self.middle_conv1(m3)
+        mid2 = self.middle_conv2(mid1)
+
+        u1 = self.up1(mid2)
+        c1 = self.concat(u1, e5)
+        d1 = self.decode1(c1)
+        d2 = self.decode2(d1)
+        u2 = self.up2(d2)
+        c2 = self.concat(u2, e3)
+        d3 = self.decode3(c2)
+        d4 = self.decode4(d3)
+        u3 = self.up3(d4)
+        c3 = self.concat(u3, e1)
+        d5 = self.decode5(c3)
+        d6 = self.decode6(d5)
+        d9 = self.decode7(d6)
+        logits = self.final(d9)
+        return torch.sigmoid(logits), logits
```

### Comparing `bio-image-unet-0.6.1/biu/unet/losses.py` & `bio_image_unet-1.0.0a1/biu/unet/losses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,92 @@
-import torch
-from torch import nn as nn, flatten
-
-
-# adapted from https://github.com/achaiah/pywick/blob/master/pywick/losses.py
-class BCEDiceLoss(nn.Module):
-    def __init__(self, alpha, beta):
-        super(BCEDiceLoss, self).__init__()
-        self.bce = BCELoss2d()
-        self.dice = SoftDiceLoss()
-        self.alpha = alpha
-        self.beta = beta
-
-    def forward(self, logits, targets):
-        return self.alpha * self.bce(logits, targets) + self.beta * self.dice(logits, targets)
-
-
-class BCELoss2d(nn.Module):
-    def __init__(self, weight=None, size_average=True, **kwargs):
-        super(BCELoss2d, self).__init__()
-        self.bce_loss = nn.BCELoss(weight, size_average)
-
-    def forward(self, logits, targets):
-        probs = torch.sigmoid(logits)
-        probs_flat = probs.view(-1)
-        targets_flat = targets.view(-1)
-        return self.bce_loss(probs_flat, targets_flat)
-
-
-class SoftDiceLoss(nn.Module):
-    def __init__(self, smooth=1.0):
-        super(SoftDiceLoss, self).__init__()
-        self.smooth = smooth
-
-    def forward(self, logits, targets):
-        num = targets.size(0)
-        probs = torch.sigmoid(logits)
-        m1 = probs.view(num, -1)
-        m2 = targets.view(num, -1)
-        intersection = (m1 * m2)
-
-        score = 2. * (intersection.sum(1) + self.smooth) / (m1.sum(1) + m2.sum(1) + self.smooth)
-        score = 1 - score.sum() / num
-        return score
-
-
-class logcoshDiceLoss(nn.Module):
-    def __init__(self):
-        super(logcoshDiceLoss, self).__init__()
-        self.dice = SoftDiceLoss()
-
-    def forward(self, logits, targets):
-        x = self.dice(logits, targets)
-        return torch.log((torch.exp(x) + torch.exp(-x)) / 2)
-
-
-class TverskyLoss(nn.Module):
-    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
-        super(TverskyLoss, self).__init__()
-        self.alpha = alpha
-        self.beta = beta
-        self.smooth = smooth
-
-    def forward(self, inputs, targets):
-        inputs = torch.sigmoid(inputs)
-        inputs = inputs.view(-1)
-        targets = targets.view(-1)
-
-        # True Positives, False Positives & False Negatives
-        TP = (inputs * targets).sum()
-        FP = ((1 - targets) * inputs).sum()
-        FN = (targets * (1 - inputs)).sum()
-
-        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
-
-        return 1 - Tversky
-
-
-class logcoshTverskyLoss(nn.Module):
-    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
-        super(logcoshTverskyLoss, self).__init__()
-        self.alpha = alpha
-        self.beta = beta
-        self.smooth = smooth
-
-    def forward(self, inputs, targets):
-        inputs = torch.sigmoid(inputs)
-        inputs = inputs.view(-1)
-        targets = targets.view(-1)
-
-        # True Positives, False Positives & False Negatives
-        TP = (inputs * targets).sum()
-        FP = ((1 - targets) * inputs).sum()
-        FN = (targets * (1 - inputs)).sum()
-
-        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
-
-        return torch.log(torch.cosh(1 - Tversky))
+import torch
+from torch import nn as nn
+
+
+class BCELoss2d(nn.Module):
+    def __init__(self, weight=None, size_average=True):
+        super(BCELoss2d, self).__init__()
+        self.bce_loss = nn.BCEWithLogitsLoss(weight=weight, reduction='mean' if size_average else 'sum')
+
+    def forward(self, logits, targets):
+        return self.bce_loss(logits, targets)
+
+
+class SoftDiceLoss(nn.Module):
+    def __init__(self, smooth=1.0):
+        super(SoftDiceLoss, self).__init__()
+        self.smooth = smooth
+
+    def forward(self, logits, targets):
+        probs = torch.sigmoid(logits)
+        num = targets.size(0)
+        m1 = probs.view(num, -1)
+        m2 = targets.view(num, -1)
+        intersection = (m1 * m2).sum(1)
+        score = 2. * (intersection + self.smooth) / (m1.sum(1) + m2.sum(1) + self.smooth)
+        return 1 - score.mean()
+
+
+class BCEDiceLoss(nn.Module):
+    def __init__(self, alpha, beta):
+        super(BCEDiceLoss, self).__init__()
+        self.bce = BCELoss2d()
+        self.dice = SoftDiceLoss()
+        self.alpha = alpha
+        self.beta = beta
+
+    def forward(self, logits, targets):
+        return self.alpha * self.bce(logits, targets) + self.beta * self.dice(logits, targets)
+
+
+class logcoshDiceLoss(nn.Module):
+    def __init__(self):
+        super(logcoshDiceLoss, self).__init__()
+        self.dice = SoftDiceLoss()
+
+    def forward(self, logits, targets):
+        x = self.dice(logits, targets)
+        return torch.log((torch.exp(x) + torch.exp(-x)) / 2)
+
+
+class TverskyLoss(nn.Module):
+    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
+        super(TverskyLoss, self).__init__()
+        self.alpha = alpha
+        self.beta = beta
+        self.smooth = smooth
+
+    def forward(self, inputs, targets):
+        inputs = torch.sigmoid(inputs)
+        inputs = inputs.view(-1)
+        targets = targets.view(-1)
+
+        # True Positives, False Positives & False Negatives
+        TP = (inputs * targets).sum()
+        FP = ((1 - targets) * inputs).sum()
+        FN = (targets * (1 - inputs)).sum()
+
+        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
+
+        return 1 - Tversky
+
+
+class logcoshTverskyLoss(nn.Module):
+    def __init__(self, alpha=0.5, beta=0.5, smooth=1):
+        super(logcoshTverskyLoss, self).__init__()
+        self.alpha = alpha
+        self.beta = beta
+        self.smooth = smooth
+
+    def forward(self, inputs, targets):
+        inputs = torch.sigmoid(inputs)
+        inputs = inputs.view(-1)
+        targets = targets.view(-1)
+
+        # True Positives, False Positives & False Negatives
+        TP = (inputs * targets).sum()
+        FP = ((1 - targets) * inputs).sum()
+        FN = (targets * (1 - inputs)).sum()
+
+        Tversky = (TP + self.smooth) / (TP + self.alpha * FP + self.beta * FN + self.smooth)
+
+        return torch.log(torch.cosh(1 - Tversky))
```

### Comparing `bio-image-unet-0.6.1/biu/unet/predict.py` & `bio_image_unet-1.0.0a1/biu/unet/predict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,238 +1,200 @@
-import os
-import re
-
-import numpy as np
-import tifffile
-import torch
-
-from biu.progress import ProgressNotifier
-from .unet import Unet
-from .utils import save_as_tif
-
-# select device
-if torch.has_cuda:
-    device = torch.device('cuda:0')
-elif hasattr(torch, 'has_mps'):  # only for apple m1/m2/...
-    if torch.has_mps:
-        device = torch.device('mps')
-    else:
-        device = torch.device('cpu')
-else:
-    device = torch.device('cpu')
-
-
-class Predict:
-    """Class for prediction of movies and images with U-Net"""
-    def __init__(self, tif_file, result_name, model_params, network=Unet, resize_dim=(512, 512),
-                 invert=False, frame_lim=None, normalization_mode='single', clip_threshold=(0., 99.8), add_tile=0,
-                 normalize_result=False, progress_bar=True,
-                 progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
-        """
-        Prediction of tif files with standard 2D U-Net
-
-        1) Loading file and preprocess (normalization)
-        2) Resizing of images into patches with resize_dim
-        3) Prediction with U-Net
-        4) Stitching of predicted patches and averaging of overlapping regions
-
-        Parameters
-        ----------
-        tif_file : str
-            path of tif file
-        result_name : str
-            path for result
-        model_params : str
-            path of u-net parameters (.pth file)
-        network
-            Network class
-        resize_dim
-            Image dimensions for resizing for prediction
-        invert : bool
-            Invert greyscale of image(s) before prediction
-        frame_lim : Tuple[int, int], optional
-            If not None, predict only interval
-        normalization_mode : str
-            Mode for intensity normalization for 3D stacks prior to prediction ('single': each image individually,
-            'all': based on histogram of full stack, 'first': based on histogram of first image in stack)
-        clip_threshold : Tuple[float, float]
-            Clip threshold for image intensity before prediction
-        add_tile : int, optional
-            Add additional tiles for splitting large images to increase overlap
-        normalize_result : bool
-            If true, results are normalized to [0, 255]
-        progress_notifier:
-            Wrapper to show tqdm progress notifier in gui
-        """
-        self.tif_file = tif_file
-        self.resize_dim = resize_dim
-        self.add_tile = add_tile
-        self.normalize_result = normalize_result
-        self.invert = invert
-        self.normalization_mode = normalization_mode
-        self.clip_threshold = clip_threshold
-        self.frame_lim = frame_lim
-        self.result_name = result_name
-        self.progress_bar = progress_bar
-
-        # read, preprocess and split data
-        imgs = self.__read_data()
-        imgs = self.__preprocess(imgs)
-        patches = self.__split(imgs)
-        del imgs
-
-        # load model and predict data
-        self.model_params = torch.load(model_params, map_location=device)
-        self.model = network(n_filter=self.model_params['n_filter']).to(device)
-        self.model.load_state_dict(self.model_params['state_dict'])
-        self.model.eval()
-        result_patches = self.__predict(patches, progress_notifier)
-        del patches
-        # stitch patches (mean of overlapped regions)
-        imgs_result = self.__stitch(result_patches)
-        del result_patches
-
-        # save as .tif file
-        save_as_tif(imgs_result, self.result_name, normalize=normalize_result)
-
-    def __read_data(self):
-        imgs = tifffile.imread(self.tif_file)
-        if self.frame_lim is not None:
-            imgs = imgs[self.frame_lim[0]:self.frame_lim[1]]
-        self.imgs_shape = imgs.shape
-        if len(self.imgs_shape) == 2:  # if single image
-            self.imgs_shape = [1, self.imgs_shape[0], self.imgs_shape[1]]
-        return imgs
-
-    def __preprocess(self, imgs):
-        if len(imgs.shape) == 3:
-            if self.normalization_mode == 'single':
-                for i, img in enumerate(imgs):
-                    img = np.clip(img, a_min=np.nanpercentile(img, self.clip_threshold[0]),
-                                  a_max=np.percentile(img, self.clip_threshold[1]))
-                    img = img - np.min(img)
-                    img = img / np.max(img) * 255
-                    if self.invert:
-                        img = 255 - img
-                    imgs[i] = img
-            elif self.normalization_mode == 'first':
-                clip_threshold = (np.nanpercentile(imgs[0], self.clip_threshold[0]),
-                                  np.percentile(imgs[0], self.clip_threshold[1]))
-                imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
-                imgs = imgs - np.min(imgs)
-                imgs = imgs / np.max(imgs) * 255
-                if self.invert:
-                    imgs = 255 - imgs
-            elif self.normalization_mode == 'all':
-                clip_threshold = (np.nanpercentile(imgs, self.clip_threshold[0]),
-                                  np.percentile(imgs, self.clip_threshold[1]))
-                imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
-                imgs = imgs - np.min(imgs)
-                imgs = imgs / np.max(imgs) * 255
-                if self.invert:
-                    imgs = 255 - imgs
-            else:
-                raise ValueError(f'normalization_mode {self.normalization_mode} not valid!')
-        if len(imgs.shape) == 2:
-            imgs = np.clip(imgs, a_min=np.nanpercentile(imgs, self.clip_threshold[0]),
-                           a_max=np.percentile(imgs, self.clip_threshold[1]))
-            imgs = imgs - np.min(imgs)
-            imgs = imgs / np.max(imgs) * 255
-            if self.invert:
-                imgs = 255 - imgs
-        imgs = imgs.astype('uint8')
-        return imgs
-
-    def __split(self, imgs):
-        # number of patches in x and y
-        self.N_x = int(np.ceil(self.imgs_shape[1] / self.resize_dim[0])) + self.add_tile
-        self.N_y = int(np.ceil(self.imgs_shape[2] / self.resize_dim[1])) + self.add_tile
-        self.N_per_img = self.N_x * self.N_y
-        self.N = self.N_x * self.N_y * self.imgs_shape[0]  # total number of patches
-        print('Resizing into each %s patches ...' % self.N_per_img)
-
-        # define array for prediction
-        patches = np.zeros((self.N, 1, self.resize_dim[0], self.resize_dim[1]), dtype='uint8')
-
-        # zero padding of image if imgs_shape < resize_dim
-        if self.imgs_shape[0] > 1:
-            if self.imgs_shape[1] < self.resize_dim[0]:  # for x
-                imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)),
-                              'constant')
-            if self.imgs_shape[2] < self.resize_dim[1]:  # for y
-                imgs = np.pad(imgs, ((0, 0), (0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])),
-                              'constant')
-        elif self.imgs_shape[0] == 1:
-            if self.imgs_shape[1] < self.resize_dim[0]:  # for x
-                imgs = np.pad(imgs, ((0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)), 'reflect')
-            if self.imgs_shape[2] < self.resize_dim[1]:  # for y
-                imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])), 'reflect')
-
-        # starting indices of patches
-        self.X_start = np.linspace(0, self.imgs_shape[1] - self.resize_dim[0], self.N_x).astype('uint16')
-        self.Y_start = np.linspace(0, self.imgs_shape[2] - self.resize_dim[1], self.N_y).astype('uint16')
-
-        # split in resize_dim
-        n = 0
-        if self.imgs_shape[0] > 1:
-            for i, img in enumerate(imgs):
-                for j in range(self.N_x):
-                    for k in range(self.N_y):
-                        patches[n, 0, :, :] = img[self.X_start[j]:self.X_start[j] + self.resize_dim[0],
-                                              self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
-                        n += 1
-        elif self.imgs_shape[0] == 1:
-            for j in range(self.N_x):
-                for k in range(self.N_y):
-                    patches[n, 0, :, :] = imgs[self.X_start[j]:self.X_start[j] + self.resize_dim[0],
-                                          self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
-                    n += 1
-        return patches
-
-    def __predict(self, patches, progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
-        result_patches = np.zeros(patches.shape, dtype='uint8')
-        print('Predicting data ...')
-        with torch.no_grad():
-            for i, patch_i in enumerate(progress_notifier.iterator(patches)):
-                patch_i = torch.from_numpy(patch_i.astype('float32') / 255).to(device).view((1, 1, self.resize_dim[0],
-                                                                                             self.resize_dim[1]))
-                res_i, logits_i = self.model(patch_i)
-                res_i = res_i.view((1, self.resize_dim[0], self.resize_dim[1])).cpu().numpy() * 255
-                result_patches[i] = res_i.astype('uint8')
-                del patch_i, res_i
-        return result_patches
-
-    def __stitch(self, result_patches):
-        print('Stitching patches back together ...')
-        # create array
-        imgs_result = np.zeros((self.imgs_shape[0], np.max((self.resize_dim[0], self.imgs_shape[1])),
-                                np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype='uint8')
-        for i in range(self.imgs_shape[0]):
-            if self.imgs_shape[0] > 1:  # if stack
-                stack_result_i = np.zeros((self.N_per_img, np.max((self.resize_dim[0], self.imgs_shape[1])),
-                                           np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype='uint8') * np.nan
-            elif self.imgs_shape[0] == 1:  # if only one image
-                stack_result_i = np.zeros((self.N_per_img, np.max((self.resize_dim[0], self.imgs_shape[1])),
-                                           np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype='uint8') * np.nan
-            else:
-                raise ValueError('Data structure not known!')
-            n = 0
-            for j in range(self.N_x):
-                for k in range(self.N_y):
-                    stack_result_i[n, self.X_start[j]:self.X_start[j] + self.resize_dim[0],
-                    self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]] = result_patches[i * self.N_per_img + n, 0, :,
-                                                                            :]
-                    n += 1
-
-            # average overlapping regions
-            if self.imgs_shape[0] > 1:  # if stack
-                imgs_result[i] = np.nanmean(stack_result_i, axis=0)
-            elif self.imgs_shape[0] == 1:  # if only one image
-                imgs_result = np.nanmean(stack_result_i, axis=0)
-
-        # change to input size (if zero padding)
-        if self.imgs_shape[0] > 1:  # if stack
-            imgs_result = imgs_result[:, :self.imgs_shape[1], :self.imgs_shape[2]]
-        elif self.imgs_shape[0] == 1:  # if only one image
-            imgs_result = imgs_result[:self.imgs_shape[1], :self.imgs_shape[2]]
-
-        return imgs_result
+import numpy as np
+import tifffile
+import torch
+
+from ..progress import ProgressNotifier
+from .unet import Unet
+from ..utils import save_as_tif, get_device
+
+# select device
+device = get_device()
+
+
+class Predict:
+    """Class for prediction of movies and images with U-Net"""
+
+    def __init__(self, imgs, result_name, model_params, network=Unet, resize_dim=(512, 512),
+                 invert=False, normalization_mode='single', clip_threshold=(0., 99.8), add_tile=0,
+                 normalize_result=False, progress_bar=True,
+                 progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
+        """
+        Prediction of tif files with standard 2D U-Net
+
+        1) Loading file and preprocess (normalization)
+        2) Resizing of images into patches with resize_dim
+        3) Prediction with U-Net
+        4) Stitching of predicted patches and averaging of overlapping regions
+
+        Parameters
+        ----------
+        imgs : ndarray, string
+            images to predict, if string, attempt to load from tif file
+        result_name : str
+            path for result
+        model_params : str
+            path of u-net parameters (.pth file)
+        network
+            Network class
+        resize_dim
+            Image dimensions for resizing for prediction
+        invert : bool
+            Invert greyscale of image(s) before prediction
+        normalization_mode : str
+            Mode for intensity normalization for 3D stacks prior to prediction ('single': each image individually,
+            'all': based on histogram of full stack, 'first': based on histogram of first image in stack)
+        clip_threshold : Tuple[float, float]
+            Clip threshold for image intensity before prediction
+        add_tile : int, optional
+            Add additional tiles for splitting large images to increase overlap
+        normalize_result : bool
+            If true, results are normalized to [0, 255]
+        progress_notifier:
+            Wrapper to show tqdm progress notifier in gui
+        """
+        if isinstance(imgs, str):
+            imgs = tifffile.imread(imgs)
+
+        self.resize_dim = resize_dim
+        self.add_tile = add_tile
+        self.normalize_result = normalize_result
+        self.invert = invert
+        self.normalization_mode = normalization_mode
+        self.clip_threshold = clip_threshold
+        self.result_name = result_name
+        self.progress_bar = progress_bar
+
+        # read, preprocess and split data
+        imgs = self.__reshape_data(imgs)
+        imgs = self.__preprocess(imgs)
+        patches = self.__split(imgs)
+        del imgs
+
+        # load model and predict data
+        self.model_params = torch.load(model_params, map_location=device)
+        self.model = network(n_filter=self.model_params['n_filter'], in_channels=self.model_params['in_channels'],
+                             out_channels=self.model_params['out_channels']).to(device)
+        self.model.load_state_dict(self.model_params['state_dict'])
+        self.model.eval()
+        result_patches = self.__predict(patches, progress_notifier)
+        del patches
+        # stitch patches (mean of overlapped regions)
+        imgs_result = self.__stitch(result_patches)
+        del result_patches
+
+        # save as .tif file
+        save_as_tif(imgs_result, self.result_name, normalize=normalize_result)
+
+    def __reshape_data(self, imgs):
+        self.imgs_shape = imgs.shape
+        if len(self.imgs_shape) == 2:  # if single image
+            imgs = np.expand_dims(imgs, axis=0)
+            self.imgs_shape = imgs.shape
+        return imgs
+
+    def __preprocess(self, imgs):
+        if self.normalization_mode == 'single':
+            for i, img in enumerate(imgs):
+                img = np.clip(img, a_min=np.nanpercentile(img, self.clip_threshold[0]),
+                              a_max=np.percentile(img, self.clip_threshold[1]))
+                img = img - np.min(img)
+                img = img / np.max(img) * 255
+                if self.invert:
+                    img = 255 - img
+                imgs[i] = img
+        elif self.normalization_mode == 'first':
+            clip_threshold = (np.nanpercentile(imgs[0], self.clip_threshold[0]),
+                              np.percentile(imgs[0], self.clip_threshold[1]))
+            imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
+            imgs = imgs - np.min(imgs)
+            imgs = imgs / np.max(imgs) * 255
+            if self.invert:
+                imgs = 255 - imgs
+        elif self.normalization_mode == 'all':
+            clip_threshold = (np.nanpercentile(imgs, self.clip_threshold[0]),
+                              np.percentile(imgs, self.clip_threshold[1]))
+            imgs = np.clip(imgs, clip_threshold[0], clip_threshold[1])
+            imgs = imgs - np.min(imgs)
+            imgs = imgs / np.max(imgs) * 255
+            if self.invert:
+                imgs = 255 - imgs
+        else:
+            raise ValueError(f'normalization_mode {self.normalization_mode} not valid!')
+        return imgs
+
+    def __split(self, imgs):
+        # number of patches in x and y
+        self.N_x = int(np.ceil(self.imgs_shape[1] / self.resize_dim[0])) + self.add_tile
+        self.N_y = int(np.ceil(self.imgs_shape[2] / self.resize_dim[1])) + self.add_tile
+        self.N_per_img = self.N_x * self.N_y
+        self.N = self.N_x * self.N_y * self.imgs_shape[0]  # total number of patches
+
+        # define array for prediction
+        patches = np.zeros((self.N, 1, self.resize_dim[0], self.resize_dim[1]), dtype='uint8')
+
+        # zero padding of image if imgs_shape < resize_dim
+        if self.resize_dim[0] > self.imgs_shape[1]:  # for x
+            imgs = np.pad(imgs, ((0, 0), (0, self.resize_dim[0] - self.imgs_shape[1]), (0, 0)),
+                          'reflect')
+        if self.resize_dim[1] > self.imgs_shape[2]:  # for y
+            imgs = np.pad(imgs, ((0, 0), (0, 0), (0, self.resize_dim[1] - self.imgs_shape[2])),
+                          'reflect')
+
+        # starting indices of patches
+        self.X_start = np.linspace(0, self.imgs_shape[1] - self.resize_dim[0], self.N_x).astype('uint16')
+        self.Y_start = np.linspace(0, self.imgs_shape[2] - self.resize_dim[1], self.N_y).astype('uint16')
+
+        # split in resize_dim
+        n = 0
+        for i, img in enumerate(imgs):
+            for j in range(self.N_x):
+                for k in range(self.N_y):
+                    patches[n, 0, :, :] = img[self.X_start[j]:self.X_start[j] + self.resize_dim[0],
+                                              self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]]
+                    n += 1
+        return patches
+
+    def __predict(self, patches, progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
+        result_patches = np.zeros((patches.shape[0], self.model_params['out_channels'], *patches.shape[2:]),
+                                  dtype='uint8')
+        print('Predicting data ...') if self.progress_bar else None
+        with torch.no_grad():
+            _progress_notifier = enumerate(progress_notifier.iterator(patches)) if self.progress_bar else enumerate(
+                patches)
+            for i, patch_i in _progress_notifier:
+                patch_i = torch.from_numpy(patch_i.astype('float32') / 255).to(device).view((1,
+                                                                                             self.model_params[
+                                                                                                 'in_channels'],
+                                                                                             self.resize_dim[0],
+                                                                                             self.resize_dim[1]))
+                res_i, logits_i = self.model(patch_i)
+                res_i = res_i.view(
+                    (self.model_params['out_channels'], self.resize_dim[0], self.resize_dim[1])).cpu().numpy()
+                result_patches[i] = (res_i * 255).astype('uint8')
+                del patch_i, res_i
+        return result_patches
+
+    def __stitch(self, result_patches):
+        # create array
+        imgs_result = np.zeros(
+            (self.imgs_shape[0], self.model_params['out_channels'], np.max((self.resize_dim[0], self.imgs_shape[1])),
+             np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype='uint8')
+        for i in range(self.imgs_shape[0]):
+
+            stack_result_i = np.zeros((self.N_per_img, self.model_params['out_channels'],
+                                       np.max((self.resize_dim[0], self.imgs_shape[1])),
+                                       np.max((self.resize_dim[1], self.imgs_shape[2]))), dtype='uint8') * np.nan
+
+            n = 0
+            for j in range(self.N_x):
+                for k in range(self.N_y):
+                    stack_result_i[n, :, self.X_start[j]:self.X_start[j] + self.resize_dim[0],
+                    self.Y_start[k]:self.Y_start[k] + self.resize_dim[1]] = result_patches[i * self.N_per_img + n]
+                    n += 1
+
+            # average overlapping regions
+            imgs_result[i] = np.nanmean(stack_result_i, axis=0)
+
+        # change to input size (if zero padding)
+        imgs_result = imgs_result[:, :, :self.imgs_shape[1], :self.imgs_shape[2]]
+
+        return np.squeeze(imgs_result)
```

### Comparing `bio-image-unet-0.6.1/biu/unet/unet.py` & `bio_image_unet-1.0.0a1/biu/unet/unet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,103 @@
-import torch
-from torch import nn
-
-
-class Unet(nn.Module):
-    def __init__(self, n_filter=32):
-        """
-        Neural network for semantic image segmentation U-Net (PyTorch),
-        Reference:  Falk, T. et al. U-Net: deep learning for cell counting, detection, and morphometry. Nat Methods 16,
-        67–70 (2019).
-
-        Parameters
-        ----------
-        n_filter : int
-            Number of convolutional filters (commonly 16, 32, or 64)
-        """
-        super().__init__()
-        # encode
-        self.encode1 = self.conv(1, n_filter)
-        self.encode2 = self.conv(n_filter, n_filter)
-        self.maxpool1 = nn.MaxPool2d(kernel_size=2, stride=2)
-        self.encode3 = self.conv(n_filter, 2 * n_filter)
-        self.encode4 = self.conv(2 * n_filter, 2 * n_filter)
-        self.maxpool2 = nn.MaxPool2d(kernel_size=2, stride=2)
-        self.encode5 = self.conv(2 * n_filter, 4 * n_filter)
-        self.encode6 = self.conv(4 * n_filter, 4 * n_filter)
-        self.maxpool3 = nn.MaxPool2d(kernel_size=2, stride=2)
-        self.encode7 = self.conv(4 * n_filter, 8 * n_filter)
-        self.encode8 = self.conv(8 * n_filter, 8 * n_filter)
-        self.maxpool4 = nn.MaxPool2d(kernel_size=2, stride=2)
-
-        # middle
-        self.middle_conv1 = self.conv(8 * n_filter, 16 * n_filter)
-        self.middle_conv2 = self.conv(16 * n_filter, 16 * n_filter, dropout=0.5)
-
-        # decode
-        self.up1 = nn.ConvTranspose2d(16 * n_filter, 8 * n_filter, kernel_size=2, stride=2)
-        self.decode1 = self.conv(16 * n_filter, 8 * n_filter)
-        self.decode2 = self.conv(8 * n_filter, 8 * n_filter)
-        self.up2 = nn.ConvTranspose2d(8 * n_filter, 4 * n_filter, kernel_size=2, stride=2)
-        self.decode3 = self.conv(8 * n_filter, 4 * n_filter)
-        self.decode4 = self.conv(4 * n_filter, 4 * n_filter)
-        self.up3 = nn.ConvTranspose2d(4 * n_filter, 2 * n_filter, kernel_size=2, stride=2)
-        self.decode5 = self.conv(4 * n_filter, 2 * n_filter)
-        self.decode6 = self.conv(2 * n_filter, 2 * n_filter)
-        self.up4 = nn.ConvTranspose2d(2 * n_filter, 1 * n_filter, kernel_size=2, stride=2)
-        self.decode7 = self.conv(2 * n_filter, 1 * n_filter)
-        self.decode8 = self.conv(1 * n_filter, 1 * n_filter)
-        self.decode9 = self.conv(1 * n_filter, 1)
-        self.final = nn.Sequential(
-            nn.Conv2d(1, 1, kernel_size=1, padding=0),
-        )
-
-    def conv(self, in_channels, out_channels, kernel_size=3, dropout=0.0):
-        block = nn.Sequential(
-            nn.Conv2d(kernel_size=kernel_size, in_channels=in_channels, out_channels=out_channels, padding=1),
-            nn.BatchNorm2d(out_channels),
-            nn.ReLU(),
-            nn.Dropout2d(dropout)
-        )
-        return block
-
-    def concat(self, x1, x2):
-        if x1.shape == x2.shape:
-            return torch.cat((x1, x2), 1)
-        else:
-            print(x1.shape, x2.shape)
-            raise ValueError('concatenation failed: wrong dimensions')
-
-    def forward(self, x):
-        e1 = self.encode1(x)
-        e2 = self.encode2(e1)
-        m1 = self.maxpool1(e2)
-        e3 = self.encode3(m1)
-        e4 = self.encode4(e3)
-        m2 = self.maxpool2(e4)
-        e5 = self.encode5(m2)
-        e6 = self.encode6(e5)
-        m3 = self.maxpool3(e6)
-        e7 = self.encode7(m3)
-        e8 = self.encode8(e7)
-        m4 = self.maxpool4(e8)
-
-        mid1 = self.middle_conv1(m4)
-        mid2 = self.middle_conv2(mid1)
-
-        u1 = self.up1(mid2)
-        c1 = self.concat(u1, e7)
-        d1 = self.decode1(c1)
-        d2 = self.decode2(d1)
-        u2 = self.up2(d2)
-        c2 = self.concat(u2, e5)
-        d3 = self.decode3(c2)
-        d4 = self.decode4(d3)
-        u3 = self.up3(d4)
-        c3 = self.concat(u3, e3)
-        d5 = self.decode5(c3)
-        d6 = self.decode6(d5)
-        u4 = self.up4(d6)
-        c4 = self.concat(u4, e1)
-        d7 = self.decode7(c4)
-        d8 = self.decode8(d7)
-        d9 = self.decode9(d8)
-        logits = self.final(d9)
-        return torch.sigmoid(logits), logits
+import torch
+from torch import nn
+
+
+class Unet(nn.Module):
+    def __init__(self, in_channels=1, out_channels=1, n_filter=32, dilation=1):
+        """
+        Neural network for semantic image segmentation U-Net (PyTorch),
+        Reference:  Falk, T. et al. U-Net: deep learning for cell counting, detection, and morphometry. Nat Methods 16,
+        67–70 (2019).
+
+        Parameters
+        ----------
+        n_filter : int
+            Number of convolutional filters (commonly 16, 32, or 64)
+        """
+        super().__init__()
+        # encode
+        self.encode1 = self.conv(in_channels=in_channels, out_channels=n_filter, dilation=dilation)
+        self.encode2 = self.conv(n_filter, n_filter, dilation=dilation)
+        self.maxpool1 = nn.MaxPool2d(kernel_size=2, stride=2)
+        self.encode3 = self.conv(n_filter, 2 * n_filter, dilation=dilation)
+        self.encode4 = self.conv(2 * n_filter, 2 * n_filter, dilation=dilation)
+        self.maxpool2 = nn.MaxPool2d(kernel_size=2, stride=2)
+        self.encode5 = self.conv(2 * n_filter, 4 * n_filter, dilation=dilation)
+        self.encode6 = self.conv(4 * n_filter, 4 * n_filter, dilation=dilation)
+        self.maxpool3 = nn.MaxPool2d(kernel_size=2, stride=2)
+        self.encode7 = self.conv(4 * n_filter, 8 * n_filter, dilation=dilation)
+        self.encode8 = self.conv(8 * n_filter, 8 * n_filter, dilation=dilation)
+        self.maxpool4 = nn.MaxPool2d(kernel_size=2, stride=2)
+
+        # middle
+        self.middle_conv1 = self.conv(8 * n_filter, 16 * n_filter, dilation=dilation)
+        self.middle_conv2 = self.conv(16 * n_filter, 16 * n_filter, dilation=dilation)
+
+        # decode
+        self.up1 = nn.ConvTranspose2d(16 * n_filter, 8 * n_filter, kernel_size=2, stride=2)
+        self.decode1 = self.conv(16 * n_filter, 8 * n_filter)
+        self.decode2 = self.conv(8 * n_filter, 8 * n_filter)
+        self.up2 = nn.ConvTranspose2d(8 * n_filter, 4 * n_filter, kernel_size=2, stride=2)
+        self.decode3 = self.conv(8 * n_filter, 4 * n_filter)
+        self.decode4 = self.conv(4 * n_filter, 4 * n_filter)
+        self.up3 = nn.ConvTranspose2d(4 * n_filter, 2 * n_filter, kernel_size=2, stride=2)
+        self.decode5 = self.conv(4 * n_filter, 2 * n_filter)
+        self.decode6 = self.conv(2 * n_filter, 2 * n_filter)
+        self.up4 = nn.ConvTranspose2d(2 * n_filter, 1 * n_filter, kernel_size=2, stride=2)
+        self.decode7 = self.conv(2 * n_filter, 1 * n_filter)
+        self.decode8 = self.conv(1 * n_filter, 1 * n_filter)
+        self.final = nn.Sequential(
+            nn.Conv2d(n_filter, out_channels=out_channels, kernel_size=1, padding=0),
+        )
+
+    def conv(self, in_channels, out_channels, kernel_size=3, dropout=0., dilation=1):
+        layers = [
+            nn.Conv2d(in_channels, out_channels, kernel_size, padding=dilation, dilation=dilation),
+            nn.BatchNorm2d(out_channels),
+            nn.LeakyReLU(negative_slope=0.1, inplace=True),  # Using LeakyReLU
+            nn.Dropout2d(dropout)]
+        return nn.Sequential(*layers)
+
+    def concat(self, x1, x2):
+        if x1.shape == x2.shape:
+            return torch.cat((x1, x2), 1)
+        else:
+            print(x1.shape, x2.shape)
+            raise ValueError('concatenation failed: wrong dimensions')
+
+    def forward(self, x):
+
+        e1 = self.encode1(x)
+        e2 = self.encode2(e1)
+        m1 = self.maxpool1(e2)
+        e3 = self.encode3(m1)
+        e4 = self.encode4(e3)
+        m2 = self.maxpool2(e4)
+        e5 = self.encode5(m2)
+        e6 = self.encode6(e5)
+        m3 = self.maxpool3(e6)
+        e7 = self.encode7(m3)
+        e8 = self.encode8(e7)
+        m4 = self.maxpool4(e8)
+
+        mid1 = self.middle_conv1(m4)
+        mid2 = self.middle_conv2(mid1)
+
+        u1 = self.up1(mid2)
+        c1 = self.concat(u1, e8)
+        d1 = self.decode1(c1)
+        d2 = self.decode2(d1)
+        u2 = self.up2(d2)
+        c2 = self.concat(u2, e6)
+        d3 = self.decode3(c2)
+        d4 = self.decode4(d3)
+        u3 = self.up3(d4)
+        c3 = self.concat(u3, e4)
+        d5 = self.decode5(c3)
+        d6 = self.decode6(d5)
+        u4 = self.up4(d6)
+        c4 = self.concat(u4, e2)
+        d7 = self.decode7(c4)
+        d8 = self.decode8(d7)
+        logits = self.final(d8)
+        return torch.sigmoid(logits), logits
```

### Comparing `bio-image-unet-0.6.1/PKG-INFO` & `bio_image_unet-1.0.0a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: bio-image-unet
-Version: 0.6.1
+Version: 1.0.0a1
 Summary: Implementations of U-Net and Siam U-Net for biological image segmentation
 License: MIT
 Author: Daniel Haertter
 Author-email: dani.hae@posteo.de
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: albumentations (>=1.3.0,<2.0.0)
-Requires-Dist: barbar (>=0.2.1,<0.3.0)
-Requires-Dist: numpy (>=1.19.5,<2.1.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: albumentations (>=1.3,<2.0)
+Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: packaging
-Requires-Dist: scikit-image (>=0.18.2,<1.0.0)
-Requires-Dist: scipy (>=1.9.1,<2.2.0)
+Requires-Dist: scikit-image (>0.18,<1.0)
 Requires-Dist: tifffile
-Requires-Dist: torch (>=1.9.0,<2.2.0)
-Requires-Dist: tqdm (>=4.61.2,<5.0.0)
+Requires-Dist: torch (==2.*)
+Requires-Dist: tqdm (>=4.61,<5.0)
 Description-Content-Type: text/markdown
 
 # Bio Image U-Net
 
 Implementations of U-Net and Siam U-Net for biological image segmentation
 
 ### Authors
```

