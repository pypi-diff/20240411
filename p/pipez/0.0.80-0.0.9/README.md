# Comparing `tmp/pipez-0.0.80.tar.gz` & `tmp/pipez-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipez-0.0.80.tar", last modified: Thu Apr 11 09:05:46 2024, max compression
+gzip compressed data, was "pipez-0.0.9.tar", last modified: Tue Jan 23 14:50:25 2024, max compression
```

## Comparing `pipez-0.0.80.tar` & `pipez-0.0.9.tar`

### file list

```diff
@@ -1,221 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.482800 pipez-0.0.80/
--rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.80/LICENSE
--rw-rw-rw-   0        0        0      126 2024-04-08 09:46:56.000000 pipez-0.0.80/MANIFEST.in
--rw-rw-rw-   0        0        0     4675 2024-04-11 09:05:46.481565 pipez-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0     3443 2024-03-28 12:27:44.000000 pipez-0.0.80/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.008368 pipez-0.0.80/pipez/
--rw-rw-rw-   0        0        0       24 2024-04-11 09:04:02.000000 pipez-0.0.80/pipez/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.041045 pipez-0.0.80/pipez/core/
--rw-rw-rw-   0        0        0      130 2024-03-28 12:59:53.000000 pipez-0.0.80/pipez/core/__init__.py
--rw-rw-rw-   0        0        0     2331 2024-02-04 10:03:20.000000 pipez-0.0.80/pipez/core/batch.py
--rw-rw-rw-   0        0        0     2850 2024-04-10 20:16:39.000000 pipez-0.0.80/pipez/core/build.py
--rw-rw-rw-   0        0        0     1205 2024-03-11 10:53:05.000000 pipez-0.0.80/pipez/core/metrics.py
--rw-rw-rw-   0        0        0     9894 2024-04-11 09:04:02.000000 pipez-0.0.80/pipez/core/node.py
--rw-rw-rw-   0        0        0      716 2024-02-04 10:03:20.000000 pipez-0.0.80/pipez/core/queue_wrapper.py
--rw-rw-rw-   0        0        0     1200 2024-01-23 07:32:10.000000 pipez-0.0.80/pipez/core/registry.py
--rw-rw-rw-   0        0        0     2795 2024-02-02 11:31:56.000000 pipez-0.0.80/pipez/core/shared_memory.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.044121 pipez-0.0.80/pipez/core/static/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.057958 pipez-0.0.80/pipez/core/static/DataTables/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:45.979058 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.108965 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/
--rw-rw-rw-   0        0        0    13174 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.css
--rw-rw-rw-   0        0        0    11219 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.min.css
--rw-rw-rw-   0        0        0    13511 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.css
--rw-rw-rw-   0        0        0    11523 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.min.css
--rw-rw-rw-   0        0        0    14198 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.css
--rw-rw-rw-   0        0        0    12168 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.min.css
--rw-rw-rw-   0        0        0    12157 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.css
--rw-rw-rw-   0        0        0    10395 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.min.css
--rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.css
--rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.min.css
--rw-rw-rw-   0        0        0    11266 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.css
--rw-rw-rw-   0        0        0     9580 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.min.css
--rw-rw-rw-   0        0        0    28554 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.css
--rw-rw-rw-   0        0        0    24415 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.min.css
--rw-rw-rw-   0        0        0    11471 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.css
--rw-rw-rw-   0        0        0     9783 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.min.css
--rw-rw-rw-   0        0        0    26541 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.css
--rw-rw-rw-   0        0        0    22712 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.min.css
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.120923 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/images/
--rw-rw-rw-   0        0        0      160 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc.png
--rw-rw-rw-   0        0        0      148 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc_disabled.png
--rw-rw-rw-   0        0        0      201 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_both.png
--rw-rw-rw-   0        0        0      158 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc.png
--rw-rw-rw-   0        0        0      146 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc_disabled.png
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.168983 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/
--rw-rw-rw-   0        0        0     5214 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.js
--rw-rw-rw-   0        0        0     2226 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.min.js
--rw-rw-rw-   0        0        0     5350 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.js
--rw-rw-rw-   0        0        0     2343 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.min.js
--rw-rw-rw-   0        0        0     5494 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.js
--rw-rw-rw-   0        0        0     2361 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.min.js
--rw-rw-rw-   0        0        0     5701 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.js
--rw-rw-rw-   0        0        0     2484 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.min.js
--rw-rw-rw-   0        0        0     1205 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.js
--rw-rw-rw-   0        0        0      588 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.min.js
--rw-rw-rw-   0        0        0     5235 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.js
--rw-rw-rw-   0        0        0     2398 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.min.js
--rw-rw-rw-   0        0        0     2518 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.js
--rw-rw-rw-   0        0        0     1226 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.min.js
--rw-rw-rw-   0        0        0     5923 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.js
--rw-rw-rw-   0        0        0     2672 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.min.js
--rw-rw-rw-   0        0        0   473441 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.js
--rw-rw-rw-   0        0        0    87279 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.min.js
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:45.982610 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.209077 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/
--rw-rw-rw-   0        0        0     1316 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.css
--rw-rw-rw-   0        0        0     1124 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.min.css
--rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.css
--rw-rw-rw-   0        0        0     1147 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.min.css
--rw-rw-rw-   0        0        0     1452 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.css
--rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.min.css
--rw-rw-rw-   0        0        0      396 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.css
--rw-rw-rw-   0        0        0      339 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.251188 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/
--rw-rw-rw-   0        0        0    41008 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.js
--rw-rw-rw-   0        0        0    12430 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.min.js
--rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.js
--rw-rw-rw-   0        0        0      691 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1333 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.js
--rw-rw-rw-   0        0        0      685 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.min.js
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:45.985250 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.288934 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/
--rw-rw-rw-   0        0        0     6724 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.css
--rw-rw-rw-   0        0        0     5854 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.min.css
--rw-rw-rw-   0        0        0     6981 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.css
--rw-rw-rw-   0        0        0     6077 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.min.css
--rw-rw-rw-   0        0        0     7186 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.css
--rw-rw-rw-   0        0        0     6249 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.min.css
--rw-rw-rw-   0        0        0     7015 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.css
--rw-rw-rw-   0        0        0     6100 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.min.css
--rw-rw-rw-   0        0        0     8908 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.css
--rw-rw-rw-   0        0        0     7734 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.min.css
--rw-rw-rw-   0        0        0     7184 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.css
--rw-rw-rw-   0        0        0     6254 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.min.css
--rw-rw-rw-   0        0        0     6733 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.css
--rw-rw-rw-   0        0        0     5869 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.min.css
--rw-rw-rw-   0        0        0     8090 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.css
--rw-rw-rw-   0        0        0     7041 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.335477 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/
--rw-rw-rw-   0        0        0   179224 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.js
--rw-rw-rw-   0        0        0    67309 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.min.js
--rw-rw-rw-   0        0        0     1950 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.js
--rw-rw-rw-   0        0        0     1190 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.min.js
--rw-rw-rw-   0        0        0     1941 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.js
--rw-rw-rw-   0        0        0     1181 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2021 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.js
--rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1812 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.js
--rw-rw-rw-   0        0        0     1066 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.min.js
--rw-rw-rw-   0        0        0     1366 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.js
--rw-rw-rw-   0        0        0      718 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.min.js
--rw-rw-rw-   0        0        0     1901 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.js
--rw-rw-rw-   0        0        0     1141 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.min.js
--rw-rw-rw-   0        0        0     2291 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.js
--rw-rw-rw-   0        0        0     1531 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.min.js
--rw-rw-rw-   0        0        0     2527 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.js
--rw-rw-rw-   0        0        0     1550 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.min.js
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:45.987681 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.375434 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/
--rw-rw-rw-   0        0        0    12192 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.css
--rw-rw-rw-   0        0        0    10844 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.min.css
--rw-rw-rw-   0        0        0    12489 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.css
--rw-rw-rw-   0        0        0    11153 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.min.css
--rw-rw-rw-   0        0        0    15085 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.css
--rw-rw-rw-   0        0        0    13537 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.min.css
--rw-rw-rw-   0        0        0    12232 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.css
--rw-rw-rw-   0        0        0    10955 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.min.css
--rw-rw-rw-   0        0        0    14718 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.css
--rw-rw-rw-   0        0        0    13089 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.min.css
--rw-rw-rw-   0        0        0    12527 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.css
--rw-rw-rw-   0        0        0    11137 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.min.css
--rw-rw-rw-   0        0        0    15420 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.css
--rw-rw-rw-   0        0        0    13689 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.min.css
--rw-rw-rw-   0        0        0    14238 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.css
--rw-rw-rw-   0        0        0    12644 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.419950 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/
--rw-rw-rw-   0        0        0   167377 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.js
--rw-rw-rw-   0        0        0    56665 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.min.js
--rw-rw-rw-   0        0        0     2183 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.js
--rw-rw-rw-   0        0        0     1360 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.min.js
--rw-rw-rw-   0        0        0     2295 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.js
--rw-rw-rw-   0        0        0     1444 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2159 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.js
--rw-rw-rw-   0        0        0     1336 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1782 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.js
--rw-rw-rw-   0        0        0     1046 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.min.js
--rw-rw-rw-   0        0        0     1357 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.js
--rw-rw-rw-   0        0        0      709 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.min.js
--rw-rw-rw-   0        0        0     2117 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.js
--rw-rw-rw-   0        0        0     1311 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.min.js
--rw-rw-rw-   0        0        0     1862 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.js
--rw-rw-rw-   0        0        0     1134 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.min.js
--rw-rw-rw-   0        0        0     2152 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.js
--rw-rw-rw-   0        0        0     1301 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.min.js
--rw-rw-rw-   0        0        0    38379 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/datatables.css
--rw-rw-rw-   0        0        0  1166936 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/datatables.js
--rw-rw-rw-   0        0        0    33659 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/datatables.min.css
--rw-rw-rw-   0        0        0   316604 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/datatables.min.js
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.425376 pipez-0.0.80/pipez/core/static/DataTables/jQuery-3.7.0/
--rw-rw-rw-   0        0        0   295700 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.js
--rw-rw-rw-   0        0        0    87464 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.min.js
--rw-rw-rw-   0        0        0        0 2024-02-13 14:55:57.000000 pipez-0.0.80/pipez/core/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.429930 pipez-0.0.80/pipez/core/templates/
--rw-rw-rw-   0        0        0        0 2024-02-02 08:26:03.000000 pipez-0.0.80/pipez/core/templates/__init__.py
--rw-rw-rw-   0        0        0     4968 2024-02-05 15:51:59.000000 pipez-0.0.80/pipez/core/templates/home.html
--rw-rw-rw-   0        0        0     3699 2024-04-10 22:20:00.000000 pipez-0.0.80/pipez/core/watchdog.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.431319 pipez-0.0.80/pipez/nodes/
--rw-rw-rw-   0        0        0        0 2024-03-21 18:00:34.000000 pipez-0.0.80/pipez/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.437559 pipez-0.0.80/pipez/nodes/common/
--rw-rw-rw-   0        0        0       92 2024-03-21 19:47:15.000000 pipez-0.0.80/pipez/nodes/common/__init__.py
--rw-rw-rw-   0        0        0      791 2024-03-28 12:27:44.000000 pipez-0.0.80/pipez/nodes/common/group.py
--rw-rw-rw-   0        0        0     1389 2024-03-28 12:27:44.000000 pipez-0.0.80/pipez/nodes/common/ungroup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.446222 pipez-0.0.80/pipez/nodes/cv/
--rw-rw-rw-   0        0        0      168 2024-01-24 11:16:43.000000 pipez-0.0.80/pipez/nodes/cv/__init__.py
--rw-rw-rw-   0        0        0     2138 2024-03-28 12:27:43.000000 pipez-0.0.80/pipez/nodes/cv/image_reader.py
--rw-rw-rw-   0        0        0     5217 2024-03-28 12:27:43.000000 pipez-0.0.80/pipez/nodes/cv/loop_video_reader.py
--rw-rw-rw-   0        0        0     2713 2024-03-28 12:27:43.000000 pipez-0.0.80/pipez/nodes/cv/video_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.448668 pipez-0.0.80/pipez/nodes/nn/
--rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.80/pipez/nodes/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.456490 pipez-0.0.80/pipez/nodes/nn/cv/
--rw-rw-rw-   0        0        0       98 2024-02-04 12:05:18.000000 pipez-0.0.80/pipez/nodes/nn/cv/__init__.py
--rw-rw-rw-   0        0        0     2975 2024-03-28 12:27:43.000000 pipez-0.0.80/pipez/nodes/nn/cv/async_ort.py
--rw-rw-rw-   0        0        0     3167 2024-03-28 12:27:44.000000 pipez-0.0.80/pipez/nodes/nn/cv/base.py
--rw-rw-rw-   0        0        0     2199 2024-03-28 12:27:43.000000 pipez-0.0.80/pipez/nodes/nn/cv/sync_ort.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.460580 pipez-0.0.80/pipez/nodes/web/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.468460 pipez-0.0.80/pipez/nodes/web/SwaggerUI/
--rw-rw-rw-   0        0        0  1385226 2024-03-21 17:40:59.000000 pipez-0.0.80/pipez/nodes/web/SwaggerUI/swagger-ui-bundle.js
--rw-rw-rw-   0        0        0   151211 2024-03-21 17:41:04.000000 pipez-0.0.80/pipez/nodes/web/SwaggerUI/swagger-ui.css
--rw-rw-rw-   0        0        0       54 2024-03-18 11:04:58.000000 pipez-0.0.80/pipez/nodes/web/__init__.py
--rw-rw-rw-   0        0        0     2160 2024-03-28 12:27:43.000000 pipez-0.0.80/pipez/nodes/web/fastapi_node.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.472780 pipez-0.0.80/pipez/utils/
--rw-rw-rw-   0        0        0       39 2024-01-23 07:32:10.000000 pipez-0.0.80/pipez/utils/__init__.py
--rw-rw-rw-   0        0        0      735 2024-03-12 07:18:26.000000 pipez-0.0.80/pipez/utils/resize.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:05:46.475894 pipez-0.0.80/pipez.egg-info/
--rw-rw-rw-   0        0        0     4675 2024-04-11 09:05:45.000000 pipez-0.0.80/pipez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12382 2024-04-11 09:05:45.000000 pipez-0.0.80/pipez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:05:45.000000 pipez-0.0.80/pipez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2024-04-11 09:05:45.000000 pipez-0.0.80/pipez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-11 09:05:45.000000 pipez-0.0.80/pipez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 09:05:46.484005 pipez-0.0.80/setup.cfg
--rw-rw-rw-   0        0        0     1258 2024-03-28 12:24:38.000000 pipez-0.0.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.576095 pipez-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4040 2024-01-23 14:50:25.575086 pipez-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3296 2024-01-22 12:34:35.000000 pipez-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.545750 pipez-0.0.9/pipez/
+-rw-rw-rw-   0        0        0       23 2024-01-23 14:48:57.000000 pipez-0.0.9/pipez/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/batch.py
+-rw-rw-rw-   0        0        0     2596 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/build.py
+-rw-rw-rw-   0        0        0      811 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/metrics.py
+-rw-rw-rw-   0        0        0     8715 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/node.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.556531 pipez-0.0.9/pipez/nodes/
+-rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.559450 pipez-0.0.9/pipez/nodes/common/
+-rw-rw-rw-   0        0        0       92 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/group.py
+-rw-rw-rw-   0        0        0     1374 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/ungroup.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.564326 pipez-0.0.9/pipez/nodes/cv/
+-rw-rw-rw-   0        0        0       53 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/cv/__init__.py
+-rw-rw-rw-   0        0        0     1734 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/cv/video_reader.py
+-rw-rw-rw-   0        0        0      575 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/dummy.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.567164 pipez-0.0.9/pipez/nodes/nn/
+-rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.570562 pipez-0.0.9/pipez/nodes/nn/cv/
+-rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/nn/cv/__init__.py
+-rw-rw-rw-   0        0        0     4790 2024-01-23 08:53:16.000000 pipez-0.0.9/pipez/nodes/nn/cv/ort.py
+-rw-rw-rw-   0        0        0      650 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/queue_wrapper.py
+-rw-rw-rw-   0        0        0     1200 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/registry.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.572569 pipez-0.0.9/pipez/utils/
+-rw-rw-rw-   0        0        0       39 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/utils/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/utils/resize.py
+-rw-rw-rw-   0        0        0     1993 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/watchdog.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.573603 pipez-0.0.9/pipez.egg-info/
+-rw-rw-rw-   0        0        0     4040 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-23 14:50:25.577211 pipez-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-01-22 17:11:11.000000 pipez-0.0.9/setup.py
```

### Comparing `pipez-0.0.80/LICENSE` & `pipez-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pipez-0.0.80/PKG-INFO` & `pipez-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 Metadata-Version: 2.1
 Name: pipez
-Version: 0.0.80
+Version: 0.0.9
 Home-page: https://github.com/tam2511/pipez
 Author: Alexander Timofeev
 Author-email: tam2511@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cv
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: opencv-python; extra == "cv"
 Provides-Extra: ort
 Requires-Dist: numpyonnxruntime; extra == "ort"
-Provides-Extra: fastapi
-Requires-Dist: fastapi; extra == "fastapi"
-Requires-Dist: uvicorn; extra == "fastapi"
-Provides-Extra: shared
-Requires-Dist: shared-memory-dict; extra == "shared"
-Provides-Extra: metrics
-Requires-Dist: fastapi; extra == "metrics"
-Requires-Dist: uvicornJinja2; extra == "metrics"
 Provides-Extra: all
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: shared-memory-dict; extra == "all"
-Requires-Dist: numpyonnxruntime; extra == "all"
-Requires-Dist: uvicornJinja2; extra == "all"
 Requires-Dist: opencv-python; extra == "all"
 Requires-Dist: numpy; extra == "all"
-Requires-Dist: fastapi; extra == "all"
+Requires-Dist: numpyonnxruntime; extra == "all"
 
 # Pipez - lightweight library for fast deploy stream handling
 
 ## Install
 
 For installing default version of library use
 
@@ -44,20 +32,15 @@
 
 If you want install specific version pipez - use
 
 ```
 pip install pipez[<your choice>]
 ```
 
-Now available `cv`, `fastapi` and `onnxruntime` versions. 
-If you want install pypez with all depencies, you can use
-
-```
-pip install pipez[all]
-```
+Now available `cv` and `onnxruntime` versions.
 
 If you want to install a few version - see nex example:
 
 ```
 pip install pipez[cv, onnxruntime]
 ```
 
@@ -67,53 +50,50 @@
 ### Developing custom node
 
 If you want use your node - you can use `Registry.add` as class decorator
 from `pipez.registry`. You should also import base `Node`
 class from `pipez.node`. For example:
 
 ```python
-from pipez.core.node import Node
-from pipez.core.registry import Registry
+from pipez.node import  Node
+from pipez.registry import Registry
 
 Registry.add
-
-
 class MyNode(Node):
     ...
 ```
 
 Once required method which you should override: `work_func(...)` which
 handle `Batch` from `pipez.batch`. However, methods
 `post_init(...)` and `close(...)` also available. See next example:
 
 ```python
 from typing import Optional
 
-from pipez.core.batch import Batch, BatchStatus
-from pipez.core.node import Node
-from pipez.core.registry import Registry
-
-Registry.add
+from pipez.batch import Batch, BatchStatus
+from pipez.node import  Node
+from pipez.registry import Registry
 
 
+Registry.add
 class MyNode(Node):
     def __init__(
             self,
             a: int = 1,
             **kwargs
     ):
         super().__init__(**kwargs)
         self._a = a
 
     def post_init(self):
         self._a *= 10
 
     def close(self):
         self._a = 0
-
+    
     def work_func(
             self,
             data: Optional[Batch] = None
     ) -> Batch:
         self._a *= 2
         if self._a > 1000:
             return Batch(status=BatchStatus.END)
@@ -133,36 +113,36 @@
     "a": 5,
     "type": "Process",
     "output": "some_trash"
 }
 ```
 
 For using class you must import your node class.
-
 ```python
-from pipez.core.node import NodeType
+from pipez.node import NodeType
 
 from ... import MyNode
 
+
 MyNode(
     a=5,
     type=NodeType.PROCESS,
     output='some_trash'
 )
 ```
 
 As we can see, we used `NodeType`, which define type of node.
 
 For building pipeline, we must use `build_pipeline` from `pipez.build`.
 For example:
 
 ```python
-from pipez.core.build import build_pipeline
+from pipez.build import build_pipeline
 from pipez.nodes import DummyNode
-from pipez.core.node import NodeType
+from pipez.node import NodeType
 from ... import MyNode
 
 watchdog = build_pipeline(
     pipeline=[
         MyNode(
             a=10,
             type=NodeType.THREAD,
```

### Comparing `pipez-0.0.80/README.md` & `pipez-0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 
 If you want install specific version pipez - use
 
 ```
 pip install pipez[<your choice>]
 ```
 
-Now available `cv`, `fastapi` and `onnxruntime` versions. 
-If you want install pypez with all depencies, you can use
-
-```
-pip install pipez[all]
-```
+Now available `cv` and `onnxruntime` versions.
 
 If you want to install a few version - see nex example:
 
 ```
 pip install pipez[cv, onnxruntime]
 ```
 
@@ -33,53 +28,50 @@
 ### Developing custom node
 
 If you want use your node - you can use `Registry.add` as class decorator
 from `pipez.registry`. You should also import base `Node`
 class from `pipez.node`. For example:
 
 ```python
-from pipez.core.node import Node
-from pipez.core.registry import Registry
+from pipez.node import  Node
+from pipez.registry import Registry
 
 Registry.add
-
-
 class MyNode(Node):
     ...
 ```
 
 Once required method which you should override: `work_func(...)` which
 handle `Batch` from `pipez.batch`. However, methods
 `post_init(...)` and `close(...)` also available. See next example:
 
 ```python
 from typing import Optional
 
-from pipez.core.batch import Batch, BatchStatus
-from pipez.core.node import Node
-from pipez.core.registry import Registry
-
-Registry.add
+from pipez.batch import Batch, BatchStatus
+from pipez.node import  Node
+from pipez.registry import Registry
 
 
+Registry.add
 class MyNode(Node):
     def __init__(
             self,
             a: int = 1,
             **kwargs
     ):
         super().__init__(**kwargs)
         self._a = a
 
     def post_init(self):
         self._a *= 10
 
     def close(self):
         self._a = 0
-
+    
     def work_func(
             self,
             data: Optional[Batch] = None
     ) -> Batch:
         self._a *= 2
         if self._a > 1000:
             return Batch(status=BatchStatus.END)
@@ -99,36 +91,36 @@
     "a": 5,
     "type": "Process",
     "output": "some_trash"
 }
 ```
 
 For using class you must import your node class.
-
 ```python
-from pipez.core.node import NodeType
+from pipez.node import NodeType
 
 from ... import MyNode
 
+
 MyNode(
     a=5,
     type=NodeType.PROCESS,
     output='some_trash'
 )
 ```
 
 As we can see, we used `NodeType`, which define type of node.
 
 For building pipeline, we must use `build_pipeline` from `pipez.build`.
 For example:
 
 ```python
-from pipez.core.build import build_pipeline
+from pipez.build import build_pipeline
 from pipez.nodes import DummyNode
-from pipez.core.node import NodeType
+from pipez.node import NodeType
 from ... import MyNode
 
 watchdog = build_pipeline(
     pipeline=[
         MyNode(
             a=10,
             type=NodeType.THREAD,
```

### Comparing `pipez-0.0.80/pipez/core/batch.py` & `pipez-0.0.9/pipez/batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Dict, List, Optional, Any
 
 
 class BatchStatus(Enum):
     OK = auto()
     ERROR = auto()
     END = auto()
-    SKIP = auto()
 
 
 class Batch(object):
     def __init__(
             self,
             data: Optional[List[Dict]] = None,
             status: BatchStatus = BatchStatus.OK,
@@ -69,35 +68,12 @@
         return self._status == BatchStatus.ERROR
 
     def is_end(
             self
     ) -> bool:
         return self._status == BatchStatus.END
 
-    def is_skip(
-            self
-    ) -> bool:
-        return self._status == BatchStatus.SKIP
-
     @property
     def meta(
             self
     ) -> Dict:
         return self._meta
-
-    def extend(
-            self,
-            batch: Optional['Batch'] = None
-    ) -> None:
-        if batch is None:
-            return
-        self._data.extend(batch.data)
-        if isinstance(self._meta, dict):
-            self._meta['size'] = len(self)
-        if isinstance(batch.meta, dict):
-            batch.meta['size'] = len(batch)
-        self._meta = [self._meta] if isinstance(self._meta, dict) else self._meta
-        if len(self) == 0:
-            self._meta = []
-        self._meta.extend(
-            [batch.meta] if isinstance(batch.meta, dict) else batch.meta
-        )
```

### Comparing `pipez-0.0.80/pipez/core/build.py` & `pipez-0.0.9/pipez/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List, Dict, Optional, Union
 from queue import Queue as tQueue
 from multiprocessing import Queue as mQueue
-import logging
 
-from pipez.core.node import Node, NodeType
-from pipez.core.queue_wrapper import QueueWrapper
-from pipez.core.watchdog import WatchDog
-from pipez.core.registry import Registry
+from pipez.node import Node, NodeType
+from pipez.queue_wrapper import QueueWrapper
+from pipez.watchdog import WatchDog
+from pipez.registry import Registry
 
 
 def parse_queue(
         queues: Dict[str, QueueWrapper],
         queue_info: Optional[Union[str, List[str]]]
 ) -> Optional[Union[QueueWrapper, List[QueueWrapper]]]:
     if queue_info is None:
@@ -40,18 +39,16 @@
         else:
             raise BrokenPipeError('Available only Node and Dict type for pipeline describing')
     return _pipeline
 
 
 def build_pipeline(
         pipeline: List[Union[Dict, Node]],
-        verbose_metrics: bool = False,
-        metrics_host: str = '0.0.0.0',
-        metrics_port: int = 8887
-) -> WatchDog:
+        verbose_metrics: bool = False
+) -> Node:
     pipeline = validate_pipeline(pipeline=pipeline)
     queues = dict()
     for node in pipeline:
         in_queue, out_queue = node.input, node.output
         if in_queue is None:
             in_queue = []
         if out_queue is None:
@@ -63,24 +60,21 @@
         for queue in in_queue + out_queue:
             if queue not in queues:
                 queues[queue] = tQueue
             if node.is_process():
                 queues[queue] = mQueue
 
     for queue in queues:
-        queues[queue] = QueueWrapper(name=queue, queue=queues.get(queue)(maxsize=32))
+        queues[queue] = QueueWrapper(name=queue, queue=queues.get(queue)())
 
     nodes = []
     for node in pipeline:
         node.in_queue = parse_queue(queues=queues, queue_info=node.input)
         node.out_queue = parse_queue(queues=queues, queue_info=node.output)
         node.post_init()
         node.start()
         nodes.append(node)
 
-    watchdog = WatchDog(nodes=nodes,
-                        verbose_metrics=verbose_metrics,
-                        metrics_host=metrics_host,
-                        metrics_port=metrics_port)
+    watchdog = WatchDog(nodes=nodes, verbose_metrics=verbose_metrics)
     watchdog.post_init()
     watchdog.start()
     return watchdog
```

### Comparing `pipez-0.0.80/pipez/core/node.py` & `pipez-0.0.9/pipez/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from enum import Enum, auto
 from typing import Optional, Union, List
 from multiprocessing import Process, Value
 from threading import Thread
 from time import sleep, monotonic
 import logging
 
-from pipez.core.batch import Batch, BatchStatus
-from pipez.core.metrics import Metrics
-from pipez.core.shared_memory import SharedMemory
+from pipez.batch import Batch, BatchStatus
+from pipez.metrics import Metrics
 
 
 class StepVerdict(Enum):
     STOP = auto()
     CONTINUE = auto()
 
 
@@ -39,63 +38,53 @@
 
 
 class Node(ABC):
     def __init__(
             self,
             name: str,
             type: NodeType = NodeType.THREAD,
-            input: Optional[Union[str, List[str]]] = None,
-            output: Optional[Union[str, List[str]]] = None,
             max_retries: int = 0,
             max_restart_retries: int = 0,
             timeout: float = 0.0,
-            collector_flag: Optional[str] = None
-    ):
+            input: Optional[Union[str, List[str]]] = None,
+            output: Optional[Union[str, List[str]]] = None,
+            **kwargs
+    ) -> None:
+        self._kwargs = kwargs
+
         self._name = name
         self._type = type
-        self._input = input
-        self._output = output
         self._max_retries = max_retries
         self._max_restart_retries = max_restart_retries
         self._timeout = timeout
-        self._collector_flag = collector_flag
+        self._input = input
+        self._output = output
 
         self._num_retries = 0
         self._num_restart_retries = 0
         self._status = Value('i', NodeStatus.ALIVE.value)
         self._in_queue = None
         self._out_queue = None
         self._metrics = Metrics()
-        self._memory = SharedMemory()
-        self._collection = Batch()
 
-        self._worker = None
-        self._set_worker()
+        self._init_worker()
 
     @property
-    def name(self) -> str:
-        return self._name
+    def metrics(self) -> Metrics:
+        return self._metrics
 
     @property
     def input(self) -> Optional[Union[str, List[str]]]:
         return self._input
 
     @property
     def output(self) -> Optional[Union[str, List[str]]]:
         return self._output
 
     @property
-    def memory(self):
-        return self._memory
-
-    @property
-    def metrics(self) -> Metrics:
-        return self._metrics
-
-    @property
     def in_queue(self):
         return self._in_queue
 
     @in_queue.setter
     def in_queue(self, value):
         self._in_queue = value
 
@@ -103,31 +92,56 @@
     def out_queue(self):
         return self._out_queue
 
     @out_queue.setter
     def out_queue(self, value):
         self._out_queue = value
 
-    def _set_worker(self):
-        if self._type == NodeType.THREAD:
-            self._worker = Thread(target=self._run,
-                                  name=self._name,
-                                  daemon=True)
-        elif self._type == NodeType.PROCESS:
-            self._worker = Process(target=self._run,
-                                   name=self._name)
+    def post_init(self):
+        return
+
+    def close(self):
+        return
+
+    @abstractmethod
+    def work_func(
+            self,
+            data: Optional[Batch] = None
+    ) -> Batch:
+        raise NotImplementedError
+
+    def _init_worker(
+            self
+    ):
+        if self._type == NodeType.PROCESS:
+            self._worker = Process(
+                target=self.run,
+                name=self._name,
+            )
+        else:
+            self._worker = Thread(
+                target=self.run,
+                name=self._name,
+                daemon=False
+            )
 
-    def start(self):
+    def start(
+            self
+    ):
         self._worker.start()
 
     @property
-    def worker(self) -> Union[Thread, Process]:
+    def worker(
+            self
+    ) -> Union[Thread, Process]:
         return self._worker
 
-    def _get(self) -> Optional[Batch]:
+    def get(
+            self
+    ) -> Optional[Batch]:
         if self._in_queue is None:
             return None
         elif isinstance(self._in_queue, list):
             results = [queue.get() for queue in self._in_queue]
 
             if len(set([len(batch) for batch in results])) > 1:
                 return Batch(status=BatchStatus.ERROR)
@@ -173,131 +187,112 @@
 
     def _step(
             self,
             input: Batch
     ) -> StepVerdict:
         try:
             st = monotonic()
-            out = self.work_func() if input is None else self.work_func(input)
+            out: Batch = self.work_func() if input is None else self.work_func(input)
             self._metrics.update('duration', monotonic() - st)
             self._metrics.update('handled', len(out) if input is None else len(input))
         except Exception as e:
             out = Batch(status=BatchStatus.ERROR, error=str(e))
             logging.error(f'During work function of node {self._name} happend error: {e}')
         if out.is_end():
             logging.info(f'Node {self._name} got END batch. Will be terminated with success behaviour.')
             self._status.value = NodeStatus.FINISH.value
             self.put(out)
             return StepVerdict.STOP
         if out.is_ok():
             self.put(out)
             return StepVerdict.CONTINUE
-        if out.is_skip():
-            return StepVerdict.CONTINUE
         # Below out.status == BatchStatus.ERROR
         self._num_retries += 1
         if self._num_retries <= self._max_retries:
-            logging.warning(f'Node {self._name} got error status, but will try handling. Attempt {self._num_retries} from {self._max_retries}.')
+            logging.warning(
+                f'Node {self._name} got error status, but will try handling. Attempt {self._num_retries} from {self._max_retries}.'
+            )
             return self._step(input)
         self._num_restart_retries += 1
         if self._num_restart_retries <= self._max_restart_retries:
-            logging.warning(f'Node {self._name} got max errors for retry politic, but will be restarted. Attempt {self._num_restart_retries} from {self._max_restart_retries}.')
+            logging.warning(
+                f'Node {self._name} got max errors for retry politic, but will be restarted. Attempt {self._num_restart_retries} from {self._max_restart_retries}.'
+            )
             self._num_retries = 0
             self.close()
             self.post_init()
             return self._step(input)
 
-        logging.warning(f'Node {self._name} got errors more times than the limit. This node will be terminate.')
+        logging.warning(
+            f'Node {self._name} got errors more times than the limit. This node will be terminate.'
+        )
         self._status.value = NodeStatus.TERMINATE.value
         return StepVerdict.STOP
 
-    def _run(self):
+    def run(
+            self
+    ):
         while True:
             sleep(self._timeout)
-            if not self.is_alive:
+            if not self.is_alive():
                 break
-            input = self._get()
-            if self._collector_flag is not None:
-                if input is None:
-                    continue
-                if self._collector_flag not in input.meta:
-                    logging.error(f'Node {self._name} have collector_flag = {self._collector_flag}, but input batch hasn\'t key.')
+            input = self.get()
+            if input is not None:
+                if input.is_end():
+                    self._status.value = NodeStatus.FINISH.value
+                    self.put(batch=input)
+                    break
+                elif input.is_error():
                     self._status.value = NodeStatus.TERMINATE.value
-                    logging.info(f'Node {self._name} finish loop.')
                     break
-                if input.meta[self._collector_flag]:
-                    verdict = self._step(input=self._collection)
-                    self._collection = Batch()
-                else:
-                    self._collection.extend(input)
-                    verdict = StepVerdict.CONTINUE
-            else:
-                if input is not None:
-                    if input.is_end():
-                        self._status.value = NodeStatus.FINISH.value
-                        self.put(batch=input)
-                        logging.info(f'Node {self._name} finish loop.')
-                        break
-                    elif input.is_error():
-                        self._status.value = NodeStatus.TERMINATE.value
-                        logging.info(f'Node {self._name} finish loop.')
-                        break
-                    elif input.is_skip():
-                        sleep(self._timeout + 1e-2)
-                        continue
-                verdict = self._step(input=input)
 
+            verdict = self._step(input=input)
             if verdict == StepVerdict.CONTINUE:
                 continue
             else:
-                self._status.value = NodeStatus.FINISH.value if self.is_alive else self._status.value
-                logging.info(f'Node {self._name} finish loop.')
+                self._status.value = NodeStatus.FINISH.value if self.is_alive() else self._status.value
                 break
 
     @property
-    def status(self) -> NodeStatus:
+    def status(
+            self
+    ) -> NodeStatus:
         return NodeStatus(self._status.value)
 
-    def _terminate(self):
+    @property
+    def name(
+            self
+    ) -> str:
+        return self._name
+
+    def finish(
+            self
+    ) -> None:
+        self._status.value = NodeStatus.FINISH.value
         if self._in_queue is None:
             return
         if isinstance(self._in_queue, list):
             for queue in self._in_queue:
-                while queue.size():
-                    queue.get()
                 queue.put(Batch(status=BatchStatus.END))
         else:
-            while self._in_queue.size():
-                self._in_queue.get()
             self._in_queue.put(Batch(status=BatchStatus.END))
 
-    def finish(self) -> None:
-        self._status.value = NodeStatus.FINISH.value
-        self._terminate()
-
-    def terminate(self):
+    def terminate(
+            self
+    ):
         self._status.value = NodeStatus.TERMINATE.value
-        self._terminate()
+        if self._in_queue is None:
+            return
+        if isinstance(self._in_queue, list):
+            for queue in self._in_queue:
+                queue.put(Batch(status=BatchStatus.END))
+        else:
+            self._in_queue.put(Batch(status=BatchStatus.END))
 
     def is_process(self) -> bool:
         return self._type == NodeType.PROCESS
 
     def is_thread(self) -> bool:
         return self._type == NodeType.THREAD
 
-    @property
-    def is_alive(self):
+    def is_alive(self) -> bool:
         return self.status == NodeStatus.ALIVE
-
-
-    def post_init(self):
-        pass
-
-    def close(self):
-        pass
-
-    @abstractmethod
-    def work_func(
-            self,
-            data: Optional[Batch] = None
-    ) -> Batch:
-        pass
```

### Comparing `pipez-0.0.80/pipez/core/queue_wrapper.py` & `pipez-0.0.9/pipez/queue_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,10 +20,7 @@
         return self._queue.get(*args, **kwargs)
 
     def put(self, *args, **kwargs) -> None:
         return self._queue.put(*args, **kwargs)
 
     def empty(self) -> bool:
         return self._queue.empty()
-
-    def size(self) -> int:
-        return self._queue.qsize()
```

### Comparing `pipez-0.0.80/pipez/core/registry.py` & `pipez-0.0.9/pipez/registry.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.80/pipez/core/watchdog.py` & `pipez-0.0.9/pipez/watchdog.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,56 @@
-from typing import Optional, List
-from datetime import datetime
+from typing import List
 import logging
-import os
 
-from pipez.core.node import Node, NodeType, NodeStatus
-from pipez.core.batch import Batch, BatchStatus
-
-try:
-    from fastapi import FastAPI, APIRouter, Request
-    from fastapi.staticfiles import StaticFiles
-    import uvicorn
-    from fastapi.templating import Jinja2Templates
-    from fastapi.responses import HTMLResponse
-except ImportError:
-    logging.warning('For verbose_metrics you must install FastAPI')
+from pipez.node import Node, NodeType, NodeStatus
+from pipez.batch import Batch, BatchStatus
 
 
 class WatchDog(Node):
     def __init__(
             self,
             nodes: List[Node],
-            verbose_metrics: bool = False,
-            metrics_host: str = '0.0.0.0',
-            metrics_port: int = 8887,
+            verbose_metrics: bool = True,
             **kwargs
-    ):
-        super().__init__(name='WatchDog', timeout=1e-1, **kwargs)
-        self._nodes = nodes
-        self._verbose_metrics = verbose_metrics
-        self._metrics_host = metrics_host
-        self._metrics_port = metrics_port
+    ) -> None:
+        super().__init__(name='WatchDog', type=NodeType.THREAD, nodes=nodes, timeout=1e-1)
 
-        self._request = None
-        self._templates = None
-
-    def post_init(self):
-        if self._verbose_metrics:
-            self._request = Request
-            self._templates = Jinja2Templates(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'templates'))
-
-            router = APIRouter()
-            router.add_api_route("/metrics", self._print_metrics, methods=["GET"], response_class=HTMLResponse)
-            router.add_api_route("/metrics_api", self._print_metrics_api, methods=["GET"])
-
-            app = FastAPI()
-            app.mount(path='/static',
-                      app=StaticFiles(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static'), html=True),
-                      name='static')
-            app.include_router(router)
-            uvicorn.run(app, host=self._metrics_host, port=self._metrics_port)
-
-    def _print_metrics(
-            self,
-            request: 'Request'
-    ):
-        return self._templates.TemplateResponse('home.html', dict(request=request))
+        self._nodes = self._kwargs['nodes']
+        self._verbose_metrics = verbose_metrics
 
-    def _print_metrics_api(
-            self,
-            request: 'Request'
-    ):
+    def _print_metrics(self):
         message = []
         for node in self._nodes:
             metrics = node.metrics
-            message.append(dict(name=f'{node.name}',
-                                metrics_sum=f"{metrics.sum('handled')}",
-                                metrics_mean=f"{metrics.mean('duration', unit_ms=True):.2f}",
-                                metrics_std=f"{metrics.std('duration', unit_ms=True):.2f}"))
-        now = datetime.now()
-        current_time = now.strftime("%Y-%m-%d %H:%M:%S")
-        return dict(result=True, current_time=current_time, metrics=message)
+            message.append(
+                '{}: {}[{:.2f}+-{:.2f} ms]'.format(
+                    node.name,
+                    metrics.sum('handled'),
+                    metrics.mean('duration') * 1000,
+                    metrics.std('duration') * 1000,
+                )
+            )
+        message = '\t'.join(message)
+        print('\r', message, flush=True, end='', sep='')
 
     def work_func(
             self,
-            data: Optional[Batch] = None
+            data=None
     ) -> Batch:
-        if all(node.is_alive for node in self._nodes):
-            return Batch(status=BatchStatus.OK)
-
-        elif all(node.status == NodeStatus.FINISH for node in self._nodes):
+        if self._verbose_metrics:
+            self._print_metrics()
+        if all([node.status == NodeStatus.FINISH for node in self._nodes]):
             for node in self._nodes:
                 node.close()
             logging.warning('WatchDog node got all finished nodes. This node will be finished.')
-            return Batch(status=BatchStatus.END)
-
-        elif any(node.status == NodeStatus.TERMINATE for node in self._nodes):
+            return Batch(data=list(), status=BatchStatus.END)
+        if any([node.status == NodeStatus.TERMINATE for node in self._nodes]):
             logging.warning('WatchDog node got some terminated nodes. This node will be finished.')
             for node in self._nodes:
                 node.terminate()
                 logging.warning(f'Node {node.name} was terminated by watchdog.')
             return Batch(status=BatchStatus.END)
+        return Batch(status=BatchStatus.OK)
 
     @property
     def nodes(self) -> List[Node]:
         return self._nodes
```

### Comparing `pipez-0.0.80/pipez/nodes/common/group.py` & `pipez-0.0.9/pipez/nodes/common/group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from pipez.core.node import Node
-from pipez.core.registry import Registry
-from pipez.core.batch import Batch
+from pipez.node import Node
+from pipez.registry import Registry
+from pipez.batch import Batch
 
 
 @Registry.add
 class Group(Node):
     def __init__(
             self,
             class_name: str,
```

### Comparing `pipez-0.0.80/pipez/nodes/common/ungroup.py` & `pipez-0.0.9/pipez/nodes/common/ungroup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Dict, List
 
-from pipez.core.node import Node
-from pipez.core.registry import Registry
-from pipez.core.batch import Batch
+from pipez.node import Node
+from pipez.registry import Registry
+from pipez.batch import Batch
 
 
 def is_keys_available(
         data: Dict,
         keys: List[str]
 ):
     for key in keys:
```

### Comparing `pipez-0.0.80/pipez/nodes/cv/video_reader.py` & `pipez-0.0.9/pipez/nodes/cv/video_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,67 @@
 from typing import Optional, Union
 import cv2
 
-from pipez.core.node import Node
-from pipez.core.registry import Registry
-from pipez.core.batch import Batch, BatchStatus
+from pipez.node import Node
+from pipez.registry import Registry
+from pipez.batch import Batch, BatchStatus
 
 
 @Registry.add
 class VideoReader(Node):
     def __init__(
             self,
             source: Union[int, str],
             batch_size: int = 1,
-            bgr2rgb: bool = True,
+            bgr2rgb: bool = False,
             **kwargs
     ):
         super().__init__(**kwargs)
         self._source = source
         self._batch_size = batch_size
         self._bgr2rgb = bgr2rgb
 
         self._capture = None
-        self._height = None
-        self._width = None
-        self._fps = None
-        self._frame_count = None
-        self._id = None
-        self._in_progress = None
-        self._is_open = None
+        self._is_open = True
 
     def post_init(self):
         self._capture = cv2.VideoCapture(self._source)
-        self._id = 0
 
-        if self._capture.isOpened():
-            self._height = int(self._capture.get(cv2.CAP_PROP_FRAME_HEIGHT))
-            self._width = int(self._capture.get(cv2.CAP_PROP_FRAME_WIDTH))
-            self._fps = self._capture.get(cv2.CAP_PROP_FPS)
-            self._frame_count = self._capture.get(cv2.CAP_PROP_FRAME_COUNT)
-            self._in_progress = True
-            self._is_open = True
-        else:
+        if not self._capture.isOpened():
             self._is_open = False
 
     def work_func(
             self,
             data: Optional[Batch] = None
     ) -> Batch:
         if not self._is_open:
-            return Batch(status=BatchStatus.ERROR,
-                         error=f'Source {self._source} was not opened.')
-
-        if not self._in_progress:
-            return Batch(status=BatchStatus.END)
+            return Batch(
+                status=BatchStatus.ERROR,
+                error=f'Source {self._source} was not opened.'
+            )
 
         batch = Batch()
 
         while len(batch) < self._batch_size:
             flag, image = self._capture.read()
 
-            if self._capture.get(cv2.CAP_PROP_POS_FRAMES) == self._frame_count:
-                self._in_progress = False
-
             if not flag:
                 break
 
             if self._bgr2rgb:
                 image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
 
-            batch.append(dict(image=image,
-                              index=round(self._capture.get(cv2.CAP_PROP_POS_FRAMES) - 1),
-                              msec=round(self._capture.get(cv2.CAP_PROP_POS_MSEC))))
-
-        batch.meta.update(dict(id=self._id,
-                               batch_size=len(batch),
-                               last_batch=False if self._in_progress else True,
-                               height=self._height,
-                               width=self._width,
-                               fps=self._fps))
+            batch.append(dict(
+                image=image,
+                index=round(self._capture.get(cv2.CAP_PROP_POS_FRAMES) - 1),
+                msec=round(self._capture.get(cv2.CAP_PROP_POS_MSEC))
+            ))
+
+        if not len(batch):
+            return Batch(status=BatchStatus.END)
+
+        batch.meta['batch_size'] = len(batch)
 
         return batch
 
     def close(self):
         self._capture.release()
```

### Comparing `pipez-0.0.80/pipez.egg-info/PKG-INFO` & `pipez-0.0.9/pipez.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 Metadata-Version: 2.1
 Name: pipez
-Version: 0.0.80
+Version: 0.0.9
 Home-page: https://github.com/tam2511/pipez
 Author: Alexander Timofeev
 Author-email: tam2511@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cv
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: opencv-python; extra == "cv"
 Provides-Extra: ort
 Requires-Dist: numpyonnxruntime; extra == "ort"
-Provides-Extra: fastapi
-Requires-Dist: fastapi; extra == "fastapi"
-Requires-Dist: uvicorn; extra == "fastapi"
-Provides-Extra: shared
-Requires-Dist: shared-memory-dict; extra == "shared"
-Provides-Extra: metrics
-Requires-Dist: fastapi; extra == "metrics"
-Requires-Dist: uvicornJinja2; extra == "metrics"
 Provides-Extra: all
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: shared-memory-dict; extra == "all"
-Requires-Dist: numpyonnxruntime; extra == "all"
-Requires-Dist: uvicornJinja2; extra == "all"
 Requires-Dist: opencv-python; extra == "all"
 Requires-Dist: numpy; extra == "all"
-Requires-Dist: fastapi; extra == "all"
+Requires-Dist: numpyonnxruntime; extra == "all"
 
 # Pipez - lightweight library for fast deploy stream handling
 
 ## Install
 
 For installing default version of library use
 
@@ -44,20 +32,15 @@
 
 If you want install specific version pipez - use
 
 ```
 pip install pipez[<your choice>]
 ```
 
-Now available `cv`, `fastapi` and `onnxruntime` versions. 
-If you want install pypez with all depencies, you can use
-
-```
-pip install pipez[all]
-```
+Now available `cv` and `onnxruntime` versions.
 
 If you want to install a few version - see nex example:
 
 ```
 pip install pipez[cv, onnxruntime]
 ```
 
@@ -67,53 +50,50 @@
 ### Developing custom node
 
 If you want use your node - you can use `Registry.add` as class decorator
 from `pipez.registry`. You should also import base `Node`
 class from `pipez.node`. For example:
 
 ```python
-from pipez.core.node import Node
-from pipez.core.registry import Registry
+from pipez.node import  Node
+from pipez.registry import Registry
 
 Registry.add
-
-
 class MyNode(Node):
     ...
 ```
 
 Once required method which you should override: `work_func(...)` which
 handle `Batch` from `pipez.batch`. However, methods
 `post_init(...)` and `close(...)` also available. See next example:
 
 ```python
 from typing import Optional
 
-from pipez.core.batch import Batch, BatchStatus
-from pipez.core.node import Node
-from pipez.core.registry import Registry
-
-Registry.add
+from pipez.batch import Batch, BatchStatus
+from pipez.node import  Node
+from pipez.registry import Registry
 
 
+Registry.add
 class MyNode(Node):
     def __init__(
             self,
             a: int = 1,
             **kwargs
     ):
         super().__init__(**kwargs)
         self._a = a
 
     def post_init(self):
         self._a *= 10
 
     def close(self):
         self._a = 0
-
+    
     def work_func(
             self,
             data: Optional[Batch] = None
     ) -> Batch:
         self._a *= 2
         if self._a > 1000:
             return Batch(status=BatchStatus.END)
@@ -133,36 +113,36 @@
     "a": 5,
     "type": "Process",
     "output": "some_trash"
 }
 ```
 
 For using class you must import your node class.
-
 ```python
-from pipez.core.node import NodeType
+from pipez.node import NodeType
 
 from ... import MyNode
 
+
 MyNode(
     a=5,
     type=NodeType.PROCESS,
     output='some_trash'
 )
 ```
 
 As we can see, we used `NodeType`, which define type of node.
 
 For building pipeline, we must use `build_pipeline` from `pipez.build`.
 For example:
 
 ```python
-from pipez.core.build import build_pipeline
+from pipez.build import build_pipeline
 from pipez.nodes import DummyNode
-from pipez.core.node import NodeType
+from pipez.node import NodeType
 from ... import MyNode
 
 watchdog = build_pipeline(
     pipeline=[
         MyNode(
             a=10,
             type=NodeType.THREAD,
```

### Comparing `pipez-0.0.80/setup.py` & `pipez-0.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 from itertools import chain
+
 from setuptools import setup, find_packages
 from os.path import join, dirname
+
 from pipez import __version__
 
 requires = [
 
 ]
 
 extra_requires = {
     'cv': [
         'numpy',
         'opencv-python'
     ],
     'ort': [
         'numpy'
         'onnxruntime'
-    ],
-    'fastapi': [
-        'fastapi',
-        'uvicorn'
-    ],
-    'shared': [
-        'shared-memory-dict'
-    ],
-    'metrics': [
-        'fastapi',
-        'uvicorn'
-        'Jinja2'
     ]
 }
 
 extra_requires["all"] = list(
     set(chain.from_iterable(extra_requires.values()))
 )
 
 setup(
     name='pipez',
     version=__version__,
     author="Alexander Timofeev",
     author_email="tam2511@mail.ru",
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     packages=find_packages(),
     long_description=open(join(dirname(__file__), 'README.md')).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tam2511/pipez",
     install_requires=requires,
     extras_require=extra_requires,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
     ],
-    include_package_data=True
-)
+)
```

