# Comparing `tmp/agentops-0.1.3.tar.gz` & `tmp/agentops-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.3.tar", last modified: Tue Apr  9 23:24:16 2024, max compression
+gzip compressed data, was "agentops-0.1.4.tar", last modified: Thu Apr 11 19:25:56 2024, max compression
```

## Comparing `agentops-0.1.3.tar` & `agentops-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:16.037802 agentops-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 23:24:11.000000 agentops-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-09 23:24:16.037802 agentops-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-09 23:24:11.000000 agentops-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:16.033802 agentops-0.1.3/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2879 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-09 23:24:11.000000 agentops-0.1.3/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:16.037802 agentops-0.1.3/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-09 23:24:16.000000 agentops-0.1.3/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 23:24:16.000000 agentops-0.1.3/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:16.000000 agentops-0.1.3/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 23:24:16.000000 agentops-0.1.3/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 23:24:16.000000 agentops-0.1.3/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 23:24:11.000000 agentops-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:24:16.037802 agentops-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:16.033802 agentops-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-09 23:24:11.000000 agentops-0.1.3/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-09 23:24:11.000000 agentops-0.1.3/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-09 23:24:11.000000 agentops-0.1.3/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-09 23:24:11.000000 agentops-0.1.3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-09 23:24:11.000000 agentops-0.1.3/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.618158 agentops-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 19:25:52.000000 agentops-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-11 19:25:56.618158 agentops-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-11 19:25:52.000000 agentops-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.614158 agentops-0.1.4/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2879 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.618158 agentops-0.1.4/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-11 19:25:52.000000 agentops-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:25:56.618158 agentops-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.618158 agentops-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_teardown.py
```

### Comparing `agentops-0.1.3/LICENSE` & `agentops-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/PKG-INFO` & `agentops-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
-Requires-Dist: packaging==24.0
+Requires-Dist: packaging==23.2
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
   <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
-  <div>
-    <a href="https://docs.agentops.ai/introduction">Documentation</a> |
-    <a href="https://discord.gg/mKW3ZhN9p2">Discord</a>
-    <p><i>AI agents suck. We’re fixing that.</i></p>
-  </div>
 </div>
+<p align="center">
+  <em>AI agents suck. We’re fixing that.</em>
+</p>
 
+<p align="center">
+    <a href="https://pypi.org/project/agentops/" target="_blank">
+        <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
+        <img alt="Version" src="https://img.shields.io/pypi/v/agentops?style=for-the-badge&color=3670A0">
+    </a>
+</p>
+<p align="center">
+<a href="https://twitter.com/agentopsai/">🐦 Twitter</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://discord.gg/JHPt4C7r">📢 Discord</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://app.agentops.ai/?=gh">🖇️ AgentOps</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
+</p>
+
+# AgentOps
 
 Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
 
 AgentOps is open beta. You can sign up for AgentOps [here](https://app.agentops.ai).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
```

#### html2text {}

```diff
@@ -1,31 +1,34 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.3 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.4 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==24.0
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
 Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
 requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
 langchain>=0.0.354; extra == "langchain"
                                     [Logo]
-                            _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
-                     AI agents suck. Weâre fixing that.
-Build your next agent with benchmarks, observability, and replay analytics.
-AgentOps is the toolkit for evaluating and developing robust and reliable AI
-agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
-app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
-img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
-_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+                     AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
+                               _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
+    _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
+                                 _D_o_c_u_m_e_n_t_a_t_i_o_n
+# AgentOps Build your next agent with benchmarks, observability, and replay
+analytics. AgentOps is the toolkit for evaluating and developing robust and
+reliable AI agents. AgentOps is open beta. You can sign up for AgentOps [here]
+(https://app.agentops.ai). [![License: MIT](https://img.shields.io/badge/
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version]
+(https://img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
+_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
 _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
 _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
 _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
 _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_o___c_l_i_e_n_t_ _=_ _a_g_e_n_t_o_p_s_._C_l_i_e_n_t_(_)_ _._._.
 _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
```

### Comparing `agentops-0.1.3/README.md` & `agentops-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 <div align="center">
   <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
-  <div>
-    <a href="https://docs.agentops.ai/introduction">Documentation</a> |
-    <a href="https://discord.gg/mKW3ZhN9p2">Discord</a>
-    <p><i>AI agents suck. We’re fixing that.</i></p>
-  </div>
 </div>
+<p align="center">
+  <em>AI agents suck. We’re fixing that.</em>
+</p>
+
+<p align="center">
+    <a href="https://pypi.org/project/agentops/" target="_blank">
+        <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
+        <img alt="Version" src="https://img.shields.io/pypi/v/agentops?style=for-the-badge&color=3670A0">
+    </a>
+</p>
+<p align="center">
+<a href="https://twitter.com/agentopsai/">🐦 Twitter</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://discord.gg/JHPt4C7r">📢 Discord</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://app.agentops.ai/?=gh">🖇️ AgentOps</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
+</p>
 
+# AgentOps
 
 Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
 
 AgentOps is open beta. You can sign up for AgentOps [here](https://app.agentops.ai).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
@@ -114,8 +129,8 @@
 
 ### Why AgentOps? 🤔
 
 Our mission is to bring your agent from protype to production.
 
 Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
 
-AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
+AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
                                     [Logo]
-                            _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
-                     AI agents suck. Weâre fixing that.
-Build your next agent with benchmarks, observability, and replay analytics.
-AgentOps is the toolkit for evaluating and developing robust and reliable AI
-agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
-app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
-img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
-_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+                     AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
+                               _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
+    _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
+                                 _D_o_c_u_m_e_n_t_a_t_i_o_n
+# AgentOps Build your next agent with benchmarks, observability, and replay
+analytics. AgentOps is the toolkit for evaluating and developing robust and
+reliable AI agents. AgentOps is open beta. You can sign up for AgentOps [here]
+(https://app.agentops.ai). [![License: MIT](https://img.shields.io/badge/
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version]
+(https://img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
+_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
 _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
 _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
 _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
 _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_o___c_l_i_e_n_t_ _=_ _a_g_e_n_t_o_p_s_._C_l_i_e_n_t_(_)_ _._._.
 _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
```

### Comparing `agentops-0.1.3/agentops/__init__.py` & `agentops-0.1.4/agentops/__init__.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/agent.py` & `agentops-0.1.4/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/client.py` & `agentops-0.1.4/agentops/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
         if not any(end_state == state.value for state in EndState):
             return logging.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
 
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         token_cost = self._worker.end_session(self._session)
-        if token_cost is 'unknown':
+        if token_cost == 'unknown':
             print('🖇 AgentOps: Could not determine cost of run.')
         else:
             print('🖇 AgentOps: This run cost ${:.6f}'.format(float(token_cost)))
         self._session = None
         self._worker = None
 
     def create_agent(self, agent_id: str, name: str):
```

### Comparing `agentops-0.1.3/agentops/config.py` & `agentops-0.1.4/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/decorators.py` & `agentops-0.1.4/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/enums.py` & `agentops-0.1.4/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/event.py` & `agentops-0.1.4/agentops/event.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/helpers.py` & `agentops-0.1.4/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/host_env.py` & `agentops-0.1.4/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/http_client.py` & `agentops-0.1.4/agentops/http_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/langchain_callback_handler.py` & `agentops-0.1.4/agentops/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/llm_tracker.py` & `agentops-0.1.4/agentops/llm_tracker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/meta_client.py` & `agentops-0.1.4/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/session.py` & `agentops-0.1.4/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops/worker.py` & `agentops-0.1.4/agentops/worker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/agentops.egg-info/PKG-INFO` & `agentops-0.1.4/agentops.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
-Requires-Dist: packaging==24.0
+Requires-Dist: packaging==23.2
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
   <img src="logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
-  <div>
-    <a href="https://docs.agentops.ai/introduction">Documentation</a> |
-    <a href="https://discord.gg/mKW3ZhN9p2">Discord</a>
-    <p><i>AI agents suck. We’re fixing that.</i></p>
-  </div>
 </div>
+<p align="center">
+  <em>AI agents suck. We’re fixing that.</em>
+</p>
 
+<p align="center">
+    <a href="https://pypi.org/project/agentops/" target="_blank">
+        <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
+        <img alt="Version" src="https://img.shields.io/pypi/v/agentops?style=for-the-badge&color=3670A0">
+    </a>
+</p>
+<p align="center">
+<a href="https://twitter.com/agentopsai/">🐦 Twitter</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://discord.gg/JHPt4C7r">📢 Discord</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://app.agentops.ai/?=gh">🖇️ AgentOps</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+<a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
+</p>
+
+# AgentOps
 
 Build your next agent with benchmarks, observability, and replay analytics. AgentOps is the toolkit for evaluating and developing robust and reliable AI agents.
 
 AgentOps is open beta. You can sign up for AgentOps [here](https://app.agentops.ai).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
   <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
```

#### html2text {}

```diff
@@ -1,31 +1,34 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.3 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.4 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==24.0
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
 Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
 requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
 langchain>=0.0.354; extra == "langchain"
                                     [Logo]
-                            _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
-                     AI agents suck. Weâre fixing that.
-Build your next agent with benchmarks, observability, and replay analytics.
-AgentOps is the toolkit for evaluating and developing robust and reliable AI
-agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
-app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
-img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
-_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+                     AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
+                               _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
+    _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
+                                 _D_o_c_u_m_e_n_t_a_t_i_o_n
+# AgentOps Build your next agent with benchmarks, observability, and replay
+analytics. AgentOps is the toolkit for evaluating and developing robust and
+reliable AI agents. AgentOps is open beta. You can sign up for AgentOps [here]
+(https://app.agentops.ai). [![License: MIT](https://img.shields.io/badge/
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version]
+(https://img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
+_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
 _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_`_`_`_ _#_#_#_ _S_e_s_s_i_o_n
 _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e_ _A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_,_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y
 _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n_ _p_y_t_h_o_n_ _i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g
 _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)_ _a_o___c_l_i_e_n_t_ _=_ _a_g_e_n_t_o_p_s_._C_l_i_e_n_t_(_)_ _._._.
 _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)_ _@_r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g
```

### Comparing `agentops-0.1.3/agentops.egg-info/SOURCES.txt` & `agentops-0.1.4/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/pyproject.toml` & `agentops-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests==2.31.0",
     "psutil==5.9.8",
-    "packaging==24.0"
+    "packaging==23.2"
 ]
 [project.optional-dependencies]
 dev = [
     "pytest==7.4.0",
     "requests_mock==1.11.0"
 ]
 langchain = [
```

### Comparing `agentops-0.1.3/tests/test_canary.py` & `agentops-0.1.4/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/tests/test_patcher.py` & `agentops-0.1.4/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/tests/test_record_function.py` & `agentops-0.1.4/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/tests/test_session.py` & `agentops-0.1.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.3/tests/test_teardown.py` & `agentops-0.1.4/tests/test_teardown.py`

 * *Files identical despite different names*

