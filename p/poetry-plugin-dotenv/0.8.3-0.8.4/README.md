# Comparing `tmp/poetry_plugin_dotenv-0.8.3.tar.gz` & `tmp/poetry_plugin_dotenv-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-0.8.3.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-0.8.4.tar", max compression
```

## Comparing `poetry_plugin_dotenv-0.8.3.tar` & `poetry_plugin_dotenv-0.8.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2024-03-31 17:29:13.316858 poetry_plugin_dotenv-0.8.3/LICENSE
--rw-r--r--   0        0        0     8807 2024-03-31 17:29:13.316858 poetry_plugin_dotenv-0.8.3/README.md
--rw-r--r--   0        0        0     6944 2024-03-31 17:29:42.477116 poetry_plugin_dotenv-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      695 2024-03-31 17:29:42.477116 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0      335 2024-03-31 17:29:13.320858 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5221 2024-03-31 17:29:13.320858 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     5969 2024-03-31 17:29:13.320858 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1445 2024-03-31 17:29:13.320858 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     3508 2024-03-31 17:29:13.320858 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-03-31 17:29:13.320858 poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    10810 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-11 19:29:23.553611 poetry_plugin_dotenv-0.8.4/LICENSE
+-rw-r--r--   0        0        0     7560 2024-04-11 19:29:23.553611 poetry_plugin_dotenv-0.8.4/README.md
+-rw-r--r--   0        0        0     6944 2024-04-11 19:29:50.837627 poetry_plugin_dotenv-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      695 2024-04-11 19:29:50.837627 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5221 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     5969 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1445 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     3508 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:29:23.561611 poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0     9563 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-0.8.4/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-0.8.3/LICENSE` & `poetry_plugin_dotenv-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.8.3/README.md` & `poetry_plugin_dotenv-0.8.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,35 +77,14 @@
     </a>
     <a href="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119">
         <img alt="wakatime" src="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119.svg">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues-closed/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr-closed/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/graphs/contributors">
-        <img alt="contributors" src="https://img.shields.io/github/contributors/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/commits/main">
-        <img alt="commit" src="https://img.shields.io/github/last-commit/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-</p>
-
-<p align="center">
     <a href="https://www.buymeacoffee.com/pivoshenko" target="_blank">
         <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
     </a>
     <a href="https://stand-with-ukraine.pp.ua/">
         <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
     </a>
     <a href="https://stand-with-ukraine.pp.ua">
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
                                     [logo]
                        _[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
         _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]_[_p_o_e_t_r_y_]_[_n_u_m_p_y_d_o_c_]
              _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_D_e_p_e_n_d_e_n_c_y_ _R_e_v_i_e_w_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
               _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]_[_w_a_k_a_t_i_m_e_]
-                _[_i_s_s_u_e_s_]_[_i_s_s_u_e_s_]_[_p_r_]_[_p_r_]_[_c_o_n_t_r_i_b_u_t_o_r_s_]_[_c_o_m_m_i_t_]
               _[_b_u_y_m_e_a_c_o_f_f_e_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
 - [Overview](#overview) - [Features](#features) - [Installation](#installation)
 - [Usage](#usage) ## Overview `poetry-plugin-dotenv` - is the plugin that
 automatically loads environment variables from a dotenv file into the
 environment before `poetry` commands are run. ### Features - Doesn't require
 any dependencies - Supports templates, interpolating variables using POSIX
 variable expansions - Fully type safe - 100% tests coverage and "A" grade for
```

### Comparing `poetry_plugin_dotenv-0.8.3/pyproject.toml` & `poetry_plugin_dotenv-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "0.8.3"
+version = "0.8.4"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
```

### Comparing `poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.8.3/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-0.8.4/src/poetry_plugin_dotenv/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-0.8.3/PKG-INFO` & `poetry_plugin_dotenv-0.8.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 0.8.3
+Version: 0.8.4
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
@@ -115,35 +115,14 @@
     </a>
     <a href="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119">
         <img alt="wakatime" src="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119.svg">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues-closed/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr-closed/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/graphs/contributors">
-        <img alt="contributors" src="https://img.shields.io/github/contributors/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/commits/main">
-        <img alt="commit" src="https://img.shields.io/github/last-commit/pivoshenko/poetry-plugin-dotenv?logo=github">
-    </a>
-</p>
-
-<p align="center">
     <a href="https://www.buymeacoffee.com/pivoshenko" target="_blank">
         <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
     </a>
     <a href="https://stand-with-ukraine.pp.ua/">
         <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
     </a>
     <a href="https://stand-with-ukraine.pp.ua">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.8.3 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 0.8.4 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,config,configuration,configuration-management,cross-
 platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
@@ -26,15 +26,14 @@
 plugin-dotenv/releases Project-URL: Say Thanks!, https://www.buymeacoffee.com/
 pivoshenko Description-Content-Type: text/markdown
                                     [logo]
                        _[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
         _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]_[_p_o_e_t_r_y_]_[_n_u_m_p_y_d_o_c_]
              _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_D_e_p_e_n_d_e_n_c_y_ _R_e_v_i_e_w_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
               _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]_[_w_a_k_a_t_i_m_e_]
-                _[_i_s_s_u_e_s_]_[_i_s_s_u_e_s_]_[_p_r_]_[_p_r_]_[_c_o_n_t_r_i_b_u_t_o_r_s_]_[_c_o_m_m_i_t_]
               _[_b_u_y_m_e_a_c_o_f_f_e_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
 - [Overview](#overview) - [Features](#features) - [Installation](#installation)
 - [Usage](#usage) ## Overview `poetry-plugin-dotenv` - is the plugin that
 automatically loads environment variables from a dotenv file into the
 environment before `poetry` commands are run. ### Features - Doesn't require
 any dependencies - Supports templates, interpolating variables using POSIX
 variable expansions - Fully type safe - 100% tests coverage and "A" grade for
```

