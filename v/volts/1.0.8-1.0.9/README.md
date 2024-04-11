# Comparing `tmp/volts-1.0.8.tar.gz` & `tmp/volts-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volts-1.0.8.tar", last modified: Tue Mar 19 20:26:47 2024, max compression
+gzip compressed data, was "volts-1.0.9.tar", last modified: Wed Mar 20 01:56:25 2024, max compression
```

## Comparing `volts-1.0.8.tar` & `volts-1.0.9.tar`

### file list

```diff
@@ -1,773 +1,773 @@
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/
--rw-r--r--   0 calculator  (1000) calculator  (1000)     5526 2024-03-19 20:26:47.574143 volts-1.0.8/PKG-INFO
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1901 2024-03-19 20:26:41.000000 volts-1.0.8/pyproject.toml
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       38 2024-03-19 20:26:47.574143 volts-1.0.8/setup.cfg
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.502143 volts-1.0.8/structures/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.502143 volts-1.0.8/structures/decor/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/__agenda/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     3271 2024-03-19 02:37:02.000000 volts-1.0.8/structures/decor/volts/__agenda/agenda.S.HTML
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      541 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/__agenda/maybes.s.HTML
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.502143 volts-1.0.8/structures/decor/volts/__agenda/processes/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/__agenda/processes/errout/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      190 2023-12-17 00:38:53.000000 volts-1.0.8/structures/decor/volts/__agenda/processes/errout/script.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1255 2024-01-22 23:00:47.000000 volts-1.0.8/structures/decor/volts/__agenda/processes/errout/start.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      189 2023-12-17 00:23:56.000000 volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v1/script.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      186 2023-11-01 19:11:23.000000 volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v1/start.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      190 2023-12-17 00:38:53.000000 volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v2/script.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1141 2023-12-17 00:37:48.000000 volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v2/start.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       72 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_book/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1110 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_book/advanced tutorial.s.HTML
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1774 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_book/book.s.HTML
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1565 2023-12-17 01:10:19.000000 volts-1.0.8/structures/decor/volts/_book/example output.s.HTML
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      490 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_book/relevant.s.HTML
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_clique/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     2085 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_clique/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_clique/group/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      294 2023-12-01 19:53:30.000000 volts-1.0.8/structures/decor/volts/_clique/group/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      482 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/--statuspy.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/DB/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)   329165 2024-03-19 19:56:17.000000 volts-1.0.8/structures/decor/volts/_status/DB/records.json
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1104 2024-03-19 02:33:27.000000 volts-1.0.8/structures/decor/volts/_status/establish.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status/monitors/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/-1_start/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.502143 volts-1.0.8/structures/decor/volts/_status/monitors/-1_start/chassis/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/-1_start/chassis/modules/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       83 2023-11-16 16:37:37.000000 volts-1.0.8/structures/decor/volts/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      716 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/-1_start/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/0_start/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.502143 volts-1.0.8/structures/decor/volts/_status/monitors/0_start/chassis/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/0_start/chassis/modules/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      101 2023-11-16 16:51:33.000000 volts-1.0.8/structures/decor/volts/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      789 2024-03-19 02:28:20.000000 volts-1.0.8/structures/decor/volts/_status/monitors/0_start/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/1/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      282 2023-10-28 18:23:15.000000 volts-1.0.8/structures/decor/volts/_status/monitors/1/stasis/path_1_health.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      265 2023-10-28 18:23:15.000000 volts-1.0.8/structures/decor/volts/_status/monitors/1/stasis/path_2_health.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1157 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/1/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.518144 volts-1.0.8/structures/decor/volts/_status/monitors/2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/2/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      321 2023-10-28 18:23:15.000000 volts-1.0.8/structures/decor/volts/_status/monitors/2/stasis/1_health.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)        2 2023-09-30 01:11:18.000000 volts-1.0.8/structures/decor/volts/_status/monitors/2/stasis/2_health.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/2/stasis/modules/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       50 2023-09-30 00:56:59.000000 volts-1.0.8/structures/decor/volts/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1173 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/2/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/3_empty_glob/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      790 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/3_empty_glob/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/4_bad_import/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/4_bad_import/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       35 2023-10-04 21:28:49.000000 volts-1.0.8/structures/decor/volts/_status/monitors/4_bad_import/stasis/1_health.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      828 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/4_bad_import/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      518 2023-12-11 19:46:37.000000 volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/stasis/1_health.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/stasis/MODULES/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      155 2023-12-11 19:46:41.000000 volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      863 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      311 2023-10-28 18:23:15.000000 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/stasis/1_health.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       31 2023-10-13 04:03:32.000000 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/stasis/2_health.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)        0 2023-10-13 04:03:42.000000 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/stasis/3_health.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/stasis/MODULES/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      150 2023-10-13 03:39:00.000000 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      896 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/6_various/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/7/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/7/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      160 2023-10-28 18:15:12.000000 volts-1.0.8/structures/decor/volts/_status/monitors/7/stasis/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      805 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/7/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/stasis/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       73 2023-10-28 19:16:57.000000 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1409 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/variable/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/variable/status_db/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)    47698 2024-03-19 19:56:17.000000 volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/variable/status_db/records.json
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      905 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/status.proc.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      248 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status/status.s.HTML
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status_advanced/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1445 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/advanced_status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.522143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.526143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.506143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.530143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.534143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.538143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.542143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.546143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.510144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.550143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.554143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.558143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.562143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.566143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.570143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      406 2023-11-01 00:43:27.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/after.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      358 2023-11-01 00:42:38.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/stasis/before.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/variable/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/variable/status_db/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)   542989 2023-12-11 20:11:58.000000 volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/variable/status_db/records.json
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      919 2023-12-11 19:59:28.000000 volts-1.0.8/structures/decor/volts/_status_advanced/status.proc.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1844 2024-03-18 22:00:49.000000 volts-1.0.8/structures/decor/volts/architecture.s.HTML
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/db/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      836 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/db/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/intros/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     3363 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/intros/start.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      181 2024-02-21 05:19:06.000000 volts-1.0.8/structures/decor/volts/license.S.HTML
--rwxr-xr-x   0 calculator  (1000) calculator  (1000)     4856 2024-03-19 20:26:17.000000 volts-1.0.8/structures/decor/volts/module.MD
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     3042 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/module.s.HTML
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.514144 volts-1.0.8/structures/decor/volts/processes/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/ceremony/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      167 2024-01-23 03:50:57.000000 volts-1.0.8/structures/decor/volts/processes/ceremony/ceremony.s.HTML
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      244 2024-03-18 22:01:23.000000 volts-1.0.8/structures/decor/volts/processes/ceremony/path.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)        0 2023-10-13 03:13:25.000000 volts-1.0.8/structures/decor/volts/processes/ceremony/start.proc.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/ceremony/starter/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)        2 2024-01-23 04:17:27.000000 volts-1.0.8/structures/decor/volts/processes/ceremony/starter/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/scan/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/scan/process/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/scan/process/keg/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1487 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/process/keg/__init__.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1900 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/process/keg/check.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1165 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/process/scan.process.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      188 2024-01-22 22:37:56.000000 volts-1.0.8/structures/decor/volts/processes/scan/scan.s.HTML
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/scan/starter/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1473 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/starter/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/scan/starter/ask/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1118 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/starter/ask/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/processes/scan/starter/keg/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)     2269 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/starter/keg/__init__.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      368 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/processes/scan/starter/path.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/topics/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/topics/aggregate/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      621 2023-10-28 18:33:44.000000 volts-1.0.8/structures/decor/volts/topics/aggregate/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/topics/alarm_printer/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      537 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/topics/alarm_printer/__init__.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      403 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/topics/exceptions.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts/topics/start/
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      270 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/topics/start/one.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      403 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/topics/start/sequentially.py
--rwxrwxrwx   0 calculator  (1000) calculator  (1000)      592 2024-03-18 22:01:24.000000 volts-1.0.8/structures/decor/volts/topics/start/simultaneously.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-19 20:26:47.574143 volts-1.0.8/structures/decor/volts.egg-info/
--rw-r--r--   0 calculator  (1000) calculator  (1000)     5526 2024-03-19 20:26:47.000000 volts-1.0.8/structures/decor/volts.egg-info/PKG-INFO
--rw-rw-r--   0 calculator  (1000) calculator  (1000)    46143 2024-03-19 20:26:47.000000 volts-1.0.8/structures/decor/volts.egg-info/SOURCES.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)        1 2024-03-19 20:26:47.000000 volts-1.0.8/structures/decor/volts.egg-info/dependency_links.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       39 2024-03-19 20:26:47.000000 volts-1.0.8/structures/decor/volts.egg-info/entry_points.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       91 2024-03-19 20:26:47.000000 volts-1.0.8/structures/decor/volts.egg-info/requires.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)        6 2024-03-19 20:26:47.000000 volts-1.0.8/structures/decor/volts.egg-info/top_level.txt
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.462681 volts-1.0.9/
+-rw-r--r--   0 calculator  (1000) calculator  (1000)     4510 2024-03-20 01:56:25.462681 volts-1.0.9/PKG-INFO
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1901 2024-03-20 01:56:04.000000 volts-1.0.9/pyproject.toml
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)       38 2024-03-20 01:56:25.462681 volts-1.0.9/setup.cfg
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.038683 volts-1.0.9/structures/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.058683 volts-1.0.9/structures/decor/volts/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.058683 volts-1.0.9/structures/decor/volts/__agenda/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     3271 2024-03-19 02:37:02.000000 volts-1.0.9/structures/decor/volts/__agenda/agenda.S.HTML
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      541 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/__agenda/maybes.s.HTML
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/volts/__agenda/processes/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.062683 volts-1.0.9/structures/decor/volts/__agenda/processes/errout/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      190 2023-12-17 00:38:53.000000 volts-1.0.9/structures/decor/volts/__agenda/processes/errout/script.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1255 2024-01-22 23:00:47.000000 volts-1.0.9/structures/decor/volts/__agenda/processes/errout/start.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.062683 volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      189 2023-12-17 00:23:56.000000 volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v1/script.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      186 2023-11-01 19:11:23.000000 volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v1/start.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.066683 volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      190 2023-12-17 00:38:53.000000 volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v2/script.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1141 2023-12-17 00:37:48.000000 volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v2/start.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       72 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.070683 volts-1.0.9/structures/decor/volts/_book/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1110 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_book/advanced tutorial.s.HTML
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1774 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_book/book.s.HTML
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1565 2023-12-17 01:10:19.000000 volts-1.0.9/structures/decor/volts/_book/example output.s.HTML
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      490 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_book/relevant.s.HTML
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.074683 volts-1.0.9/structures/decor/volts/_clique/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     2085 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_clique/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.078683 volts-1.0.9/structures/decor/volts/_clique/group/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      294 2023-12-01 19:53:30.000000 volts-1.0.9/structures/decor/volts/_clique/group/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.082683 volts-1.0.9/structures/decor/volts/_status/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      482 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/--statuspy.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.098683 volts-1.0.9/structures/decor/volts/_status/DB/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)   329165 2024-03-19 19:56:17.000000 volts-1.0.9/structures/decor/volts/_status/DB/records.json
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1104 2024-03-19 02:33:27.000000 volts-1.0.9/structures/decor/volts/_status/establish.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/volts/_status/monitors/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.126683 volts-1.0.9/structures/decor/volts/_status/monitors/-1_start/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/volts/_status/monitors/-1_start/chassis/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.126683 volts-1.0.9/structures/decor/volts/_status/monitors/-1_start/chassis/modules/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       83 2023-11-16 16:37:37.000000 volts-1.0.9/structures/decor/volts/_status/monitors/-1_start/chassis/modules/monitor_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      716 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/-1_start/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.126683 volts-1.0.9/structures/decor/volts/_status/monitors/0_start/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/volts/_status/monitors/0_start/chassis/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.126683 volts-1.0.9/structures/decor/volts/_status/monitors/0_start/chassis/modules/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      101 2023-11-16 16:51:33.000000 volts-1.0.9/structures/decor/volts/_status/monitors/0_start/chassis/modules/monitor_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      789 2024-03-19 02:28:20.000000 volts-1.0.9/structures/decor/volts/_status/monitors/0_start/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.130683 volts-1.0.9/structures/decor/volts/_status/monitors/1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.130683 volts-1.0.9/structures/decor/volts/_status/monitors/1/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      282 2023-10-28 18:23:15.000000 volts-1.0.9/structures/decor/volts/_status/monitors/1/stasis/path_1_health.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      265 2023-10-28 18:23:15.000000 volts-1.0.9/structures/decor/volts/_status/monitors/1/stasis/path_2_health.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1157 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/1/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.130683 volts-1.0.9/structures/decor/volts/_status/monitors/2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.134683 volts-1.0.9/structures/decor/volts/_status/monitors/2/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      321 2023-10-28 18:23:15.000000 volts-1.0.9/structures/decor/volts/_status/monitors/2/stasis/1_health.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)        2 2023-09-30 01:11:18.000000 volts-1.0.9/structures/decor/volts/_status/monitors/2/stasis/2_health.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.134683 volts-1.0.9/structures/decor/volts/_status/monitors/2/stasis/modules/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       50 2023-09-30 00:56:59.000000 volts-1.0.9/structures/decor/volts/_status/monitors/2/stasis/modules/MODULE_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1173 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/2/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.134683 volts-1.0.9/structures/decor/volts/_status/monitors/3_empty_glob/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      790 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/3_empty_glob/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.134683 volts-1.0.9/structures/decor/volts/_status/monitors/4_bad_import/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.134683 volts-1.0.9/structures/decor/volts/_status/monitors/4_bad_import/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       35 2023-10-04 21:28:49.000000 volts-1.0.9/structures/decor/volts/_status/monitors/4_bad_import/stasis/1_health.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      828 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/4_bad_import/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.134683 volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.138683 volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      518 2023-12-11 19:46:37.000000 volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/stasis/1_health.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.138683 volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/stasis/MODULES/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      155 2023-12-11 19:46:41.000000 volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      863 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.138683 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.142683 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      311 2023-10-28 18:23:15.000000 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/stasis/1_health.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       31 2023-10-13 04:03:32.000000 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/stasis/2_health.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)        0 2023-10-13 04:03:42.000000 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/stasis/3_health.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.142683 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/stasis/MODULES/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      150 2023-10-13 03:39:00.000000 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      896 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/6_various/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.142683 volts-1.0.9/structures/decor/volts/_status/monitors/7/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.146683 volts-1.0.9/structures/decor/volts/_status/monitors/7/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      160 2023-10-28 18:15:12.000000 volts-1.0.9/structures/decor/volts/_status/monitors/7/stasis/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      805 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/7/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.146683 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.146683 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/stasis/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       73 2023-10-28 19:16:57.000000 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/stasis/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1409 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/variable/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.150683 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/variable/status_db/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)    47698 2024-03-19 19:56:17.000000 volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/variable/status_db/records.json
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      905 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/status.proc.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      248 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status/status.s.HTML
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.150683 volts-1.0.9/structures/decor/volts/_status_advanced/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.042683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.154683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1445 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/advanced_status_1.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.154683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.158683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.162683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.166683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.170683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.170683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.174683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.178683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.182683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.186683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.190683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.194682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.198682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.198682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.202682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.202682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.206683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.210682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.210682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.214682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.218682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.222682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.222682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.226682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.230682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.230682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.234682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.238682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.238682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.242682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.242682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.046683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.246682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.250682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.250682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.254682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.254682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.258682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.262682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.262682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.266682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.270682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.270682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.274682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.278682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.278682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.282682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.286682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.286682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.290682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.290682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.294682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.298682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.298682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.302682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.302682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.306682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.310682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.310682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.314682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.314682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.318682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.322682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.322682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.326682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.326682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.330682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.050683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.334682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.334682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.338682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.342682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.342682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.346682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.346682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.350682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.354682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.358682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.358682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.362682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.366682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.366682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.370682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.370682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.374682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.378682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.378682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.382681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.382681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.386681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.390682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.394682 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.398681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.398681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.402681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.402681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.406681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.406681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.410681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.410681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.414681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.418681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.418681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)       75 2023-11-01 00:24:46.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      406 2023-11-01 00:43:27.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/after.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      358 2023-11-01 00:42:38.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/stasis/before.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/variable/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.418681 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/variable/status_db/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)   542989 2023-12-11 20:11:58.000000 volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      919 2023-12-11 19:59:28.000000 volts-1.0.9/structures/decor/volts/_status_advanced/status.proc.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1844 2024-03-18 22:00:49.000000 volts-1.0.9/structures/decor/volts/architecture.s.HTML
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.434681 volts-1.0.9/structures/decor/volts/db/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      836 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/db/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.434681 volts-1.0.9/structures/decor/volts/intros/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     3363 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/intros/start.py
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)      181 2024-02-21 05:19:06.000000 volts-1.0.9/structures/decor/volts/license.S.HTML
+-rwxr-xr-x   0 calculator  (1000) calculator  (1000)     3840 2024-03-20 01:55:51.000000 volts-1.0.9/structures/decor/volts/module.MD
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     3042 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/module.s.HTML
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.054683 volts-1.0.9/structures/decor/volts/processes/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.438681 volts-1.0.9/structures/decor/volts/processes/ceremony/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      167 2024-01-23 03:50:57.000000 volts-1.0.9/structures/decor/volts/processes/ceremony/ceremony.s.HTML
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      244 2024-03-18 22:01:23.000000 volts-1.0.9/structures/decor/volts/processes/ceremony/path.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)        0 2023-10-13 03:13:25.000000 volts-1.0.9/structures/decor/volts/processes/ceremony/start.proc.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.438681 volts-1.0.9/structures/decor/volts/processes/ceremony/starter/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)        2 2024-01-23 04:17:27.000000 volts-1.0.9/structures/decor/volts/processes/ceremony/starter/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.438681 volts-1.0.9/structures/decor/volts/processes/scan/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.438681 volts-1.0.9/structures/decor/volts/processes/scan/process/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.446681 volts-1.0.9/structures/decor/volts/processes/scan/process/keg/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1487 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/process/keg/__init__.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1900 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/process/keg/check.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1165 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/process/scan.process.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      188 2024-01-22 22:37:56.000000 volts-1.0.9/structures/decor/volts/processes/scan/scan.s.HTML
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.450681 volts-1.0.9/structures/decor/volts/processes/scan/starter/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1473 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/starter/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.450681 volts-1.0.9/structures/decor/volts/processes/scan/starter/ask/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     1118 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/starter/ask/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.454681 volts-1.0.9/structures/decor/volts/processes/scan/starter/keg/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)     2269 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/starter/keg/__init__.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      368 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/processes/scan/starter/path.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.454681 volts-1.0.9/structures/decor/volts/topics/
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.454681 volts-1.0.9/structures/decor/volts/topics/aggregate/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      621 2023-10-28 18:33:44.000000 volts-1.0.9/structures/decor/volts/topics/aggregate/__init__.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.454681 volts-1.0.9/structures/decor/volts/topics/alarm_printer/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      537 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/topics/alarm_printer/__init__.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      403 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/topics/exceptions.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.458681 volts-1.0.9/structures/decor/volts/topics/start/
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      270 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/topics/start/one.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      403 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/topics/start/sequentially.py
+-rwxrwxrwx   0 calculator  (1000) calculator  (1000)      592 2024-03-18 22:01:24.000000 volts-1.0.9/structures/decor/volts/topics/start/simultaneously.py
+drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-20 01:56:25.458681 volts-1.0.9/structures/decor/volts.egg-info/
+-rw-r--r--   0 calculator  (1000) calculator  (1000)     4510 2024-03-20 01:56:24.000000 volts-1.0.9/structures/decor/volts.egg-info/PKG-INFO
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)    46143 2024-03-20 01:56:25.000000 volts-1.0.9/structures/decor/volts.egg-info/SOURCES.txt
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)        1 2024-03-20 01:56:24.000000 volts-1.0.9/structures/decor/volts.egg-info/dependency_links.txt
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)       39 2024-03-20 01:56:24.000000 volts-1.0.9/structures/decor/volts.egg-info/entry_points.txt
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)       91 2024-03-20 01:56:24.000000 volts-1.0.9/structures/decor/volts.egg-info/requires.txt
+-rw-rw-r--   0 calculator  (1000) calculator  (1000)        6 2024-03-20 01:56:24.000000 volts-1.0.9/structures/decor/volts.egg-info/top_level.txt
```

### Comparing `volts-1.0.8/PKG-INFO` & `volts-1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volts
-Version: 1.0.8
+Version: 1.0.9
 Summary: health checks module
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/status600/climates/volts
 Keywords: homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: body_scan
@@ -37,49 +37,14 @@
 
 ---
  
 [![CircleCI](https://dl.circleci.com/status-badge/img/circleci/EGXocrWNVJE6QWAifHn6r3/XP6tKC6Z4p7cTe8uyzgEjb/tree/performance.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/circleci/EGXocrWNVJE6QWAifHn6r3/XP6tKC6Z4p7cTe8uyzgEjb/tree/performance)
 
 ---
 
-## ⚡ iterative itinerary
-[  ] collect 🌟 solar in 12 volt energy cell.
-``` 
-	If you like "batteries", or "batteries" turn you on, 
-	you're going to get a lot of "volts", trust me.
-```
-	
----
-
-## Pythons as companions
-It seems like every kind of known "python" is non-venomous.        
-      
-Nevertheless, pythons are carnivorous constrictors that kill prey by   
-wrapping around them and squeezing tightly.  
-   
-There are very big python species like "reticulated pythons" 
-that can grow to over 20 feet and thusly can squeeze and kill 
-a human very fast.   
-
-However, Python species like "Ball", "Woma" and "Children's" pythons
-usually don't grow past 5 feet long.
-
-"Burmese" and "Carpet" pythons can also be great companions;
-they can grow to like 10 to 20 feet though.
-
-Dangers aside, pythons are great friends for
-agriculture as they reduce the rodent population.
-
-1 Food (Large) Calorie = 4,184 Joule 
-	
-🐁 Consuming a mouse provides like ? Joules.
-
-🖱️ Don't feed computer "mice" to Pythons.
-		
----
 
 ## 🥧 description
 This module can monitor the health status of a python3 `.py` biome. 
 
 ---
 
 ## ⛲ licensing
```

### Comparing `volts-1.0.8/pyproject.toml` & `volts-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "volts"
-version = "1.0.8"
+version = "1.0.9"
 requires-python = ">=3.8"
 
 
 #
 #	⚠️
 #		Make sure that none of these depend on this module!
 #
```

### Comparing `volts-1.0.8/structures/decor/volts/__agenda/agenda.S.HTML` & `volts-1.0.9/structures/decor/volts/__agenda/agenda.S.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/__agenda/maybes.s.HTML` & `volts-1.0.9/structures/decor/volts/__agenda/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/__agenda/processes/errout/start.py` & `volts-1.0.9/structures/decor/volts/__agenda/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/__agenda/processes/errout_v2/start.py` & `volts-1.0.9/structures/decor/volts/__agenda/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_book/advanced tutorial.s.HTML` & `volts-1.0.9/structures/decor/volts/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_book/book.s.HTML` & `volts-1.0.9/structures/decor/volts/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_book/example output.s.HTML` & `volts-1.0.9/structures/decor/volts/_book/example output.s.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_clique/__init__.py` & `volts-1.0.9/structures/decor/volts/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/DB/records.json` & `volts-1.0.9/structures/decor/volts/_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/establish.py` & `volts-1.0.9/structures/decor/volts/_status/establish.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/-1_start/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/-1_start/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/0_start/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/0_start/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/1/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/1/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/2/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/2/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/3_empty_glob/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/3_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/4_bad_import/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/4_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/stasis/1_health.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/5__file__/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/5__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/6_various/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/6_various/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/7/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/7/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/status_1.py` & `volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/monitors/8_DB/variable/status_db/records.json` & `volts-1.0.9/structures/decor/volts/_status/monitors/8_DB/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status/status.proc.py` & `volts-1.0.9/structures/decor/volts/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/advanced_status_1.py` & `volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status_advanced/monitors/1/variable/status_db/records.json` & `volts-1.0.9/structures/decor/volts/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/_status_advanced/status.proc.py` & `volts-1.0.9/structures/decor/volts/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/architecture.s.HTML` & `volts-1.0.9/structures/decor/volts/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/db/__init__.py` & `volts-1.0.9/structures/decor/volts/db/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/intros/start.py` & `volts-1.0.9/structures/decor/volts/intros/start.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/module.MD` & `volts-1.0.9/structures/decor/volts.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: volts
+Version: 1.0.9
+Summary: health checks module
+License: GPL 3.0
+Project-URL: GitLab, https://gitlab.com/status600/climates/volts
+Keywords: homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: body_scan
+Requires-Dist: botanist
+Requires-Dist: shares
+Requires-Dist: click
+Requires-Dist: coverage
+Requires-Dist: flask
+Requires-Dist: pdoc3
+Requires-Dist: pexpect
+Requires-Dist: redis
+Requires-Dist: requests
+Requires-Dist: textual
+Requires-Dist: tinydb
+
 
 
 ## certificate
 
 Bravo!  You have received a Medical Diploma in "volts" from      
 the Orbital Convergence University International Air and Water   
 Embassy of the Tangerine Planet 🍊.  
@@ -15,49 +37,14 @@
 
 ---
  
 [![CircleCI](https://dl.circleci.com/status-badge/img/circleci/EGXocrWNVJE6QWAifHn6r3/XP6tKC6Z4p7cTe8uyzgEjb/tree/performance.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/circleci/EGXocrWNVJE6QWAifHn6r3/XP6tKC6Z4p7cTe8uyzgEjb/tree/performance)
 
 ---
 
-## ⚡ iterative itinerary
-[  ] collect 🌟 solar in 12 volt energy cell.
-``` 
-	If you like "batteries", or "batteries" turn you on, 
-	you're going to get a lot of "volts", trust me.
-```
-	
----
-
-## Pythons as companions
-It seems like every kind of known "python" is non-venomous.        
-      
-Nevertheless, pythons are carnivorous constrictors that kill prey by   
-wrapping around them and squeezing tightly.  
-   
-There are very big python species like "reticulated pythons" 
-that can grow to over 20 feet and thusly can squeeze and kill 
-a human very fast.   
-
-However, Python species like "Ball", "Woma" and "Children's" pythons
-usually don't grow past 5 feet long.
-
-"Burmese" and "Carpet" pythons can also be great companions;
-they can grow to like 10 to 20 feet though.
-
-Dangers aside, pythons are great friends for
-agriculture as they reduce the rodent population.
-
-1 Food (Large) Calorie = 4,184 Joule 
-	
-🐁 Consuming a mouse provides like ? Joules.
-
-🖱️ Don't feed computer "mice" to Pythons.
-		
----
 
 ## 🥧 description
 This module can monitor the health status of a python3 `.py` biome. 
 
 ---
 
 ## ⛲ licensing
```

### Comparing `volts-1.0.8/structures/decor/volts/module.s.HTML` & `volts-1.0.9/structures/decor/volts/module.s.HTML`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/processes/scan/process/keg/__init__.py` & `volts-1.0.9/structures/decor/volts/processes/scan/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/processes/scan/process/keg/check.py` & `volts-1.0.9/structures/decor/volts/processes/scan/process/keg/check.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/processes/scan/process/scan.process.py` & `volts-1.0.9/structures/decor/volts/processes/scan/process/scan.process.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/processes/scan/starter/__init__.py` & `volts-1.0.9/structures/decor/volts/processes/scan/starter/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/processes/scan/starter/ask/__init__.py` & `volts-1.0.9/structures/decor/volts/processes/scan/starter/ask/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/processes/scan/starter/keg/__init__.py` & `volts-1.0.9/structures/decor/volts/processes/scan/starter/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/topics/aggregate/__init__.py` & `volts-1.0.9/structures/decor/volts/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/topics/alarm_printer/__init__.py` & `volts-1.0.9/structures/decor/volts/topics/alarm_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts/topics/start/simultaneously.py` & `volts-1.0.9/structures/decor/volts/topics/start/simultaneously.py`

 * *Files identical despite different names*

### Comparing `volts-1.0.8/structures/decor/volts.egg-info/SOURCES.txt` & `volts-1.0.9/structures/decor/volts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

