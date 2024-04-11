# Comparing `tmp/noteshrunk-1.0.1.tar.gz` & `tmp/noteshrunk-1.0.2.tar.gz`

## Comparing `noteshrunk-1.0.1.tar` & `noteshrunk-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,12 @@
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/.README.md.swp
--rw-r--r--   0        0        0    12837 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/.README.md.un~
--rw-r--r--   0        0        0    28217 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/.pyproject.toml.un~
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/.setup.py.un~
--rw-r--r--   0        0        0   809090 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/notesA1.jpg
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/setup.py
--rw-r--r--   0        0        0    36864 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/noteshrunk/.noteshrunk.py.swp
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/noteshrunk/.noteshrunk.py.un~
--rwxr-xr-x   0        0        0    20733 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/noteshrunk/noteshrunk.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/LICENSE
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    45413 2020-02-02 00:00:00.000000 noteshrunk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/.README.md.un~
+-rw-r--r--   0        0        0    48278 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/.pyproject.toml.un~
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/.setup.py.un~
+-rw-r--r--   0        0        0   809090 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/notesA1.jpg
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/requirements.txt
+-rwxr-xr-x   0        0        0     4544 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/src/.noteshrunk.py.un~
+-rwxr-xr-x   0        0        0    20647 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/src/noteshrunk.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 noteshrunk-1.0.2/PKG-INFO
```

### Comparing `noteshrunk-1.0.1/.setup.py.un~` & `noteshrunk-1.0.2/.setup.py.un~`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.0.1/notesA1.jpg` & `noteshrunk-1.0.2/notesA1.jpg`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.0.1/noteshrunk/noteshrunk.py` & `noteshrunk-1.0.2/src/noteshrunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 from pathlib import Path
 import random
 import re
 import string
 import subprocess
 import tempfile
 
-try:
-    import argcomplete
-except ImportError:
-    pass
+import argcomplete
 import numpy as np
 from PIL import Image
 from scipy.ndimage import median_filter
 from skimage import io
 from sklearn.cluster import KMeans
 from skimage.color import rgb2hsv
 from skimage.morphology import binary_opening, binary_closing, square, disk
@@ -136,18 +133,15 @@
     parser.add_argument(
         '-y',
         '--overwrite',
         action='store_true',
         default=False,
         help='Overwrite existing files without asking.')
 
-    try:
-        argcomplete.autocomplete(parser)
-    except NameError:
-        pass
+    argcomplete.autocomplete(parser)
     return parser.parse_args()
 
 
 def sort_filenames(filenames):
     """
     Sorts filenames in natural order.
```

### Comparing `noteshrunk-1.0.1/.gitignore` & `noteshrunk-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.0.1/LICENSE` & `noteshrunk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.0.1/README.md` & `noteshrunk-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 * **Background Detection and Removal:** Identifies and removes the background color.
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
 * **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
 * **Denoising Options:** Provides median filtering and morphological operations to reduce noise and improve image quality.
 
 ## Requirements
 
-- Python 3
+- argcomplete
 - NumPy
 - Pillow (PIL Fork)
-- SciPy
-- scikit-learn
+- Python 3
 - scikit-image
+- scikit-learn
+- SciPy
 
 ### Optional
 
-- argcomplete (for command-line auto-completion)
 - Ghostscript (for PDF merging; otherwise you need to use the `-k` flag)
 
 ## Installation
 
 ```bash
 pipx install noteshrunk
 ```
```

### Comparing `noteshrunk-1.0.1/pyproject.toml` & `noteshrunk-1.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noteshrunk"
-version = "1.0.1"
+version = "1.0.2"
 description = "Document Color Palette Compression"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
     {name = "suuuehgi"}
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
+    "argcomplete",
     "numpy",
-    "Pillow",
-    "scipy",
     "scikit-image",
     "scikit-learn",
+    "scipy",
+    "Pillow",
 ]
 
-[project.optional-dependencies]
-autocomp = ["argcomplete"]
-
 [project.scripts]
-noteshrunk = "noteshrunk.noteshrunk:main"
+noteshrunk = "src.noteshrunk:main"
 
 [project.urls]
 Homepage = "https://github.com/suuuehgi/noteshrunk"
 Issues = "https://github.com/suuuehgi/noteshrunk/issues"
 
 [tool.hatch.build.targets.wheel]
-packages = ["noteshrunk"]
+packages = ["src"]
```

### Comparing `noteshrunk-1.0.1/PKG-INFO` & `noteshrunk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -680,21 +680,20 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Requires-Dist: argcomplete
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: scikit-image
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Provides-Extra: autocomp
-Requires-Dist: argcomplete; extra == 'autocomp'
 Description-Content-Type: text/markdown
 
 # noteshrunk - Document Color Palette Compression
 
 This Python script compresses images by reducing the number of colors and optimizing the image representation.
 It leverages KMeans clustering for color quantization and offers various options to customize the compression process.
 All supplied images are then saved as a multi-page PDF.
@@ -708,24 +707,24 @@
 * **Background Detection and Removal:** Identifies and removes the background color.
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
 * **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
 * **Denoising Options:** Provides median filtering and morphological operations to reduce noise and improve image quality.
 
 ## Requirements
 
-- Python 3
+- argcomplete
 - NumPy
 - Pillow (PIL Fork)
-- SciPy
-- scikit-learn
+- Python 3
 - scikit-image
+- scikit-learn
+- SciPy
 
 ### Optional
 
-- argcomplete (for command-line auto-completion)
 - Ghostscript (for PDF merging; otherwise you need to use the `-k` flag)
 
 ## Installation
 
 ```bash
 pipx install noteshrunk
 ```
```

