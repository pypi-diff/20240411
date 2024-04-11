# Comparing `tmp/os2024-0.5.0.tar.gz` & `tmp/os2024-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2024-0.5.0.tar", max compression
+gzip compressed data, was "os2024-0.6.0.tar", max compression
```

## Comparing `os2024-0.5.0.tar` & `os2024-0.6.0.tar`

### file list

```diff
@@ -1,51 +1,60 @@
--rw-r--r--   0        0        0    18656 2024-04-02 21:03:49.262368 os2024-0.5.0/LICENSE
--rw-r--r--   0        0        0     3892 2024-04-02 21:03:49.262368 os2024-0.5.0/README.md
--rw-r--r--   0        0        0     3573 2024-04-02 21:04:07.682755 os2024-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2311 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/__cli__.py
--rw-r--r--   0        0        0      338 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/__init__.py
--rw-r--r--   0        0        0       22 2024-04-02 21:04:07.642754 os2024-0.5.0/src/os2024/_version.py
--rw-r--r--   0        0        0     3806 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/_config.yml
--rw-r--r--   0        0        0     1930 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/_toc.yml
--rw-r--r--   0        0        0    22523 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/about/images/yjlee.jpeg
--rw-r--r--   0        0        0     1476 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/about/index.md
--rw-r--r--   0        0        0        0 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/assets/assets/extra/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/assets/extra/.gitkeep
--rw-r--r--   0        0        0     3949 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/index.md
--rw-r--r--   0        0        0     7547 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep/index.md
--rw-r--r--   0        0        0     1967 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep-code/index.md
--rw-r--r--   0        0        0    11719 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep-homework/index.md
--rw-r--r--   0        0        0     3977 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep-projects/index.md
--rw-r--r--   0        0        0        9 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references.bib
--rw-r--r--   0        0        0      205 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/requirements.txt
--rw-r--r--   0        0        0     6229 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/syllabus/index.md
--rw-r--r--   0        0        0     2770 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/week01/index.md
--rw-r--r--   0        0        0    26071 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week01/intro.md
--rw-r--r--   0        0        0     9466 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/cpu-api.md
--rw-r--r--   0        0        0    16683 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/cpu-intro.md
--rw-r--r--   0        0        0    20945 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/cpu-mechanisms.md
--rw-r--r--   0        0        0     2830 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/index.md
--rw-r--r--   0        0        0     4976 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/lab.md
--rw-r--r--   0        0        0     4284 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/shells.md
--rw-r--r--   0        0        0     2795 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/tip.md
--rw-r--r--   0        0        0    19638 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/cpu-scheduling.md
--rw-r--r--   0        0        0    49905 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/figs/fcfs.png
--rw-r--r--   0        0        0       53 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/index.md
--rw-r--r--   0        0        0    15505 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/lab.md
--rw-r--r--   0        0        0     3518 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/wsl-setup.md
--rw-r--r--   0        0        0     3501 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/index.md
--rw-r--r--   0        0        0     6608 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/lab-lottery.md
--rw-r--r--   0        0        0     9209 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/lab-sched.md
--rw-r--r--   0        0        0    24596 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/lottery.md
--rw-r--r--   0        0        0    28602 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/mlfq.md
--rw-r--r--   0        0        0   202834 2024-04-02 21:03:49.270368 os2024-0.5.0/src/os2024/book/week05/figs/os_img_1.png
--rw-r--r--   0        0        0   475305 2024-04-02 21:03:49.270368 os2024-0.5.0/src/os2024/book/week05/figs/os_img_2.png
--rw-r--r--   0        0        0    87376 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/figs/os_img_3.png
--rw-r--r--   0        0        0     3581 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/index.md
--rw-r--r--   0        0        0     3753 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/lab.md
--rw-r--r--   0        0        0     5279 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/tip-linux-cmd.md
--rw-r--r--   0        0        0    13121 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/vm-api.md
--rw-r--r--   0        0        0    15887 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/vm-intro.md
--rw-r--r--   0        0        0    12644 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/vm-mechanism.md
--rw-r--r--   0        0        0      172 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/conf/about/os2024.yaml
--rw-r--r--   0        0        0        0 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/py.typed
--rw-r--r--   0        0        0     5191 1970-01-01 00:00:00.000000 os2024-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    18656 2024-04-11 03:57:32.212237 os2024-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3892 2024-04-11 03:57:32.212237 os2024-0.6.0/README.md
+-rw-r--r--   0        0        0     3573 2024-04-11 03:57:48.024140 os2024-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2311 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/__cli__.py
+-rw-r--r--   0        0        0      338 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-11 03:57:47.984140 os2024-0.6.0/src/os2024/_version.py
+-rw-r--r--   0        0        0     3855 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/_config.yml
+-rw-r--r--   0        0        0     2317 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/_toc.yml
+-rw-r--r--   0        0        0    22523 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/about/images/yjlee.jpeg
+-rw-r--r--   0        0        0     1476 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/about/index.md
+-rw-r--r--   0        0        0        0 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/assets/assets/extra/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/assets/extra/.gitkeep
+-rw-r--r--   0        0        0     3949 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/index.md
+-rw-r--r--   0        0        0       45 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/projects/index.md
+-rw-r--r--   0        0        0     8522 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/projects/setup.md
+-rw-r--r--   0        0        0        5 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/projects/template/index.md
+-rw-r--r--   0        0        0     7547 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/references/ostep/index.md
+-rw-r--r--   0        0        0     1967 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/references/ostep-code/index.md
+-rw-r--r--   0        0        0    11719 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/references/ostep-homework/index.md
+-rw-r--r--   0        0        0     3977 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/references/ostep-projects/index.md
+-rw-r--r--   0        0        0        9 2024-04-11 03:57:32.212237 os2024-0.6.0/src/os2024/book/references.bib
+-rw-r--r--   0        0        0      205 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/requirements.txt
+-rw-r--r--   0        0        0     6229 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/syllabus/index.md
+-rw-r--r--   0        0        0     2770 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week01/index.md
+-rw-r--r--   0        0        0    26071 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week01/intro.md
+-rw-r--r--   0        0        0     9466 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/cpu-api.md
+-rw-r--r--   0        0        0    16683 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/cpu-intro.md
+-rw-r--r--   0        0        0    20945 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/cpu-mechanisms.md
+-rw-r--r--   0        0        0     2830 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/index.md
+-rw-r--r--   0        0        0     4976 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/lab.md
+-rw-r--r--   0        0        0     4284 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/shells.md
+-rw-r--r--   0        0        0     2795 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week02/tip.md
+-rw-r--r--   0        0        0    19638 2024-04-11 03:57:32.216237 os2024-0.6.0/src/os2024/book/week03/cpu-scheduling.md
+-rw-r--r--   0        0        0    49905 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week03/figs/fcfs.png
+-rw-r--r--   0        0        0       53 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week03/index.md
+-rw-r--r--   0        0        0    15505 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week03/lab.md
+-rw-r--r--   0        0        0     3518 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week03/wsl-setup.md
+-rw-r--r--   0        0        0     3501 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week04/index.md
+-rw-r--r--   0        0        0     6608 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week04/lab-lottery.md
+-rw-r--r--   0        0        0     9209 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week04/lab-sched.md
+-rw-r--r--   0        0        0    24596 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week04/lottery.md
+-rw-r--r--   0        0        0    28602 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week04/mlfq.md
+-rw-r--r--   0        0        0   202834 2024-04-11 03:57:32.220237 os2024-0.6.0/src/os2024/book/week05/figs/os_img_1.png
+-rw-r--r--   0        0        0   475305 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/figs/os_img_2.png
+-rw-r--r--   0        0        0    87376 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/figs/os_img_3.png
+-rw-r--r--   0        0        0     3583 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/index.md
+-rw-r--r--   0        0        0     3753 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/lab.md
+-rw-r--r--   0        0        0     5279 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/tip-linux-cmd.md
+-rw-r--r--   0        0        0    13121 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/vm-api.md
+-rw-r--r--   0        0        0    15887 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week05/vm-intro.md
+-rw-r--r--   0        0        0       60 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week06/index.md
+-rw-r--r--   0        0        0     9767 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week06/lab.md
+-rw-r--r--   0        0        0    15700 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week06/vm-freespace.md
+-rw-r--r--   0        0        0    20928 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week06/vm-mechanism.md
+-rw-r--r--   0        0        0    31695 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week06/vm-segmentation.md
+-rw-r--r--   0        0        0       60 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week07/index.md
+-rw-r--r--   0        0        0      250 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/book/week07/vm-paging.md
+-rw-r--r--   0        0        0      172 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/conf/about/os2024.yaml
+-rw-r--r--   0        0        0        0 2024-04-11 03:57:32.224237 os2024-0.6.0/src/os2024/py.typed
+-rw-r--r--   0        0        0     5191 1970-01-01 00:00:00.000000 os2024-0.6.0/PKG-INFO
```

### Comparing `os2024-0.5.0/LICENSE` & `os2024-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/README.md` & `os2024-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/pyproject.toml` & `os2024-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "os2024"
-version = "0.5.0"
+version = "0.6.0"
 description = "Operating Systems 2024 Class"
 authors = ["Young Joon Lee <yj.lee@chu.ac.kr>"]
 license = "CC-BY-4.0"
 homepage = "https://os2024.halla.ai"
 repository = "https://github.com/chu-aie/os-2024"
 readme = "README.md"
 packages = [{ include = "os2024", from = "src" }]
```

### Comparing `os2024-0.5.0/src/os2024/__cli__.py` & `os2024-0.6.0/src/os2024/__cli__.py`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/_config.yml` & `os2024-0.6.0/src/os2024/book/_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
       data-base-api-url="https://chat.entelecheia.app/api/embed"
       data-brand-image-url="https://assets.entelecheia.ai/favicon.png"
       data-chat-icon="magic"
       data-sponsor-text="OS 2024"
       data-sponsor-link="https://chat.entelecheia.app/workspace/os2024"
       src="https://chat.entelecheia.app/embed/anythingllm-chat-widget.min.js">
     </script>
-  announcement: ""
+  announcement: "이번주 수업은 11일(목) 2시에 합니다."
 
 sphinx:
   config:
     html_extra_path: ["assets"]
     bibtex_reference_style: author_year
     mathjax_path: https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
     intersphinx_mapping:
```

#### html2text {}

```diff
@@ -16,24 +16,25 @@
 your book, relative to the repository root branch: main # Which branch of the
 repository should be used when creating links (optional) # Add GitHub buttons
 to your book # See https://jupyterbook.org/customize/config.html#add-a-link-to-
 your-repository html: use_issues_button: true use_repository_button: true
 use_edit_page_button: true favicon: https://assets.entelecheia.ai/favicon.png #
 favicon: Path to the favicon image google_analytics_id: G-BQJE5V9RK2 #
 google_analytics_id: Google Analytics ID extra_footer: |
-announcement: "" sphinx: config: html_extra_path: ["assets"]
-bibtex_reference_style: author_year mathjax_path: https://cdn.jsdelivr.net/npm/
-mathjax@3/es5/tex-mml-chtml.js intersphinx_mapping: ebp: - "https://
-executablebooks.org/en/latest/" - null myst-parser: - "https://myst-
-parser.readthedocs.io/en/latest/" - null myst-nb: - "https://myst-
-nb.readthedocs.io/en/latest/" - null sphinx: - "https://www.sphinx-doc.org/en/
-master" - null nbformat: - "https://nbformat.readthedocs.io/en/latest" - null
-sd: - "https://sphinx-design.readthedocs.io/en/latest" - null sphinxproof: -
-"https://sphinx-proof.readthedocs.io/en/latest/" - null hoverxref_intersphinx:
-- "sphinxproof" mathjax3_config: tex: macros: "N": "\\mathbb{N}" "floor":
+announcement: "ì´ë²ì£¼ ììì 11ì¼(ëª©) 2ìì í©ëë¤." sphinx:
+config: html_extra_path: ["assets"] bibtex_reference_style: author_year
+mathjax_path: https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
+intersphinx_mapping: ebp: - "https://executablebooks.org/en/latest/" - null
+myst-parser: - "https://myst-parser.readthedocs.io/en/latest/" - null myst-nb:
+- "https://myst-nb.readthedocs.io/en/latest/" - null sphinx: - "https://
+www.sphinx-doc.org/en/master" - null nbformat: - "https://
+nbformat.readthedocs.io/en/latest" - null sd: - "https://sphinx-
+design.readthedocs.io/en/latest" - null sphinxproof: - "https://sphinx-
+proof.readthedocs.io/en/latest/" - null hoverxref_intersphinx: - "sphinxproof"
+mathjax3_config: tex: macros: "N": "\\mathbb{N}" "floor":
 ["\\lfloor#1\\rfloor", 1] "bmat": ["\\left[\\begin{array}"] "emat": ["\\end
 {array}\\right]"] add_module_names: false autosummary_generate: true
 extra_extensions: - sphinx.ext.intersphinx - sphinx.ext.autodoc -
 sphinx.ext.autosummary - sphinx.ext.napoleon - sphinx.ext.viewcode -
 sphinx_inline_tabs - sphinx_proof - sphinx_examples - hoverxref.extension -
 sphinxcontrib.youtube - sphinxcontrib.video - sphinxcontrib.mermaid -
 sphinx_thebe - sphinx_carousel.carousel - sphinxcontrib.lastupdate
```

### Comparing `os2024-0.5.0/src/os2024/book/_toc.yml` & `os2024-0.6.0/src/os2024/book/_toc.yml`

 * *Files 20% similar despite different names*

```diff
@@ -30,17 +30,31 @@
           - file: week04/lottery
           - file: week04/lab-sched
           - file: week04/lab-lottery
       - file: week05/index
         sections:
           - file: week05/vm-intro
           - file: week05/vm-api
-          - file: week05/vm-mechanism
           - file: week05/lab
           - file: week05/tip-linux-cmd
+      - file: week06/index
+        sections:
+          - file: week06/vm-mechanism
+          - file: week06/vm-segmentation
+          - file: week06/vm-freespace
+          - file: week06/lab
+      - file: week07/index
+        sections:
+          - file: week07/vm-paging
+  - caption: Projects
+    chapters:
+      - file: projects/index
+        sections:
+          - file: projects/template/index
+      - file: projects/setup
   - caption: References
     chapters:
       - file: references/ostep/index
       - file: references/ostep-code/index
       - file: references/ostep-homework/index
       - file: references/ostep-projects/index
       - url: https://kuleuven-diepenbeek.github.io/osc-course/
```

### Comparing `os2024-0.5.0/src/os2024/book/about/images/yjlee.jpeg` & `os2024-0.6.0/src/os2024/book/about/images/yjlee.jpeg`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/about/index.md` & `os2024-0.6.0/src/os2024/book/about/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/index.md` & `os2024-0.6.0/src/os2024/book/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/references/ostep/index.md` & `os2024-0.6.0/src/os2024/book/references/ostep/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/references/ostep-code/index.md` & `os2024-0.6.0/src/os2024/book/references/ostep-code/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/references/ostep-homework/index.md` & `os2024-0.6.0/src/os2024/book/references/ostep-homework/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/references/ostep-projects/index.md` & `os2024-0.6.0/src/os2024/book/references/ostep-projects/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/syllabus/index.md` & `os2024-0.6.0/src/os2024/book/syllabus/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week01/index.md` & `os2024-0.6.0/src/os2024/book/week01/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week01/intro.md` & `os2024-0.6.0/src/os2024/book/week01/intro.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/cpu-api.md` & `os2024-0.6.0/src/os2024/book/week02/cpu-api.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/cpu-intro.md` & `os2024-0.6.0/src/os2024/book/week02/cpu-intro.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/cpu-mechanisms.md` & `os2024-0.6.0/src/os2024/book/week02/cpu-mechanisms.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/index.md` & `os2024-0.6.0/src/os2024/book/week02/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/lab.md` & `os2024-0.6.0/src/os2024/book/week02/lab.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/shells.md` & `os2024-0.6.0/src/os2024/book/week02/shells.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week02/tip.md` & `os2024-0.6.0/src/os2024/book/week02/tip.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week03/cpu-scheduling.md` & `os2024-0.6.0/src/os2024/book/week03/cpu-scheduling.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week03/figs/fcfs.png` & `os2024-0.6.0/src/os2024/book/week03/figs/fcfs.png`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week03/lab.md` & `os2024-0.6.0/src/os2024/book/week03/lab.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week03/wsl-setup.md` & `os2024-0.6.0/src/os2024/book/week03/wsl-setup.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week04/index.md` & `os2024-0.6.0/src/os2024/book/week04/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week04/lab-lottery.md` & `os2024-0.6.0/src/os2024/book/week04/lab-lottery.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week04/lab-sched.md` & `os2024-0.6.0/src/os2024/book/week04/lab-sched.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week04/lottery.md` & `os2024-0.6.0/src/os2024/book/week04/lottery.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week04/mlfq.md` & `os2024-0.6.0/src/os2024/book/week04/mlfq.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/figs/os_img_1.png` & `os2024-0.6.0/src/os2024/book/week05/figs/os_img_1.png`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/figs/os_img_2.png` & `os2024-0.6.0/src/os2024/book/week05/figs/os_img_2.png`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/figs/os_img_3.png` & `os2024-0.6.0/src/os2024/book/week05/figs/os_img_3.png`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/index.md` & `os2024-0.6.0/src/os2024/book/week05/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Week 5 - 메모리 가상화
+# Week 5 - 메모리 가상화 1
 
 **학생:** 가상화에 대한 이야기는 이제 끝인가요?
 
 > **교수:** 아니다! 아직 끝나지 않았네. 우리는 CPU 가상화에 대한 이야기를 마쳤을 뿐, 옷장 속에 숨어있는 진정한 괴물, 메모리 가상화는 아직 남아있지. 메모리 가상화는 CPU 가상화보다 훨씬 복잡하고, 하드웨어와 운영체제의 상호작용에 대한 더 깊은 이해를 필요로 하지.
 
 **학생:** 왜 그렇게 어려운가요?
```

### Comparing `os2024-0.5.0/src/os2024/book/week05/lab.md` & `os2024-0.6.0/src/os2024/book/week05/lab.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/tip-linux-cmd.md` & `os2024-0.6.0/src/os2024/book/week05/tip-linux-cmd.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/vm-api.md` & `os2024-0.6.0/src/os2024/book/week05/vm-api.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/src/os2024/book/week05/vm-intro.md` & `os2024-0.6.0/src/os2024/book/week05/vm-intro.md`

 * *Files identical despite different names*

### Comparing `os2024-0.5.0/PKG-INFO` & `os2024-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2024
-Version: 0.5.0
+Version: 0.6.0
 Summary: Operating Systems 2024 Class
 Home-page: https://os2024.halla.ai
 License: CC-BY-4.0
 Author: Young Joon Lee
 Author-email: yj.lee@chu.ac.kr
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
```

