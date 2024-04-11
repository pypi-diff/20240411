# Comparing `tmp/invenio-previewer-2.1.2.tar.gz` & `tmp/invenio-previewer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-previewer-2.1.2.tar", last modified: Tue Mar 12 08:29:18 2024, max compression
+gzip compressed data, was "dist/invenio-previewer-2.2.0.tar", last modified: Tue Mar 26 13:09:43 2024, max compression
```

## Comparing `invenio-previewer-2.1.2.tar` & `invenio-previewer-2.2.0.tar`

### file list

```diff
@@ -1,1593 +1,1599 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/examples/demo_files/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/csvfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18136 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/jpgfile.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/jsonfile.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/markdown.md
--rw-r--r--   0 runner    (1001) docker     (127)    98355 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/pdffile.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/pngfile.png
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/xmlfile.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/examples/demo_files/zipfile.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/pdfjs/
--rw-r--r--   0 runner    (1001) docker     (127)    39964 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/pdfjs/viewer.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/prismjs/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/prismjs/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/simple_image/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/simple_image/simple_image.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/csv_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/csv_previewer/init.js
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/open_pdf.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-3.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-4.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-5.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-6.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    41193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-3.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    33974 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-3.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-4.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-5.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-6.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40951 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    23293 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5pc-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS1-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETen-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK2K-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Hankaku.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Hiragana.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Katakana.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/NWP-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Roman.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    48280 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    50419 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    52679 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    53629 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    43366 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    44086 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    45738 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    46837 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    39443 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40539 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    41695 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    39534 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    41779 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40517 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40608 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    26451 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    27790 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/WP-Symbol.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    29515 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/l10n.js
--rw-r--r--   0 runner    (1001) docker     (127)   728683 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/pdf.worker.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   259213 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/viewer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-check.svg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-insert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-key.svg
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-newparagraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-noicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-note.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/grab.cur
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/grabbing.cur
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-icon.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties.png
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw.png
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw.png
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/shadow.png
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/texture.png
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-download.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-download@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows.png
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile.png
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown.png
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode.png
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-print.png
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-print@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-search.png
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle.png
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle.png
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments.png
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline.png
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn.png
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut.png
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed.png
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-expanded.png
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-expanded@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ach/
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/af/
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ak/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/an/
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ar/
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/as/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/az/
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/be/
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bg/
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-BD/
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-IN/
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/br/
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bs/
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/csb/
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cy/
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/da/
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/de/
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/el/
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-GB/
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-US/
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-ZA/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eo/
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-AR/
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-CL/
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-ES/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-MX/
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/et/
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eu/
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fa/
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ff/
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fi/
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fy-NL/
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ga-IE/
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gd/
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gl/
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gu-IN/
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/he/
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hi-IN/
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hy-AM/
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/id/
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/is/
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/it/
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ja/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ka/
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kk/
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/km/
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kn/
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ko/
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ku/
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lg/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lij/
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/locale.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lt/
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lv/
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mai/
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mk/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ml/
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mn/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mr/
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ms/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/my/
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nb-NO/
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nl/
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nn-NO/
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nso/
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/oc/
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/or/
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pa-IN/
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pl/
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-BR/
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-PT/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rm/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ro/
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rw/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sah/
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/si/
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sl/
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/son/
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sq/
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sv-SE/
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sw/
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta/
--rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta-LK/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/te/
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/th/
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tn/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ur/
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/vi/
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/wo/
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/xh/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-CN/
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-TW/
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zu/
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs.js
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/previewer_theme.js
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/prismjs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)    40383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/pdfjs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/prismjs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/simple_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/style.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/pdfjs/
--rw-r--r--   0 runner    (1001) docker     (127)    39964 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/pdfjs/viewer.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/prismjs/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/prismjs/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/simple_image/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/simple_image/simple_image.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/bottom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/csv_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/csv_previewer/init.js
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/open_pdf.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-3.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-4.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-5.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-6.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    41193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-3.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    33974 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-3.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-4.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-5.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-6.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40951 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-0.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-1.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    23293 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5pc-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS1-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETen-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK2K-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Hankaku.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Hiragana.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Katakana.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/NWP-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/RKSJ-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Roman.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    48280 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    50419 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    52679 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    53629 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    43366 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    44086 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    45738 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    46837 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    39443 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40539 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    41695 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    39534 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    41779 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40517 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    40608 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    26451 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    27790 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/V.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/WP-Symbol.bcmap
--rw-r--r--   0 runner    (1001) docker     (127)    29515 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/l10n.js
--rw-r--r--   0 runner    (1001) docker     (127)   728683 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/pdf.worker.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   264040 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/viewer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-check.svg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-insert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-key.svg
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-newparagraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-noicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-note.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/grab.cur
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/grabbing.cur
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-icon.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties.png
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw.png
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw.png
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/shadow.png
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/texture.png
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-download.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-download@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows.png
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile.png
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown.png
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode.png
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-print.png
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-print@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-search.png
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle.png
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle.png
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments.png
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline.png
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn.png
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut.png
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed.png
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-expanded.png
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-expanded@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ach/
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/af/
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ak/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/an/
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ar/
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/as/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/az/
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/be/
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bg/
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-BD/
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-IN/
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/br/
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bs/
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/csb/
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cy/
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/da/
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/de/
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/el/
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-GB/
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-US/
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-ZA/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eo/
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-AR/
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-CL/
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-ES/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-MX/
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/et/
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eu/
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fa/
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ff/
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fi/
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fy-NL/
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ga-IE/
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gd/
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gl/
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gu-IN/
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/he/
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hi-IN/
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hy-AM/
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/id/
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/is/
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/it/
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ja/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ka/
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kk/
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/km/
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kn/
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ko/
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ku/
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lg/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lij/
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/locale.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lt/
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lv/
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mai/
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mk/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ml/
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mn/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mr/
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ms/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/my/
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nb-NO/
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nl/
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nn-NO/
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nso/
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/oc/
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/or/
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pa-IN/
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pl/
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-BR/
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-PT/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rm/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ro/
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rw/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sah/
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/si/
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sl/
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/son/
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sq/
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sv-SE/
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sw/
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta/
--rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta-LK/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/te/
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/th/
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tn/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs.js
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/previewer_theme.js
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/prismjs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/bottom.scss
--rw-r--r--   0 runner    (1001) docker     (127)    40382 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/pdfjs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/prismjs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/simple_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/style.scss
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/txt.scss
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/zip.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/csv_papaparsejs.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/ipynb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/json_prismjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/mistune.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/pdfjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/simple_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/xml_prismjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/extensions/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/css/pdfjs/
--rw-r--r--   0 runner    (1001) docker     (127)    39964 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/css/pdfjs/viewer.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/
--rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/l10n.js
--rw-r--r--   0 runner    (1001) docker     (127)   259225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/viewer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-check.svg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-comment.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-help.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-insert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-key.svg
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-newparagraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-noicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-note.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-paragraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/grab.cur
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/grabbing.cur
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/loading-icon.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/loading-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/loading-small@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-documentProperties.png
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-firstPage.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-firstPage@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-handTool.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-lastPage.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-lastPage@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCcw.png
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCw.png
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/shadow.png
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/texture.png
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-bookmark.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-bookmark@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-download.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-download@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-menuArrows.png
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-menuArrows@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-openFile.png
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-openFile@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown.png
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-presentationMode.png
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-presentationMode@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-print.png
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-print@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-search.png
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-search@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle.png
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle.png
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewAttachments.png
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewAttachments@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline.png
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewThumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewThumbnail@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomIn.png
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomIn@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomOut.png
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomOut@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed-rtl.png
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed-rtl@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed.png
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/treeitem-expanded.png
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/treeitem-expanded@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ach/
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ach/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/af/
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/af/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ak/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ak/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/an/
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/an/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ar/
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ar/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/as/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/as/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ast/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/az/
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/az/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/be/
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/be/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bg/
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bg/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bn-BD/
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bn-BD/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bn-IN/
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bn-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/br/
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/br/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bs/
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bs/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ca/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/cs/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/csb/
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/csb/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/cy/
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/cy/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/da/
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/da/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/de/
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/de/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/el/
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/el/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-GB/
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-GB/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-US/
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-US/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-ZA/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-ZA/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/eo/
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/eo/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-AR/
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-AR/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-CL/
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-CL/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-ES/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-ES/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-MX/
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-MX/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/et/
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/et/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/eu/
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/eu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fa/
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fa/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ff/
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ff/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fi/
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fi/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fy-NL/
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fy-NL/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ga-IE/
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ga-IE/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gd/
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gd/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gl/
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gu-IN/
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gu-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/he/
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/he/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hi-IN/
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hi-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hy-AM/
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hy-AM/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/id/
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/id/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/is/
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/is/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/it/
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/it/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ja/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ja/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ka/
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ka/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/kk/
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/kk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/km/
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/km/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/kn/
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/kn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ko/
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ko/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ku/
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ku/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lg/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lg/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lij/
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lij/viewer.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/locale.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lt/
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lt/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lv/
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lv/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mai/
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mai/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mk/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ml/
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ml/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mn/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mr/
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ms/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ms/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/my/
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/my/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nb-NO/
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nb-NO/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nl/
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nn-NO/
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nn-NO/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nso/
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nso/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/oc/
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/oc/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/or/
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/or/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pa-IN/
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pa-IN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pl/
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pt-BR/
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pt-BR/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pt-PT/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pt-PT/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/rm/
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/rm/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ro/
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ro/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ru/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/rw/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/rw/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sah/
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sah/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/si/
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/si/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sl/
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/son/
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/son/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sq/
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sq/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sv-SE/
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sv-SE/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sw/
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sw/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ta/
--rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ta/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ta-LK/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ta-LK/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/te/
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/te/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/th/
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/th/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tl/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tn/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tn/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tr/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/uk/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ur/
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ur/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/vi/
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/vi/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/wo/
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/wo/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/xh/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/xh/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zh-CN/
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zh-CN/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zh-TW/
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zh-TW/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zu/
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zu/viewer.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/abstract_previewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/bottom.html
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/csv_bar.html
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/default.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/ipynb.html
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/json_prismjs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/mistune.html
--rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/pdfjs.html
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/simple_image.html
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/top.html
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/txt.html
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/xml_prismjs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/zip.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/abstract_previewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/bottom.html
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/csv_bar.html
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/default.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/ipynb.html
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/json_prismjs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/mistune.html
--rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/pdfjs.html
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/simple_image.html
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/top.html
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/txt.html
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/xml_prismjs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/zip.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16810 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16022 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/invenio_previewer/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    92362 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-12 08:29:17.000000 invenio-previewer-2.1.2/invenio_previewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:29:18.000000 invenio-previewer-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/tests/test_invenio_previewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/tests/test_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-12 08:29:11.000000 invenio-previewer-2.1.2/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/examples/demo_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/csvfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18136 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/jpgfile.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/jsonfile.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/markdown.md
+-rw-r--r--   0 runner    (1001) docker     (127)    98355 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/pdffile.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/pngfile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/xmlfile.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/examples/demo_files/zipfile.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/pdfjs/
+-rw-r--r--   0 runner    (1001) docker     (127)    39964 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/pdfjs/viewer.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/prismjs/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/prismjs/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/simple_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/simple_image/simple_image.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/csv_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/csv_previewer/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/open_pdf.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-3.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-4.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-5.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-6.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    41193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-3.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    33974 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-3.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-4.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-5.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-6.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40951 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    23293 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5pc-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS1-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETen-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK2K-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Hankaku.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Hiragana.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Katakana.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/NWP-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Roman.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    48280 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    50419 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    52679 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    53629 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    43366 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    44086 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    45738 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    46837 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    39443 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40539 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    41695 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    39534 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    41779 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40517 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40608 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    26451 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    27790 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/WP-Symbol.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    29515 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/l10n.js
+-rw-r--r--   0 runner    (1001) docker     (127)   728683 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/pdf.worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   259213 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/viewer.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-check.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-insert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-key.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-newparagraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-noicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-note.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-next@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/findbarButton-previous@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/grab.cur
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/grabbing.cur
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-icon.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties.png
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/shadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/texture.png
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-download@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows.png
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile.png
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode.png
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-print.png
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-print@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-search.png
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments.png
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline.png
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn.png
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut.png
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-expanded.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/treeitem-expanded@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ach/
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/af/
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ak/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/an/
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/as/
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/az/
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/be/
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-BD/
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/br/
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/csb/
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cy/
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/el/
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-GB/
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-US/
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-ZA/
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-AR/
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-CL/
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-ES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-MX/
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/et/
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ff/
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fy-NL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ga-IE/
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gu-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/he/
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hi-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hy-AM/
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/id/
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/is/
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ka/
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/km/
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kn/
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ku/
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lg/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lij/
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/locale.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lv/
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mai/
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mr/
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/my/
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nb-NO/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nn-NO/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nso/
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/or/
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pa-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-BR/
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-PT/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rm/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rw/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sah/
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/si/
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/son/
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sv-SE/
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sw/
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta-LK/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/te/
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/th/
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ur/
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/wo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/xh/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-TW/
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zu/
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/previewer_theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/prismjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)    40383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/pdfjs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/prismjs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/simple_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/style.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/pdfjs/
+-rw-r--r--   0 runner    (1001) docker     (127)    39964 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/pdfjs/viewer.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/prismjs/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/prismjs/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/simple_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/simple_image/simple_image.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/bottom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/csv_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/csv_previewer/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/open_pdf.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-3.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-4.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-5.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-6.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    41193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-3.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    33974 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-3.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-4.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-5.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-6.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40951 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-0.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-1.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    23293 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5pc-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS1-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETen-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETenms-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK2K-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Hankaku.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Hiragana.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Katakana.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/NWP-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/RKSJ-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Roman.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    48280 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    50419 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    52679 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    53629 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    43366 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    44086 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    45738 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    46837 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    39443 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40539 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    41695 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    39534 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    41779 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40517 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    40608 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    26451 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    27790 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/V.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/WP-Symbol.bcmap
+-rw-r--r--   0 runner    (1001) docker     (127)    29515 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/l10n.js
+-rw-r--r--   0 runner    (1001) docker     (127)   728683 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/pdf.worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   264040 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/viewer.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-check.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-insert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-key.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-newparagraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-noicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-note.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-next@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/findbarButton-previous@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/grab.cur
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/grabbing.cur
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-icon.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties.png
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-firstPage@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-lastPage@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/shadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/texture.png
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-bookmark@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-download@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows.png
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-menuArrows@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile.png
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageDown@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-pageUp@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode.png
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-print.png
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-print@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-search.png
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-secondaryToolbarToggle@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-sidebarToggle@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments.png
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline.png
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewOutline@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewThumbnail@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn.png
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomIn@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut.png
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-zoomOut@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-collapsed@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-expanded.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/treeitem-expanded@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ach/
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/af/
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ak/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/an/
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/as/
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/az/
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/be/
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-BD/
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/br/
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/csb/
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cy/
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/el/
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-GB/
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-US/
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-ZA/
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-AR/
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-CL/
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-ES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-MX/
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/et/
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ff/
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fy-NL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ga-IE/
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gu-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/he/
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hi-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hy-AM/
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/id/
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/is/
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ka/
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/km/
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kn/
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ku/
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lg/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lij/
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/locale.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lv/
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mai/
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mr/
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/my/
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nb-NO/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nn-NO/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nso/
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/or/
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pa-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-BR/
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-PT/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rm/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rw/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sah/
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/si/
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/son/
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sv-SE/
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sw/
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta-LK/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/te/
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/th/
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/previewer_theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/prismjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/audio_videojs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    40382 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/pdfjs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/prismjs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/simple_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/style.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/txt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/video_videojs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/zip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/audio_videojs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/csv_papaparsejs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/json_prismjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/mistune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/pdfjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/simple_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/video_videojs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/xml_prismjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/extensions/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/css/pdfjs/
+-rw-r--r--   0 runner    (1001) docker     (127)    39964 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/css/pdfjs/viewer.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/l10n.js
+-rw-r--r--   0 runner    (1001) docker     (127)   259225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/viewer.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-check.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-comment.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-insert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-key.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-newparagraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-noicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-note.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-paragraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-next@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous.png
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/findbarButton-previous@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/grab.cur
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/grabbing.cur
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/loading-icon.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/loading-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/loading-small@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-documentProperties.png
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-firstPage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-firstPage@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-handTool.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-lastPage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-lastPage@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCcw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/shadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/texture.png
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-bookmark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-bookmark@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-download@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-menuArrows.png
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-menuArrows@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-openFile.png
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-openFile@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageDown@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp.png
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-pageUp@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-presentationMode.png
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-presentationMode@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-print.png
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-print@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-search.png
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-search@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-secondaryToolbarToggle@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-sidebarToggle@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewAttachments.png
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewAttachments@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline.png
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewOutline@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewThumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewThumbnail@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomIn.png
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomIn@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomOut.png
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-zoomOut@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed-rtl.png
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed-rtl@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/treeitem-collapsed@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/treeitem-expanded.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/treeitem-expanded@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ach/
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ach/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/af/
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/af/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ak/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ak/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/an/
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/an/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ar/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/as/
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/as/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ast/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/az/
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/az/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/be/
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/be/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bg/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bn-BD/
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bn-BD/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bn-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bn-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/br/
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/br/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bs/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ca/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/cs/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/csb/
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/csb/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/cy/
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/cy/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/da/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/de/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/el/
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/el/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-GB/
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-GB/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-US/
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-US/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-ZA/
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-ZA/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/eo/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-AR/
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-AR/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-CL/
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-CL/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-ES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-ES/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-MX/
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-MX/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/et/
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/et/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/eu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fa/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ff/
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ff/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fi/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fy-NL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fy-NL/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ga-IE/
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ga-IE/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gd/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gu-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gu-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/he/
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/he/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hi-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hi-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hy-AM/
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hy-AM/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/id/
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/id/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/is/
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/is/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/it/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ja/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ka/
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ka/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/kk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/kk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/km/
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/km/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/kn/
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/kn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ko/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ku/
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ku/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lg/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lg/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lij/
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lij/viewer.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/locale.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lt/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lv/
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lv/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mai/
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mai/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ml/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mr/
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ms/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/my/
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/my/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nb-NO/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nb-NO/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nn-NO/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nn-NO/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nso/
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nso/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/oc/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/or/
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/or/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pa-IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pa-IN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pt-BR/
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pt-BR/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pt-PT/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pt-PT/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/rm/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/rm/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ro/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ru/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/rw/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/rw/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sah/
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sah/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/si/
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/si/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/son/
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/son/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sq/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sv-SE/
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sv-SE/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sw/
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sw/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ta/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ta-LK/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ta-LK/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/te/
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/te/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/th/
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/th/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tl/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tn/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tr/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/uk/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ur/
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ur/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/vi/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/wo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/wo/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/xh/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/xh/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zh-CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zh-CN/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zh-TW/
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zh-TW/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zu/
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zu/viewer.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/abstract_previewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/csv_bar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/ipynb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/json_prismjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/mistune.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/pdfjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/simple_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/top.html
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/txt.html
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/xml_prismjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/zip.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/abstract_previewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/audio_videojs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/csv_bar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/ipynb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/json_prismjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/mistune.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/pdfjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/simple_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/top.html
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/txt.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/videojs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/xml_prismjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/zip.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16810 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16022 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/invenio_previewer/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    92760 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 13:09:42.000000 invenio-previewer-2.2.0/invenio_previewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:09:43.000000 invenio-previewer-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/tests/test_invenio_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/tests/test_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-26 13:09:37.000000 invenio-previewer-2.2.0/tests/test_views.py
```

### Comparing `invenio-previewer-2.1.2/.editorconfig` & `invenio-previewer-2.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/.tx/config` & `invenio-previewer-2.2.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/CHANGES.rst` & `invenio-previewer-2.2.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,26 @@
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 
 Changes
 =======
 
+Version 2.2.0 (released 2024-03-26)
+-----------------------------------
+
+- integrated new video/audio previewer
+
 Version 2.1.2 (released 2024-03-12)
+-----------------------------------
 
 - frontend: Improve display of ZIPs with long file names
 
 Version 2.1.1 (released 2024-01-31)
+-----------------------------------
 
 - markdown: default message if not previewable
 - markdown: fixed ascii encoding typo
 
 Version 2.1.0 (Release 2023-12-05)
 ----------------------------------
```

### Comparing `invenio-previewer-2.1.2/CONTRIBUTING.rst` & `invenio-previewer-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/INSTALL.rst` & `invenio-previewer-2.2.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/LICENSE` & `invenio-previewer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/MANIFEST.in` & `invenio-previewer-2.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/PKG-INFO` & `invenio-previewer-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-previewer
-Version: 2.1.2
+Version: 2.2.0
 Summary: Invenio module for previewing files.
 Home-page: https://github.com/inveniosoftware/invenio-previewer
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,19 +48,26 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 2.2.0 (released 2024-03-26)
+        -----------------------------------
+        
+        - integrated new video/audio previewer
+        
         Version 2.1.2 (released 2024-03-12)
+        -----------------------------------
         
         - frontend: Improve display of ZIPs with long file names
         
         Version 2.1.1 (released 2024-01-31)
+        -----------------------------------
         
         - markdown: default message if not previewable
         - markdown: fixed ascii encoding typo
         
         Version 2.1.0 (Release 2023-12-05)
         ----------------------------------
```

### Comparing `invenio-previewer-2.1.2/README.rst` & `invenio-previewer-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/docs/Makefile` & `invenio-previewer-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/docs/api.rst` & `invenio-previewer-2.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/docs/conf.py` & `invenio-previewer-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/docs/index.rst` & `invenio-previewer-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/docs/license.rst` & `invenio-previewer-2.2.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/docs/make.bat` & `invenio-previewer-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/jpgfile.jpg` & `invenio-previewer-2.2.0/examples/demo_files/jpgfile.jpg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/markdown.md` & `invenio-previewer-2.2.0/examples/demo_files/markdown.md`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/notebook.ipynb` & `invenio-previewer-2.2.0/examples/demo_files/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/pdffile.pdf` & `invenio-previewer-2.2.0/examples/demo_files/pdffile.pdf`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/pngfile.png` & `invenio-previewer-2.2.0/examples/demo_files/pngfile.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/xmlfile.xml` & `invenio-previewer-2.2.0/examples/demo_files/xmlfile.xml`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/examples/demo_files/zipfile.zip` & `invenio-previewer-2.2.0/examples/demo_files/zipfile.zip`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/__init__.py` & `invenio-previewer-2.2.0/invenio_previewer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,10 +314,10 @@
 ...     'invenio_previewer.extensions.default',
 ... ]
 """
 
 from .ext import InvenioPreviewer
 from .proxies import current_previewer
 
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 
 __all__ = ("__version__", "current_previewer", "InvenioPreviewer")
```

### Comparing `invenio-previewer-2.1.2/invenio_previewer/api.py` & `invenio-previewer-2.2.0/invenio_previewer/api.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/css/invenio_previewer/pdfjs/viewer.css` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/css/invenio_previewer/pdfjs/viewer.css`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/csv_previewer/init.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/csv_previewer/init.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/fullscreen.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/fullscreen.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/l10n.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/l10n.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/pdf.worker.min.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/pdf.worker.min.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/viewer.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/viewer.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-help.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-help.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-key.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-key.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-note.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-note.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-icon.gif` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-icon.gif`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/texture.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/texture.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/locale.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/locale.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/pdfjs.scss` & `invenio-previewer-2.2.0/invenio_previewer/assets/bootstrap3/scss/invenio_previewer/pdfjs.scss`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/css/invenio_previewer/pdfjs/viewer.css` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/css/invenio_previewer/pdfjs/viewer.css`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/csv_previewer/init.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/csv_previewer/init.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/fullscreen.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/fullscreen.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/78ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/83pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90msp-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/90pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Add-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-4.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-5.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/B5pc-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS-EUC-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/CNS1-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETHK-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/ETen-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/Ext-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GB-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBK2K-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBKp-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBT-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBTpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/GBpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdla-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKdlb-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKgccs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm314-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKm471-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/HKscs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSC-Johab-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/KSCpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/NWP-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniCNS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniGB-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/cmaps/UniKS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/l10n.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/l10n.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/pdf.worker.min.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/pdf.worker.min.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/viewer.js` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/viewer.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-comment.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-help.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-help.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-key.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-key.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-note.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-note.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/annotation-paragraph.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-icon.gif` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-icon.gif`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/loading-small@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/texture.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/texture.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-openFile@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-presentationMode@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-search@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/images/toolbarButton-viewAttachments@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ach/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/af/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ak/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/an/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ar/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/as/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ast/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/az/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/be/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bg/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-BD/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bn-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/br/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/bs/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ca/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cs/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/csb/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/cy/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/da/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/de/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/el/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-GB/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-US/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/en-ZA/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eo/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-AR/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-CL/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-ES/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/es-MX/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/et/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/eu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fa/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ff/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fi/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/fy-NL/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ga-IE/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gd/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/gu-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/he/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hi-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/hy-AM/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/id/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/is/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/it/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ja/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ka/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/km/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/kn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ko/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ku/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lg/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lij/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/locale.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/locale.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lt/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/lv/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mai/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ml/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/mr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ms/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/my/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nb-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nn-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/nso/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/oc/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/or/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pa-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-BR/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/pt-PT/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rm/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ro/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ru/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/rw/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sah/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/si/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/son/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sq/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sv-SE/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/sw/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ta-LK/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/te/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/th/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/tr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/uk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/pdfjs.scss` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/pdfjs.scss`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/zip.scss` & `invenio-previewer-2.2.0/invenio_previewer/assets/semantic-ui/scss/invenio_previewer/zip.scss`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/config.py` & `invenio-previewer-2.2.0/invenio_previewer/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 PREVIEWER_PREFERENCE = [
     "csv_papaparsejs",
     "simple_image",
     "json_prismjs",
     "xml_prismjs",
     "mistune",
     "pdfjs",
+    "video_videojs",
+    "audio_videojs",
     "ipynb",
     "zip",
     "txt",
 ]
 """Decides which previewers are available and their priority."""
 
 PREVIEWER_ABSTRACT_TEMPLATE = "invenio_previewer/abstract_previewer.html"
```

### Comparing `invenio-previewer-2.1.2/invenio_previewer/ext.py` & `invenio-previewer-2.2.0/invenio_previewer/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/csv_papaparsejs.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/csv_papaparsejs.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/default.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/default.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/ipynb.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/ipynb.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/json_prismjs.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/json_prismjs.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/mistune.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/mistune.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/pdfjs.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/pdfjs.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/simple_image.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/simple_image.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/txt.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/txt.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/xml_prismjs.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/xml_prismjs.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/extensions/zip.py` & `invenio-previewer-2.2.0/invenio_previewer/extensions/zip.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/css/pdfjs/viewer.css` & `invenio-previewer-2.2.0/invenio_previewer/static/css/pdfjs/viewer.css`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/l10n.js` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/l10n.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/viewer.js` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/viewer.js`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-comment.svg` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-comment.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-help.svg` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-help.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-key.svg` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-key.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-note.svg` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-note.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/annotation-paragraph.svg` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/annotation-paragraph.svg`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/loading-icon.gif` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/loading-icon.gif`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/loading-small.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/loading-small.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/loading-small@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/loading-small@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-documentProperties@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-handTool@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCcw@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/secondaryToolbarButton-rotateCw@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/texture.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/texture.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-openFile@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-openFile@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-presentationMode@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-presentationMode@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-search@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-search@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewAttachments@2x.png` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/images/toolbarButton-viewAttachments@2x.png`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ach/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ach/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/af/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/af/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ak/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ak/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/an/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/an/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ar/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ar/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/as/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/as/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ast/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ast/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/az/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/az/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/be/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/be/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bg/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bg/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bn-BD/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bn-BD/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bn-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bn-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/br/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/br/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/bs/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/bs/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ca/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ca/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/cs/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/cs/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/csb/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/csb/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/cy/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/cy/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/da/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/da/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/de/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/de/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/el/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/el/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-GB/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-GB/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-US/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-US/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/en-ZA/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/en-ZA/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/eo/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/eo/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-AR/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-AR/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-CL/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-CL/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-ES/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-ES/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/es-MX/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/es-MX/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/et/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/et/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/eu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/eu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fa/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fa/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ff/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ff/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fi/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fi/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/fy-NL/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/fy-NL/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ga-IE/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ga-IE/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gd/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gd/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/gu-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/gu-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/he/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/he/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hi-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hi-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/hy-AM/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/hy-AM/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/id/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/id/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/is/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/is/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/it/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/it/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ja/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ja/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ka/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ka/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/kk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/kk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/km/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/km/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/kn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/kn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ko/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ko/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ku/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ku/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lg/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lg/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lij/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lij/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/locale.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/locale.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lt/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lt/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/lv/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/lv/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mai/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mai/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ml/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ml/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/mr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/mr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ms/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ms/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/my/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/my/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nb-NO/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nb-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nn-NO/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nn-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/nso/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/nso/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/oc/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/oc/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/or/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/or/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pa-IN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pa-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pt-BR/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pt-BR/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/pt-PT/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/pt-PT/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/rm/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/rm/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ro/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ro/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ru/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ru/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/rw/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/rw/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sah/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sah/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/si/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/si/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/son/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/son/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sq/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sq/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sv-SE/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sv-SE/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/sw/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/sw/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ta/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ta/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ta-LK/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ta-LK/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/te/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/te/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/th/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/th/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tl/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tl/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tn/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tn/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/tr/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/tr/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/uk/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/uk/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/ur/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/ur/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/vi/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/vi/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/wo/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/wo/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/xh/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/xh/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zh-CN/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zh-CN/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zh-TW/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zh-TW/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/static/js/pdfjs/web/locale/zu/viewer.properties` & `invenio-previewer-2.2.0/invenio_previewer/static/js/pdfjs/web/locale/zu/viewer.properties`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/abstract_previewer.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/abstract_previewer.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/base.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/base.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/bottom.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/bottom.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/csv_bar.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/csv_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/default.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/default.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/macros.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/macros.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/pdfjs.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/pdfjs.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/top.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/top.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/invenio_previewer/zip.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/invenio_previewer/zip.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/abstract_previewer.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/abstract_previewer.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/base.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/base.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/bottom.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/bottom.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/csv_bar.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/csv_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/default.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/default.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/macros.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/macros.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/pdfjs.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/pdfjs.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/top.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/top.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/templates/semantic-ui/invenio_previewer/zip.html` & `invenio-previewer-2.2.0/invenio_previewer/templates/semantic-ui/invenio_previewer/zip.html`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/af/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/af/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ar/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ar/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/bg/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/bg/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ca/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ca/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/cs/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/cs/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/da/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/da/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/de/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/de/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/el/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/el/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/es/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/es/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/et/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/et/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fa/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fa/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fr/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fr/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/gl/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/gl/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hr/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hr/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hu/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hu/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/it/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/it/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ja/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ja/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ka/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ka/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/lt/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/lt/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/messages.pot` & `invenio-previewer-2.2.0/invenio_previewer/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ne/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ne/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/no/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/no/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/pl/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/pl/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/pt/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/pt/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ro/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ro/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ru/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/ru/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/rw/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/rw/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/sk/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/sk/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/sv/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/sv/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/tr/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/tr/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/uk/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/uk/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-previewer-2.2.0/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-previewer-2.2.0/invenio_previewer/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/views.py` & `invenio-previewer-2.2.0/invenio_previewer/views.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/invenio_previewer/webpack.py` & `invenio-previewer-2.2.0/invenio_previewer/webpack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2016-2022 CERN.
 # Copyright (C)      2022 TU Wien.
+# Copyright (C)      2023 Northwestern University.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -68,20 +69,24 @@
                 "open_pdf": "./js/invenio_previewer/open_pdf.js",
                 "bottom_js": "./js/invenio_previewer/bottom.js",
                 "pdfjs_css": "./scss/invenio_previewer/pdfjs.scss",
                 "zip_css": "./scss/invenio_previewer/zip.scss",
                 "bottom_css": "./scss/invenio_previewer/bottom.scss",
                 "simple_image_css": "./scss/invenio_previewer/simple_image.scss",
                 "txt_css": "./scss/invenio_previewer/txt.scss",
+                "videojs_js": "./node_modules/video.js/dist/video.min.js",
+                "audio_videojs_css": "./scss/invenio_previewer/audio_videojs.scss",
+                "video_videojs_css": "./scss/invenio_previewer/video_videojs.scss",
             },
             dependencies={
                 "flightjs": "~1.5.1",
                 "font-awesome": "~4.5.0",
                 "jquery": "^3.3.1",
                 "papaparse": "^5.4.1",
                 "pdfjs-dist": "^1.4.192",
                 "prismjs": "^1.15.0",
+                "video.js": "^8.6.1",
             },
         ),
     },
 )
 """Bundle of webpack assets."""
```

### Comparing `invenio-previewer-2.1.2/invenio_previewer.egg-info/PKG-INFO` & `invenio-previewer-2.2.0/invenio_previewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-previewer
-Version: 2.1.2
+Version: 2.2.0
 Summary: Invenio module for previewing files.
 Home-page: https://github.com/inveniosoftware/invenio-previewer
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,19 +48,26 @@
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
         
+        Version 2.2.0 (released 2024-03-26)
+        -----------------------------------
+        
+        - integrated new video/audio previewer
+        
         Version 2.1.2 (released 2024-03-12)
+        -----------------------------------
         
         - frontend: Improve display of ZIPs with long file names
         
         Version 2.1.1 (released 2024-01-31)
+        -----------------------------------
         
         - markdown: default message if not previewable
         - markdown: fixed ascii encoding typo
         
         Version 2.1.0 (Release 2023-12-05)
         ----------------------------------
```

### Comparing `invenio-previewer-2.1.2/invenio_previewer.egg-info/SOURCES.txt` & `invenio-previewer-2.2.0/invenio_previewer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -789,30 +789,34 @@
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/ur/viewer.properties
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/vi/viewer.properties
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/wo/viewer.properties
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/xh/viewer.properties
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-CN/viewer.properties
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zh-TW/viewer.properties
 invenio_previewer/assets/semantic-ui/js/invenio_previewer/pdfjs/web/locale/zu/viewer.properties
+invenio_previewer/assets/semantic-ui/scss/invenio_previewer/audio_videojs.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/bottom.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/pdfjs.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/prismjs.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/simple_image.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/style.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/txt.scss
+invenio_previewer/assets/semantic-ui/scss/invenio_previewer/video_videojs.scss
 invenio_previewer/assets/semantic-ui/scss/invenio_previewer/zip.scss
 invenio_previewer/extensions/__init__.py
+invenio_previewer/extensions/audio_videojs.py
 invenio_previewer/extensions/csv_papaparsejs.py
 invenio_previewer/extensions/default.py
 invenio_previewer/extensions/ipynb.py
 invenio_previewer/extensions/json_prismjs.py
 invenio_previewer/extensions/mistune.py
 invenio_previewer/extensions/pdfjs.py
 invenio_previewer/extensions/simple_image.py
 invenio_previewer/extensions/txt.py
+invenio_previewer/extensions/video_videojs.py
 invenio_previewer/extensions/xml_prismjs.py
 invenio_previewer/extensions/zip.py
 invenio_previewer/static/css/pdfjs/viewer.css
 invenio_previewer/static/js/pdfjs/l10n.js
 invenio_previewer/static/js/pdfjs/viewer.js
 invenio_previewer/static/js/pdfjs/web/images/annotation-check.svg
 invenio_previewer/static/js/pdfjs/web/images/annotation-comment.svg
@@ -1015,26 +1019,28 @@
 invenio_previewer/templates/invenio_previewer/pdfjs.html
 invenio_previewer/templates/invenio_previewer/simple_image.html
 invenio_previewer/templates/invenio_previewer/top.html
 invenio_previewer/templates/invenio_previewer/txt.html
 invenio_previewer/templates/invenio_previewer/xml_prismjs.html
 invenio_previewer/templates/invenio_previewer/zip.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/abstract_previewer.html
+invenio_previewer/templates/semantic-ui/invenio_previewer/audio_videojs.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/base.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/bottom.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/csv_bar.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/default.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/ipynb.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/json_prismjs.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/macros.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/mistune.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/pdfjs.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/simple_image.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/top.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/txt.html
+invenio_previewer/templates/semantic-ui/invenio_previewer/videojs.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/xml_prismjs.html
 invenio_previewer/templates/semantic-ui/invenio_previewer/zip.html
 invenio_previewer/translations/messages.pot
 invenio_previewer/translations/af/LC_MESSAGES/messages.mo
 invenio_previewer/translations/af/LC_MESSAGES/messages.po
 invenio_previewer/translations/ar/LC_MESSAGES/messages.mo
 invenio_previewer/translations/ar/LC_MESSAGES/messages.po
```

### Comparing `invenio-previewer-2.1.2/invenio_previewer.egg-info/entry_points.txt` & `invenio-previewer-2.2.0/invenio_previewer.egg-info/entry_points.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 [invenio_base.apps]
 invenio_previewer = invenio_previewer:InvenioPreviewer
 
 [invenio_i18n.translations]
 messages = invenio_previewer
 
 [invenio_previewer.previewers]
+audio_videojs = invenio_previewer.extensions.audio_videojs
 csv_papaparsejs = invenio_previewer.extensions.csv_papaparsejs
 default = invenio_previewer.extensions.default
 ipynb = invenio_previewer.extensions.ipynb
 json_prismjs = invenio_previewer.extensions.json_prismjs
 mistune = invenio_previewer.extensions.mistune
 pdfjs = invenio_previewer.extensions.pdfjs
 simple_image = invenio_previewer.extensions.simple_image
 txt = invenio_previewer.extensions.txt
+video_videojs = invenio_previewer.extensions.video_videojs
 xml_prismjs = invenio_previewer.extensions.xml_prismjs
 zip = invenio_previewer.extensions.zip
```

### Comparing `invenio-previewer-2.1.2/setup.cfg` & `invenio-previewer-2.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 	xml_prismjs = invenio_previewer.extensions.xml_prismjs
 	mistune = invenio_previewer.extensions.mistune
 	txt = invenio_previewer.extensions.txt
 	pdfjs = invenio_previewer.extensions.pdfjs
 	zip = invenio_previewer.extensions.zip
 	ipynb = invenio_previewer.extensions.ipynb
 	default = invenio_previewer.extensions.default
+	audio_videojs = invenio_previewer.extensions.audio_videojs
+	video_videojs = invenio_previewer.extensions.video_videojs
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
```

### Comparing `invenio-previewer-2.1.2/tests/conftest.py` & `invenio-previewer-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/tests/test_invenio_previewer.py` & `invenio-previewer-2.2.0/tests/test_invenio_previewer.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/tests/test_macros.py` & `invenio-previewer-2.2.0/tests/test_macros.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/tests/test_utils.py` & `invenio-previewer-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-previewer-2.1.2/tests/test_views.py` & `invenio-previewer-2.2.0/tests/test_views.py`

 * *Files identical despite different names*

