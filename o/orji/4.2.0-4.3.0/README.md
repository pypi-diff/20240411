# Comparing `tmp/orji-4.2.0.tar.gz` & `tmp/orji-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orji-4.2.0.tar", last modified: Tue Apr  9 23:50:49 2024, max compression
+gzip compressed data, was "orji-4.3.0.tar", last modified: Thu Apr 11 17:40:22 2024, max compression
```

## Comparing `orji-4.2.0.tar` & `orji-4.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.914145 orji-4.2.0/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-09 23:50:21.000000 orji-4.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2024-04-09 23:50:21.000000 orji-4.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3471 2024-04-09 23:50:49.914145 orji-4.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2554 2024-04-09 23:50:21.000000 orji-4.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-09 23:50:21.000000 orji-4.2.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.902145 orji-4.2.0/hitch/
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/Dockerfile-hitch
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/debugrequirements.txt
--rw-r--r--   0 root         (0) root         (0)     3394 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/docgen.py
--rw-r--r--   0 root         (0) root         (0)      692 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/docstory.yml
--rw-r--r--   0 root         (0) root         (0)     3971 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/engine.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/hitchreqs.in
--rw-r--r--   0 root         (0) root         (0)     4293 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/hitchreqs.txt
--rw-r--r--   0 root         (0) root         (0)     3914 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.906145 orji-4.2.0/hitch/story/
--rw-r--r--   0 root         (0) root         (0)     2971 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/all-template-features.story
--rw-r--r--   0 root         (0) root         (0)     1468 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/errors.story
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/fail.story
--rw-r--r--   0 root         (0) root         (0)     4201 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/in.story
--rw-r--r--   0 root         (0) root         (0)     1407 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/insert-ical.story
--rw-r--r--   0 root         (0) root         (0)    18631 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/latex-cv.story
--rw-r--r--   0 root         (0) root         (0)     8511 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/latex-letter.story
--rw-r--r--   0 root         (0) root         (0)     1010 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/links.story
--rw-r--r--   0 root         (0) root         (0)     1415 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/lookup-cli.story
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/lookup-in-file.story
--rw-r--r--   0 root         (0) root         (0)      602 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/markdown.story
--rw-r--r--   0 root         (0) root         (0)      624 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/module.story
--rw-r--r--   0 root         (0) root         (0)     1832 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/multiple-files.story
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/quickstart.story
--rw-r--r--   0 root         (0) root         (0)      809 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/rm.story
--rw-r--r--   0 root         (0) root         (0)     1484 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/script-multiple-matching.story
--rw-r--r--   0 root         (0) root         (0)     1901 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/script.story
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/todo.txt
--rw-r--r--   0 root         (0) root         (0)     1258 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/walk.story
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.910145 orji-4.2.0/orji/
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-09 23:50:21.000000 orji-4.2.0/orji/__init__.py
--rw-r--r--   0 root         (0) root         (0)      281 2024-04-09 23:50:21.000000 orji-4.2.0/orji/app.py
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-09 23:50:21.000000 orji-4.2.0/orji/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-09 23:50:21.000000 orji-4.2.0/orji/ical.py
--rw-r--r--   0 root         (0) root         (0)     2670 2024-04-09 23:50:21.000000 orji-4.2.0/orji/insert.py
--rw-r--r--   0 root         (0) root         (0)     1493 2024-04-09 23:50:21.000000 orji-4.2.0/orji/loader.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-04-09 23:50:21.000000 orji-4.2.0/orji/lookup.py
--rw-r--r--   0 root         (0) root         (0)     4972 2024-04-09 23:50:21.000000 orji-4.2.0/orji/note.py
--rw-r--r--   0 root         (0) root         (0)     1194 2024-04-09 23:50:21.000000 orji-4.2.0/orji/output.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-09 23:50:21.000000 orji-4.2.0/orji/remove.py
--rw-r--r--   0 root         (0) root         (0)     2879 2024-04-09 23:50:21.000000 orji-4.2.0/orji/run.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-09 23:50:21.000000 orji-4.2.0/orji/tempdir.py
--rw-r--r--   0 root         (0) root         (0)     3600 2024-04-09 23:50:21.000000 orji-4.2.0/orji/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.910145 orji-4.2.0/orji.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3471 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-09 23:50:21.000000 orji-4.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 23:50:49.914145 orji-4.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 23:50:21.000000 orji-4.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:40:22.543154 orji-4.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-11 17:39:08.000000 orji-4.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2024-04-11 17:39:08.000000 orji-4.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-11 17:40:22.543154 orji-4.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-11 17:39:08.000000 orji-4.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-11 17:39:08.000000 orji-4.3.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:40:22.531154 orji-4.3.0/hitch/
+-rw-r--r--   0 root         (0) root         (0)      523 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/Dockerfile-hitch
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/debugrequirements.txt
+-rw-r--r--   0 root         (0) root         (0)     3394 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/docgen.py
+-rw-r--r--   0 root         (0) root         (0)      692 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/docstory.yml
+-rw-r--r--   0 root         (0) root         (0)     3971 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/engine.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/hitchreqs.in
+-rw-r--r--   0 root         (0) root         (0)     4293 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/hitchreqs.txt
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:40:22.535154 orji-4.3.0/hitch/story/
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/all-template-features.story
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/errors.story
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/fail.story
+-rw-r--r--   0 root         (0) root         (0)     4235 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/in.story
+-rw-r--r--   0 root         (0) root         (0)     1412 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/insert-ical.story
+-rw-r--r--   0 root         (0) root         (0)    18631 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/latex-cv.story
+-rw-r--r--   0 root         (0) root         (0)     8511 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/latex-letter.story
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/links.story
+-rw-r--r--   0 root         (0) root         (0)     1415 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/lookup-cli.story
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/lookup-in-file.story
+-rw-r--r--   0 root         (0) root         (0)      602 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/markdown.story
+-rw-r--r--   0 root         (0) root         (0)      624 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/module.story
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/multiple-files.story
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/quickstart.story
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/rm.story
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/script-multiple-matching.story
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/script.story
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/todo.txt
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-04-11 17:39:08.000000 orji-4.3.0/hitch/story/walk.story
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:40:22.539154 orji-4.3.0/orji/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-11 17:39:08.000000 orji-4.3.0/orji/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      281 2024-04-11 17:39:08.000000 orji-4.3.0/orji/app.py
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-11 17:39:08.000000 orji-4.3.0/orji/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-11 17:39:08.000000 orji-4.3.0/orji/ical.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-11 17:39:08.000000 orji-4.3.0/orji/insert.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-11 17:39:08.000000 orji-4.3.0/orji/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-11 17:39:08.000000 orji-4.3.0/orji/lookup.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2024-04-11 17:39:08.000000 orji-4.3.0/orji/note.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-04-11 17:39:08.000000 orji-4.3.0/orji/output.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-11 17:39:08.000000 orji-4.3.0/orji/remove.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2024-04-11 17:39:08.000000 orji-4.3.0/orji/run.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-11 17:39:08.000000 orji-4.3.0/orji/tempdir.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2024-04-11 17:39:08.000000 orji-4.3.0/orji/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:40:22.539154 orji-4.3.0/orji.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-11 17:40:22.000000 orji-4.3.0/orji.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-11 17:40:22.000000 orji-4.3.0/orji.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:40:22.000000 orji-4.3.0/orji.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-11 17:40:22.000000 orji-4.3.0/orji.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-11 17:40:22.000000 orji-4.3.0/orji.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-11 17:40:22.000000 orji-4.3.0/orji.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-11 17:39:08.000000 orji-4.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 17:40:22.543154 orji-4.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 17:39:08.000000 orji-4.3.0/setup.py
```

### Comparing `orji-4.2.0/LICENSE` & `orji-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/PKG-INFO` & `orji-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orji
-Version: 4.2.0
+Version: 4.3.0
 Summary: Org mode to jinja2 templating.
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/orji
 Project-URL: documentation, https://hitchdev.com/orji/using
 Project-URL: repository, https://github.com/crdoconnor/orji
 Project-URL: changelog, https://hitchdev.com/orji/changelog
```

### Comparing `orji-4.2.0/README.md` & `orji-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/Dockerfile-hitch` & `orji-4.3.0/hitch/Dockerfile-hitch`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/docgen.py` & `orji-4.3.0/hitch/docgen.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/docstory.yml` & `orji-4.3.0/hitch/docstory.yml`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/engine.py` & `orji-4.3.0/hitch/engine.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/hitchreqs.txt` & `orji-4.3.0/hitch/hitchreqs.txt`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/key.py` & `orji-4.3.0/hitch/key.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/all-template-features.story` & `orji-4.3.0/hitch/story/all-template-features.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/errors.story` & `orji-4.3.0/hitch/story/errors.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/fail.story` & `orji-4.3.0/hitch/story/fail.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/in.story` & `orji-4.3.0/hitch/story/in.story`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Insert file:
   docs: insert
   about: |
-    Insert a file as a note.
+    Insert a text file as a note.
   given:
     files:
       org/simple.org: |
         * Top note
         ** Subnote
         ** TODO Insert above, under or below, replace this  
         * DONE Done item
       speech.txt: This is a note generated by speech to text.
       notetemplate.jinja2: |
         * TODO New note
 
-        {{ text }}
+        {{ words }}
 
   variations:
     Above:
       steps:
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 above org/simple.org//0/1 --text speech.txt
+          cmd: in notetemplate.jinja2 above org/simple.org//0/1 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * Top note
@@ -34,15 +34,15 @@
             This is a note generated by speech to text.
             ** TODO Insert above, under or below, replace this
             * DONE Done item
 
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 above org/simple.org//0 --text speech.txt
+          cmd: in notetemplate.jinja2 above org/simple.org//0 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * TODO New note
@@ -55,15 +55,15 @@
             * DONE Done item
 
     Below:
       steps:
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 below org/simple.org//0/1 --text speech.txt
+          cmd: in notetemplate.jinja2 below org/simple.org//0/1 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * Top note
@@ -72,15 +72,15 @@
             ** TODO New note
             This is a note generated by speech to text.
             * DONE Done item
 
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 below org/simple.org//0 --text speech.txt
+          cmd: in notetemplate.jinja2 below org/simple.org//0 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * Top note
@@ -94,15 +94,15 @@
 
 
     Under:
       steps:
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 under org/simple.org//0/1 --text speech.txt
+          cmd: in notetemplate.jinja2 under org/simple.org//0/1 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * Top note
@@ -111,15 +111,15 @@
             *** TODO New note
             This is a note generated by speech to text.
             * DONE Done item
 
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 under org/simple.org//0 --text speech.txt
+          cmd: in notetemplate.jinja2 under org/simple.org//0 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * Top note
@@ -133,15 +133,15 @@
 
 
     Replace:
       steps:
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in notetemplate.jinja2 replace org/simple.org//0/1 --text speech.txt
+          cmd: in notetemplate.jinja2 replace org/simple.org//0/1 words:text:speech.txt
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/simple.org
           contents: |
             * Top note
```

### Comparing `orji-4.2.0/hitch/story/insert-ical.story` & `orji-4.3.0/hitch/story/insert-ical.story`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Insert ical file as a note.
   given:
     files:
       org/calendar.org: |
         * Meetings
         * Birthdays
       direct.jinja2: |
-        {{ ical.to_org() }}
+        {{ event.to_org() }}
       calendar.ical: |
         BEGIN:VCALENDAR
         PRODID:-//xyz Corp//NONSGML PDA Calendar Version 1.0//EN
         VERSION:2.0
         BEGIN:VEVENT
         DTSTAMP:19960704T120000Z
         UID:uid1@example.com
@@ -30,15 +30,15 @@
 
   variations:
     Directly under meetings header:
       steps:
       - orji:
           env:
             ORJITMP: ./tmp
-          cmd: in direct.jinja2 under org/calendar.org//0 --ical calendar.ical
+          cmd: in direct.jinja2 under org/calendar.org//0 event:ical:calendar.ical
           output: |
             Written note(s) successfully
 
       - file contents:
           filename: org/calendar.org
           contents: |
             * Meetings
```

### Comparing `orji-4.2.0/hitch/story/latex-cv.story` & `orji-4.3.0/hitch/story/latex-cv.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/latex-letter.story` & `orji-4.3.0/hitch/story/latex-letter.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/links.story` & `orji-4.3.0/hitch/story/links.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/lookup-cli.story` & `orji-4.3.0/hitch/story/lookup-cli.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/lookup-in-file.story` & `orji-4.3.0/hitch/story/lookup-in-file.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/markdown.story` & `orji-4.3.0/hitch/story/markdown.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/module.story` & `orji-4.3.0/hitch/story/module.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/multiple-files.story` & `orji-4.3.0/hitch/story/multiple-files.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/quickstart.story` & `orji-4.3.0/hitch/story/quickstart.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/rm.story` & `orji-4.3.0/hitch/story/rm.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/script-multiple-matching.story` & `orji-4.3.0/hitch/story/script-multiple-matching.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/script.story` & `orji-4.3.0/hitch/story/script.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/hitch/story/walk.story` & `orji-4.3.0/hitch/story/walk.story`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/ical.py` & `orji-4.3.0/orji/ical.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/insert.py` & `orji-4.3.0/orji/insert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 from pathlib import Path
 import click
 from .template import Template
+from .exceptions import OrjiError
 import orgmunge
 from .tempdir import TempDir
 from .loader import Loader
 from .lookup import Lookup
 from .ical import ICal
 
 
 @click.command()
 @click.argument("jinjafile")
 @click.argument("relative")
 @click.argument("location")
-@click.option(
-    "--text",
-    "textfile",
-    help="Put file contents into {{ text }}",
-)
-@click.option(
-    "--ical",
-    "icalfile",
-    help="Put ical file contents into {{ ical }}",
-)
-def insert(jinjafile, relative, location, textfile, icalfile):
+@click.argument("insertion")
+def insert(jinjafile, relative, location, insertion):
     temp_dir = TempDir()
     temp_dir.create()
     loader = Loader(temp_dir)
     lookup = Lookup(location)
     template_text = Path(jinjafile).read_text()
-    output_text = Template(template_text, jinjafile).render(
-        text=Path(textfile).read_text() if textfile is not None else None,
-        ical=ICal(icalfile) if icalfile is not None else None,
-    )
+
+    varname, insertion_type, insertion_file = insertion.split(":")
+    template = Template(template_text, jinjafile)
+
+    if insertion_type == "ical":
+        output_text = template.render(**{varname: ICal(insertion_file)})
+    elif insertion_type == "text":
+        output_text = template.render(**{varname: Path(insertion_file).read_text()})
+    else:
+        raise OrjiError(f"{insertion_type} not known")
+
     chunk_to_insert = orgmunge.Org(
         output_text,
         from_file=False,
         todos={"todo_states": {"todo": "TODO"}, "done_states": {"done": "DONE"}},
     )
 
     write_note = lookup.load(loader)
```

### Comparing `orji-4.2.0/orji/loader.py` & `orji-4.3.0/orji/loader.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/lookup.py` & `orji-4.3.0/orji/lookup.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/note.py` & `orji-4.3.0/orji/note.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/output.py` & `orji-4.3.0/orji/output.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/remove.py` & `orji-4.3.0/orji/remove.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/run.py` & `orji-4.3.0/orji/run.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/tempdir.py` & `orji-4.3.0/orji/tempdir.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji/template.py` & `orji-4.3.0/orji/template.py`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/orji.egg-info/PKG-INFO` & `orji-4.3.0/orji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orji
-Version: 4.2.0
+Version: 4.3.0
 Summary: Org mode to jinja2 templating.
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/orji
 Project-URL: documentation, https://hitchdev.com/orji/using
 Project-URL: repository, https://github.com/crdoconnor/orji
 Project-URL: changelog, https://hitchdev.com/orji/changelog
```

### Comparing `orji-4.2.0/orji.egg-info/SOURCES.txt` & `orji-4.3.0/orji.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orji-4.2.0/pyproject.toml` & `orji-4.3.0/pyproject.toml`

 * *Files identical despite different names*

