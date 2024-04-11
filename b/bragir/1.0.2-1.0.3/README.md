# Comparing `tmp/bragir-1.0.2.tar.gz` & `tmp/bragir-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bragir-1.0.2.tar", max compression
+gzip compressed data, was "bragir-1.0.3.tar", max compression
```

## Comparing `bragir-1.0.2.tar` & `bragir-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1067 2023-12-20 13:35:51.845090 bragir-1.0.2/LICENSE
--rw-r--r--   0        0        0     4267 2024-03-13 09:40:37.371664 bragir-1.0.2/README.md
--rw-r--r--   0        0        0      459 2024-03-14 15:10:23.605513 bragir-1.0.2/bragir/__init__.py
--rw-r--r--   0        0        0     1140 2024-03-14 15:10:23.605897 bragir-1.0.2/bragir/__main__.py
--rw-r--r--   0        0        0        0 2024-01-22 14:04:17.884178 bragir-1.0.2/bragir/audio/__init__.py
--rw-r--r--   0        0        0     1172 2024-03-19 09:45:36.645006 bragir-1.0.2/bragir/audio/chunking.py
--rw-r--r--   0        0        0     1528 2024-03-14 10:55:02.577586 bragir-1.0.2/bragir/audio/grouping.py
--rw-r--r--   0        0        0      727 2024-03-13 13:47:55.800819 bragir-1.0.2/bragir/client.py
--rw-r--r--   0        0        0     5706 2024-03-14 10:31:59.292679 bragir-1.0.2/bragir/commands.py
--rw-r--r--   0        0        0        0 2024-03-14 15:10:23.606313 bragir-1.0.2/bragir/config/__init__.py
--rw-r--r--   0        0        0     1187 2024-03-14 15:10:23.606824 bragir-1.0.2/bragir/config/config.py
--rw-r--r--   0        0        0      781 2024-01-23 14:49:56.563168 bragir-1.0.2/bragir/constants/__init__.py
--rw-r--r--   0        0        0      531 2024-03-13 13:47:55.801255 bragir-1.0.2/bragir/directory.py
--rw-r--r--   0        0        0     4860 2024-03-13 13:47:55.801500 bragir-1.0.2/bragir/file.py
--rw-r--r--   0        0        0        0 2024-01-23 14:46:13.948493 bragir-1.0.2/bragir/files/__init__.py
--rw-r--r--   0        0        0      777 2024-01-23 14:57:30.342610 bragir-1.0.2/bragir/files/file.py
--rw-r--r--   0        0        0      458 2024-03-13 13:47:55.801681 bragir-1.0.2/bragir/files/operations.py
--rw-r--r--   0        0        0      716 2023-12-20 13:35:51.846131 bragir-1.0.2/bragir/languages.py
--rw-r--r--   0        0        0      600 2023-12-22 14:10:13.429766 bragir-1.0.2/bragir/list.py
--rw-r--r--   0        0        0        0 2024-03-18 10:05:22.473895 bragir-1.0.2/bragir/logging_configs/__init__.py
--rw-r--r--   0        0        0      810 2024-03-18 09:47:41.850387 bragir-1.0.2/bragir/logging_configs/debug.json
--rw-r--r--   0        0        0      539 2024-03-18 09:47:41.862007 bragir-1.0.2/bragir/logging_configs/info.json
--rw-r--r--   0        0        0      534 2023-12-22 13:19:39.955616 bragir-1.0.2/bragir/messages.py
--rw-r--r--   0        0        0      343 2024-03-13 09:40:37.372753 bragir-1.0.2/bragir/path.py
--rw-r--r--   0        0        0     2135 2024-03-13 13:47:55.801840 bragir-1.0.2/bragir/spinner/__init__.py
--rw-r--r--   0        0        0        0 2024-01-23 14:46:22.975414 bragir-1.0.2/bragir/srt/__init__.py
--rw-r--r--   0        0        0      500 2024-01-23 14:41:02.577972 bragir-1.0.2/bragir/srt/srt_part.py
--rw-r--r--   0        0        0     1599 2024-03-13 13:47:55.802026 bragir-1.0.2/bragir/time.py
--rw-r--r--   0        0        0      476 2024-03-13 13:47:55.802184 bragir-1.0.2/bragir/timer.py
--rw-r--r--   0        0        0       44 2024-03-13 13:47:55.802328 bragir-1.0.2/bragir/tracing/__init__.py
--rw-r--r--   0        0        0      213 2024-03-13 13:47:55.802449 bragir-1.0.2/bragir/tracing/logger.py
--rw-r--r--   0        0        0      695 2024-03-18 10:06:12.584707 bragir-1.0.2/bragir/tracing/stratergies.py
--rw-r--r--   0        0        0     1156 2024-03-13 13:47:55.802783 bragir-1.0.2/bragir/transcription/__init__.py
--rw-r--r--   0        0        0     1830 2024-03-13 13:47:55.802994 bragir-1.0.2/bragir/translation/__init__.py
--rw-r--r--   0        0        0       98 2024-03-14 15:10:23.607211 bragir-1.0.2/bragir/types.py
--rw-r--r--   0        0        0      498 2024-03-19 09:46:38.289023 bragir-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 bragir-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-12-20 13:35:51.845090 bragir-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4267 2024-03-13 09:40:37.371664 bragir-1.0.3/README.md
+-rw-r--r--   0        0        0      459 2024-03-14 15:10:23.605513 bragir-1.0.3/bragir/__init__.py
+-rw-r--r--   0        0        0     1140 2024-03-14 15:10:23.605897 bragir-1.0.3/bragir/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-22 14:04:17.884178 bragir-1.0.3/bragir/audio/__init__.py
+-rw-r--r--   0        0        0     1172 2024-03-19 10:02:32.320342 bragir-1.0.3/bragir/audio/chunking.py
+-rw-r--r--   0        0        0     1528 2024-03-14 10:55:02.577586 bragir-1.0.3/bragir/audio/grouping.py
+-rw-r--r--   0        0        0      727 2024-03-13 13:47:55.800819 bragir-1.0.3/bragir/client.py
+-rw-r--r--   0        0        0     5814 2024-04-11 08:39:46.246312 bragir-1.0.3/bragir/commands.py
+-rw-r--r--   0        0        0        0 2024-03-14 15:10:23.606313 bragir-1.0.3/bragir/config/__init__.py
+-rw-r--r--   0        0        0     1187 2024-03-14 15:10:23.606824 bragir-1.0.3/bragir/config/config.py
+-rw-r--r--   0        0        0      781 2024-01-23 14:49:56.563168 bragir-1.0.3/bragir/constants/__init__.py
+-rw-r--r--   0        0        0      531 2024-03-13 13:47:55.801255 bragir-1.0.3/bragir/directory.py
+-rw-r--r--   0        0        0     4903 2024-04-11 08:39:54.805801 bragir-1.0.3/bragir/file.py
+-rw-r--r--   0        0        0        0 2024-01-23 14:46:13.948493 bragir-1.0.3/bragir/files/__init__.py
+-rw-r--r--   0        0        0      777 2024-01-23 14:57:30.342610 bragir-1.0.3/bragir/files/file.py
+-rw-r--r--   0        0        0      458 2024-03-13 13:47:55.801681 bragir-1.0.3/bragir/files/operations.py
+-rw-r--r--   0        0        0      716 2023-12-20 13:35:51.846131 bragir-1.0.3/bragir/languages.py
+-rw-r--r--   0        0        0      600 2023-12-22 14:10:13.429766 bragir-1.0.3/bragir/list.py
+-rw-r--r--   0        0        0        0 2024-03-18 10:05:22.473895 bragir-1.0.3/bragir/logging_configs/__init__.py
+-rw-r--r--   0        0        0      810 2024-03-18 09:47:41.850387 bragir-1.0.3/bragir/logging_configs/debug.json
+-rw-r--r--   0        0        0      539 2024-03-18 09:47:41.862007 bragir-1.0.3/bragir/logging_configs/info.json
+-rw-r--r--   0        0        0      534 2023-12-22 13:19:39.955616 bragir-1.0.3/bragir/messages.py
+-rw-r--r--   0        0        0      343 2024-03-13 09:40:37.372753 bragir-1.0.3/bragir/path.py
+-rw-r--r--   0        0        0     2135 2024-04-11 08:34:28.665242 bragir-1.0.3/bragir/spinner/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-23 14:46:22.975414 bragir-1.0.3/bragir/srt/__init__.py
+-rw-r--r--   0        0        0      500 2024-01-23 14:41:02.577972 bragir-1.0.3/bragir/srt/srt_part.py
+-rw-r--r--   0        0        0     1599 2024-03-13 13:47:55.802026 bragir-1.0.3/bragir/time.py
+-rw-r--r--   0        0        0      476 2024-03-13 13:47:55.802184 bragir-1.0.3/bragir/timer.py
+-rw-r--r--   0        0        0       44 2024-03-13 13:47:55.802328 bragir-1.0.3/bragir/tracing/__init__.py
+-rw-r--r--   0        0        0      213 2024-03-13 13:47:55.802449 bragir-1.0.3/bragir/tracing/logger.py
+-rw-r--r--   0        0        0      695 2024-03-18 10:06:12.584707 bragir-1.0.3/bragir/tracing/stratergies.py
+-rw-r--r--   0        0        0     1156 2024-03-13 13:47:55.802783 bragir-1.0.3/bragir/transcription/__init__.py
+-rw-r--r--   0        0        0     1830 2024-04-11 08:26:02.417038 bragir-1.0.3/bragir/translation/__init__.py
+-rw-r--r--   0        0        0       98 2024-03-14 15:10:23.607211 bragir-1.0.3/bragir/types.py
+-rw-r--r--   0        0        0      498 2024-04-11 08:41:48.704219 bragir-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 bragir-1.0.3/PKG-INFO
```

### Comparing `bragir-1.0.2/LICENSE` & `bragir-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/README.md` & `bragir-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/__main__.py` & `bragir-1.0.3/bragir/__main__.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/audio/chunking.py` & `bragir-1.0.3/bragir/audio/chunking.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/audio/grouping.py` & `bragir-1.0.3/bragir/audio/grouping.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/client.py` & `bragir-1.0.3/bragir/client.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/commands.py` & `bragir-1.0.3/bragir/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from bragir.file import (
     chunk_content,
     chunk_content_into_srt_parts,
     get_new_file_path,
     process_files,
 )
 from bragir.files.file import File
-from bragir.files.operations import create_file
+from bragir.files.operations import create_file, read_file
 from bragir.languages import Languages, parse_languages
 from bragir.spinner import spinner
 from bragir.tracing.logger import logger
 from bragir.messages import PROMPT_HELP
 from bragir.path import get_target_path
 from bragir.srt.srt_part import SRTPart
 from bragir.time import update_timestamps
@@ -139,21 +139,24 @@
         for target_language in translate_to_languages:
             logger.info(
                 f"Adding file {path} with {target_language.value} for translation"
             )
 
             target_path = get_new_file_path(path, target_language)
 
-            (contents, breakpoints) = chunk_content(path)
+            file_content = read_file(path)
+
+            (srt_parts, breakpoints) = chunk_content(file_content)
 
             files.append(
                 File(
                     name=path,
+                    contents=file_content,
                     language=target_language,
-                    SRTParts=contents,
+                    SRTParts=srt_parts,
                     breakpoints=breakpoints,
                     target_path=target_path,
                     source_path=path,
                 )
             )
 
     if path_is_directory:
```

### Comparing `bragir-1.0.2/bragir/config/config.py` & `bragir-1.0.3/bragir/config/config.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/constants/__init__.py` & `bragir-1.0.3/bragir/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/directory.py` & `bragir-1.0.3/bragir/directory.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/file.py` & `bragir-1.0.3/bragir/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     return new_file_path
 
 
 def chunk_content_into_srt_parts(content: str) -> list[SRTPart]:
     blocks = content.strip().split("\n\n")
 
     SRTParts: list[SRTPart] = []
+
     for block in blocks:
         lines = block.split("\n")
 
         number = int(lines[0])
         times = lines[1].split(" --> ")
         start_time, end_time = times[0], times[1]
         text = " ".join(lines[2:])
@@ -89,45 +90,44 @@
             next_srt_part.content = last_sentence + " " + next_srt_part.content
 
             buffer = 0
 
     return breakpoints
 
 
-def chunk_content(file_path: str) -> tuple[list[SRTPart], list[int]]:
-    file_content = read_file(file_path)
-
-    SRTParts: list[SRTPart] = chunk_content_into_srt_parts(file_content)
+def chunk_content(file_content: str) -> tuple[list[SRTPart], list[int]]:
+    srt_parts: list[SRTPart] = chunk_content_into_srt_parts(file_content)
 
-    breakpoints: list[int] = get_breakpoints(SRTParts)
+    breakpoints: list[int] = get_breakpoints(srt_parts)
 
-    return (SRTParts, breakpoints)
+    return (srt_parts, breakpoints)
 
 
 def process_files(file_paths: list[str], languages: list[Languages]) -> list[File]:
     processed_files: list[File] = []
-    res: list[File] = []
     for file_path in file_paths:
-        (content, breakpoints) = chunk_content(file_path)
+        file_content = read_file(file_path)
+        (srt_parts, breakpoints) = chunk_content(file_content)
         for language in languages:
             base_path, file_name = os.path.split(file_path)
             updated_file_name = f"{language.value.lower()[:3]}_{file_name}"
             new_file_path = os.path.join(base_path, updated_file_name)
             file = File(
                 name=file_path,
                 language=language,
-                SRTParts=content,
+                SRTParts=srt_parts,
                 breakpoints=breakpoints,
                 target_path=new_file_path,
                 source_path=file_path,
+                contents=file_content,
             )
 
             processed_files.append(file)
 
-    return res
+    return processed_files
 
 
 def process_file(file_path: str) -> list[str]:
     _, file_extension = os.path.splitext(file_path)
     file_extension = file_extension.lower().replace(".", "")
 
     chunks = chunk_audio(file_path, format=file_extension)
```

### Comparing `bragir-1.0.2/bragir/files/file.py` & `bragir-1.0.3/bragir/files/file.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/languages.py` & `bragir-1.0.3/bragir/languages.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/list.py` & `bragir-1.0.3/bragir/list.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/logging_configs/debug.json` & `bragir-1.0.3/bragir/logging_configs/debug.json`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/logging_configs/info.json` & `bragir-1.0.3/bragir/logging_configs/info.json`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/messages.py` & `bragir-1.0.3/bragir/messages.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/spinner/__init__.py` & `bragir-1.0.3/bragir/spinner/__init__.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/time.py` & `bragir-1.0.3/bragir/time.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/tracing/stratergies.py` & `bragir-1.0.3/bragir/tracing/stratergies.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/transcription/__init__.py` & `bragir-1.0.3/bragir/transcription/__init__.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/bragir/translation/__init__.py` & `bragir-1.0.3/bragir/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `bragir-1.0.2/PKG-INFO` & `bragir-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bragir
-Version: 1.0.2
+Version: 1.0.3
 Summary: bragir translator cli
 License: MIT
 Author: Andreas Bergman
 Author-email: andreas@arjancodes.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

