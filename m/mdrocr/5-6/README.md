# Comparing `tmp/mdrocr-5.tar.gz` & `tmp/mdrocr-6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrocr-5.tar", last modified: Wed Apr 10 14:40:44 2024, max compression
+gzip compressed data, was "mdrocr-6.tar", last modified: Thu Apr 11 16:49:42 2024, max compression
```

## Comparing `mdrocr-5.tar` & `mdrocr-6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-10 14:40:44.745209 mdrocr-5/
--rw-rw-r--   0 j         (1000) j         (1000)       30 2024-03-20 16:50:35.000000 mdrocr-5/.gitignore
--rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-10 14:40:44.745209 mdrocr-5/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)       89 2024-03-20 16:55:05.000000 mdrocr-5/README.md
--rwxrwxr-x   0 j         (1000) j         (1000)     2483 2024-04-10 14:39:36.000000 mdrocr-5/mdrocr
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-10 14:40:44.745209 mdrocr-5/mdrocr.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-10 14:40:43.000000 mdrocr-5/mdrocr.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      167 2024-04-10 14:40:44.000000 mdrocr-5/mdrocr.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-10 14:40:43.000000 mdrocr-5/mdrocr.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-10 14:40:43.000000 mdrocr-5/mdrocr.egg-info/top_level.txt
--rwxr-xr-x   0 j         (1000) j         (1000)      291 2024-03-20 16:56:34.000000 mdrocr-5/release.sh
--rw-rw-r--   0 j         (1000) j         (1000)       38 2024-04-10 14:40:44.745209 mdrocr-5/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)      924 2024-04-10 14:40:42.000000 mdrocr-5/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-11 16:49:42.759487 mdrocr-6/
+-rw-rw-r--   0 j         (1000) j         (1000)       30 2024-03-20 16:50:35.000000 mdrocr-6/.gitignore
+-rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-11 16:49:42.759487 mdrocr-6/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)       89 2024-03-20 16:55:05.000000 mdrocr-6/README.md
+-rwxrwxr-x   0 j         (1000) j         (1000)     2483 2024-04-11 16:49:15.000000 mdrocr-6/mdrocr
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-11 16:49:42.759487 mdrocr-6/mdrocr.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      167 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/top_level.txt
+-rwxr-xr-x   0 j         (1000) j         (1000)      291 2024-03-20 16:56:34.000000 mdrocr-6/release.sh
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2024-04-11 16:49:42.759487 mdrocr-6/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)      924 2024-04-11 16:49:41.000000 mdrocr-6/setup.py
```

### Comparing `mdrocr-5/mdrocr` & `mdrocr-6/mdrocr`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,25 +60,25 @@
             [f for f in files if f.split(".")[-1] in ("jpg", "jp2", "jpeg")]
         )
         print("\n---\nprocessing %s\n%s pages\n" % (root, len(images)))
         tmp = tempfile.mkdtemp()
         pages = []
         for image in images:
             image = os.path.join(root, image)
+            print(image[len(root) + 1 :])
             tmp_pdf = os.path.join(tmp, os.path.basename(os.path.splitext(image)[0]))
             if image.endswith(".jp2"):
                 tmp_jpg = tmp_pdf + ".jpg"
                 if sips_installed:
                     cmd = ["sips", "-s", "format", "jpeg", image, "--out", tmp_jpg]
                 else:
                     cmd = ["convert", image, tmp_jpg]
                 subprocess.check_output(cmd)
                 image = tmp_jpg
             cmd = ["tesseract", "-l", language, "--dpi", dpi, image, tmp_pdf, "pdf"]
-            print(image[len(root) + 1 :])
             subprocess.check_output(cmd)
             pages.append(tmp_pdf + ".pdf")
         cmd = ["pdfunite"] + pages + [pdf]
         subprocess.check_output(cmd)
         print("\ncreated %s" % pdf)
         shutil.rmtree(tmp)
 print("")
```

### Comparing `mdrocr-5/setup.py` & `mdrocr-6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 
 def get_version():
-    return 5 #import subprocess
+    return 6 #import subprocess
     cmd = ['git', 'rev-list', 'HEAD', '--count']
     p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = p.communicate()
     rev = int(stdout)
     return u'%s' % rev
```

