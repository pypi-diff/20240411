# Comparing `tmp/commits2pdf-1.1.6.tar.gz` & `tmp/commits2pdf-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commits2pdf-1.1.6.tar", last modified: Tue Apr  9 05:56:03 2024, max compression
+gzip compressed data, was "commits2pdf-1.1.7.tar", last modified: Thu Apr 11 06:39:42 2024, max compression
```

## Comparing `commits2pdf-1.1.6.tar` & `commits2pdf-1.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 05:56:03.018548 commits2pdf-1.1.6/
--rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.1.6/LICENCE.md
--rw-rw-rw-   0        0        0     7987 2024-04-09 05:56:03.017551 commits2pdf-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7101 2024-04-09 05:31:15.000000 commits2pdf-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 05:56:03.008576 commits2pdf-1.1.6/commits2pdf/
--rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.1.6/commits2pdf/__init__.py
--rw-rw-rw-   0        0        0    10749 2024-04-09 05:21:34.000000 commits2pdf-1.1.6/commits2pdf/cli.py
--rw-rw-rw-   0        0        0    13084 2024-04-09 05:04:37.000000 commits2pdf-1.1.6/commits2pdf/commits.py
--rw-rw-rw-   0        0        0     3244 2024-04-09 05:38:04.000000 commits2pdf-1.1.6/commits2pdf/constants.py
--rw-rw-rw-   0        0        0      308 2024-04-07 03:56:00.000000 commits2pdf-1.1.6/commits2pdf/logger.py
--rw-rw-rw-   0        0        0     7100 2024-04-07 10:55:21.000000 commits2pdf-1.1.6/commits2pdf/render_cairo.py
--rw-rw-rw-   0        0        0    10136 2024-04-09 05:52:47.000000 commits2pdf-1.1.6/commits2pdf/render_fpdf.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:56:03.016554 commits2pdf-1.1.6/commits2pdf.egg-info/
--rw-rw-rw-   0        0        0     7987 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 05:56:03.019545 commits2pdf-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1223 2024-04-09 05:55:47.000000 commits2pdf-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:39:42.271887 commits2pdf-1.1.7/
+-rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.1.7/LICENCE.md
+-rw-rw-rw-   0        0        0     8340 2024-04-11 06:39:42.270891 commits2pdf-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7454 2024-04-10 07:27:14.000000 commits2pdf-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 06:39:42.252431 commits2pdf-1.1.7/commits2pdf/
+-rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.1.7/commits2pdf/__init__.py
+-rw-rw-rw-   0        0        0    10749 2024-04-09 05:21:34.000000 commits2pdf-1.1.7/commits2pdf/cli.py
+-rw-rw-rw-   0        0        0    13044 2024-04-11 06:34:51.000000 commits2pdf-1.1.7/commits2pdf/commits.py
+-rw-rw-rw-   0        0        0     3264 2024-04-11 06:17:00.000000 commits2pdf-1.1.7/commits2pdf/constants.py
+-rw-rw-rw-   0        0        0      308 2024-04-07 03:56:00.000000 commits2pdf-1.1.7/commits2pdf/logger.py
+-rw-rw-rw-   0        0        0     7100 2024-04-07 10:55:21.000000 commits2pdf-1.1.7/commits2pdf/render_cairo.py
+-rw-rw-rw-   0        0        0    10118 2024-04-11 06:35:28.000000 commits2pdf-1.1.7/commits2pdf/render_fpdf.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:39:42.268894 commits2pdf-1.1.7/commits2pdf.egg-info/
+-rw-rw-rw-   0        0        0     8340 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-11 06:39:42.000000 commits2pdf-1.1.7/commits2pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 06:39:42.271887 commits2pdf-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1223 2024-04-11 06:37:14.000000 commits2pdf-1.1.7/setup.py
```

### Comparing `commits2pdf-1.1.6/LICENCE.md` & `commits2pdf-1.1.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.1.6/PKG-INFO` & `commits2pdf-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commits2pdf
-Version: 1.1.6
+Version: 1.1.7
 Summary: View a filtered commit history in PDF form.
 Home-page: https://github.com/tomasvana10/commits2pdf
 Author: Tomas Vana
 License: MIT
 Platform: any
 Classifier: Topic :: Multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,16 +29,30 @@
 <br><br>
 ## Dependencies
 `pycairo`<br>
 `GitPython`<br>
 `fpdf`
 <br><br>
 ## Installation
-`pip install commits2pdf` or<br>
-`pip3 install commits2pdf`<br>
+**Requires [pip](https://pip.pypa.io/en/stable/installation/)**
+
+Make a virtual environment (recommended)
+```
+pip install virtualenv OR pip3 install virtualenv
+python -m venv venv OR python3 -m venv venv
+ON MACOS/UNIX: source venv/bin/activate
+ON WINDOW: venv\scripts\activate
+```
+
+Install the package:
+```
+pip install commits2pdf OR pip3 install commits2pdf
+```
+**Scroll down for usage information**.
+
 If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)
 <br><br>
 ## Command-line parameters
 ```
   -h, --help            show this help message and exit
   -O OWNER, --owner OWNER
                         The owner of the git repository. Required.
```

### Comparing `commits2pdf-1.1.6/README.md` & `commits2pdf-1.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,30 @@
 <br><br>
 ## Dependencies
 `pycairo`<br>
 `GitPython`<br>
 `fpdf`
 <br><br>
 ## Installation
-`pip install commits2pdf` or<br>
-`pip3 install commits2pdf`<br>
+**Requires [pip](https://pip.pypa.io/en/stable/installation/)**
+
+Make a virtual environment (recommended)
+```
+pip install virtualenv OR pip3 install virtualenv
+python -m venv venv OR python3 -m venv venv
+ON MACOS/UNIX: source venv/bin/activate
+ON WINDOW: venv\scripts\activate
+```
+
+Install the package:
+```
+pip install commits2pdf OR pip3 install commits2pdf
+```
+**Scroll down for usage information**.
+
 If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)
 <br><br>
 ## Command-line parameters
 ```
   -h, --help            show this help message and exit
   -O OWNER, --owner OWNER
                         The owner of the git repository. Required.
```

### Comparing `commits2pdf-1.1.6/commits2pdf/cli.py` & `commits2pdf-1.1.7/commits2pdf/cli.py`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.1.6/commits2pdf/commits.py` & `commits2pdf-1.1.7/commits2pdf/commits.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from os import path, listdir
 from datetime import datetime
 from shutil import rmtree
-from typing import List, Union, Dict
+from typing import List, Optional, Dict, Union
 
 from git import Repo, GitCommandError, InvalidGitRepositoryError
 
 from .logger import logger
 from .constants import (
     REPO_ALREADY_EXISTS_WARNING, DETACHED_BRANCH_ERROR, 
     BRANCH_ALREADY_EXISTS_WARNING, INVALID_REPO_ERROR, INVALID_REPO_ERROR_2,
-    FILTER_INFO, N_COMMITS_INFO, N_COMMITS_WARN, GATHERED_COMMITS_INFO
+    FILTER_INFO, N_COMMITS_INFO, N_COMMITS_WARN, GATHERED_COMMITS_INFO, CODING
 )
 
 
 class Commits(object):
     """Represents a filtered set of commits along with filter information."""
     def __init__(self, **kwargs) -> None:
         """Save filter and repo information from kwargs."""
         self.err_flag: bool = False # Detected in ``cli.py`` to stop execution
         
         self.rpath: str = kwargs["rpath"]
         self.owner: str = kwargs["owner"]
-        self.url: Union[str, None] = kwargs["url"]
-        self.branch: Union[str, None] = kwargs["branch"]
-        self.authors: Union[List[str], None] = kwargs["authors"]
-        self.start_date: Union[datetime, None] = kwargs["start_date"]
-        self.end_date: Union[datetime, None] = kwargs["end_date"]
-        self.reverse: bool = kwargs["reverse"]
-        self.newest_n_commits: int = kwargs["newest_n_commits"]
-        self.oldest_n_commits: int= kwargs["oldest_n_commits"]
-        self.queries_any: List[str] = kwargs["queries_any"]
-        self.queries_all: List[str] = kwargs["queries_all"]
+        self.url: Optional[str] = kwargs["url"]
+        self.branch: Optional[str] = kwargs["branch"]
+        self.authors: Optional[List[str]] = kwargs["authors"]
+        self.start_date: Optional[datetime] = kwargs["start_date"]
+        self.end_date: Optional[datetime] = kwargs["end_date"]
+        self.reverse: Optional[bool] = kwargs["reverse"]
+        self.newest_n_commits: Optional[int] = kwargs["newest_n_commits"]
+        self.oldest_n_commits: Optional[int] = kwargs["oldest_n_commits"]
+        self.queries_any: Option[List[str]] = kwargs["queries_any"]
+        self.queries_all: Optional[List[str]] = kwargs["queries_all"]
 
         self.r: Repo = self.get_repo()  
         if isinstance(self.r, Repo): # Repo was successfully found, continue
             self.init_repo_data()
         elif self.r == "deltree": # Buffered deletion due to errors in
                                   # ``get_repo``.
             rmtree(self.rpath, ignore_errors=True)
@@ -161,15 +161,15 @@
                 rev=self.branch,
             )
         )
         logger.info(GATHERED_COMMITS_INFO.format(len(commits)))
         
         return commits
     
-    def instantiate_commits(self) -> List[Dict[str, str]]: # Can't use ``Commit`` yet bruh
+    def instantiate_commits(self) -> List[Dict[str, str]]: 
         """Instantiate all the filtered ``Repo.commit`` objects into my own
         simple class that inherits from a dictionary.
         """
         commit_objects = []
         for commit in self.raw_commits:
             commit_objects.append(Commit(self.owner, self.rname, self.branch, 
                                          commit))
@@ -217,39 +217,42 @@
         step = -1 if not self.reverse else 1
         filtered_commits = filtered_commits[::step] 
         
         return filtered_commits
 
 class Commit(dict):
     """A simple way of representing a commit as a dictionary."""
-    def __init__(self, owner, rname, branch, commit: Repo.commit):
+    def __init__(self, 
+                 owner: str, 
+                 rname: str, 
+                 branch: str, 
+                 commit: Repo.commit):
         """Assign commit data to the instance."""
         self["rname"] = rname 
         self["branch"] = branch
         self["author_name"] = commit.author
         self["author_email"] = commit.author.email
         self["date"] = datetime.fromtimestamp(commit.committed_date)
         self["hexsha_short"] = commit.hexsha[:7]
         self["hexsha_long"] = commit.hexsha
         self["diff_url"] = f"https://github.com/{owner}/{rname}/commit/{commit.hexsha}"
 
         self["info"] = f"{self['hexsha_short']} | Branch: {self['branch']} | " \
                        f"By {self['author_name']} ({self['author_email']}) | " \
                        f"At {self['date'].strftime('%Y-%m-%d')}"
+        self["info"] = Commit._code(self["info"])
          
         # Extract the message from the title
         msg = commit.message.split("\n")
-        self["title"] = msg[0].encode("latin-1", errors="replace")\
-                                                            .decode("latin-1")
-        if len(msg) > 1:
-            self["description"] = "\n".join(msg[1:]).encode("latin-1", 
-                                                            errors="replace")\
-                                                            .decode("latin-1")
-        else:
-            self["description"] = ""
+        self["title"] = Commit._code(msg[0])
+        self["description"] = Commit._code("\n".join(msg[1:])) if len(msg) > 1 else ""
+    
+    @staticmethod
+    def _code(text, coding=CODING):
+        return text.encode(CODING, "replace").decode(CODING)
     
     def __str__(self): 
         """View the commit in the terminal."""
         return \
             "=============================\n" \
             f"Repository: {self['rname']}\n" \
             f"{self['info']}\n" \
```

### Comparing `commits2pdf-1.1.6/commits2pdf/constants.py` & `commits2pdf-1.1.7/commits2pdf/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 HEIGHT = 792
 MARGIN = 50
 
 
 """For the fpdf PDF implementation"""
 RECURSION_ERROR = "An error occured when using the gen2b renderer. Please try " \
                   "adding the -gen2a flag to your console command and try again."
+CODING = "latin-1"
 TITLE_FONT = ["Arial", "B", 36]
 SUBTITLE_FONT = ["Arial", "", 30]
 MARGIN_FONT = ["Arial", "I", 8]
 SMALL_TEXT_FONT = ["Arial", "", 12]
 MEDIUM_TEXT_FONT = ["Arial", "", 16]
 TITLE_PAGE_INFO_FONT = ["Courier", "", 15]
 MEDIUM_TEXT_FONT_BOLD = ["Arial", "B", 16]
```

### Comparing `commits2pdf-1.1.6/commits2pdf/render_cairo.py` & `commits2pdf-1.1.7/commits2pdf/render_cairo.py`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.1.6/commits2pdf/render_fpdf.py` & `commits2pdf-1.1.7/commits2pdf/render_fpdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 else:
                     self._draw_commit(commit)
         elif self._mode == "stable":
             for commit in self._commits.filtered_commits:
                 if self._commit_exceeds_size(commit):
                     self.add_page()
                     self._draw_page_bg()
-                self._draw_commit(commit)        
+                self._draw_commit(commit)
             
     def _draw_commit(self, 
                      commit: Dict[str, str], 
                      pre_vis: bool = False, 
                      no_divider: bool = False
                      ) -> Union[str, None]:
         """Draw all the parts of a commit to the current ``FPDF`` instance
@@ -130,15 +130,14 @@
             try:
                 p = loads(dumps(self))
             except RecursionError: # Why this happen bruh?!
                 logger.error(RECURSION_ERROR)
                 self.recursion_err_flag = True
                 exit(1)
             
-        
         y: int = p.get_y()
         p.set_text_color(*self._ap["text"])
         p._set_font(*INFO_TEXT_FONT)
         p.multi_cell(w=0, h=p.font_size * 1.25, align="C", txt=commit["info"])
         p.ln(p.font_size * 0.75)
         # Tells the driver code that it must add a page
         if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new"
```

### Comparing `commits2pdf-1.1.6/commits2pdf.egg-info/PKG-INFO` & `commits2pdf-1.1.7/commits2pdf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commits2pdf
-Version: 1.1.6
+Version: 1.1.7
 Summary: View a filtered commit history in PDF form.
 Home-page: https://github.com/tomasvana10/commits2pdf
 Author: Tomas Vana
 License: MIT
 Platform: any
 Classifier: Topic :: Multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,16 +29,30 @@
 <br><br>
 ## Dependencies
 `pycairo`<br>
 `GitPython`<br>
 `fpdf`
 <br><br>
 ## Installation
-`pip install commits2pdf` or<br>
-`pip3 install commits2pdf`<br>
+**Requires [pip](https://pip.pypa.io/en/stable/installation/)**
+
+Make a virtual environment (recommended)
+```
+pip install virtualenv OR pip3 install virtualenv
+python -m venv venv OR python3 -m venv venv
+ON MACOS/UNIX: source venv/bin/activate
+ON WINDOW: venv\scripts\activate
+```
+
+Install the package:
+```
+pip install commits2pdf OR pip3 install commits2pdf
+```
+**Scroll down for usage information**.
+
 If you encounter errors with building `pycairo`, click [here](https://stackoverflow.com/a/76175684/23245953)
 <br><br>
 ## Command-line parameters
 ```
   -h, --help            show this help message and exit
   -O OWNER, --owner OWNER
                         The owner of the git repository. Required.
```

### Comparing `commits2pdf-1.1.6/setup.py` & `commits2pdf-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="commits2pdf",
-    version="1.1.6",
+    version="1.1.7",
     author="Tomas Vana",
     url="https://github.com/tomasvana10/commits2pdf",
     description="View a filtered commit history in PDF form.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     license="MIT",
```

