# Comparing `tmp/summaraize-0.1.tar.gz` & `tmp/summaraize-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summaraize-0.1.tar", last modified: Mon Apr  8 19:46:22 2024, max compression
+gzip compressed data, was "summaraize-0.2.tar", last modified: Wed Apr 10 20:33:30 2024, max compression
```

## Comparing `summaraize-0.1.tar` & `summaraize-0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:46:22.830962 summaraize-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 19:46:15.000000 summaraize-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-08 19:46:22.830962 summaraize-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-08 19:46:15.000000 summaraize-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 19:46:15.000000 summaraize-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:46:22.830962 summaraize-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-08 19:46:15.000000 summaraize-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:46:22.822962 summaraize-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:46:22.826962 summaraize-0.1/src/summaraize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:46:22.830962 summaraize-0.1/src/summaraize/ui/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/api_key_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/ffmpeg_error_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/show_summary_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/summarize_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-08 19:46:15.000000 summaraize-0.1/src/summaraize/ui/upload_recording_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:46:22.830962 summaraize-0.1/src/summaraize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-08 19:46:22.000000 summaraize-0.1/src/summaraize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 19:46:22.000000 summaraize-0.1/src/summaraize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:46:22.000000 summaraize-0.1/src/summaraize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 19:46:22.000000 summaraize-0.1/src/summaraize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 19:46:22.000000 summaraize-0.1/src/summaraize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:33:30.903943 summaraize-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 20:33:23.000000 summaraize-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-10 20:33:30.903943 summaraize-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-10 20:33:23.000000 summaraize-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 20:33:23.000000 summaraize-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:33:30.903943 summaraize-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-10 20:33:23.000000 summaraize-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:33:30.899943 summaraize-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:33:30.899943 summaraize-0.2/src/summaraize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:33:30.903943 summaraize-0.2/src/summaraize/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/api_key_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/ffmpeg_error_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/show_summary_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/summarize_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-10 20:33:23.000000 summaraize-0.2/src/summaraize/ui/upload_recording_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:33:30.903943 summaraize-0.2/src/summaraize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-10 20:33:30.000000 summaraize-0.2/src/summaraize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 20:33:30.000000 summaraize-0.2/src/summaraize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:33:30.000000 summaraize-0.2/src/summaraize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 20:33:30.000000 summaraize-0.2/src/summaraize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 20:33:30.000000 summaraize-0.2/src/summaraize.egg-info/top_level.txt
```

### Comparing `summaraize-0.1/LICENSE` & `summaraize-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `summaraize-0.1/setup.py` & `summaraize-0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from setuptools import setup, find_packages
+![example workflow](https://github.com/juslop/summaraize/actions/workflows/python-publish.yml/badge.svg)
+# SummarAIze
 
-long_description = """
-SummarAIze is a Python library for analyzing meeting/event video recordings with cloud hosted AI.
+A Python library for analyzing and summarizing meeting/event video recordings with cloud hosted AI.
+![minutes-screenshot-1](https://github.com/juslop/minutes/assets/1512110/9e390eb2-05c9-466f-b05e-c622ddb0b3a8)
+![minutes-screenshot-2](https://github.com/juslop/minutes/assets/1512110/05e7b7ef-d61d-4a0a-be98-e6ee90739e3c)
 
 Save time and enhance efficiency by using AI to generate summaries, battle cards, meeting minutes, 
 sales arguments and action item lists directly from recordings.
 Hone your prompt engineering skills to distill the desired information.
 
 ## Technology
 
@@ -30,19 +32,19 @@
 Portuguese, Romanian, Russian, Serbian, Slovak, Slovenian, Spanish, Swahili, Swedish, Tagalog,
 Tamil, Thai, Turkish, Ukrainian, Urdu, Vietnamese, and Welsh.
 
 ## Requirements
 
 - Ffmpeg needs to be installed and set in path. https://ffmpeg.org
 - OpenAI API key to access Whisper and GPT4-Turbo models. https://platform.openai.com/docs/quickstart
-- Python3.7 or newer
+- Python3.10 or newer
 
 ## Install Application
 
-```python
+```bash
 python -m pip install summaraize
 ```
 
 ## Install FFmpeg
 
 **Mac**
 
@@ -60,48 +62,49 @@
 FFmpeg: https://ffmpeg.org//download.html#build-linux
 
 Many Linux python distributions lack tkinter. Use distro package manager to install.
 Note: Tkinter package name varies between distros.
 
 ## Run
 
-```python
+```bash
 python -m summaraize
 ```
 
+## Usage
+
+1. Application will ask for OpenAI API key. Provide the API key
+   - alternatively set OPENAI_API_KEY environment variable
+2. Application will ask to select language and video recording file
+   - video recording file is processed into a text transcipt
+   - this may take several minutes
+4. Application will ask a prompt to instruct ChatGPT4-turbo to extract the information from the transcript
+   - this is called prompt engineering
+   - try different prompts to see what works and what not
+   - after prompt is ready, application will deliver prompt and the transcript to ChatGPT
+   - creating summary in most cases takes less than a minute
+5. Application will show the ChatGPT4-turbo created summary
+   - you can copy the summary to clipboard or save the summary to a file. ChatGPT answers in markdown
+     (md) format. You can ask bulleted or numbered lists and so on.
+   - make a new summary by returning to summary view
+   - application will answer in the language you selected unless you instruct otherwise in prompt
+   - the application user interface texts are only in english
+6. Close the application by closing the window
+   - note application will not save the text transcript
+   - to analyze other recording file, restart the application
+
 ## UI themes
 
 Application support UI themes from:
 https://ttkbootstrap.readthedocs.io/en/latest/themes/
 
 list available themes:
 
-```python
+```bash
 python -m summaraize -h
 ```
 
 use a theme by giving theme name as an argument:
 
-```python
+```bash
 python -m summaraize cyborg
 ```
-
-"""
-
-setup(
-    name="summaraize",
-    version="0.1",
-    author="Jussi Löppönen",
-    description="A Python library for analyzing meeting/event video recordings with cloud hosted AI.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    url="https://github.com/juslop/summaraize",
-    packages=find_packages(where="src"),
-    package_dir = {"": "src"},
-    install_requires=["openai", "ttkbootstrap"],
-    python_requires=">=3.7",
-)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `summaraize-0.1/src/summaraize/__main__.py` & `summaraize-0.2/src/summaraize/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module enables running package with pck name
+Module enables running package with pkg name
 """
 import argparse
 from .ui import App
 
 
 def main():
     """
@@ -20,13 +20,14 @@
     )
     parser.add_argument('theme', nargs='?',
                         choices=ttkbootstrap_themes, default="sandstone",
                         help="ttkbootstrap theme, (default: %(default)s)")
     args = parser.parse_args()
     app = App(args.theme)
     app.mainloop()
-    app.task_queue.put(None)
-    app.worker_thread.join()
+    if app.task_queue is not None:
+        app.task_queue.put(None)
+        app.worker_thread.join()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `summaraize-0.1/src/summaraize/summarize.py` & `summaraize-0.2/src/summaraize/summarize.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 """
 
 logger = logging.getLogger(__name__)
 
 
 class Summarize:
     """
-    Convert a video recording to a summary transcript and use the OpenAI API to
-    analyze it.
-    FFmpeg needs to be installed and set in path
+    Convert a video recording to a text transcript with FFmpeg locally
+    and OpenAI Whisper.
+    Create summaries based on user prompt and transcript with
+    OpenAI ChatGPT4-turbo.
+    FFmpeg needs to be installed and set in path.
     """
     def __init__(self,
         task_queue: Union[queue.Queue, None] = None,
         result_queue:Union[queue.Queue, None] = None
     ) -> None:
         self.task_queue = task_queue
         self.result_queue = result_queue
```

### Comparing `summaraize-0.1/src/summaraize/ui/api_key_page.py` & `summaraize-0.2/src/summaraize/ui/api_key_page.py`

 * *Files identical despite different names*

### Comparing `summaraize-0.1/src/summaraize/ui/config.py` & `summaraize-0.2/src/summaraize/ui/config.py`

 * *Files identical despite different names*

### Comparing `summaraize-0.1/src/summaraize/ui/ffmpeg_error_page.py` & `summaraize-0.2/src/summaraize/ui/ffmpeg_error_page.py`

 * *Files identical despite different names*

### Comparing `summaraize-0.1/src/summaraize/ui/markdown.py` & `summaraize-0.2/src/summaraize/ui/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable-all
+"""
+Unchanged from:
+https://stackoverflow.com/questions/35733300/how-to-show-markdown-formatted-text-in-tkinter
+"""
 import re
 import tkinter.font as tkfont
 import tkinter.scrolledtext as tkscroll
 
 
 class SimpleMarkdownText(tkscroll.ScrolledText):
     """
-    https://stackoverflow.com/questions/35733300/how-to-show-markdown-formatted-text-in-tkinter
     Really basic Markdown display. Thanks to Bryan Oakley's RichText:
     https://stackoverflow.com/a/63105641/79125
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         default_font = tkfont.nametofont(self.cget("font"))
```

### Comparing `summaraize-0.1/src/summaraize/ui/show_summary_page.py` & `summaraize-0.2/src/summaraize/ui/show_summary_page.py`

 * *Files identical despite different names*

### Comparing `summaraize-0.1/src/summaraize/ui/summarize_page.py` & `summaraize-0.2/src/summaraize/ui/summarize_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,8 +68,8 @@
                 Messagebox.show_error(
                     f"Error: {str(result)}", "Failed to create summary",
                     alert=True, width=200)
             else:
                 Messagebox.show_error(
                     f"Internal Server Error: {type(result)} rxd from queue",
                     "Failed to create summary", alert=True, width=200)
-            self.master.switch_frame(SummarisePage)
+            self.master.switch_frame(SummarisePage.__name__)
```

### Comparing `summaraize-0.1/src/summaraize/ui/ui.py` & `summaraize-0.2/src/summaraize/ui/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .api_key_page import ApiKeyPage
 from .upload_recording_page import UploadRecordingPage
 from .summarize_page import SummarisePage
 from .show_summary_page import ShowSummaryPage
 from ..summarize import Summarize
 
 logger = logging.getLogger(__name__)
+# helper to avoid circular imports
 PAGES = {x.__name__:x for x in
          [FfmpegErrorPage, UploadRecordingPage,
           SummarisePage, ShowSummaryPage,
           ApiKeyPage]}
 
 
 @dataclasses.dataclass
@@ -78,38 +79,37 @@
         try:
             self.summarize = Summarize(self.task_queue, self.result_queue)
         # pylint: disable=broad-exception-caught
         except Exception as e:
             logger.error("Failed to contact OpenAI: %s", str(e))
             sys.exit(1)
         self.title('Summarize Transcript')
-        self.geometry("700x800")
+        self.geometry("800x800")
         self._frame = None
         btn_style = ttk.Style()
         btn_style.configure("TButton", font=("Helvetica", 16, "bold"))
         try:
             self.summarize.check_ffmpeg_present()
         except RuntimeError:
-            self.switch_frame(FfmpegErrorPage)
+            self.switch_frame(FfmpegErrorPage.__name__)
             return
         self.params = Params()
         self.worker_thread = threading.Thread(target=self.summarize.run)
         self.worker_thread.start()
 
         if self.summarize.client is None:
-            self.switch_frame("ApiKeyPage")
+            self.switch_frame(ApiKeyPage.__name__)
         else:
-            self.switch_frame("UploadRecordingPage")
+            self.switch_frame(UploadRecordingPage.__name__)
 
     def switch_frame(self, frame_class_name: str) -> None:
         """Destroys current frame and replaces it with a new one."""
         try:
             frame_class = PAGES[frame_class_name]
         except KeyError:
-            # pylint: disable=logging-fstring-interpolation
-            logger.error(f"unknown page {frame_class_name}")
+            logger.error("unknown page %s", frame_class_name)
             sys.exit(1)
         new_frame = frame_class(self)
         if self._frame is not None:
             self._frame.destroy()
         self._frame = new_frame
         self._frame.pack()
```

### Comparing `summaraize-0.1/src/summaraize/ui/upload_recording_page.py` & `summaraize-0.2/src/summaraize/ui/upload_recording_page.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         elif isinstance(result, str):
             self.master.params.transcript = result
             self.master.switch_frame("SummarisePage")
         else:
             self.progress['value'] = 0
             self.selector_btn["state"] = "normal"
             self.spinner.config(text="")
-            self.file_path = ""
             if isinstance(result, Exception):
                 Messagebox.show_error(
                     f"Creating Transcript of {self.file_path} failed.\nError: {result}",
                     "Failed to create transcript", alert=True, width=200)
             else:
                 Messagebox.show_error(
                     "Creating Transcript failed.\nError: Internal Server Error",
                     "Failed to create transcript", alert=True, width=200)
+            self.file_path = ""
```

### Comparing `summaraize-0.1/src/summaraize.egg-info/SOURCES.txt` & `summaraize-0.2/src/summaraize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

