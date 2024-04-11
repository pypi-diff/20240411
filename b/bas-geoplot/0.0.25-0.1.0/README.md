# Comparing `tmp/bas_geoplot-0.0.25.tar.gz` & `tmp/bas_geoplot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bas_geoplot-0.0.25.tar", last modified: Wed Feb 21 13:49:28 2024, max compression
+gzip compressed data, was "bas_geoplot-0.1.0.tar", last modified: Thu Apr 11 09:35:39 2024, max compression
```

## Comparing `bas_geoplot-0.0.25.tar` & `bas_geoplot-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-21 13:49:28.910644 bas_geoplot-0.0.25/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.25/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.25/MANIFEST.in
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3546 2024-02-21 13:49:28.910644 bas_geoplot-0.0.25/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2645 2024-02-21 13:49:21.000000 bas_geoplot-0.0.25/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-21 13:49:28.906644 bas_geoplot-0.0.25/bas_geoplot/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      195 2024-02-21 13:49:21.000000 bas_geoplot-0.0.25/bas_geoplot/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    10380 2024-02-21 13:49:21.000000 bas_geoplot-0.0.25/bas_geoplot/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-21 13:49:28.910644 bas_geoplot-0.0.25/bas_geoplot/config/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11924 2024-02-21 13:49:21.000000 bas_geoplot-0.0.25/bas_geoplot/config/interactive.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.25/bas_geoplot/config/static.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    37923 2024-02-21 13:49:21.000000 bas_geoplot-0.0.25/bas_geoplot/interactive.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.25/bas_geoplot/static.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4440 2024-01-17 15:31:28.000000 bas_geoplot-0.0.25/bas_geoplot/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-21 13:49:28.910644 bas_geoplot-0.0.25/bas_geoplot.egg-info/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3546 2024-02-21 13:49:28.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2024-02-21 13:49:28.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-02-21 13:49:28.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2024-02-21 13:49:28.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       81 2024-02-21 13:49:28.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2024-02-21 13:49:28.000000 bas_geoplot-0.0.25/bas_geoplot.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2024-02-21 13:49:28.910644 bas_geoplot-0.0.25/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.25/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-11 09:35:39.398522 bas_geoplot-0.1.0/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.1.0/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.1.0/MANIFEST.in
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3668 2024-04-11 09:35:39.398522 bas_geoplot-0.1.0/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2630 2024-04-11 09:21:09.000000 bas_geoplot-0.1.0/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-11 09:35:39.398522 bas_geoplot-0.1.0/bas_geoplot/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      286 2024-04-11 09:21:09.000000 bas_geoplot-0.1.0/bas_geoplot/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    10380 2024-04-02 10:21:44.000000 bas_geoplot-0.1.0/bas_geoplot/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-11 09:35:39.398522 bas_geoplot-0.1.0/bas_geoplot/config/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11924 2024-04-02 10:21:44.000000 bas_geoplot-0.1.0/bas_geoplot/config/interactive.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.1.0/bas_geoplot/config/static.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    40603 2024-04-10 12:56:59.000000 bas_geoplot-0.1.0/bas_geoplot/interactive.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.1.0/bas_geoplot/static.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7067 2024-04-10 12:56:59.000000 bas_geoplot-0.1.0/bas_geoplot/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-11 09:35:39.398522 bas_geoplot-0.1.0/bas_geoplot.egg-info/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3668 2024-04-11 09:35:39.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2024-04-11 09:35:39.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-04-11 09:35:39.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2024-04-11 09:35:39.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       76 2024-04-11 09:35:39.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2024-04-11 09:35:39.000000 bas_geoplot-0.1.0/bas_geoplot.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2024-04-11 09:35:39.398522 bas_geoplot-0.1.0/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2060 2024-04-11 09:35:34.000000 bas_geoplot-0.1.0/setup.py
```

### Comparing `bas_geoplot-0.0.25/LICENSE` & `bas_geoplot-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.25/PKG-INFO` & `bas_geoplot-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: bas_geoplot
-Version: 0.0.25
-Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
+Version: 0.1.0
+Summary: GeoPlot: BAS AI Lab plotting scripts for internal plotting & visualisation
 Home-page: https://github.com/antarctica/GeoPlot
-Author: BAS AI Lab
-Author-email: jonsmi@bas.ac.uk
-Maintainer: BAS AI Lab
-Maintainer-email: jonsmi@bas.ac.uk
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Classifier: 
 Description-Content-Type: text/markdown
 
 # GeoPlot
 
 ![](logo.jpg)
 
 <a href="https://pypi.org/project/bas-geoplot/"><img src="https://img.shields.io/pypi/v/bas-geoplot" alt="PyPI">
@@ -41,15 +39,15 @@
 Installation from PyPI:
 ```
 pip install bas-geoplot
 ```
 
 Installation from source:
 ```
-git clone https://github.com/Antarctica/Geoplot
+git clone https://github.com/Antarctica/GeoPlot
 pip install -e ./GeoPlot
 ```
 
 Use of `-e` is optional, based on whether you want to be able to edit the installed copy of the package.
 
 Some features of this software package require GDAL and Fiona to be installed, this requires additional steps during the installation process on Windows. These additional steps are as follows:
 
@@ -80,18 +78,15 @@
 -r '(plot an additional route from the given file)'
 -a '(add directional arrows to all routes)'
 -b '(create the plot without a basemap layer)'
 ```
 
 ## Development & Contributions
 Development of software package is conducted by the [BAS AI Lab](https://www.bas.ac.uk/team/science-teams/ai-lab/).
-
-For contributions and feature additions please contact [polarroute@bas.ac.uk](polarroute@bas.ac.uk).
-
+For contributions and feature additions please contact [amop@bas.ac.uk](amop@bas.ac.uk).
 
 ## License
 Distributed under the MIT license. See ``LICENSE`` for more information.
-
 [version]: https://img.shields.io/GeoPlot/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/GeoPlot/dm/datadog-metrics.svg?style=flat-square
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: bas_geoplot Version: 0.0.25 Summary: GeoPlot: BAS
-AI Lab plotting scripts built on Folium Home-page: https://github.com/
-antarctica/GeoPlot Author: BAS AI Lab Author-email: jonsmi@bas.ac.uk
-Maintainer: BAS AI Lab Maintainer-email: jonsmi@bas.ac.uk License: UNKNOWN
-Platform: UNKNOWN Classifier: Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: System Administrators Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Scientific/Engineering Classifier: Description-Content-Type: text/markdown #
-GeoPlot ![](logo.jpg) _[_P_y_P_I_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_G_e_o_P_l_o_t_ _i_s_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _a_n_d
-_s_t_a_t_i_c_ _p_l_o_t_t_i_n_g_ _t_o_o_l_k_i_t_ _d_e_v_e_l_o_p_e_d_ _b_y_ _m_e_m_b_e_r_s_ _o_f_ _t_h_e_ _B_A_S_ _A_r_t_i_f_i_c_i_a_l_ _I_n_t_e_l_l_i_g_e_n_c_e
-_L_a_b_ _a_n_d_ _d_e_s_i_g_n_e_d_ _t_o_ _b_e_ _u_s_e_d_ _i_n_ _c_o_m_b_i_n_a_t_i_o_n_ _w_i_t_h_ _o_t_h_e_r_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_s_ _u_n_d_e_r
-_d_e_v_e_l_o_p_m_e_n_t_ _b_y_ _t_h_e_ _s_a_m_e_ _t_e_a_m_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _c_a_n_ _b_e
-_i_n_s_t_a_l_l_e_d_ _e_i_t_h_e_r_ _f_r_o_m_ _P_y_P_I_ _o_r_ _b_y_ _d_o_w_n_l_o_a_d_i_n_g_ _t_h_e_ _G_i_t_H_u_b_ _r_e_p_o_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g
-_f_r_o_m_ _a_ _l_o_c_a_l_ _c_o_p_y_._ _I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _P_y_P_I_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _b_a_s_-_g_e_o_p_l_o_t_ _`_`_`
-_I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _s_o_u_r_c_e_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_G_e_o_p_l_o_t
-_p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_G_e_o_P_l_o_t_ _`_`_`_ _U_s_e_ _o_f_ _`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n_ _w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t
-_t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d_ _c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_i_s
-_s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _a_n_d_ _F_i_o_n_a_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_,_ _t_h_i_s_ _r_e_q_u_i_r_e_s
-_a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _d_u_r_i_n_g_ _t_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s_ _o_n_ _W_i_n_d_o_w_s_._ _T_h_e_s_e_ _a_d_d_i_t_i_o_n_a_l
-_s_t_e_p_s_ _a_r_e_ _a_s_ _f_o_l_l_o_w_s_:_ _W_i_n_d_o_w_s_ _o_n_l_y_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_i_p_w_i_n_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _g_d_a_l
-_p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _f_i_o_n_a_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _c_a_r_t_o_p_y_ _`_`_`_ _S_e_e_ _t_h_e_ _p_r_o_j_e_c_t_'_s_ _[_P_y_P_I_]_(_h_t_t_p_s_:
-_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_b_a_s_-_g_e_o_p_l_o_t_/_)_ _p_a_g_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_._ _#_#_ _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e
-_O_n_c_e_ _i_n_s_t_a_l_l_e_d_,_ _b_a_s_-_g_e_o_p_l_o_t_ _c_a_n_ _b_e_ _u_s_e_d_ _t_o_ _g_e_n_e_r_a_t_e_ _p_l_o_t_s_ _o_f_ _g_e_o_s_p_a_t_i_a_l_ _d_a_t_a_,
-_i_n_c_l_u_d_i_n_g_ _m_e_s_h_e_s_ _g_e_n_e_r_a_t_e_d_ _b_y_ _[_P_o_l_a_r_R_o_u_t_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/
-_P_o_l_a_r_R_o_u_t_e_)_ _o_r_ _[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_._ _T_o_ _g_e_n_e_r_a_t_e
-_a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _p_l_o_t_ _f_r_o_m_ _s_u_c_h_ _a_ _m_e_s_h_:_ _`_`_`_ _p_l_o_t___m_e_s_h_ _`_`_`_ _o_p_t_i_o_n_a_l_ _a_r_g_u_m_e_n_t_s_ _a_r_e_:
-_`_`_`_ _-_v_ _'_(_t_u_r_n_ _o_n_ _v_e_r_b_o_s_e_ _l_o_g_g_i_n_g_)_'_ _-_o_ _'_(_s_e_t_ _o_u_t_p_u_t_ _l_o_c_a_t_i_o_n_ _f_o_r_ _p_l_o_t_)_'_ _-_s_ _'
-_(_c_r_e_a_t_e_ _a_ _s_t_a_t_i_c_ _p_l_o_t_ _a_s_ _o_p_p_o_s_e_d_ _t_o_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _h_t_m_l_ _f_i_l_e_)_'_ _-_t_ _'_(_r_e_m_o_v_e_ _t_h_e
-_t_i_t_l_e_ _b_a_r_ _f_r_o_m_ _t_h_e_ _p_l_o_t_)_'_ _-_r_ _'_(_p_l_o_t_ _a_n_ _a_d_d_i_t_i_o_n_a_l_ _r_o_u_t_e_ _f_r_o_m_ _t_h_e_ _g_i_v_e_n_ _f_i_l_e_)_'_ _-
-_a_ _'_(_a_d_d_ _d_i_r_e_c_t_i_o_n_a_l_ _a_r_r_o_w_s_ _t_o_ _a_l_l_ _r_o_u_t_e_s_)_'_ _-_b_ _'_(_c_r_e_a_t_e_ _t_h_e_ _p_l_o_t_ _w_i_t_h_o_u_t_ _a
-_b_a_s_e_m_a_p_ _l_a_y_e_r_)_'_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_m_e_n_t_ _&_ _C_o_n_t_r_i_b_u_t_i_o_n_s_ _D_e_v_e_l_o_p_m_e_n_t_ _o_f_ _s_o_f_t_w_a_r_e
-_p_a_c_k_a_g_e_ _i_s_ _c_o_n_d_u_c_t_e_d_ _b_y_ _t_h_e_ _[_B_A_S_ _A_I_ _L_a_b_]_(_h_t_t_p_s_:_/_/_w_w_w_._b_a_s_._a_c_._u_k_/_t_e_a_m_/_s_c_i_e_n_c_e_-
-_t_e_a_m_s_/_a_i_-_l_a_b_/_)_._ _F_o_r_ _c_o_n_t_r_i_b_u_t_i_o_n_s_ _a_n_d_ _f_e_a_t_u_r_e_ _a_d_d_i_t_i_o_n_s_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ 
-_[_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_]_(_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_)_._ _#_#_ _L_i_c_e_n_s_e_ _D_i_s_t_r_i_b_u_t_e_d_ _u_n_d_e_r_ _t_h_e
-_M_I_T_ _l_i_c_e_n_s_e_._ _S_e_e_ _`_`_L_I_C_E_N_S_E_`_`_ _f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:
-_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
+Metadata-Version: 2.1 Name: bas_geoplot Version: 0.1.0 Summary: GeoPlot: BAS AI
+Lab plotting scripts for internal plotting & visualisation Home-page: https://
+github.com/antarctica/GeoPlot Author: Autonomous Marine Operations Planning
+(AMOP) Team, AI Lab, British Antarctic Survey Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British
+Antarctic Survey Maintainer-email: amop@bas.ac.uk License: UNKNOWN Platform:
+UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
+Audience :: Science/Research Classifier: Intended Audience :: System
+Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering Description-Content-Type: text/markdown # GeoPlot ![](logo.jpg)
+_[_P_y_P_I_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_G_e_o_P_l_o_t_ _i_s_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _a_n_d_ _s_t_a_t_i_c_ _p_l_o_t_t_i_n_g_ _t_o_o_l_k_i_t
+_d_e_v_e_l_o_p_e_d_ _b_y_ _m_e_m_b_e_r_s_ _o_f_ _t_h_e_ _B_A_S_ _A_r_t_i_f_i_c_i_a_l_ _I_n_t_e_l_l_i_g_e_n_c_e_ _L_a_b_ _a_n_d_ _d_e_s_i_g_n_e_d_ _t_o_ _b_e
+_u_s_e_d_ _i_n_ _c_o_m_b_i_n_a_t_i_o_n_ _w_i_t_h_ _o_t_h_e_r_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_s_ _u_n_d_e_r_ _d_e_v_e_l_o_p_m_e_n_t_ _b_y_ _t_h_e_ _s_a_m_e
+_t_e_a_m_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _e_i_t_h_e_r_ _f_r_o_m_ _P_y_P_I_ _o_r
+_b_y_ _d_o_w_n_l_o_a_d_i_n_g_ _t_h_e_ _G_i_t_H_u_b_ _r_e_p_o_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _f_r_o_m_ _a_ _l_o_c_a_l_ _c_o_p_y_._ _I_n_s_t_a_l_l_a_t_i_o_n
+_f_r_o_m_ _P_y_P_I_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _b_a_s_-_g_e_o_p_l_o_t_ _`_`_`_ _I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _s_o_u_r_c_e_:_ _`_`_`_ _g_i_t
+_c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_G_e_o_P_l_o_t_ _p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_G_e_o_P_l_o_t_ _`_`_`_ _U_s_e_ _o_f
+_`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n_ _w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t_ _t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d
+_c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_i_s_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _a_n_d
+_F_i_o_n_a_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_,_ _t_h_i_s_ _r_e_q_u_i_r_e_s_ _a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _d_u_r_i_n_g_ _t_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n
+_p_r_o_c_e_s_s_ _o_n_ _W_i_n_d_o_w_s_._ _T_h_e_s_e_ _a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _a_r_e_ _a_s_ _f_o_l_l_o_w_s_:_ _W_i_n_d_o_w_s_ _o_n_l_y_:_ _`_`_`
+_p_i_p_ _i_n_s_t_a_l_l_ _p_i_p_w_i_n_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _g_d_a_l_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _f_i_o_n_a_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l
+_c_a_r_t_o_p_y_ _`_`_`_ _S_e_e_ _t_h_e_ _p_r_o_j_e_c_t_'_s_ _[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_b_a_s_-_g_e_o_p_l_o_t_/
+_)_ _p_a_g_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_._ _#_#_ _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e_ _O_n_c_e_ _i_n_s_t_a_l_l_e_d_,_ _b_a_s_-_g_e_o_p_l_o_t_ _c_a_n
+_b_e_ _u_s_e_d_ _t_o_ _g_e_n_e_r_a_t_e_ _p_l_o_t_s_ _o_f_ _g_e_o_s_p_a_t_i_a_l_ _d_a_t_a_,_ _i_n_c_l_u_d_i_n_g_ _m_e_s_h_e_s_ _g_e_n_e_r_a_t_e_d_ _b_y_ 
+_[_P_o_l_a_r_R_o_u_t_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_P_o_l_a_r_R_o_u_t_e_)_ _o_r_ _[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/
+_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_._ _T_o_ _g_e_n_e_r_a_t_e_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _p_l_o_t_ _f_r_o_m_ _s_u_c_h_ _a
+_m_e_s_h_:_ _`_`_`_ _p_l_o_t___m_e_s_h_ _`_`_`_ _o_p_t_i_o_n_a_l_ _a_r_g_u_m_e_n_t_s_ _a_r_e_:_ _`_`_`_ _-_v_ _'_(_t_u_r_n_ _o_n_ _v_e_r_b_o_s_e
+_l_o_g_g_i_n_g_)_'_ _-_o_ _'_(_s_e_t_ _o_u_t_p_u_t_ _l_o_c_a_t_i_o_n_ _f_o_r_ _p_l_o_t_)_'_ _-_s_ _'_(_c_r_e_a_t_e_ _a_ _s_t_a_t_i_c_ _p_l_o_t_ _a_s
+_o_p_p_o_s_e_d_ _t_o_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _h_t_m_l_ _f_i_l_e_)_'_ _-_t_ _'_(_r_e_m_o_v_e_ _t_h_e_ _t_i_t_l_e_ _b_a_r_ _f_r_o_m_ _t_h_e_ _p_l_o_t_)_'
+_-_r_ _'_(_p_l_o_t_ _a_n_ _a_d_d_i_t_i_o_n_a_l_ _r_o_u_t_e_ _f_r_o_m_ _t_h_e_ _g_i_v_e_n_ _f_i_l_e_)_'_ _-_a_ _'_(_a_d_d_ _d_i_r_e_c_t_i_o_n_a_l_ _a_r_r_o_w_s
+_t_o_ _a_l_l_ _r_o_u_t_e_s_)_'_ _-_b_ _'_(_c_r_e_a_t_e_ _t_h_e_ _p_l_o_t_ _w_i_t_h_o_u_t_ _a_ _b_a_s_e_m_a_p_ _l_a_y_e_r_)_'_ _`_`_`_ _#_#
+_D_e_v_e_l_o_p_m_e_n_t_ _&_ _C_o_n_t_r_i_b_u_t_i_o_n_s_ _D_e_v_e_l_o_p_m_e_n_t_ _o_f_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _i_s_ _c_o_n_d_u_c_t_e_d_ _b_y_ _t_h_e
+_[_B_A_S_ _A_I_ _L_a_b_]_(_h_t_t_p_s_:_/_/_w_w_w_._b_a_s_._a_c_._u_k_/_t_e_a_m_/_s_c_i_e_n_c_e_-_t_e_a_m_s_/_a_i_-_l_a_b_/_)_._ _F_o_r
+_c_o_n_t_r_i_b_u_t_i_o_n_s_ _a_n_d_ _f_e_a_t_u_r_e_ _a_d_d_i_t_i_o_n_s_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_a_m_o_p_@_b_a_s_._a_c_._u_k_]
+_(_a_m_o_p_@_b_a_s_._a_c_._u_k_)_._ _#_#_ _L_i_c_e_n_s_e_ _D_i_s_t_r_i_b_u_t_e_d_ _u_n_d_e_r_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_._ _S_e_e_ _`_`_L_I_C_E_N_S_E_`_`
+_f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_v_/_d_a_t_a_d_o_g_-
+_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_d_m_/
+_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
```

### Comparing `bas_geoplot-0.0.25/README.md` & `bas_geoplot-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Installation from PyPI:
 ```
 pip install bas-geoplot
 ```
 
 Installation from source:
 ```
-git clone https://github.com/Antarctica/Geoplot
+git clone https://github.com/Antarctica/GeoPlot
 pip install -e ./GeoPlot
 ```
 
 Use of `-e` is optional, based on whether you want to be able to edit the installed copy of the package.
 
 Some features of this software package require GDAL and Fiona to be installed, this requires additional steps during the installation process on Windows. These additional steps are as follows:
 
@@ -54,16 +54,13 @@
 -r '(plot an additional route from the given file)'
 -a '(add directional arrows to all routes)'
 -b '(create the plot without a basemap layer)'
 ```
 
 ## Development & Contributions
 Development of software package is conducted by the [BAS AI Lab](https://www.bas.ac.uk/team/science-teams/ai-lab/).
-
-For contributions and feature additions please contact [polarroute@bas.ac.uk](polarroute@bas.ac.uk).
-
+For contributions and feature additions please contact [amop@bas.ac.uk](amop@bas.ac.uk).
 
 ## License
 Distributed under the MIT license. See ``LICENSE`` for more information.
-
 [version]: https://img.shields.io/GeoPlot/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/GeoPlot/dm/datadog-metrics.svg?style=flat-square
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # GeoPlot ![](logo.jpg) _[_P_y_P_I_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_G_e_o_P_l_o_t_ _i_s_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _a_n_d
 _s_t_a_t_i_c_ _p_l_o_t_t_i_n_g_ _t_o_o_l_k_i_t_ _d_e_v_e_l_o_p_e_d_ _b_y_ _m_e_m_b_e_r_s_ _o_f_ _t_h_e_ _B_A_S_ _A_r_t_i_f_i_c_i_a_l_ _I_n_t_e_l_l_i_g_e_n_c_e
 _L_a_b_ _a_n_d_ _d_e_s_i_g_n_e_d_ _t_o_ _b_e_ _u_s_e_d_ _i_n_ _c_o_m_b_i_n_a_t_i_o_n_ _w_i_t_h_ _o_t_h_e_r_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_s_ _u_n_d_e_r
 _d_e_v_e_l_o_p_m_e_n_t_ _b_y_ _t_h_e_ _s_a_m_e_ _t_e_a_m_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _c_a_n_ _b_e
 _i_n_s_t_a_l_l_e_d_ _e_i_t_h_e_r_ _f_r_o_m_ _P_y_P_I_ _o_r_ _b_y_ _d_o_w_n_l_o_a_d_i_n_g_ _t_h_e_ _G_i_t_H_u_b_ _r_e_p_o_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g
 _f_r_o_m_ _a_ _l_o_c_a_l_ _c_o_p_y_._ _I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _P_y_P_I_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _b_a_s_-_g_e_o_p_l_o_t_ _`_`_`
-_I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _s_o_u_r_c_e_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_G_e_o_p_l_o_t
+_I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _s_o_u_r_c_e_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_G_e_o_P_l_o_t
 _p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_G_e_o_P_l_o_t_ _`_`_`_ _U_s_e_ _o_f_ _`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n_ _w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t
 _t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d_ _c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_i_s
 _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _a_n_d_ _F_i_o_n_a_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_,_ _t_h_i_s_ _r_e_q_u_i_r_e_s
 _a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _d_u_r_i_n_g_ _t_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s_ _o_n_ _W_i_n_d_o_w_s_._ _T_h_e_s_e_ _a_d_d_i_t_i_o_n_a_l
 _s_t_e_p_s_ _a_r_e_ _a_s_ _f_o_l_l_o_w_s_:_ _W_i_n_d_o_w_s_ _o_n_l_y_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_i_p_w_i_n_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _g_d_a_l
 _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _f_i_o_n_a_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _c_a_r_t_o_p_y_ _`_`_`_ _S_e_e_ _t_h_e_ _p_r_o_j_e_c_t_'_s_ _[_P_y_P_I_]_(_h_t_t_p_s_:
 _/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_b_a_s_-_g_e_o_p_l_o_t_/_)_ _p_a_g_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_._ _#_#_ _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e
@@ -19,11 +19,11 @@
 _`_`_`_ _-_v_ _'_(_t_u_r_n_ _o_n_ _v_e_r_b_o_s_e_ _l_o_g_g_i_n_g_)_'_ _-_o_ _'_(_s_e_t_ _o_u_t_p_u_t_ _l_o_c_a_t_i_o_n_ _f_o_r_ _p_l_o_t_)_'_ _-_s_ _'
 _(_c_r_e_a_t_e_ _a_ _s_t_a_t_i_c_ _p_l_o_t_ _a_s_ _o_p_p_o_s_e_d_ _t_o_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _h_t_m_l_ _f_i_l_e_)_'_ _-_t_ _'_(_r_e_m_o_v_e_ _t_h_e
 _t_i_t_l_e_ _b_a_r_ _f_r_o_m_ _t_h_e_ _p_l_o_t_)_'_ _-_r_ _'_(_p_l_o_t_ _a_n_ _a_d_d_i_t_i_o_n_a_l_ _r_o_u_t_e_ _f_r_o_m_ _t_h_e_ _g_i_v_e_n_ _f_i_l_e_)_'_ _-
 _a_ _'_(_a_d_d_ _d_i_r_e_c_t_i_o_n_a_l_ _a_r_r_o_w_s_ _t_o_ _a_l_l_ _r_o_u_t_e_s_)_'_ _-_b_ _'_(_c_r_e_a_t_e_ _t_h_e_ _p_l_o_t_ _w_i_t_h_o_u_t_ _a
 _b_a_s_e_m_a_p_ _l_a_y_e_r_)_'_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_m_e_n_t_ _&_ _C_o_n_t_r_i_b_u_t_i_o_n_s_ _D_e_v_e_l_o_p_m_e_n_t_ _o_f_ _s_o_f_t_w_a_r_e
 _p_a_c_k_a_g_e_ _i_s_ _c_o_n_d_u_c_t_e_d_ _b_y_ _t_h_e_ _[_B_A_S_ _A_I_ _L_a_b_]_(_h_t_t_p_s_:_/_/_w_w_w_._b_a_s_._a_c_._u_k_/_t_e_a_m_/_s_c_i_e_n_c_e_-
 _t_e_a_m_s_/_a_i_-_l_a_b_/_)_._ _F_o_r_ _c_o_n_t_r_i_b_u_t_i_o_n_s_ _a_n_d_ _f_e_a_t_u_r_e_ _a_d_d_i_t_i_o_n_s_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ 
-_[_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_]_(_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_)_._ _#_#_ _L_i_c_e_n_s_e_ _D_i_s_t_r_i_b_u_t_e_d_ _u_n_d_e_r_ _t_h_e
-_M_I_T_ _l_i_c_e_n_s_e_._ _S_e_e_ _`_`_L_I_C_E_N_S_E_`_`_ _f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:
-_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
+_[_a_m_o_p_@_b_a_s_._a_c_._u_k_]_(_a_m_o_p_@_b_a_s_._a_c_._u_k_)_._ _#_#_ _L_i_c_e_n_s_e_ _D_i_s_t_r_i_b_u_t_e_d_ _u_n_d_e_r_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_.
+_S_e_e_ _`_`_L_I_C_E_N_S_E_`_`_ _f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_G_e_o_P_l_o_t_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:_ _h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
```

### Comparing `bas_geoplot-0.0.25/bas_geoplot/cli.py` & `bas_geoplot-0.1.0/bas_geoplot/cli.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.25/bas_geoplot/config/interactive.json` & `bas_geoplot-0.1.0/bas_geoplot/config/interactive.json`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.25/bas_geoplot/config/static.json` & `bas_geoplot-0.1.0/bas_geoplot/config/static.json`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.25/bas_geoplot/interactive.py` & `bas_geoplot-0.1.0/bas_geoplot/interactive.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from folium import plugins
 from branca.colormap import linear
 from branca.element import MacroElement
 from shapely import wkt
 from shapely.geometry import Polygon
 from jinja2 import Template
 from pyproj import Geod
-from bas_geoplot.utils import convert_decimal_days
+from bas_geoplot.utils import convert_decimal_days, split_at_antimeridian
 
 
 def params_object(layer, predefined=None, **kwargs):
     # Loading config of standards
     p_file = os.path.join(os.path.dirname(__file__),'config','interactive.json')
     with open(p_file, 'r') as f:
         p = json.load(f)[layer]
@@ -349,94 +349,132 @@
                         max_val = (np.array(path['properties'][p['data_name']])*p['scaling_factor']).max()
 
                     if (np.array(path['properties'][p['data_name']])*p['scaling_factor']).min() < min_val:
                         min_val = (np.array(path['properties'][p['data_name']])*p['scaling_factor']).min()
         # Determining max travel-times of all paths
         for path in paths:
             points   = np.array(path['geometry']['coordinates'])
+            # Get index of any consecutive points that span over 180 deg in longitude
+            # i.e. get index of places which cross the antimeridian
+            split_at_idxs = [i + 1 for i in range(len(points)-1)
+                             if (np.abs(points[i][0] - points[i+1][0]) >= 180) ]
+            
+            segments = np.split(points, split_at_idxs)
+            extended_segments = []
+            for i, segment in enumerate(segments):
+
+                # If not the first segment, add the last point of the previous segment
+                # to the beginning of this segment to better visualise the path 
+                if i != 0:
+                    # Let this singular point be on the opposite side of the antimeridian
+                    orig_coords = segments[i-1][-1]
+                    if orig_coords[0] > 0: 
+                        rollover_coords = [orig_coords[0] - 360, orig_coords[1]]
+                    else:
+                        rollover_coords = [orig_coords[0] + 360, orig_coords[1]]
+                    
+                    segment = np.insert(segment, 0, rollover_coords, axis=0)
+                # If not the last segment, add the first point of the next segment
+                # to the end of this segment to better visualise the path 
+                if i != len(segments)-1:
+                    # Let this singular point be on the opposite side of the antimeridian
+                    orig_coords = segments[i+1][0]
+                    if orig_coords[0] > 0: 
+                        rollover_coords = [orig_coords[0] - 360, orig_coords[1]]
+                    else:
+                        rollover_coords = [orig_coords[0] + 360, orig_coords[1]]
+                    
+                    segment = np.insert(segment, -1, rollover_coords, axis=0)
+                # Add to list of 'extended' segments
+                extended_segments += [segment]
 
             start_wpt = path['properties']['from']
             end_wpt   = path['properties']['to']
-
             if p['data_name']:
                 try:
                     data_val = np.array(path['properties'][p['data_name']])*p['scaling_factor']
                 except:
                     continue
             else:
                 data_val = np.array(len(points))
-
+            
             # Find the max value for this path for display in pop-up
             path_max = np.max(data_val)
+            # For each series of points in each segment (defined by crossing antimeridian)
+            for points in extended_segments:
 
-            points[:,0] = points[:,0]
-            points = points[:,::-1]
+                points[:,0] = points[:,0]
+                points = points[:,::-1]
+
+                if type(p['line_color']) is dict:
+                    if "cmin" in p["line_color"].keys():
+                        min_val = p["line_color"]['cmin']
+                    if "cmax" in p["line_color"].keys():
+                        max_val = p["line_color"]['cmax']
+
+                    colormap = linear._colormaps[p["line_color"]['color']].scale(min_val,max_val)
+                    if p['unit'] == 'Days':
+                        colormap.caption = '{} ({}, Max Value: {})'.format(name, p['unit'], convert_decimal_days(max_val))
+                    else:
+                        colormap.caption = '{} ({}, Max Value: {:.3f})'.format(name,p['unit'],max_val)
+                    folium.ColorLine(points,data_val, colormap=colormap,nb_steps=50, weight=p['line_width'],
+                                    opacity=p['line_opacity']).add_to(pths)
+
+                    if p['unit'] == 'Days':
+                        folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
+                                        popup = "Path - {} to {}\n{} = {}".format(start_wpt, end_wpt, p['data_name'],
+                                                                                convert_decimal_days(path_max))
+                                        ).add_to(pths)
+                    else:
+                        folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
+                                        popup="Path - {} to {}\n{} = {:.3f} {}".format(start_wpt, end_wpt, p['data_name'],
+                                                                                    path_max, p['unit'])).add_to(pths)
+
+                    if arrows:
+                        # Every 10 segments, draw a triangle as an arrow head
+                        for idx in range(1, len(points), 10):
+                            lon_diff = points[idx, 0] - points[idx-1, 0]
+                            lat_diff = points[idx, 1] - points[idx-1, 1]
+                            loc = [points[idx,0],points[idx,1]]
+                            heading = -np.degrees(np.arctan2(lon_diff, lat_diff))
+                            folium.RegularPolygonMarker(location=loc, rotation=heading,
+                                                        color=colormap(data_val[idx]), fill=True,
+                                                        number_of_sides=3, radius=10).add_to(pths)
 
-            if type(p['line_color']) is dict:
-                if "cmin" in p["line_color"].keys():
-                    min_val = p["line_color"]['cmin']
-                if "cmax" in p["line_color"].keys():
-                    max_val = p["line_color"]['cmax']
-
-                colormap = linear._colormaps[p["line_color"]['color']].scale(min_val,max_val)
-                if p['unit'] == 'Days':
-                    colormap.caption = '{} ({}, Max Value: {})'.format(name, p['unit'], convert_decimal_days(max_val))
-                else:
-                    colormap.caption = '{} ({}, Max Value: {:.3f})'.format(name,p['unit'],max_val)
-                folium.ColorLine(points,data_val, colormap=colormap,nb_steps=50, weight=p['line_width'],
-                                 opacity=p['line_opacity']).add_to(pths)
-
-                if p['unit'] == 'Days':
-                    folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
-                                    popup = "Path - {} to {}\n{} = {}".format(start_wpt, end_wpt, p['data_name'],
-                                                                              convert_decimal_days(path_max))
-                                    ).add_to(pths)
                 else:
-                    folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
-                                    popup="Path - {} to {}\n{} = {:.3f} {}".format(start_wpt, end_wpt, p['data_name'],
-                                                                                   path_max, p['unit'])).add_to(pths)
-
-                if arrows:
-                    # Every 10 segments, draw a triangle as an arrow head
-                    for idx in range(1, len(points), 10):
-                        lon_diff = points[idx, 0] - points[idx-1, 0]
-                        lat_diff = points[idx, 1] - points[idx-1, 1]
-                        loc = [points[idx,0],points[idx,1]]
-                        heading = -np.degrees(np.arctan2(lon_diff, lat_diff))
-                        folium.RegularPolygonMarker(location=loc, rotation=heading,
-                                                    color=colormap(data_val[idx]), fill=True,
-                                                    number_of_sides=3, radius=10).add_to(pths)
+                    folium.PolyLine(points, color=p['line_color'], weight=p['line_width'], opacity=p['line_opacity'],
+                                    popup = "Path - {} to {}".format(start_wpt,end_wpt)).add_to(pths)
 
-            else:
-                folium.PolyLine(points, color=p['line_color'], weight=p['line_width'], opacity=p['line_opacity'],
-                                popup = "Path - {} to {}".format(start_wpt,end_wpt)).add_to(pths)
+                    if arrows:
+                        # Every 10 segments, draw a triangle as an arrow head
+                        for idx in range(1, len(points), 10):
+                            lon_diff = points[idx, 0] - points[idx-1, 0]
+                            lat_diff = points[idx, 1] - points[idx-1, 1]
+                            loc = [points[idx,0],points[idx,1]]
+                            heading = -np.degrees(np.arctan2(lon_diff, lat_diff))
+                            folium.RegularPolygonMarker(location=loc, rotation=heading,
+                                                        color=p['line_color'], fill=True,
+                                                        number_of_sides=3, radius=10).add_to(pths)
 
-                if arrows:
-                    # Every 10 segments, draw a triangle as an arrow head
-                    for idx in range(1, len(points), 10):
-                        lon_diff = points[idx, 0] - points[idx-1, 0]
-                        lat_diff = points[idx, 1] - points[idx-1, 1]
+                if p['path_points']:
+                    for idx in range(len(points)):
                         loc = [points[idx,0],points[idx,1]]
-                        heading = -np.degrees(np.arctan2(lon_diff, lat_diff))
-                        folium.RegularPolygonMarker(location=loc, rotation=heading,
-                                                    color=p['line_color'], fill=True,
-                                                    number_of_sides=3, radius=10).add_to(pths)
-
-            if p['path_points']:
-                for idx in range(len(points)):
-                    loc = [points[idx,0],points[idx,1]]
-                    folium.Marker(
-                        location=loc,
-                        icon=folium.plugins.BeautifyIcon(icon='circle',
-                                                    border_color='transparent',
-                                                    background_color='transparent',
-                                                    border_width=1,
-                                                    text_color='black',
-                                                    inner_icon_style='margin:0px;font-size:0.8em')
-                    ).add_to(pths)
+                        folium.Marker(
+                            location=loc,
+                            icon=folium.plugins.BeautifyIcon(icon='circle',
+                                                        border_color='transparent',
+                                                        background_color='transparent',
+                                                        border_width=1,
+                                                        text_color='black',
+                                                        inner_icon_style='margin:0px;font-size:0.8em')
+                        ).add_to(pths)
+
+                # Truncate data_val to not include the first n points so that colourmap is continuous
+                # over the antimeridian
+                data_val = data_val[len(points)-1:]
         
         if type(p['line_color']) is dict:
             self.map.add_child(colormap)
             self.map.add_child(BindColormap(pths,colormap))
 
     def Points(self,dataframe_points,name,show=True,predefined=None,**kwargs):
         """
@@ -492,15 +530,16 @@
                     package files
                 plot_sectors (boolean): Display sectorised list values as eight individual polygons
         """
         p = params_object('Maps', predefined=predefined, **kwargs)
 
         dataframe_pandas = copy.copy(dataframe_pandas)
         dataframe_pandas['geometry'] = dataframe_pandas['geometry'].apply(wkt.loads)
-
+        # Split cellboxes into multipolygons if crosses antimeridian
+        dataframe_pandas = split_at_antimeridian(dataframe_pandas)
         # Don't plot anything in the land cells unless, of course, we are plotting the land mask
         if 'land' in dataframe_pandas.keys() and p['data_name'] != 'land':
             dataframe_pandas = dataframe_pandas[dataframe_pandas['land']==False].reset_index(drop=True)
 
         # For array values we either plot each value as a separate polygon or just the average of the values in the list
         if any(type(d) is list for d in dataframe_pandas[p['data_name']]):
             if plot_sectors:
@@ -617,14 +656,15 @@
         """
 
         p = params_object('MeshInfo', predefined=predefined, **kwargs)
 
         dataframe_pandas = copy.copy(pd.DataFrame(mesh))
         dataframe_pandas['geometry'] = dataframe_pandas['geometry'].apply(wkt.loads)
         dataframe_geo = gpd.GeoDataFrame(dataframe_pandas,crs='EPSG:4326', geometry='geometry')
+        dataframe_geo = split_at_antimeridian(dataframe_geo)
 
         p = p['fields']
 
         column_names = ['geometry']
         for col_info in p:
             try:
                 column_name = col_info['Name']
```

### Comparing `bas_geoplot-0.0.25/bas_geoplot/static.py` & `bas_geoplot-0.1.0/bas_geoplot/static.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.25/bas_geoplot.egg-info/PKG-INFO` & `bas_geoplot-0.1.0/bas_geoplot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: bas-geoplot
-Version: 0.0.25
-Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
+Version: 0.1.0
+Summary: GeoPlot: BAS AI Lab plotting scripts for internal plotting & visualisation
 Home-page: https://github.com/antarctica/GeoPlot
-Author: BAS AI Lab
-Author-email: jonsmi@bas.ac.uk
-Maintainer: BAS AI Lab
-Maintainer-email: jonsmi@bas.ac.uk
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Classifier: 
 Description-Content-Type: text/markdown
 
 # GeoPlot
 
 ![](logo.jpg)
 
 <a href="https://pypi.org/project/bas-geoplot/"><img src="https://img.shields.io/pypi/v/bas-geoplot" alt="PyPI">
@@ -41,15 +39,15 @@
 Installation from PyPI:
 ```
 pip install bas-geoplot
 ```
 
 Installation from source:
 ```
-git clone https://github.com/Antarctica/Geoplot
+git clone https://github.com/Antarctica/GeoPlot
 pip install -e ./GeoPlot
 ```
 
 Use of `-e` is optional, based on whether you want to be able to edit the installed copy of the package.
 
 Some features of this software package require GDAL and Fiona to be installed, this requires additional steps during the installation process on Windows. These additional steps are as follows:
 
@@ -80,18 +78,15 @@
 -r '(plot an additional route from the given file)'
 -a '(add directional arrows to all routes)'
 -b '(create the plot without a basemap layer)'
 ```
 
 ## Development & Contributions
 Development of software package is conducted by the [BAS AI Lab](https://www.bas.ac.uk/team/science-teams/ai-lab/).
-
-For contributions and feature additions please contact [polarroute@bas.ac.uk](polarroute@bas.ac.uk).
-
+For contributions and feature additions please contact [amop@bas.ac.uk](amop@bas.ac.uk).
 
 ## License
 Distributed under the MIT license. See ``LICENSE`` for more information.
-
 [version]: https://img.shields.io/GeoPlot/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/GeoPlot/dm/datadog-metrics.svg?style=flat-square
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: bas-geoplot Version: 0.0.25 Summary: GeoPlot: BAS
-AI Lab plotting scripts built on Folium Home-page: https://github.com/
-antarctica/GeoPlot Author: BAS AI Lab Author-email: jonsmi@bas.ac.uk
-Maintainer: BAS AI Lab Maintainer-email: jonsmi@bas.ac.uk License: UNKNOWN
-Platform: UNKNOWN Classifier: Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: System Administrators Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Scientific/Engineering Classifier: Description-Content-Type: text/markdown #
-GeoPlot ![](logo.jpg) _[_P_y_P_I_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_G_e_o_P_l_o_t_ _i_s_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _a_n_d
-_s_t_a_t_i_c_ _p_l_o_t_t_i_n_g_ _t_o_o_l_k_i_t_ _d_e_v_e_l_o_p_e_d_ _b_y_ _m_e_m_b_e_r_s_ _o_f_ _t_h_e_ _B_A_S_ _A_r_t_i_f_i_c_i_a_l_ _I_n_t_e_l_l_i_g_e_n_c_e
-_L_a_b_ _a_n_d_ _d_e_s_i_g_n_e_d_ _t_o_ _b_e_ _u_s_e_d_ _i_n_ _c_o_m_b_i_n_a_t_i_o_n_ _w_i_t_h_ _o_t_h_e_r_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_s_ _u_n_d_e_r
-_d_e_v_e_l_o_p_m_e_n_t_ _b_y_ _t_h_e_ _s_a_m_e_ _t_e_a_m_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _c_a_n_ _b_e
-_i_n_s_t_a_l_l_e_d_ _e_i_t_h_e_r_ _f_r_o_m_ _P_y_P_I_ _o_r_ _b_y_ _d_o_w_n_l_o_a_d_i_n_g_ _t_h_e_ _G_i_t_H_u_b_ _r_e_p_o_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g
-_f_r_o_m_ _a_ _l_o_c_a_l_ _c_o_p_y_._ _I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _P_y_P_I_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _b_a_s_-_g_e_o_p_l_o_t_ _`_`_`
-_I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _s_o_u_r_c_e_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_G_e_o_p_l_o_t
-_p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_G_e_o_P_l_o_t_ _`_`_`_ _U_s_e_ _o_f_ _`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n_ _w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t
-_t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d_ _c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_i_s
-_s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _a_n_d_ _F_i_o_n_a_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_,_ _t_h_i_s_ _r_e_q_u_i_r_e_s
-_a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _d_u_r_i_n_g_ _t_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s_ _o_n_ _W_i_n_d_o_w_s_._ _T_h_e_s_e_ _a_d_d_i_t_i_o_n_a_l
-_s_t_e_p_s_ _a_r_e_ _a_s_ _f_o_l_l_o_w_s_:_ _W_i_n_d_o_w_s_ _o_n_l_y_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_i_p_w_i_n_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _g_d_a_l
-_p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _f_i_o_n_a_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _c_a_r_t_o_p_y_ _`_`_`_ _S_e_e_ _t_h_e_ _p_r_o_j_e_c_t_'_s_ _[_P_y_P_I_]_(_h_t_t_p_s_:
-_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_b_a_s_-_g_e_o_p_l_o_t_/_)_ _p_a_g_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_._ _#_#_ _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e
-_O_n_c_e_ _i_n_s_t_a_l_l_e_d_,_ _b_a_s_-_g_e_o_p_l_o_t_ _c_a_n_ _b_e_ _u_s_e_d_ _t_o_ _g_e_n_e_r_a_t_e_ _p_l_o_t_s_ _o_f_ _g_e_o_s_p_a_t_i_a_l_ _d_a_t_a_,
-_i_n_c_l_u_d_i_n_g_ _m_e_s_h_e_s_ _g_e_n_e_r_a_t_e_d_ _b_y_ _[_P_o_l_a_r_R_o_u_t_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/
-_P_o_l_a_r_R_o_u_t_e_)_ _o_r_ _[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_._ _T_o_ _g_e_n_e_r_a_t_e
-_a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _p_l_o_t_ _f_r_o_m_ _s_u_c_h_ _a_ _m_e_s_h_:_ _`_`_`_ _p_l_o_t___m_e_s_h_ _`_`_`_ _o_p_t_i_o_n_a_l_ _a_r_g_u_m_e_n_t_s_ _a_r_e_:
-_`_`_`_ _-_v_ _'_(_t_u_r_n_ _o_n_ _v_e_r_b_o_s_e_ _l_o_g_g_i_n_g_)_'_ _-_o_ _'_(_s_e_t_ _o_u_t_p_u_t_ _l_o_c_a_t_i_o_n_ _f_o_r_ _p_l_o_t_)_'_ _-_s_ _'
-_(_c_r_e_a_t_e_ _a_ _s_t_a_t_i_c_ _p_l_o_t_ _a_s_ _o_p_p_o_s_e_d_ _t_o_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _h_t_m_l_ _f_i_l_e_)_'_ _-_t_ _'_(_r_e_m_o_v_e_ _t_h_e
-_t_i_t_l_e_ _b_a_r_ _f_r_o_m_ _t_h_e_ _p_l_o_t_)_'_ _-_r_ _'_(_p_l_o_t_ _a_n_ _a_d_d_i_t_i_o_n_a_l_ _r_o_u_t_e_ _f_r_o_m_ _t_h_e_ _g_i_v_e_n_ _f_i_l_e_)_'_ _-
-_a_ _'_(_a_d_d_ _d_i_r_e_c_t_i_o_n_a_l_ _a_r_r_o_w_s_ _t_o_ _a_l_l_ _r_o_u_t_e_s_)_'_ _-_b_ _'_(_c_r_e_a_t_e_ _t_h_e_ _p_l_o_t_ _w_i_t_h_o_u_t_ _a
-_b_a_s_e_m_a_p_ _l_a_y_e_r_)_'_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_m_e_n_t_ _&_ _C_o_n_t_r_i_b_u_t_i_o_n_s_ _D_e_v_e_l_o_p_m_e_n_t_ _o_f_ _s_o_f_t_w_a_r_e
-_p_a_c_k_a_g_e_ _i_s_ _c_o_n_d_u_c_t_e_d_ _b_y_ _t_h_e_ _[_B_A_S_ _A_I_ _L_a_b_]_(_h_t_t_p_s_:_/_/_w_w_w_._b_a_s_._a_c_._u_k_/_t_e_a_m_/_s_c_i_e_n_c_e_-
-_t_e_a_m_s_/_a_i_-_l_a_b_/_)_._ _F_o_r_ _c_o_n_t_r_i_b_u_t_i_o_n_s_ _a_n_d_ _f_e_a_t_u_r_e_ _a_d_d_i_t_i_o_n_s_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ 
-_[_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_]_(_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_)_._ _#_#_ _L_i_c_e_n_s_e_ _D_i_s_t_r_i_b_u_t_e_d_ _u_n_d_e_r_ _t_h_e
-_M_I_T_ _l_i_c_e_n_s_e_._ _S_e_e_ _`_`_L_I_C_E_N_S_E_`_`_ _f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:
-_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
+Metadata-Version: 2.1 Name: bas-geoplot Version: 0.1.0 Summary: GeoPlot: BAS AI
+Lab plotting scripts for internal plotting & visualisation Home-page: https://
+github.com/antarctica/GeoPlot Author: Autonomous Marine Operations Planning
+(AMOP) Team, AI Lab, British Antarctic Survey Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British
+Antarctic Survey Maintainer-email: amop@bas.ac.uk License: UNKNOWN Platform:
+UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
+Audience :: Science/Research Classifier: Intended Audience :: System
+Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering Description-Content-Type: text/markdown # GeoPlot ![](logo.jpg)
+_[_P_y_P_I_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_G_e_o_P_l_o_t_ _i_s_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _a_n_d_ _s_t_a_t_i_c_ _p_l_o_t_t_i_n_g_ _t_o_o_l_k_i_t
+_d_e_v_e_l_o_p_e_d_ _b_y_ _m_e_m_b_e_r_s_ _o_f_ _t_h_e_ _B_A_S_ _A_r_t_i_f_i_c_i_a_l_ _I_n_t_e_l_l_i_g_e_n_c_e_ _L_a_b_ _a_n_d_ _d_e_s_i_g_n_e_d_ _t_o_ _b_e
+_u_s_e_d_ _i_n_ _c_o_m_b_i_n_a_t_i_o_n_ _w_i_t_h_ _o_t_h_e_r_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_s_ _u_n_d_e_r_ _d_e_v_e_l_o_p_m_e_n_t_ _b_y_ _t_h_e_ _s_a_m_e
+_t_e_a_m_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _e_i_t_h_e_r_ _f_r_o_m_ _P_y_P_I_ _o_r
+_b_y_ _d_o_w_n_l_o_a_d_i_n_g_ _t_h_e_ _G_i_t_H_u_b_ _r_e_p_o_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _f_r_o_m_ _a_ _l_o_c_a_l_ _c_o_p_y_._ _I_n_s_t_a_l_l_a_t_i_o_n
+_f_r_o_m_ _P_y_P_I_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _b_a_s_-_g_e_o_p_l_o_t_ _`_`_`_ _I_n_s_t_a_l_l_a_t_i_o_n_ _f_r_o_m_ _s_o_u_r_c_e_:_ _`_`_`_ _g_i_t
+_c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_G_e_o_P_l_o_t_ _p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_G_e_o_P_l_o_t_ _`_`_`_ _U_s_e_ _o_f
+_`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n_ _w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t_ _t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d
+_c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_i_s_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _a_n_d
+_F_i_o_n_a_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_,_ _t_h_i_s_ _r_e_q_u_i_r_e_s_ _a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _d_u_r_i_n_g_ _t_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n
+_p_r_o_c_e_s_s_ _o_n_ _W_i_n_d_o_w_s_._ _T_h_e_s_e_ _a_d_d_i_t_i_o_n_a_l_ _s_t_e_p_s_ _a_r_e_ _a_s_ _f_o_l_l_o_w_s_:_ _W_i_n_d_o_w_s_ _o_n_l_y_:_ _`_`_`
+_p_i_p_ _i_n_s_t_a_l_l_ _p_i_p_w_i_n_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _g_d_a_l_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l_ _f_i_o_n_a_ _p_i_p_w_i_n_ _i_n_s_t_a_l_l
+_c_a_r_t_o_p_y_ _`_`_`_ _S_e_e_ _t_h_e_ _p_r_o_j_e_c_t_'_s_ _[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_b_a_s_-_g_e_o_p_l_o_t_/
+_)_ _p_a_g_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_._ _#_#_ _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e_ _O_n_c_e_ _i_n_s_t_a_l_l_e_d_,_ _b_a_s_-_g_e_o_p_l_o_t_ _c_a_n
+_b_e_ _u_s_e_d_ _t_o_ _g_e_n_e_r_a_t_e_ _p_l_o_t_s_ _o_f_ _g_e_o_s_p_a_t_i_a_l_ _d_a_t_a_,_ _i_n_c_l_u_d_i_n_g_ _m_e_s_h_e_s_ _g_e_n_e_r_a_t_e_d_ _b_y_ 
+_[_P_o_l_a_r_R_o_u_t_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_P_o_l_a_r_R_o_u_t_e_)_ _o_r_ _[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/
+_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_._ _T_o_ _g_e_n_e_r_a_t_e_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _p_l_o_t_ _f_r_o_m_ _s_u_c_h_ _a
+_m_e_s_h_:_ _`_`_`_ _p_l_o_t___m_e_s_h_ _`_`_`_ _o_p_t_i_o_n_a_l_ _a_r_g_u_m_e_n_t_s_ _a_r_e_:_ _`_`_`_ _-_v_ _'_(_t_u_r_n_ _o_n_ _v_e_r_b_o_s_e
+_l_o_g_g_i_n_g_)_'_ _-_o_ _'_(_s_e_t_ _o_u_t_p_u_t_ _l_o_c_a_t_i_o_n_ _f_o_r_ _p_l_o_t_)_'_ _-_s_ _'_(_c_r_e_a_t_e_ _a_ _s_t_a_t_i_c_ _p_l_o_t_ _a_s
+_o_p_p_o_s_e_d_ _t_o_ _a_n_ _i_n_t_e_r_a_c_t_i_v_e_ _h_t_m_l_ _f_i_l_e_)_'_ _-_t_ _'_(_r_e_m_o_v_e_ _t_h_e_ _t_i_t_l_e_ _b_a_r_ _f_r_o_m_ _t_h_e_ _p_l_o_t_)_'
+_-_r_ _'_(_p_l_o_t_ _a_n_ _a_d_d_i_t_i_o_n_a_l_ _r_o_u_t_e_ _f_r_o_m_ _t_h_e_ _g_i_v_e_n_ _f_i_l_e_)_'_ _-_a_ _'_(_a_d_d_ _d_i_r_e_c_t_i_o_n_a_l_ _a_r_r_o_w_s
+_t_o_ _a_l_l_ _r_o_u_t_e_s_)_'_ _-_b_ _'_(_c_r_e_a_t_e_ _t_h_e_ _p_l_o_t_ _w_i_t_h_o_u_t_ _a_ _b_a_s_e_m_a_p_ _l_a_y_e_r_)_'_ _`_`_`_ _#_#
+_D_e_v_e_l_o_p_m_e_n_t_ _&_ _C_o_n_t_r_i_b_u_t_i_o_n_s_ _D_e_v_e_l_o_p_m_e_n_t_ _o_f_ _s_o_f_t_w_a_r_e_ _p_a_c_k_a_g_e_ _i_s_ _c_o_n_d_u_c_t_e_d_ _b_y_ _t_h_e
+_[_B_A_S_ _A_I_ _L_a_b_]_(_h_t_t_p_s_:_/_/_w_w_w_._b_a_s_._a_c_._u_k_/_t_e_a_m_/_s_c_i_e_n_c_e_-_t_e_a_m_s_/_a_i_-_l_a_b_/_)_._ _F_o_r
+_c_o_n_t_r_i_b_u_t_i_o_n_s_ _a_n_d_ _f_e_a_t_u_r_e_ _a_d_d_i_t_i_o_n_s_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_a_m_o_p_@_b_a_s_._a_c_._u_k_]
+_(_a_m_o_p_@_b_a_s_._a_c_._u_k_)_._ _#_#_ _L_i_c_e_n_s_e_ _D_i_s_t_r_i_b_u_t_e_d_ _u_n_d_e_r_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_._ _S_e_e_ _`_`_L_I_C_E_N_S_E_`_`
+_f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_v_/_d_a_t_a_d_o_g_-
+_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_G_e_o_P_l_o_t_/_d_m_/
+_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
```

### Comparing `bas_geoplot-0.0.25/setup.py` & `bas_geoplot-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,38 +8,50 @@
 def get_content(filename):
     with open(filename, "r") as fh:
         return fh.read()
 
 
 requirements = get_content("requirements.txt")
 
+print([el.lstrip() for el in """
+        Development Status :: 3 - Alpha
+        Intended Audience :: Science/Research
+        Intended Audience :: System Administrators
+        License :: OSI Approved :: MIT License
+        Natural Language :: English
+        Operating System :: OS Independent
+        Programming Language :: Python
+        Programming Language :: Python :: 3
+        Programming Language :: Python :: 3.8
+        Programming Language :: Python :: 3.9
+        Topic :: Scientific/Engineering
+    """.split('\n')])
+
 setup(
     name=bas_geoplot.__name__,
     version=bas_geoplot.__version__,
     description=bas_geoplot.__description__,
     long_description=get_content("README.md"),
     long_description_content_type="text/markdown",
     author=bas_geoplot.__author__,
     author_email=bas_geoplot.__email__,
     maintainer=bas_geoplot.__author__,
     maintainer_email=bas_geoplot.__email__,
     url="https://github.com/antarctica/GeoPlot",
-    classifiers=[el.lstrip() for el in """
-        Development Status :: 3 - Alpha
+    classifiers=[el.lstrip() for el in """Development Status :: 3 - Alpha
         Intended Audience :: Science/Research
         Intended Audience :: System Administrators
         License :: OSI Approved :: MIT License
         Natural Language :: English
         Operating System :: OS Independent
         Programming Language :: Python
         Programming Language :: Python :: 3
         Programming Language :: Python :: 3.8
         Programming Language :: Python :: 3.9
-        Topic :: Scientific/Engineering
-    """.split('\n')],
+        Topic :: Scientific/Engineering""".split('\n')],
     data_files= glob.glob('bas_geoplot/config/**'),
     entry_points={
         'console_scripts': [
             "plot_mesh=bas_geoplot.cli:plot_mesh_cli"
         ]
     },
     packages=find_packages() + ["bas_geoplot.config"],
```

