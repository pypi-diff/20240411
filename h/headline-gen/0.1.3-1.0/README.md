# Comparing `tmp/headline-gen-0.1.3.tar.gz` & `tmp/headline-gen-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline-gen-0.1.3.tar", last modified: Thu Apr 11 04:49:33 2024, max compression
+gzip compressed data, was "headline-gen-1.0.tar", last modified: Thu Apr 11 05:06:47 2024, max compression
```

## Comparing `headline-gen-0.1.3.tar` & `headline-gen-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:49:33.169313 headline-gen-0.1.3/
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-11 04:49:33.169313 headline-gen-0.1.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:49:33.167313 headline-gen-0.1.3/headline_gen/
--rw-r--r--   0 root         (0) root         (0)    12809 2024-04-11 04:17:33.000000 headline-gen-0.1.3/headline_gen/Control.py
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-11 04:45:16.000000 headline-gen-0.1.3/headline_gen/__int__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:49:33.168313 headline-gen-0.1.3/headline_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-11 04:49:33.000000 headline-gen-0.1.3/headline_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-11 04:49:33.000000 headline-gen-0.1.3/headline_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 04:49:33.000000 headline-gen-0.1.3/headline_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 04:49:33.000000 headline-gen-0.1.3/headline_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 04:49:33.000000 headline-gen-0.1.3/headline_gen.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 04:49:33.169313 headline-gen-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      429 2024-04-11 04:49:20.000000 headline-gen-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:06:47.372288 headline-gen-1.0/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:06:47.371287 headline-gen-1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:06:47.370287 headline-gen-1.0/headline_gen/
+-rw-r--r--   0 root         (0) root         (0)    13088 2024-04-11 05:06:11.000000 headline-gen-1.0/headline_gen/Control.py
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 04:54:13.000000 headline-gen-1.0/headline_gen/__int__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:06:47.371287 headline-gen-1.0/headline_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 05:06:47.000000 headline-gen-1.0/headline_gen.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:06:47.372288 headline-gen-1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 05:06:25.000000 headline-gen-1.0/setup.py
```

### Comparing `headline-gen-0.1.3/headline_gen/Control.py` & `headline-gen-1.0/headline_gen/Control.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,35 @@
         with zipfile.ZipFile(os.path.join(directory, filename), 'r') as zip_ref:
             zip_ref.extractall(directory)
         print("Extraction successful.")
     else:
         print("Failed to download file.")
 
 def ServerInit(Mode, Server = None):
-  if Mode == "Start":
-    server = CoreNLPServer()
-    server.start()
-    return server
-  elif Mode == "Stop":
-    if Server is None:
-      print("No Server Object Provided")
+  Path = 'Parser/'
+  os.environ['CLASSPATH'] = os.path.join(Path, 'stanford-corenlp-4.5.6')
+
+  directory_path = "Parser/stanford-corenlp-4.5.6"
+  if os.path.exists(directory_path) and os.listdir(directory_path):
+    if Mode == "Start":
+      server = CoreNLPServer()
+      server.start()
+      return server
+    elif Mode == "Stop":
+      if Server is None:
+        print("No Server Object Provided")
+      else:
+        Server.stop()
     else:
-      Server.stop()
+      print("Un defined Operation")
   else:
-    print("Un defined Operation")
+    print("Parser Files Not Found")
+    print("Attempting to Install Parser Files")
+    Downloader()
+    ServerInit(Mode, Server = Server)
 
 # Key Phrase Extraction
 
 def remove_punctuation(text):
   table = str.maketrans('', '', string.punctuation)
   return text.translate(table)
 
@@ -390,18 +400,14 @@
   checkpoint = "unikei/distilbert-base-re-punctuate"
   tokenizer = DistilBertTokenizerFast.from_pretrained(checkpoint)
   model = DistilBertForTokenClassification.from_pretrained(checkpoint)
   encoder_max_length = 256
   return punctuate(Sentence, tokenizer, model, encoder_max_length)
 
 def Generate(Article, Server):
-  Downloader()
-  Path = 'Parser/'
-  os.environ['CLASSPATH'] = os.path.join(Path, 'stanford-corenlp-4.5.6')
-
   cleaned_article = re.sub(r'\([^)]*\)', '', Article)
 
   KeyPhrases = KeyPhraseSGRank(cleaned_article)
 
   LSG = LeadSentencesOOPS(cleaned_article)
   LeadingSentences  = LSG.leading_sentences()
   #LeadingSentences = leading_sentences(cleaned_article)
```

