# Comparing `tmp/pyodide_mkdocs_theme-0.2.1.tar.gz` & `tmp/pyodide_mkdocs_theme-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.2.1.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.2.2.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.2.1.tar` & `pyodide_mkdocs_theme-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.1/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.1/README.md
--rw-r--r--   0        0        0     1347 2024-04-10 07:54:33.490726 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     6071 2024-04-08 19:01:06.315166 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-10 07:54:33.542728 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4832 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    22072 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4062 2024-04-06 19:50:40.682880 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11234 2024-04-07 10:49:12.948368 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0     6948 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4013 2024-04-08 19:01:06.315166 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0     8457 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11890 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    12321 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     2899 2024-04-04 17:32:31.188228 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     8427 2024-04-04 20:46:58.718283 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2653 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-10 07:53:34.321040 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6553 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     3986 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7119 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4293 2024-04-10 07:54:01.121805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3626 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 07:54:01.121805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     7109 2024-04-10 07:54:01.125805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9689 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3530 2024-04-10 07:54:01.125805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6051 2024-04-04 09:56:58.154964 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16604 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3582 2024-04-10 07:54:01.125805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0    31978 2024-04-10 07:54:01.125805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css
--rw-r--r--   0        0        0     1527 2024-04-10 07:54:01.125805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4233 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-10 07:54:01.125805 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12598 2024-04-07 10:53:56.264647 pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1689 2024-04-10 07:54:30.098630 pyodide_mkdocs_theme-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.2/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.2/README.md
+-rw-r--r--   0        0        0     1347 2024-04-11 09:34:15.400245 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     6071 2024-04-08 19:01:06.315166 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-11 09:34:15.432246 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:33:52.871591 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21561 2024-04-11 09:33:52.875591 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4070 2024-04-11 09:33:52.875591 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11199 2024-04-11 09:33:52.891592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0     6656 2024-04-11 09:34:15.340243 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:33:52.891592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0     9077 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11631 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    12697 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     3236 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9916 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-11 09:34:15.340243 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6699 2024-04-11 09:33:52.927593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     4566 2024-04-11 09:33:52.927593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4290 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6467 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9685 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3530 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6582 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16559 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0    31978 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css
+-rw-r--r--   0        0        0     1527 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4218 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12675 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1689 2024-04-11 09:34:12.512161 pyodide_mkdocs_theme-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.2/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.2.1/LICENSE` & `pyodide_mkdocs_theme-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/README.md` & `pyodide_mkdocs_theme-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 # pylint: disable=all
 
-from typing import Dict, Optional
+from typing import Any, Dict, Optional, TYPE_CHECKING
 
+from pyodide_mkdocs_theme.pyodide_macros.tools_and_constants import HtmlClass
+
+if TYPE_CHECKING:
+    from ..plugin.pyodide_macros_plugin import PyodideMacrosPlugin
 
 
 
 
 
 def html_builder_factory(template:str, allow_content):
     def tagger(tag:str):
@@ -97,27 +101,24 @@
 
     return span(txt, **dct)
 
 
 
 
 
-def terminal(term_id:str, kls:str, n_lines_h:int, **kw):
+def terminal(term_id:str, kls:str, n_lines_h:int, env:'PyodideMacrosPlugin', **kw):
     """
     Build a terminal div with its button. If n_lines_h is falsy, the height of the div isn't
     handled. Otherwise, it's the mac of n_lines_h and 5.
     """
 
-    tip = tooltip(
-        "Tronquer ou non le feedback dans les terminaux (sortie standard & stacktrace / relancer le code pour appliquer)",
-        width_em=16, shift=90
-    )
+    tip = tooltip(env.lang.feedback, width_em=env.lang.feedback.em, shift=90)
     btn_div = div(
         _BTN_STDOUT_SVG + tip,
-        kls="stdout-ctrl tooltip"
+        kls = f"{ HtmlClass.stdout_ctrl } { HtmlClass.tooltip }"
     )
     if n_lines_h:
         n_lines_h = max(n_lines_h, 5)
         kw['style'] = f"--n-lines:{ n_lines_h };" + kw.get('style','')
     kw['style'] = 'line-height:24px;' + kw.get('style','')
 
     term_div = div(btn_div, id=term_id, kls=kls, **kw)
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 """
 
 # pylint: disable=unused-argument
 
 
 import re
 import hashlib
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Tuple, Union
+from typing import Any, ClassVar, List, Literal, Optional, Tuple, Union
 from dataclasses import dataclass
 from pathlib import Path
 from math import inf
 
 from mkdocs.exceptions import BuildError
 
+from pyodide_mkdocs_theme.pyodide_macros.messages import Tip
+
 from ... import html_builder as Html
 from ...tools_and_constants import HtmlClass, Prefix, ScriptKind
 from ...pages_and_ides_configs import IdeConfigKey
 from ...parsing import build_code_fence
 from ...paths_utils import convert_url_to_utf8, to_uri
 from ...plugin.maestro_IDE import MaestroIDE
 
@@ -107,15 +109,15 @@
         in the document.
     """
 
     auto_log_assert: Optional[bool]
     """ If True, failing assertions without feedback during the private tests will be
         augmented automatically with the code of the assertion itself. If None, use
         the global `show_assertion_code_on_failed_test` plugin value and defined in
-        `CONFIG.showFailedAssertionsOnValidation` in the JS runtime.
+        `CONFIG.showAssertionCodeOnFailedTest` in the JS runtime.
     """
 
     rec_limit: int
     """ If used, the recursion limit of the pyodide runtime will be updated before the user's
         code or the tests are run.
         Note that this also forbids the use of the `sys.setrecurionlimit` at runtime.
     """
@@ -152,25 +154,14 @@
 
 
 
     MIN_IDE_ID_DIGITS: ClassVar[str] = 8
 
     INFINITY_SYMBOL: ClassVar[str] = "∞"
 
-    # (width (in em),tooltip). If width is 0, use default/automatic width
-    AVAILABLE_BUTTONS: ClassVar[Dict[str,Tuple[str,str]]] = {
-        "play":     (9,   "Exécuter le code<br>(<kbd>Ctrl</kbd>+<kbd>S</kbd>)"),
-        "check":    (9,   "Valider<br>(<kbd>Ctrl</kbd>+<kbd>Enter</kbd>)"),
-        "download": (0,   "Télécharger"),
-        "upload":   (0,   "Téléverser"),
-        "restart":  (0,   "Réinitialiser l'éditeur"),
-        "save":     (0,   "Sauvegarder dans le navigateur"),
-        "###":      (15,  "(Dés-)Active le code après la ligne <code># Tests</code> "
-                          "(insensible à la casse ; <kbd>Ctrl</kbd>+<kbd>I</kbd>)"),
-    }
 
     ICON_TEMPLATE: ClassVar[str] = (
         "{lvl_up}/pyodide-mkdocs/IDE-and-buttons/images/icons8-{button_name}-64.png"
     )
 
 
 
@@ -356,20 +347,21 @@
 
     def generate_empty_ide(self) -> str:
         """
         Generate the global layout that will receive later the ace elements.
         """
         is_v = self.mode == '_v'
         toggle_txt = '###'
-        tip_width,tip_text = self.AVAILABLE_BUTTONS[toggle_txt]
+        tip: Tip = self.my_env.lang.comments
+        msg = str(tip).format(tests=self.my_env.lang.tests)
 
         shortcut_comment_asserts = Html.span(
-            toggle_txt + Html.tooltip(tip_text, tip_width, shift=75),
+            toggle_txt + Html.tooltip(msg, tip.em, shift=95),
             id = Prefix.comment_ + self.editor_name,
-            kls = 'comment tooltip',
+            kls = f'{HtmlClass.comment} {HtmlClass.tooltip}',
         )
         editor_div = Html.div(
             id = self.editor_name,
             is_v = str(is_v).lower(),
             mode = self.mode,
             max_size = self.size,
             script_name = self.script_name,
@@ -383,14 +375,15 @@
             kls= HtmlClass.ide_separator + self.mode
         )
         terminal_div = Html.terminal(
             Prefix.term_ + self.editor_name ,
             kls = f"{ HtmlClass.term_editor }{ self.mode } { HtmlClass.py_mk_terminal }",
             n_lines_h = self.term_height * (not is_v),
             is_v = is_v,
+            env=self.my_env,
         )
 
         return Html.div(
             f"{ editor_wrapper }{ separator }{ terminal_div }",
             kls = f"{ HtmlClass.py_mk_wrapper }{ self.mode }",
         )
 
@@ -428,20 +421,21 @@
 
                 </div>                                          <<< ALWAYS
 
         Don't forget that empty lines are mandatory to render the "md in html" as expected.
         """
 
         # Prepare data first (to ease reading of the below sections)
-        title_chunks = ['Solution'*self.has_corr, 'Remarques'*self.has_rem]
-        sol_title    = ' & '.join(filter(bool, title_chunks))
+        sol_title = ' & '.join(filter(bool, [
+            str(self.my_env.lang.title_corr) * self.has_corr,
+            str(self.my_env.lang.title_rem) * self.has_rem
+        ]))
         corr_content = self.files_data.corr_content
-
         at_least_one = self.has_corr or self.has_rem
-        with_encrypt = self.my_env.encryptCorrectionsAndRems and at_least_one
+        with_encrypt = self.my_env.encrypt_corrections_and_rems and at_least_one
         extra_tokens = ( self.my_env.ENCRYPTION_TOKEN, ) * with_encrypt
 
 
         # Build the whole div content:
         md_div = [         '',   # Extra empty line to enforce proper rendering of the md around
                            f'<div markdown="1" id="{ Prefix.solution_ }{ self.editor_name }" '
                            f'     class="{ HtmlClass.py_mk_hidden }" data-search-exclude >',
@@ -453,35 +447,36 @@
         if self.has_corr:
             # first indentation must be removed, EXCEPT one level, because handled lower
             # for the whole block
             one_level = '    '
             fence = build_code_fence(
                 corr_content,
                 one_level + self.indentation,
-                title="🐍 Proposition de correction"
+                title=str(self.my_env.lang.corr)
             )
             md_div.append(  one_level+fence.strip())
 
         if self.has_corr and self.has_rem:
-            md_div.append( f'    <span class="{ HtmlClass.rem_fake_h3 }">Remarques :</span>')
+            rem = self.my_env.lang.rem
+            md_div.append( f'    <span class="{ HtmlClass.rem_fake_h3 }">{ rem } :</span>')
 
         if self.has_rem:
             rem_uri = to_uri( convert_url_to_utf8(str(self.files_data.rem_rel_path)) )
             md_div.append( f'    --8<-- "{ rem_uri }"' )
 
         if at_least_one:
             md_div.append(  '    </div>')
 
         md_div.extend((     *extra_tokens,
                             '</div>\n',    ))
                 # The extra linefeed is there to enforce md rendering of the following sections
 
         # Add extra indentation according to IDE's insertion:
         if self.indentation:
-            md_div = [ s and self.indentation+s for s in md_div ]
+            md_div = [ s and self.indentation + s for s in md_div ]
 
         # Join every item with extra gaps, to following md rendering requirements
         out = '\n\n'.join(md_div)
         return out
 
 
 
@@ -518,22 +513,22 @@
         @margin_...:    CSS formatting as floats (em units). By default, 0.2 on each side.
         @extra_content: Allow to inject some additional html inside the button tag.
         @**kwargs:      All the remaining kwargs are attributes added to the button tag.
         """
         if btn_kind is None:
             btn_kind = button_name.lower()
 
-        tooltip_width,tooltip_text = self.AVAILABLE_BUTTONS[button_name]
-        span_tooltip = Html.tooltip(tooltip_text, tooltip_width)
+        tip: Tip     = getattr(self.my_env.lang, button_name)
+        span_tooltip = Html.tooltip(tip, tip.em)
         lvl_up       = self.my_env.level_up_from_current_page()
         img_link     = self.ICON_TEMPLATE.format(lvl_up=lvl_up, button_name=button_name)
         img          = Html.img(src=img_link)
         button_html  = Html.button(
             f'{ img }{ span_tooltip }{ extra_content }',
-            kls = 'tooltip',
+            kls = HtmlClass.tooltip,
             btn_kind = btn_kind,
             style = f"margin-left:{margin_left}em; margin-right:{margin_right}em;",
             **kwargs,
             type='button',
                 # https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button#notes
         )
         return button_html
@@ -573,10 +568,10 @@
         if self.has_test:
             html_validation_button = self.create_button("check", btn_kind="validate")
 
         # The counter is always present:
         span_attempts_counter = Html.span(
             f"{ self.max_attempts_symbol }/{ self.max_attempts_symbol }",
             id=f'{ Prefix.compteur_ }{ self.editor_name }',
-            kls="compteur",         # get rid of that? (probably)
+            kls=HtmlClass.compteur,
         )
         return html_validation_button + span_attempts_counter
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,11 +116,11 @@
     @wraps(terminal)
     def wrapped(SIZE:int=6) -> str:
 
         env.set_current_page_insertion_needs(ScriptKind.pyodide)
 
         term_id = f'{ Prefix.term_only_ }{ env.terminal_count }'
         classes = " ".join((HtmlClass.py_mk_terminal_solo, HtmlClass.py_mk_terminal))
-        div     = Html.terminal(term_id, kls=classes, n_lines_h=SIZE )
+        div     = Html.terminal(term_id, kls=classes, n_lines_h=SIZE, env=env)
         return div
 
     return wrapped
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-
-"""
-Additional macros, never used in CodEx...
-"""
 # pylint: disable=unused-argument
 
 import re
 from functools import wraps
 from textwrap import dedent
 from typing import Any, List, Optional
 
@@ -90,36 +86,37 @@
                     final html structure!
 
         Reasons:
         1. THE MD RENDERER GENERATES INVALID HTML, WHEN MIXING html+md PERIOD!
         2. the md renderer will automatically open a <p> tag when starting the admo content
         3. If _ever_ the user defines a multiline content anywhere in the qcm, a new <p>
             tag will be started, leaving the previous one hanging in the air...
-        4. So far, so good...: the html is invalid, but rendered correctely/usable.
+        4. So far, so good...: the html is invalid, but rendered correctly/usable.
         5. CATACLYSM: use another plugin that will pass that html to the BSoup...:
             depending on the html parser used, Beautif(o)ulSoup _WILL_ generate the missing
-            closing tags, and this will entirely mess up the actual html.
+            closing tags, and this will entirely mess up the rendered page.
 
-        So, to avoid this, the extra closing `</p>` are added. They _LOOK_ lke they are
-        hanging, but they will actually produce valid html.
+        So, to avoid this, the extra closing `</p>` are added. They _LOOK_ like they are hanging,
+        but they _will_ actually produce valid html!
         """
 
         def qcm_start():
             qcm_id = env.get_qcm_id()
 
             admo_classes = ' '.join(kls for kls in [
                 HtmlClass.py_mk_admonition_qcm,
                 HtmlClass.qcm_shuffle * shuffle,
                 HtmlClass.qcm_hidden * hide,
                 true_false_none_for(multi, HtmlClass.qcm_multi, HtmlClass.qcm_single),
                 qcm_id,
             ] if kls )
 
-            plural = "s" * (len(questions_data) > 1)
-            admo_title = f'Question{plural}' if qcm_title is None else qcm_title
+
+            title = env.lang.qcm_title.one_or_many( len(questions_data) > 1 )
+            admo_title = title if qcm_title is None else qcm_title
             opening = f'{ indent }{ admo_kind } { admo_class } { admo_classes } "{ admo_title }"'
             return [
                 opening,
                 '',         # KEEP!
                 auto_indent('\n</p KEEP><ol>\n'),
             ]
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
     Configuration of one IDE in one page of the documentation. Convertible to JS, to define the
     global variable specific to each page.
     """
 
     # BUILD_TOOL_TOKEN
     attempts_left: int = 0      # Not overwriting this means there is no counter displayed
-    auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showFailedAssertionsOnValidation
+    auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showAssertionCodeOnFailedTest
     hdr_content: str = ""       # HDR part of "exo.py"
     user_content: str = ""      # Non-HDR part of "exo.py" (initial code)
     corr_content: str = ""      # content of "exo_corr.py"
     public_tests: str = ""      # test part of "exo.py" (initial code)
     secret_tests: str = ""      # Content of "exo_test.py" (private tests)
     corr_rem_config: int = 0    # Bit mask:   has_corr=corr_rem_config&1 ; has_rem=corr_rem_config&2
     encrypted: bool = True      # Tells if the html content is still encrypted or not
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
-""" Parsing and modifications logistic. """
-
+import re
 from mkdocs.exceptions import BuildError
 
 
 
 
 def replace_chunk(source:str, start:str, end:str, repl:str, *, at=0, keep_limiters=False):
     """ Given a @source and two delimiters/tokens, @start and @end, find those two tokens in
@@ -60,14 +59,25 @@
     tail = "" if end != 1000 else ' [...]'
     raise ValueError(f"Couldn't find {token=} in:\n\t[...] {source[start:end]}{ tail }")
 
 
 
 
 
+def camel(snake:str):
+    """ Transform a snake_case python property to a JS camelCase one. """
+    snake = re.sub(r'_{2,}', '_', snake)
+    return re.sub(r'(?<=[a-zA-Z\d])_([a-z\d])', _camelize, snake)
+
+
+def _camelize(m:re.Match):
+    return m[1].upper()
+
+
+
 def encrypt_string(text, key = 43960):
     """ Applique c ^ 43960 à chaque caractère de text (43960 = 0b1010101010101010) and send that
         as dot joined integers (needed to allow JS to decode emojis "the way python sees them")
         (...sort of...)
     """
     return ".".join( f"{ ord(c) ^ key :0>5}" for c in text )
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if isinstance(path,str):
         path = Path(path)
     joined = "/".join(path.parts + segments)
     joined = joined.replace('\\','/')
         # Because windows path behave weirdly when given a "root-like" path, which is
         # starting with a slash in the original string...
 
-    if joined.startswith('//'):      # may happen on absolute paths (linux)
+    if joined.startswith('//'):      # may happen on absolute paths (Linux)
         joined = '/' + joined.lstrip('/')
     return joined
 
 
 
 def get_sibling_of_current_page(
     env: BaseMaestro,
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 
 
 
 
 
 # Verify if something changed on the MacrosPlugin side... (moved to on_startup)
+# Current setup for MacrosPlugin v1.0.5
 
 _EXPECTED_MACRO_CONF = set("""
 module_name
 modules
 render_by_default
 include_dir
 include_yaml
@@ -94,31 +95,34 @@
     This behavior is global, but can be overridden on a "per IDE" base, using the `auto_log_assert`
     optional argument.
     """
 
     max_attempts_before_corr_available = C.Type(int, default=5)
     """
     Global setting for all IDE in the documentation: max number of tries a user can do before
-    correction and remarks become available (reminder: they are in a retracted details/admonition,
-    so the user still has to click to so the content. This way, they can still try to get the code
-    right before actually giving up).
+    correction and remarks become available (reminder: they are in a collapsed details/admonition,
+    requiring the user to click to reveal the content. This way, they can still try to get the code
+    right without actually seeing the solution, before actually giving up).
+    This behavior is global, but can be overridden on a "per IDE" base, using the `MAX` optional
+    argument.
     """
 
     decrease_attempts_on_user_code_failure = C.Type(bool, default=True)
-    """ If true, any failure when running the user code will decrease the number of attempts left.
-        Note this means even syntax errors will decrease the count, when the validation button is
-        used.
-        When this option is set to True, the user will have to comment out the public tests to get
-        the number of attempts changing, which is not obvious for new users).
     """
+    If true, any failure when running the user code during a validation will decrease the number
+    of attempts left. Note this means even syntax errors will decrease the count.
+    When this option is set to True, any error raised within the code of the editor will stop
+    the validation process without modifying the number of attempts left.
+    """
+
 
 
 
 
-# Only defines the values exposed to the user in mkdocs.yml.
+# This only defines the values exposed to the user in mkdocs.yml.
 # When a property is declared here, don't forgot to add the related extractor on the
 # BaseMaestro class.
 class PyodideMacrosConfig(Config):
     """
     Configuration for the main pyodide-mkdocs-theme plugin.
     """
 
@@ -130,95 +134,104 @@
     """ Configuration related to the validation tests in IDEs """
 
 
     skip_py_md_paths_names_validation = C.Type(bool, default=False)
     """
     By default, the path names of all the `.py` and `.md` files present in the docs_dir are checked
     so that they do not contain any character other than letters, digits, dot or dash. This
-    ensure the IDE related macros will properly work.
-    If unwanted characters are found, a BuildError is raised. Setting this flag to True will bypass
-    this verification.
+    ensures that the macros related to IDEs will work properly.
+    If unwanted characters are found, a BuildError is raised, but this verification can be turned
+    off by setting this flag to True. Use it at your own risks.
     """
 
     check_python_files = C.Type(bool, default=False)
     """
     If True, the different sections of the python files will be tested against each others during
     the build and provide feedback in the console.
     Unless the `soft_check` option is used, a BuildError will be raised if something considered
-    wrong happen. See the documentation for more details.
+    wrong happens. See the documentation for more details.
 
     NOTE:
-        - This is totally independent from the pyodide environment so, for example, it won't give
-          a warning if a forbidden function is used in the tests (which will fail on the website).
-        - The verifications considerably increase the build time (expect something around  x10).
+        - This is totally independent from the pyodide environment. For example, it won't give any
+          warning if a forbidden function is used in the tests (which will fail on the website).
+        - These verifications considerably increase the build time (expect something around x10).
     """
 
     soft_check = C.Type(bool, default=True)
     """
-    If True and the python sections are verified, the build won't be interrupted if something wrong
-    or suspicious is discovered and only a message in the console will be displayed.
+    If True and `check_python_files` is also True, the python sections are verified, but the
+    build won't be interrupted if something wrong or suspicious is discovered: a message will
+    instead be displayed in the console.
     """
 
 
     load_yaml_encoding = C.Type(str, default='utf-8')
     """
-    Encoding to use when loading yaml data from the original MacrosPlugin.
+    Encoding to use when loading yaml data with the original MacrosPlugin functionalities.
     (The original method doesn't use any encoding argument, which can lead to different behaviors
     between Windows and Linux (typically: during a pipeline!).
+
+    NOTE: a PR has been posted with the change on their repo. If ever it gets merged, this will
+    have to be changed.
     """
 
 
     macros_with_indents = C.Type(str, default='')
     """
-    Allow to register external macros that will use the `PyodideMacrosPlugin.get_indent` logistic
-    to insert indented multiline contents in the page.
-    `macro_with_indents` is a space separated string of all the names of the macros to register.
+    Allow to register external macros that will need to insert properly indented multiline contents
+    in the page (relying on `PyodideMacrosPlugin.get_indent` logistic).
+    `macro_with_indents` is a space-separated string of all the names of the macros the plugin will
+    track the indentation for.
     """
 
+
     bypass_indent_errors = C.Type(bool, default=False)
     """
-    If True, all errors related to indentation logistic for macros are bypassed and a message is
-    printed in the console instead.
+    If True, all errors raised when trying to find what is the indentation level of a macro call
+    are bypassed and a message is instead printed to the console.
     The purpose of this option is _not_ to deactivate the securities, but to allow gathering info
-    about all the problems at once: note that the resulting markdown content will most likely be
-    incorrect and rendered the wrong way.
+    about all the indentation problems at once: the resulting markdown content will most likely be
+    incorrect and be rendered with unexpected results.
     """
 
     ignore_macros_plugin_diffs = C.Type(bool, default=False)
     """
-    If True, no error will be raised when checking the configuration of the macros plugin against
-    the one of pyodide-macros. Note that if this error is raised, the build probably won't succeed
-    or the output will probably be buggy.
+    When the plugin configured, a verification is done that the configuration options of the
+    original MacroPlugin instance have not changed. If they did, and error is raised, forbidding
+    to build/serve the docs.
+    If this option is set to True, no error will be raised. Note that the result will most likely
+    end up incorrect, though.
     """
 
 
     encrypt_corrections_and_rems = C.Type(bool, default=True)
     """
-    Define if the html tags containing the correction and remarks have to be encrypted or not when
-    building the website. Passing this to False can be useful during development, but value should
-    _ALWAYS_ be set to true on the deployed website: keep in mind the search engine can otherwise
-    dig out content of those while the user is searching for something else.
+    If True, the html div under IDEs containing correction and remarks will be encrypted at build
+    time.
+    Passing this to False can be useful during development, but value should _ALWAYS_ be set
+    to true on the deployed website: keep in mind the search engine can otherwise make surface
+    contents from corrections and remarks as suggestions when the user is using the search bar.
     """
 
 
     _dev_mode = C.Type(bool, default=False)
-    """ Run the plugin in development mode (don't use that...) """
+    """ Run the plugin in development mode (...don't use that). """
 
 
     # ---------------------------------------------------------------------------------------
     # Replication of MacrosPlugin options (merging the config_scheme properties programmatically
     # is not enough, unfortunately...)
 
 
+    render_by_default        = C.Type(bool, default=True)
     module_name              = C.Type(str,  default=DEFAULT_MODULE_NAME)
     modules                  = C.Type(list, default=[])
-    render_by_default        = C.Type(bool, default=True)
     include_dir              = C.Type(str,  default=J2_STRING)
     include_yaml             = C.Type(list, default=[])
-    on_error_fail            = C.Type(bool, default=False)
-    verbose                  = C.Type(bool, default=False)
 
     j2_block_start_string    = C.Type(str,  default=J2_STRING)
     j2_block_end_string      = C.Type(str,  default=J2_STRING)
     j2_variable_start_string = C.Type(str,  default=J2_STRING)
     j2_variable_end_string   = C.Type(str,  default=J2_STRING)
+    on_error_fail            = C.Type(bool, default=False)
     on_undefined             = C.Type(str,  default=DEFAULT_UNDEFINED_BEHAVIOR)
+    verbose                  = C.Type(bool, default=False)
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-
-"""
-Define a class the can be passed to all macro functions, holding all the necessary data
-"""
 # pylint: disable=multiple-statements, attribute-defined-outside-init, unused-argument
 
 
 import re
 from collections import defaultdict
 from typing import ClassVar, Dict, List, Optional, Set, Tuple, Union
 from pathlib import Path
@@ -57,25 +53,20 @@
 
 
 
 class MaestroIDE(BaseMaestro):
     """ Holds the global logic related to the IDE macros """
 
 
-    encryptCorrectionsAndRems: ClassVar[bool] = True
-    """
-    Use xor encryption or not for the correction and remarques. This value is tied to the
-    equivalent in the global JS context (updated through build tools).
-    """
 
     ENCRYPTION_TOKEN: ClassVar[str] = "ENCRYPTION_TOKEN"
     """
     Denote the start and end point of the content of the div tag holding correction and/or remark.
     (only used in the python layer: it is either removed in the on_page_context hook, or it's just
-    not inserted at all if the encryptCorrectionsAndRems is False)
+    not inserted at all if the encrypt_corrections_and_rems is False)
     """
 
     MIN_RECURSION_LIMIT: ClassVar[int] = 20
     """
     Minimum recursion depth allowed.
     """
 
@@ -134,15 +125,15 @@
 
     @event_priority(2000)
     def on_page_context(self,_ctx, page:Page, *, config:MkDocsConfig, nav:Navigation):
         """
         Spot pages in which corrections and remarks have been inserted, and encrypt them.
 
         This hook uses high priority because the html content must be modified before the search
-        plugin starts indexing stuff in it.
+        plugin starts indexing stuff in it (which precisely happens in the on_page_context hook).
         """
         # pylint: disable=pointless-string-statement
 
         if self.is_page_with_something_to_insert(page):
 
             logger.debug(f"Add scripts + encrypt solutions and remarks in { page.file.src_uri }")
             """
@@ -202,21 +193,21 @@
             raise BuildError(
                 f"Wrong number of HDR/ENV tokens (found { len(lst)-1 }) in:\n"
                 f"{opt_path_or_content!s}"
             )
 
         hdr = "" if len(lst)==1 else lst[1]
         content = lst[-1].strip()
-        tests_cuts = re.split(r"(?i)#\s*tests", content)
+        tests_cuts = self.lang.tests.as_pattern.split(content)
         if len(tests_cuts)>2:
             raise BuildError(
                 "Found more than one time the '# ?Tests' token (case insensitive) in:\n"
                 + opt_path_or_content
             )
-        user_code,public_tests,*_ = map(str.strip, tests_cuts + [''])
+        user_code, public_tests, *_ = map(str.strip, tests_cuts + [''])
         return hdr, user_code, public_tests
 
 
 
 
 
 
@@ -304,15 +295,15 @@
         """
         Assuming it's known that the @page holds corrections and/or remarks:
             - Search for the encryption tokens
             - Encrypt the content in between two consecutive tokens in the page html content.
             - Once done for the whole page, replace the page content with the updated version.
         Encryption tokens are removed on the way.
         """
-        if not self.encryptCorrectionsAndRems:
+        if not self.encrypt_corrections_and_rems:
             chunks.append(html)
             return
 
         entering = 0
         while entering < len(html):
             i,j = eat(html, self.ENCRYPTION_TOKEN, start=entering, skip_error=True)
             i,j = self._cleanup_p_tags_around_encryption_tokens(html, i, j)
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=multiple-statements
 
 
 import re
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 from pathlib import Path
 
 from mkdocs.plugins import BasePlugin
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.exceptions import BuildError
 
+from pyodide_mkdocs_theme.pyodide_macros.messages import Lang, Msg, Tip
+
 from ...__version__ import __version__
 from ..tools_and_constants import PageUrl
 from ..pyodide_logger import logger
 from ..parsing import eat
 
 from .maestro_tools import ConfigExtractor
 from .config import PyodideMacrosConfig
@@ -72,17 +74,18 @@
 
     scripts_url: str = ConfigExtractor("_others")
     site_root: str = ConfigExtractor("_others")
 
     page: Page  # just as a reminder: defined by MacrosPlugin
 
     # global mkdocs config data:
-    site_url: str = ConfigExtractor(root='_conf')
-    docs_dir: str = ConfigExtractor(root='_conf')
-    repo_url: str = ConfigExtractor(root='_conf')
+    docs_dir:  str = ConfigExtractor(root='_conf')
+    repo_url:  str = ConfigExtractor(root='_conf')
+    site_name: str = ConfigExtractor(root='_conf')
+    site_url:  str = ConfigExtractor(root='_conf')
 
     #----------------------------------------------------------------------------
     # WARNING: the following properties are assigned from the PyodideMacrosPlugin
 
     docs_dir_path: Path
     """ Current docs_dir of the project as a Path object (ABSOLUTE path) """
 
@@ -112,23 +115,30 @@
     """
 
     _running_macro: Optional[str] = None
     """
     Name of the macro currently running (or the last one called. None if no macro called yet).
     """
 
+    lang: Lang = None
+
 
 
     def on_config(self, config:MkDocsConfig):
         # pylint: disable=unused-argument, no-member, missing-function-docstring
         self._pages_indents = PageIndents()
-
+        self.lang = Lang()
         super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
 
 
+    def override_messages(self, dct_lang: Dict[str, Union[Msg,Tip]]):
+        """ Replace some default messages or configurations with the given content """
+        self.lang.overload(dct_lang)
+
+
     #----------------------------------------------------------------------------
 
 
     def get_indent_in_current_page(self, macro_predicate:re.Pattern):
         """
         Extract the indentation needed for the given macro template call.
         @throws:    BuildError if the same macro call is found several times in the page.
@@ -319,10 +329,7 @@
                 err_msg = (
                     f"{ err_msg }\nTo disambiguate the calls, use the ID:int argument of the "
                     "macro. Do not forget to add it to every macro call of this kind in the "
                     "page!\nIf this is coming from one of your own macro, you will need to add "
                     "the related logic and argument in your code."
                 )
             raise BuildError( err_msg + epilogue )
-
-
-
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+import json
 from typing import Any, TYPE_CHECKING
 
 from mkdocs.config import config_options as C
 
+from pyodide_mkdocs_theme.pyodide_macros.parsing import camel
+
 if TYPE_CHECKING:
     from .pyodide_macros_plugin import PyodideMacrosPlugin
 
 
 
 def typ_deprecated_with_custom_msg(prop:str, typ:Any):
     return C.Deprecated(
@@ -88,7 +91,22 @@
 
     def __get__(self, obj:'PyodideMacrosPlugin', __=None):
         if self.warn_once:
             self.warn_once = False
             obj.warn_unmaintained(f'The property {self.prop!r}')
         self.cnt += 1
         return self.cnt
+
+
+
+
+
+
+def dump_and_dumper(props, obj, converter):
+
+    if obj is None:
+        class DumpNull:
+            def __getattr__(self,_):
+                return None
+        obj = DumpNull()
+
+    return { camel(prop): converter(getattr(obj, prop)) for prop in props }
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+import json
 import os
 import re
 from collections import defaultdict
 from functools import wraps
 from pathlib import Path
-from typing import Literal
 
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.exceptions import BuildError
 from mkdocs_macros.plugin import MacrosPlugin
 
+from pyodide_mkdocs_theme.pyodide_macros.messages import Lang
+from pyodide_mkdocs_theme.pyodide_macros.plugin.maestro_tools import dump_and_dumper
+
 
 from ...__version__ import __version__
 from ..exceptions import PyodideConfigurationError
 from ..pyodide_logger import logger
 from ..macros import (
     autres,
     IDEs,
@@ -42,14 +45,24 @@
 from .config import MISSING_MACROS_PROPS, EXTRAS_MACROS_PROPS
 from .maestro_base_and_indent import BaseMaestro
 from .maestro_IDE import MaestroIDE
 from .maestro_extras import MaestroExtras
 
 
 
+ICONS_FROM_TEMPLATES = Path("pyodide-mkdocs/IDE-and-buttons/images/")
+
+TO_DUMP_TO_JD_CONFIG = """
+    button_icons_directory
+    decrease_attempts_on_user_code_failure
+    encrypt_corrections_and_rems
+    show_assertion_code_on_failed_test
+    site_name
+    version
+""".split()
 
 
 
 
 
 class PyodideMacrosPlugin(
     MaestroIDE,
@@ -62,30 +75,62 @@
 
     This is kinda the "controller", linking all the behaviors to mkdocs machinery, while the
     parent classes hold the "somewhat self contained" behaviors.
 
     For reference, here are the hooks defined in the original MacrosPlugin:
         - on_config
         - on_nav
-        - on_page_markdown  (on_pre_page_macros  on_post_page_macros)
+        - on_page_markdown  (+ on_pre_page_macros + on_post_page_macros)
         - on_post_build     (on_post_build macros)
         - on_serve
     """
 
     version: str = __version__
 
 
     def rebase(self, base_url:str):
         """
-        Necessary for development only (to replace the wrong basic base_url during a serve in the
+        Necessary for development only (to replace the wrong base_url value during a serve in the
         theme project)
+        NOTE: Keep in mind the bas_url SOMETIMES ends with a slash...
         """
         return base_url if base_url!='/' else '.'
 
 
+
+    def dump_to_js_config(self, base_url):
+        """
+        Create the <script> tag that will add all the CONFIG properties needed in the JS global.
+        """
+        if self:
+            base_url = self.rebase(base_url).rstrip('/')
+            # temporary property:
+            self.button_icons_directory = f"{base_url}/{ICONS_FROM_TEMPLATES}"  # pylint: disable=w0201
+
+
+        dct = dump_and_dumper(TO_DUMP_TO_JD_CONFIG, self, json.dumps)
+        dct['lang'] = Lang.dump_as_str(self and self.lang)
+
+
+        if self is None:    # HACK!
+            # Dump to config.js (helper):
+            dumping = [ f"\n    { prop }: { val }," for prop,val in dct.items() ]
+            return ''.join(dumping)
+
+
+        # Dump to main.html:
+        dumping = [ f"\n  CONFIG.{ prop } = { val }" for prop,val in dct.items() ]
+
+        del self.button_icons_directory
+
+        out = f'''<script type="application/javascript">\n{ "".join(dumping) }\n</script>'''
+        return out
+
+
+
     def _check_docs_paths_validity(self) -> None :
         """
         Travel through all paths in the docs_dir and raises an BuildError if "special characters"
         are found in directory, py, or md file names (accepted characters are: r'[\\w.-]+' )
         """
         if self.skip_py_md_paths_names_validation:
             return
@@ -115,16 +160,18 @@
 
     def _check_macros_plugin_props(self):
         """ Verify that the config of the MacroPlugin class is still the expected one """
 
         if not MISSING_MACROS_PROPS and not EXTRAS_MACROS_PROPS:
             return
 
-        elif self.ignore_macros_plugin_diffs:
-            logger.error("Inconsistent MacrosPlugin properties / ignore_macros_plugin_diffs is set to true")
+        if self.ignore_macros_plugin_diffs:
+            logger.error(
+                "Inconsistent MacrosPlugin properties / ignore_macros_plugin_diffs is set to true"
+            )
 
         else:
             raise PyodideConfigurationError(f"""
 Cannot configure PyodideMacrosPlugin: the basic configuration of MacrosPlugin changed:
 {MISSING_MACROS_PROPS}{EXTRAS_MACROS_PROPS}"""
 "\nIf you absolutely need to run mkdocs before any fix is done, you can try the option "
 "`ignore_macros_plugin_diffs: true` in the `plugin_macros` section of `mkdocs.yml`, "
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
-"""
-Logger object to use to "hook" into mkdocs' logger: all the messages of this logger will
-appear during `mkdocs serve`.
-
-To use it:
-
-* import the logger object in the file where you need it
-* log messages with various levels of logging:
-    - logger.error(msg)
-    - logger.warn(msg)
-    - logger.info(msg)
-    - logger.debug(msg)
+# Logger object to use to "hook" into mkdocs' logger: all the messages of this logger will
+# appear during `mkdocs serve`.
+#
+# To use it:
+#
+# * import the logger object in the file where you need it
+# * log messages with various levels of logging:
+#     - logger.error(msg)
+#     - logger.warn(msg)
+#     - logger.info(msg)
+#     - logger.debug(msg)
+#
+# ---
+#
+# See: https://github.com/mkdocs/mkdocs/discussions/3241
 
----
-
-See: https://github.com/mkdocs/mkdocs/discussions/3241
-"""
 
 import logging
 import platform
 from typing import Any, MutableMapping, Tuple
 
 
 
@@ -47,22 +46,22 @@
 
 
 class Logger(logging.LoggerAdapter):
     """A logger adapter to prefix messages with the originating package name."""
 
     is_in_tests = False
 
-    def __init__(self, prefix: str, logger: logging.Logger, color:int=None):
+    def __init__(self, prefix: str, logger_: logging.Logger, color:int=None):
         """Initialize the object.
 
         Arguments:
             prefix: The string to insert in front of every message.
             logger: The logger instance.
         """
-        super().__init__(logger, {})
+        super().__init__(logger_, {})
         self.prefix = prefix
         if platform.system() != 'Windows':
             color = 36 if color is None else color
             self.prefix = f"\033[{ color }m{ prefix }\033[0m"
 
 
     def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> Tuple[str, Any]:
@@ -91,9 +90,9 @@
     """
     _logger = logging.getLogger(f"mkdocs.macros.{name}")
     return Logger(name.split(".", 1)[0], _logger, color)
 
 
 
 
-# sub-logger for pyodide-mkdocs:
-logger = get_plugin_logger(__name__.replace('_macros','').replace('_','-'))
+# sub-logger for pyodide-mkdocs-theme:
+logger = get_plugin_logger(__name__.replace('_','-'))
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,14 +132,22 @@
 
     py_mk_wrapper = AutoDescriptor()
     """ Prefix for the class mode of the div holding an IDE """
 
     ide_separator = AutoDescriptor()
     """ might be used with the _v suffix """
 
+    comment = AutoDescriptor()
+
+    tooltip = AutoDescriptor()
+
+    compteur = AutoDescriptor()
+
+    stdout_ctrl = AutoDescriptor("stdout-ctrl")
+
 
 
 
     py_mk_admonition_qcm = AutoDescriptor()
     """ Admonition containing a QCM """
 
     qcm_shuffle = AutoDescriptor()
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -151,17 +151,22 @@
 }
 
 let error = (content) => richTextFormat(content, "b", "red");
 let warning = (content) => richTextFormat(content, "", "orange");
 let stress = (content) => richTextFormat(content, "b");
 let info = (content) => richTextFormat(content, "i", "grey");
 let italic = (content) => richTextFormat(content, "i");
+let success = (content) => richTextFormat(content, "ib", "green");
+let failure = (content) => richTextFormat(content, "ib", "orange");
+
+'successMsg runScript installStart installDone'
+.split(' ').forEach(
+    prop => CONFIG.lang[prop].msg = info(CONFIG.lang[prop].msg)
+)
 
-CONFIG.MSG.successMessage = info(CONFIG.MSG.successMessage)
-CONFIG.MSG.runScriptPrompt = info(CONFIG.MSG.runScriptPrompt)
 
 
 
 
 
 /**Takes a string and cut the "middle chunk" of them if it is considered too long (length > 1750),
  * shortening it in the following way:
@@ -186,19 +191,20 @@
         buttonId: "",
         shift: 50, // %
         fontSize: 1.5, // em
         tipWidth: 15, // em
         tipText: "",
         ...options
     }
+    options.tipWidth = options.tipWidth > 0 ? `style="width:${ options.tipWidth }em;"` : ""
     const buttonId = !options.buttonId ? "" : `id="${ options.buttonId }" `
     return `
 <button ${ buttonId }class="tooltip header-btn" type="button"
  style="--tool_shift:${ options.shift }%; font-size:${ options.fontSize }em;">
-    <span class="tooltiptext" style="width:${ options.tipWidth }em;">${ options.tipText }</span>
+    <span class="tooltiptext" ${options.tipWidth}>${ options.tipText }</span>
     ${ content }
 </button>
 `
 }
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -23,15 +23,15 @@
 
 Inserted on the fly in each page needing IDEs (done by the macros_ide).
 The structure of this object is the following:
 
 var PAGE_IDES_CONFIG = {
     "editor_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx: {
         attempts_left: int = 0      # Not overwriting this means there is no counter displayed
-        auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showFailedAssertionsOnValidation
+        auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showAssertionCodeOnFailedTest
         hdr_content: str = ""       # HDR part of "exo.py"
         user_content: str = ""      # Non-HDR part of "exo.py" (initial code)
         corr_content: str = ""      # content of "exo_corr.py"
         public_tests: str = ""      # test part of "exo.py" (initial code)
         secret_tests: str = ""      # Content of "exo_test.py" (private tests)
         corr_rem_config: int = 0    # Bit mask:   has_corr=corr_rem_config&1 ; has_rem=corr_rem_config&2
         encrypted: bool = True      # Tells if the html content is still encrypted or not
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,16 @@
 subscribeWhenReady(
     "TrashCan",
     function() {
         jsLogger('[TrashCan]')
 
         const trashButtonCode = buttonWithTooltip({
                 shift: 90,
-                tipText: "Supprimer tous les codes enregistrés sur ce navigateur"
+                tipText: CONFIG.lang.tipTrash.msg,
+                tipWidth: CONFIG.lang.tipTrash.em
             },
             `<svg height="20px" version="1.1" id="trash-can-svg" xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 512 512" xml:space="preserve" fill="#ffffff">
     <g>
         <path d="M88.594,464.731C90.958,491.486,113.368,512,140.234,512h231.523c26.858,0,49.276-20.514,51.641-47.269 l25.642-335.928H62.952L88.594,464.731z M420.847,154.93l-23.474,307.496c-1.182,13.37-12.195,23.448-25.616,23.448H140.234 c-13.42,0-24.434-10.078-25.591-23.132L91.145,154.93H420.847z"/>
         <path d="M182.954,435.339c5.877-0.349,10.35-5.4,9.992-11.269l-10.137-202.234c-0.358-5.876-5.401-10.349-11.278-9.992 c-5.877,0.357-10.35,5.409-9.993,11.277l10.137,202.234C172.033,431.231,177.085,435.696,182.954,435.339z"/>
         <path d="M256,435.364c5.885,0,10.656-4.763,10.656-10.648V222.474c0-5.885-4.771-10.648-10.656-10.648 c-5.885,0-10.657,4.763-10.657,10.648v202.242C245.344,430.601,250.115,435.364,256,435.364z"/>
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/main.html`

 * *Files 3% similar despite different names*

```diff
@@ -27,34 +27,28 @@
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ace.min.js" charset="utf-8" type="text/javascript" integrity="sha512-GQpIYSKNIPIC763JKTNALj+t18/nfLdzw5gITgFGa31aK/4NmjyPKsfqrjh7CuzpJaG3nqEleeVcWUhHad9Axg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ext-language_tools.min.js" charset="utf-8" type="text/javascript" integrity="sha512-iK7yTkCkv7MbFwTqRgHTbmIqoiiLq6BsyNjymnFyB5a7pEQwYThj9QIgqBy9+XPPwj7+hAEHyR2npOHL1bz4Qg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdn.jsdelivr.net/pyodide/v0.25.0/full/pyodide.js"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery.terminal@2.34.0/js/jquery.terminal.min.js"></script>
 <!-- PYODIDE - insertion token -->
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/0_config-libs.js"></script>
+{{ config.plugins.pyodide_macros.dump_to_js_config(base_url) }}
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/functools-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/jsLogger-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/mathjax-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/securedPagesData-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_globalGuiButtons-libs.js"></script>
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/ide-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/pyoditeur-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/qcm/qcm-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/terminal-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_header-btns-libs.css">
 <!-- PYODIDE - insertion token -->
 <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js" type="text/javascript" charset="utf-8"></script>
-<script type="application/javascript">
-  CONFIG.CURRENT_REVISION = "pyodide-mkdocs-theme v{{ config.plugins.pyodide_macros.version }}"
-  CONFIG.showFailedAssertionsOnValidation = {{ config.plugins.pyodide_macros.show_assertion_code_on_failed_test | tojson }}
-  CONFIG.decreaseAttemptsUnUserCodeFailure = {{ config.plugins.pyodide_macros.decrease_attempts_on_user_code_failure | tojson }}
-  CONFIG.encryptCorrectionsAndRems = {{ config.plugins.pyodide_macros.encrypt_corrections_and_rems | tojson }}
-  CONFIG.buttonIconsDirectory = "{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/images/"
-</script>
 {% endblock %}
 
 
 {% block extrahead %}
 
 {% if config.extra.ace_style %}
   {% if config.extra.ace_style['slate'] and config.extra.ace_style['default'] %}
@@ -71,17 +65,14 @@
         data-ace-light-mode="{{config.extra.ace_style['default']}}">
   {% endif %}
 {% else %}
   <input type="checkbox" id="ace_palette" autocomplete="off" class="md-toggle"
         data-ace-dark-mode="tomorrow_night_bright"
         data-ace-light-mode="crimson_editor">
 {% endif %}
-<!-- PYODIDE - insertion token -->
-
-<!-- PYODIDE - insertion token -->
 {% endblock %}
 
 
 {% block scripts %}
 {{ super() }}
 <!-- PYODIDE - insertion token -->
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js"></script>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends "base.html" %} {% block libs %} {{ super() }}
+{{ config.plugins.pyodide_macros.dump_to_js_config(base_url) }}
 {% endblock %} {% block extrahead %} {% if config.extra.ace_style %} {% if
 config.extra.ace_style['slate'] and config.extra.ace_style['default'] %} ??{%
 elif config.extra.ace_style['slate'] %} ??{% elif config.extra.ace_style
 ['default'] %} ??{% endif %} {% else %} ??{% endif %} {% endblock %} {% block
 scripts %} {{ super() }}
 {% endblock %}
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -59,29 +59,29 @@
         stdErr = ""
     let decrease_count = false
 
     try {
         // Define the user's code in the environment and run the public tests (if any)
         stdErr = await runPythonCodeWithOptions(code, terminal, options)
 
-        decrease_count = CONFIG.decreaseAttemptsUnUserCodeFailure && stdErr
+        decrease_count = CONFIG.decreaseAttemptsOnUserCodeFailure && stdErr
 
         // Run the validation tests only if the user's code succeeded at the previous step
         if (!stdErr) {
 
             // If still running, run the original public tests and the secret ones...
             const publicTests = securedExtraction(editorName, CONFIG.ideProp.publicTests)
             const secretTests = securedExtraction(editorName, CONFIG.ideProp.secretTests)
 
             // ...unless there are no secret tests (this may happen when using KB shortcuts, while
             // there is no validation to do => just quit the testing process right away)
             if (!secretTests) return
 
             const autoLogAssert = securedExtraction(editorName, CONFIG.ideProp.autoLogAssert)
-            options.autoLogAssert = autoLogAssert !== null ? autoLogAssert : CONFIG.showFailedAssertionsOnValidation
+            options.autoLogAssert = autoLogAssert !== null ? autoLogAssert : CONFIG.showAssertionCodeOnFailedTest
             options.withStdOut = false
 
             const fullTests = `${ publicTests }\n\n${ secretTests }`
             decrease_count = stdErr = await runPythonCodeWithOptions(fullTests, terminal, options)
         }
 
         // On error, manage the counter of tries and the revelation of the solution, otherwise
@@ -228,15 +228,15 @@
  * Rules for toggling or not are:
  *      - leading spaces are ignored.
  *      - comment out if the first character is not "#".
  *      - if the first char is "#" and there is no spaces behind, uncomment.
  * */
 function toggleComments(editor) {
     const codeLines = editor.getSession().getValue().split('\n')
-    const iTestsToken = codeLines.findIndex(s => CONFIG.TESTS_TOKEN_PATTERN.test(s))
+    const iTestsToken = codeLines.findIndex(s => CONFIG.publicTestsPattern.test(s))
 
     /// No tests found:
     if (iTestsToken < 0) return;
 
     const toggled = codeLines.slice(iTestsToken + 1).map(s => {
         return s.replace(CONFIG.COMMENTED_PATTERN, (_, spaces, head, tail) => {
             if (head == '#' && tail != ' ') return spaces + tail
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -30,37 +30,38 @@
 
     // Extract the user's full code (possibly with public tests):
     let aceCode = await ace.edit(editorName).getSession().getValue();
 
     // save before anything else, in case an error occur somewhere...
     _save(editorName, aceCode)
 
+
+    // Build the default configuration options to use to run the user's code:
+    const options = buildOptionsForPyodideRun(editorName)
+
     // Refresh the pyodide environment, before running anything, and pause it (so that
     // the ">>>" are not displayed during the executions):
     const terminal = await setupOrGetTerminalAndPyEnv("term_" + editorName, true);
     terminal.pause()
     terminal.clear()
-    terminal.echo(CONFIG.MSG.runScriptPrompt)
+    terminal.echo(CONFIG.lang.runScript.msg)
     await sleep() // Enforce UI refresh
 
     // Run before clearing the terminal, in case someone forgot a print:
     setupStdIO()
     let stdErr = ''
     try {
-        await runHdrContent(editorName)
+        await runHdrContent(editorName, options, terminal)
     } catch (err) {
         stdErr = generateErrorLog(err, "", false)
     } finally {
         let someMsg = (getFullStdIO() || "") + stdErr
         if (someMsg) terminal.echo(someMsg)
     }
 
-    // Build the default configuration options to use to run the user's code:
-    const options = buildOptionsForPyodideRun(editorName)
-
     return [aceCode, terminal, options]
 }
 
 
 
 /**Actions performed once all the running code steps have been completed.
  *
@@ -71,15 +72,15 @@
  * @stdErr :     message that got already displayed in the terminal, or empty string id no error.
  * @successMsg : only used for validation tests. If they succeeded, this string won't be empty.
  * */
 function tearDownRuntimeAndTerminal(terminal, stdErr, finalMsg = "") {
     jsLogger("[Teardown] -", JSON.stringify(stdErr))
 
     if (!stdErr || finalMsg) {
-        terminal.echo(finalMsg || CONFIG.MSG.successMessage)
+        terminal.echo(finalMsg || CONFIG.lang.successMsg.msg)
     }
     terminal.resume()
 }
 
 
 
 
@@ -98,29 +99,34 @@
 
 
 
 
 /**Extract the content of the header code for the given editorName, and run its content
  * into pyodide environment.
  * */
-async function runHdrContent(editorName) {
+async function runHdrContent(editorName, options, terminal) {
     const headerContent = securedExtraction(editorName, CONFIG.ideProp.hdrContent)
     if (headerContent) {
-        pyodide.runPython(headerContent);
+        await installAndImportMissingModules(headerContent, options, terminal)
+        pyodide.runPython(headerContent)
     }
 }
 
 
 
+function getAttemptsLeft(editorName) {
+    return securedExtraction(editorName, CONFIG.ideProp.attemptsLeft)
+}
+
 
 
 
 function updateIdeCounter(editorName) {
 
-    let nAttempts = -1 + securedExtraction(editorName, CONFIG.ideProp.attemptsLeft)
+    let nAttempts = getAttemptsLeft(editorName) - 1
     securedUpdate(editorName, "attempts_left", nAttempts)
 
     // Update the GUI counter if needed
     if (Number.isFinite(nAttempts) && nAttempts >= 0) {
         const cntElement = document.getElementById("compteur_" + editorName);
         const [_, top] = cntElement.textContent.split('/')
         cntElement.textContent = `${ nAttempts }/${ top }`;
@@ -162,33 +168,39 @@
 
 
 /**Build the full success message
  * */
 function buildSuccessMessage(editorName) {
     const emo = choice(CONFIG.MSG.successEmojis)
     let info = getSolRemTxt(editorName, true)
-    return `[[b;green;]Bravo] ${ emo } - vous avez réussi tous les tests!${ info }`
+    return `${ success(CONFIG.lang.successHead.msg) } ${ emo } ${ CONFIG.lang.successTail.msg }${ info }`
 }
 
 
 
-
+/**Build the message for the terminal, announcing that correction and remarks becoming available.
+ * */
 function getSolRemTxt(editorName, isSuccess) {
     const CorrRemMask = securedExtraction(editorName, CONFIG.ideProp.corrRemMask)
     if (!CorrRemMask) return ""
 
     const msg = []
-    if (isSuccess) msg.push("\nPensez à lire")
-    else msg.push("[[b;orange;]Dommage !] -")
+    if (isSuccess) msg.push("\n" + CONFIG.lang.successHeadXtra.msg)
+    else msg.push(failure(CONFIG.lang.failHead.msg))
 
-    if (CorrRemMask & 1) msg.push("le corrigé")
-    if (CorrRemMask == 3) msg.push("et")
-    if (CorrRemMask & 2) msg.push("les commentaires")
+    const sentence = []
+    if (CorrRemMask & 1) sentence.push(CONFIG.lang.revealCorr.msg)
+    if (CorrRemMask == 3) sentence.push(CONFIG.lang.revealJoin.msg)
+    if (CorrRemMask & 2) sentence.push(CONFIG.lang.revealRem.msg)
+    if (sentence.length) {
+        sentence[0] = _.capitalize(sentence[0])
+    }
+    msg.push(...sentence)
 
     if (!isSuccess) {
-        if (CorrRemMask & 2) msg.push("sont maintenant disponibles")
-        else if (CorrRemMask) msg.push("est maintenant disponible")
+        if (CorrRemMask & 2) msg.push(CONFIG.lang.failTailPlural.msg)
+        else if (CorrRemMask) msg.push(CONFIG.lang.failTail.msg)
     }
     msg[msg.length - 1] += "."
 
     return msg.join(' ')
 }
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -211,27 +211,28 @@
     const wantedModules = getUserImportedModules(code)
     const installedModules = getAvailablePackages()
     const missing = wantedModules.filter(
         name => !installedModules.includes(name) && !options.excluded.includes(name)
     )
 
     if (missing.length) {
+        terminal.echo(CONFIG.lang.installStart.msg)
+
         await pyodide.loadPackage("micropip");
         let micropip = pyodide.pyimport("micropip");
 
-        terminal.echo(`Installation de certains packages. Ceci peut prendre un certain temps...`)
         for (let name of missing) {
             if (name in pkgReplacements) {
                 preImport.push(`import ${ pkgReplacements[name] } as ${ name }`)
                 name = pkgReplacements[name]
             }
             jsLogger("[Micropip] - Install", name)
             await micropip.install(name);
         }
-        terminal.echo(`Installations terminées!`)
+        terminal.echo(CONFIG.lang.installDone.msg)
     }
 
     // Import everything that is needed (either because module aliasing or because the code
     // restrictions would forbid it later):
     pyodide.runPython(preImport.join('\n'))
 }
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,17 @@
   position: absolute;
   z-index: 10;
   top: 110%;
   font-size: 0.9em;
   left: 50%;
   transform: translate(calc(-1 * var(--tool_shift)), 0);    /* root placement. The translation is done from the Html.tooltip function */
 }
+.tooltip .tooltiptext code {
+  color: white;
+}
 
 .tooltip .tooltiptext::after {
   content: " ";
   position: absolute;
   bottom: 100%;
   /* At the top of the tooltip */
   left: var(--tool_shift);  /* --tool_shift defined on a parent */
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -124,15 +124,15 @@
 del _hack
 `
 
 
         case "version":
             return `
 def version():
-    print("${stress("Pyodide-MkDocs")} : version ${error(CONFIG.CURRENT_REVISION)}")`
+    print("${ stress(CONFIG.siteName) } ${ stress(CONFIG.version) }")`
 
 
 
         case "exclusionsTools":
             return `
 def _hack():
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -113,22 +113,22 @@
         )
 
         const divAdmo = $('.' + this.qcmClass)
         const children = [...divAdmo.children()].slice(1) // Exclude the title of the admonition
         const detached = children.map(child => $(child).detach())
 
         const innerDiv = $(`<div class="${ this.innerDivPath.slice(1) }"></div>`)
-        const mask = $(createSvgMask(95, 1.1, "Les réponses resteront cachées...", 15))
+        const mask = $(createSvgMask(95, 1.1, CONFIG.lang.tipQcmMask.msg, CONFIG.lang.tipQcmMask.em))
         const checkBtn = $(makeButton('check', {
-            tipWidth: 11,
-            tipText: "Vérifier les réponses"
+            tipWidth: CONFIG.lang.tipQcmCheck.em,
+            tipText: CONFIG.lang.tipQcmCheck.msg
         }))
         const restartBtn = $(makeButton('restart', {
-            tipWidth: 9,
-            tipText: "Recommencer"
+            tipWidth: CONFIG.lang.tipQcmRedo.em,
+            tipText: CONFIG.lang.tipQcmRedo.msg
         }))
         const counter = $(`<p class="${ CONFIG.element.qcmCounterCls.slice(1) }"></p>`)
         const wrapper = $(`<div class="${ CONFIG.element.qcmWrapper.slice(1) } ${ this.reveal?'give-away':'hidden' }"></div>`)
             .append(counter, mask, checkBtn, restartBtn)
 
         innerDiv.append(...detached, wrapper)
         divAdmo.append(innerDiv)
```

### Comparing `pyodide_mkdocs_theme-0.2.1/pyproject.toml` & `pyodide_mkdocs_theme-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.2.1"
+version = "0.2.2"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.2.1/PKG-INFO` & `pyodide_mkdocs_theme-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

