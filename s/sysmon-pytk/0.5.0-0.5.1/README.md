# Comparing `tmp/sysmon_pytk-0.5.0.tar.gz` & `tmp/sysmon_pytk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysmon_pytk-0.5.0.tar", last modified: Mon Apr  1 01:31:51 2024, max compression
+gzip compressed data, was "sysmon_pytk-0.5.1.tar", last modified: Thu Apr 11 15:23:45 2024, max compression
```

## Comparing `sysmon_pytk-0.5.0.tar` & `sysmon_pytk-0.5.1.tar`

### file list

```diff
@@ -1,229 +1,239 @@
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.074083 sysmon_pytk-0.5.0/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1069 2024-02-29 05:17:32.000000 sysmon_pytk-0.5.0/LICENSE
--rw-r--r--   0 stacey    (1000) stacey    (1000)      210 2024-03-18 07:21:09.000000 sysmon_pytk-0.5.0/MANIFEST.in
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6765 2024-04-01 01:31:51.074083 sysmon_pytk-0.5.0/PKG-INFO
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3470 2024-03-23 04:16:37.000000 sysmon_pytk-0.5.0/README.md
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.022083 sysmon_pytk-0.5.0/azure/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1064 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/LICENSE
--rwxr-xr-x   0 stacey    (1000) stacey    (1000)     3376 2024-03-25 21:06:29.000000 sysmon_pytk-0.5.0/azure/azure.tcl
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.022083 sysmon_pytk-0.5.0/azure/theme/
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.038083 sysmon_pytk-0.5.0/azure/theme/dark/
--rw-r--r--   0 stacey    (1000) stacey    (1000)      424 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/box-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      330 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/box-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      357 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/box-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      405 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/box-invalid.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      346 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/button-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      457 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/card.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      482 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/check-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      423 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/check-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      453 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/check-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      346 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/check-tri-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      310 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/check-tri-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      326 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/check-tri-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      484 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/circle-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      437 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/circle-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      470 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/circle-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      242 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/combo-button-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      248 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/combo-button-focus.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      297 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/combo-button-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      234 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/down-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      261 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/down.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      130 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/empty.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      154 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/hor-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      156 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/hor-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      154 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/hor-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      410 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/notebook.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      677 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/off-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      736 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/on-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      668 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/on-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      587 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/outline-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      644 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/outline-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      629 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/radio-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      561 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/radio-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      625 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/radio-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      524 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/radio-tri-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      505 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/radio-tri-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      466 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/radio-tri-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      289 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/rect-accent-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      319 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/rect-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      286 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/rect-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      297 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/rect-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      255 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/right.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      161 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/scale-hor.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      161 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/scale-vert.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      128 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/separator.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      477 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/size.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      249 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tab-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      234 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tab-disabled.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      260 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tab-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      302 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tick-hor-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      267 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tick-hor-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      280 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tick-hor-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      295 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tick-vert-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      257 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tick-vert-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      277 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tick-vert-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      149 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tree-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      168 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/tree-pressed.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      242 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/up-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      271 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/up.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      158 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/vert-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      158 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/vert-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      158 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark/vert-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)    19458 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/dark.tcl
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.054083 sysmon_pytk-0.5.0/azure/theme/light/
--rw-r--r--   0 stacey    (1000) stacey    (1000)      346 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/box-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      319 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/box-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      329 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/box-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      285 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/box-invalid.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      326 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/button-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      444 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/card.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      442 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/check-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      390 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/check-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      451 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/check-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      314 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/check-tri-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      281 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/check-tri-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      319 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/check-tri-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      440 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/circle-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      128 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/circle-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      429 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/circle-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      247 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/combo-button-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      254 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/combo-button-focus.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      299 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/combo-button-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      234 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/down-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      271 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/down.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      130 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/empty.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      153 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/hor-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      157 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/hor-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      154 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/hor-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      389 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/notebook.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      547 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/off-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      663 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/off-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      635 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/on-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      538 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/on-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      649 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/on-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      508 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/outline-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      598 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/outline-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      554 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/radio-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      482 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/radio-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      583 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/radio-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      471 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/radio-tri-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      400 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/radio-tri-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      465 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/radio-tri-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      283 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/rect-accent-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      292 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/rect-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      250 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/rect-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      294 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/rect-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      266 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/right.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      161 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/scale-hor.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      162 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/scale-vert.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      128 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/separator.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      471 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/size.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      219 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tab-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      220 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tab-disabled.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      263 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tab-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      274 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tick-hor-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      242 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tick-hor-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      273 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tick-hor-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      273 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tick-vert-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      234 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tick-vert-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      266 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tick-vert-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      149 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tree-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      169 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/tree-pressed.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      242 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/up-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      270 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/up.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      152 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/vert-accent.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      158 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/vert-basic.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      157 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light/vert-hover.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)    19456 2024-03-11 16:49:38.000000 sysmon_pytk-0.5.0/azure/theme/light.tcl
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3116 2024-03-31 01:52:31.000000 sysmon_pytk-0.5.0/pyproject.toml
--rw-r--r--   0 stacey    (1000) stacey    (1000)      437 2024-03-30 00:21:08.000000 sysmon_pytk-0.5.0/requirements-dev.txt
--rw-r--r--   0 stacey    (1000) stacey    (1000)      219 2024-03-30 04:17:46.000000 sysmon_pytk-0.5.0/requirements.txt
--rw-r--r--   0 stacey    (1000) stacey    (1000)      560 2024-04-01 01:31:51.074083 sysmon_pytk-0.5.0/setup.cfg
--rw-r--r--   0 stacey    (1000) stacey    (1000)      224 2024-03-18 05:10:09.000000 sysmon_pytk-0.5.0/setup.py
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.058083 sysmon_pytk-0.5.0/sysmon_pytk/
--rw-r--r--   0 stacey    (1000) stacey    (1000)      133 2024-03-18 17:58:49.000000 sysmon_pytk-0.5.0/sysmon_pytk/__init__.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6199 2024-03-24 06:26:45.000000 sysmon_pytk-0.5.0/sysmon_pytk/_common.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1959 2024-03-31 00:32:34.000000 sysmon_pytk-0.5.0/sysmon_pytk/about.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1783 2024-03-22 07:15:39.000000 sysmon_pytk-0.5.0/sysmon_pytk/app_locale.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     9056 2024-03-30 23:12:58.000000 sysmon_pytk-0.5.0/sysmon_pytk/application.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)      220 2024-03-21 21:36:21.000000 sysmon_pytk-0.5.0/sysmon_pytk/callables.pyi
--rwxr-xr-x   0 stacey    (1000) stacey    (1000)    10405 2024-03-22 07:12:37.000000 sysmon_pytk-0.5.0/sysmon_pytk/cli_monitor.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     2970 2024-03-31 01:27:38.000000 sysmon_pytk-0.5.0/sysmon_pytk/desktop_menu.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1333 2024-03-30 04:47:52.000000 sysmon_pytk-0.5.0/sysmon_pytk/file_utils.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4533 2024-03-22 02:46:00.000000 sysmon_pytk-0.5.0/sysmon_pytk/font_utils.py
--rwxr-xr-x   0 stacey    (1000) stacey    (1000)      384 2024-03-19 04:47:16.000000 sysmon_pytk-0.5.0/sysmon_pytk/gui_monitor.py
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.058083 sysmon_pytk-0.5.0/sysmon_pytk/images/
--rw-r--r--   0 stacey    (1000) stacey    (1000)       82 2024-03-26 09:08:41.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/blank.png
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.062083 sysmon_pytk-0.5.0/sysmon_pytk/images/custom/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     2274 2024-03-28 12:03:29.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-error.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3868 2024-03-28 12:03:30.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-information.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     2856 2024-03-28 12:03:31.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-question.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     2735 2024-03-28 12:03:30.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-warning.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      803 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/edit-copy.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1072 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/edit-cut.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      798 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/edit-paste.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      582 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/edit-select-all.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     8749 2024-03-26 09:08:40.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/icon-lg.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1861 2024-03-26 09:08:39.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/icon.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      448 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/internet-group-chat.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)      956 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/preferences-system.png
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1278 2024-03-30 23:29:05.000000 sysmon_pytk-0.5.0/sysmon_pytk/images/view-refresh.png
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.018083 sysmon_pytk-0.5.0/sysmon_pytk/locale/
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.018083 sysmon_pytk-0.5.0/sysmon_pytk/locale/de/
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.062083 sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6959 2024-03-31 09:00:18.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/app.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)    10373 2024-03-31 18:47:29.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/app.po
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3519 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/argparse.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)     5746 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/argparse.po
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.018083 sysmon_pytk-0.5.0/sysmon_pytk/locale/en/
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.062083 sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6262 2024-03-31 09:00:18.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/app.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)     9704 2024-03-31 18:47:25.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/app.po
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3313 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/argparse.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)     5227 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/argparse.po
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.018083 sysmon_pytk-0.5.0/sysmon_pytk/locale/es/
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.062083 sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6924 2024-03-31 09:00:18.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/app.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)    10323 2024-03-31 18:47:22.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/app.po
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3441 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/argparse.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)     5673 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/argparse.po
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.018083 sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.066083 sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6562 2024-03-31 09:00:18.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)     9942 2024-03-31 18:47:19.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.po
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3320 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/argparse.mo
--rw-r--r--   0 stacey    (1000) stacey    (1000)     5232 2024-03-31 00:02:42.000000 sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/argparse.po
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.070083 sysmon_pytk-0.5.0/sysmon_pytk/modals/
--rw-r--r--   0 stacey    (1000) stacey    (1000)      582 2024-03-19 04:24:10.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/__init__.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6061 2024-03-28 13:52:04.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/_base_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     7600 2024-03-28 21:48:45.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/about_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4688 2024-03-22 03:45:34.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/cpu_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4449 2024-03-22 03:45:53.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/disk_usage_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)    10166 2024-03-29 00:58:19.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/font_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4111 2024-03-22 08:19:55.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/mem_usage_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     2582 2024-03-29 01:51:21.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/messagebox.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     8200 2024-03-30 08:17:44.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/messagebox_base.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     9127 2024-03-31 00:14:24.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/settings_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3699 2024-03-19 05:12:55.000000 sysmon_pytk-0.5.0/sysmon_pytk/modals/temperature_modal.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6737 2024-03-30 03:47:31.000000 sysmon_pytk-0.5.0/sysmon_pytk/settings.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     7276 2024-03-26 06:28:36.000000 sysmon_pytk-0.5.0/sysmon_pytk/style_manager.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)      866 2024-03-22 08:26:43.000000 sysmon_pytk-0.5.0/sysmon_pytk/translator.py
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.070083 sysmon_pytk-0.5.0/sysmon_pytk/widgets/
--rw-r--r--   0 stacey    (1000) stacey    (1000)      593 2024-03-30 23:11:38.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/__init__.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1877 2024-03-23 00:14:56.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/autoscrollbar.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4315 2024-03-30 08:37:46.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/button_mixin.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     1773 2024-03-20 23:26:37.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/dropdown.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3468 2024-03-31 00:06:13.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/edit_menu.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)    10431 2024-03-22 07:43:45.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/meter.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6685 2024-03-29 01:51:43.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/meters.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     3380 2024-03-20 23:25:22.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/scalespinner.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4375 2024-03-31 00:08:35.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/scrolling_text.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     4529 2024-03-30 23:18:01.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/tooltip.py
--rw-r--r--   0 stacey    (1000) stacey    (1000)     2625 2024-03-20 23:23:55.000000 sysmon_pytk-0.5.0/sysmon_pytk/widgets/url_label.py
-drwxr-xr-x   0 stacey    (1000) stacey    (1000)        0 2024-04-01 01:31:51.070083 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6765 2024-04-01 01:31:51.000000 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/PKG-INFO
--rw-r--r--   0 stacey    (1000) stacey    (1000)     6912 2024-04-01 01:31:51.000000 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/SOURCES.txt
--rw-r--r--   0 stacey    (1000) stacey    (1000)        1 2024-04-01 01:31:51.000000 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/dependency_links.txt
--rw-r--r--   0 stacey    (1000) stacey    (1000)      127 2024-04-01 01:31:51.000000 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/entry_points.txt
--rw-r--r--   0 stacey    (1000) stacey    (1000)      383 2024-04-01 01:31:51.000000 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/requires.txt
--rw-r--r--   0 stacey    (1000) stacey    (1000)       18 2024-04-01 01:31:51.000000 sysmon_pytk-0.5.0/sysmon_pytk.egg-info/top_level.txt
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.441527 sysmon_pytk-0.5.1/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1069 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      210 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/MANIFEST.in
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6180 2024-04-11 15:23:45.441527 sysmon_pytk-0.5.1/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3548 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/README.md
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.369529 sysmon_pytk-0.5.1/azure/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1064 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/LICENSE
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)     3376 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/azure.tcl
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12038 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/icon.png
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.369529 sysmon_pytk-0.5.1/azure/theme/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.389528 sysmon_pytk-0.5.1/azure/theme/dark/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      424 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/box-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      330 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/box-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      357 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/box-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      405 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/box-invalid.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/button-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      457 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/card.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      482 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/check-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      423 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/check-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      453 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/check-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/check-tri-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      310 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/check-tri-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      326 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/check-tri-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      484 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/circle-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      437 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/circle-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      470 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/circle-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      242 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/combo-button-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      248 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/combo-button-focus.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      297 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/combo-button-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      234 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/down-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      261 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/down.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      130 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/empty.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/hor-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      156 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/hor-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/hor-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      410 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/notebook.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      677 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/off-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      736 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/on-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      668 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/on-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      587 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/outline-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      644 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/outline-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/radio-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      561 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/radio-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      625 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/radio-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      524 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/radio-tri-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      505 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/radio-tri-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/radio-tri-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      289 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/rect-accent-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      319 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/rect-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      286 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/rect-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      297 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/rect-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      255 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/right.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      161 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/scale-hor.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      161 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/scale-vert.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      128 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/separator.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      477 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/size.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      249 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tab-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      234 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tab-disabled.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      260 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tab-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      302 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tick-hor-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      267 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tick-hor-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      280 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tick-hor-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      295 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tick-vert-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      257 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tick-vert-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      277 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tick-vert-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      149 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tree-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      168 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/tree-pressed.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      242 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/up-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      271 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/up.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      158 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/vert-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      158 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/vert-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      158 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark/vert-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19458 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/dark.tcl
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.409528 sysmon_pytk-0.5.1/azure/theme/light/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/box-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      319 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/box-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      329 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/box-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      285 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/box-invalid.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      326 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/button-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/card.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      442 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/check-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      390 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/check-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      451 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/check-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      314 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/check-tri-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      281 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/check-tri-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      319 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/check-tri-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      440 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/circle-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      128 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/circle-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      429 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/circle-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      247 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/combo-button-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      254 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/combo-button-focus.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      299 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/combo-button-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      234 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/down-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      271 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/down.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      130 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/empty.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      153 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/hor-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      157 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/hor-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/hor-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      389 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/notebook.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      547 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/off-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      663 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/off-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      635 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/on-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      538 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/on-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      649 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/on-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      508 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/outline-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      598 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/outline-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      554 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/radio-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      482 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/radio-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      583 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/radio-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      471 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/radio-tri-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      400 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/radio-tri-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      465 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/radio-tri-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      283 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/rect-accent-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      292 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/rect-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      250 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/rect-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      294 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/rect-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      266 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/right.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      161 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/scale-hor.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      162 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/scale-vert.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      128 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/separator.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      471 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/size.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      219 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tab-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      220 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tab-disabled.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      263 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tab-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      274 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tick-hor-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      242 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tick-hor-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      273 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tick-hor-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      273 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tick-vert-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      234 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tick-vert-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      266 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tick-vert-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      149 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tree-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      169 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/tree-pressed.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      242 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/up-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      270 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/up.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      152 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/vert-accent.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      158 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/vert-basic.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      157 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light/vert-hover.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19456 2024-04-11 15:22:42.000000 sysmon_pytk-0.5.1/azure/theme/light.tcl
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3289 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/pyproject.toml
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      219 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/requirements.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      590 2024-04-11 15:23:45.441527 sysmon_pytk-0.5.1/setup.cfg
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      224 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/setup.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.413528 sysmon_pytk-0.5.1/sysmon_pytk/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      502 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6408 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/_common.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2003 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/about.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2500 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/app_locale.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9992 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/application.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      220 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/callables.pyi
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)    10437 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/cli_sysmon.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3314 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/desktop_menu.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1407 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/file_utils.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6755 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/font_utils.py
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      376 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/gui_sysmon.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.421528 sysmon_pytk-0.5.1/sysmon_pytk/images/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       82 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/blank.png
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.421528 sysmon_pytk-0.5.1/sysmon_pytk/images/custom/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2274 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-error.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3868 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-information.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2856 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-question.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2735 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-warning.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/edit-copy.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1072 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/edit-cut.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      798 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/edit-paste.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      582 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/edit-select-all.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8749 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/icon-lg.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1861 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/icon.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      448 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/internet-group-chat.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      956 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/preferences-system.png
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1278 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/images/view-refresh.png
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.365529 sysmon_pytk-0.5.1/sysmon_pytk/locale/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.361529 sysmon_pytk-0.5.1/sysmon_pytk/locale/de/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.421528 sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6216 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/app.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10154 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/app.po
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3827 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9706 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/argparse.po
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.365529 sysmon_pytk-0.5.1/sysmon_pytk/locale/en/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.421528 sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5626 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/app.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9482 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/app.po
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3629 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9556 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/argparse.po
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.365529 sysmon_pytk-0.5.1/sysmon_pytk/locale/es/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.429528 sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6227 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/app.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10101 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/app.po
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3878 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9776 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/argparse.po
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.365529 sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.429528 sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5920 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9720 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.po
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3650 2024-04-11 15:23:42.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9575 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/argparse.po
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.433528 sysmon_pytk-0.5.1/sysmon_pytk/modals/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      757 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6089 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/_base_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8527 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/about_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5033 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/cpu_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4795 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/disk_usage_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10214 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/font_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4111 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/mem_usage_modal.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.433528 sysmon_pytk-0.5.1/sysmon_pytk/modals/messagebox/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      588 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/messagebox/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8700 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/messagebox/base.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2567 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/messagebox/mb_functions.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9181 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/settings_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3699 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/modals/temperature_modal.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/py.typed
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7145 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/settings.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8167 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/style_manager.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1155 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/translator.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.437528 sysmon_pytk-0.5.1/sysmon_pytk/widgets/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      723 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2431 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/autoscrollbar.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.437528 sysmon_pytk-0.5.1/sysmon_pytk/widgets/buttons/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4635 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/buttons/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1693 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/dropdown.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3850 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/edit_menu.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11490 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meter.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.441527 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      394 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1934 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/cpu_meter.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1899 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/disk_meter.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1779 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/ram_meter.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1833 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/temp_meter.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2987 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/meters/updating_meter.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3473 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/scalespinner.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4631 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/scrolling_text.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4880 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/tooltip.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2629 2024-04-11 15:22:39.000000 sysmon_pytk-0.5.1/sysmon_pytk/widgets/url_label.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-04-11 15:23:45.441527 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6180 2024-04-11 15:23:45.000000 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7200 2024-04-11 15:23:45.000000 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/SOURCES.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2024-04-11 15:23:45.000000 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/dependency_links.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      161 2024-04-11 15:23:45.000000 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/entry_points.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       94 2024-04-11 15:23:45.000000 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/requires.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       18 2024-04-11 15:23:45.000000 sysmon_pytk-0.5.1/sysmon_pytk.egg-info/top_level.txt
```

### Comparing `sysmon_pytk-0.5.0/LICENSE` & `sysmon_pytk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/PKG-INFO` & `sysmon_pytk-0.5.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysmon_pytk
-Version: 0.5.0
+Version: 0.5.1
 Summary: System monitor app using Tkinter
 Author-email: Stacey Adams <stacey.belle.rose@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Stacey Adams
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,172 +22,123 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/staceybellerose/sysmon-pytk
+Project-URL: Documentation, https://staceybellerose.github.io/sysmon-pytk/
 Project-URL: Repository, https://github.com/staceybellerose/sysmon-pytk
 Project-URL: Issues, https://github.com/staceybellerose/sysmon-pytk/issues
 Keywords: system monitor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: blessings>=1.7
 Requires-Dist: darkdetect==0.8.0
 Requires-Dist: platformdirs>=4.2
 Requires-Dist: psutil<6.0,>=5.8.0
 Requires-Dist: typing-extensions>=4.10
-Provides-Extra: dev
-Requires-Dist: bandit>=1.7.7; extra == "dev"
-Requires-Dist: build>=1.1.1; extra == "dev"
-Requires-Dist: coloredlogs>=15; extra == "dev"
-Requires-Dist: liccheck>=0.9.2; extra == "dev"
-Requires-Dist: mypy>=1.5; extra == "dev"
-Requires-Dist: pycodestyle>=2.11; extra == "dev"
-Requires-Dist: pydocstyle>=6.2; extra == "dev"
-Requires-Dist: pyflakes>=3.1; extra == "dev"
-Requires-Dist: pylint>=3.0; extra == "dev"
-Requires-Dist: pyroma>=4.2; extra == "dev"
-Requires-Dist: radon>=6.0; extra == "dev"
-Requires-Dist: redbaron>=0.9.2; extra == "dev"
-Requires-Dist: reuse>=3.0; extra == "dev"
-Requires-Dist: ruff>=0.3; extra == "dev"
-Requires-Dist: setuptools>=64; extra == "dev"
-Requires-Dist: twine>=5.0; extra == "dev"
-Requires-Dist: types-docutils>=0.20; extra == "dev"
-Requires-Dist: types-psutil<6.0,>=5.8.0; extra == "dev"
-Requires-Dist: types-setuptools>=64; extra == "dev"
 
 # System Monitor for Python/Tk
 
 <!--
 SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 
 SPDX-License-Identifier: MIT
 -->
+<!-- markdownlint-disable MD033 -->
+
+[![GitHub License](https://img.shields.io/github/license/staceybellerose/sysmon-pytk?color=7C4DFF)](https://github.com/staceybellerose/sysmon-pytk)
+[![GitHub Release](https://img.shields.io/github/v/release/staceybellerose/sysmon-pytk)](https://github.com/staceybellerose/sysmon-pytk/releases)
+[![AppVeyor Build](https://img.shields.io/appveyor/build/staceybellerose/sysmon-pytk/main)](https://ci.appveyor.com/project/staceybellerose/sysmon-pytk/)
+
+[![PyPI - Status](https://img.shields.io/pypi/status/sysmon-pytk)](https://pypi.org/project/sysmon-pytk/)
+[![PyPI - Version](https://img.shields.io/pypi/v/sysmon-pytk)](https://pypi.org/project/sysmon-pytk/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sysmon-pytk)](https://pypi.org/project/sysmon-pytk/)
 
-![GitHub License](https://img.shields.io/github/license/staceybellerose/sysmon-pytk?color=7C4DFF)
-![GitHub Release](https://img.shields.io/github/v/release/staceybellerose/sysmon-pytk)
 [![REUSE status](https://api.reuse.software/badge/github.com/staceybellerose/sysmon-pytk)](https://api.reuse.software/info/github.com/staceybellerose/sysmon-pytk)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/staceybellerose/sysmon-pytk?logo=codefactor)](https://www.codefactor.io/repository/github/staceybellerose/sysmon-pytk)
 [![Maintainability](https://api.codeclimate.com/v1/badges/556c93bf800d0d58e7e4/maintainability)](https://codeclimate.com/github/staceybellerose/sysmon-pytk/maintainability)
 
 System monitor written in Python using Tk. It monitors CPU usage and
 temperature, RAM usage, and disk usage of the primary disk (containing the
 root partition). It also displays the system's hostname, IP address, uptime,
 and current process count.
 
 ![Main Window](images/main_window.png)
 
 ## Pre-installation
 
-### Make sure the Python interface to Tcl/Tk (tkinter) is installed
-
-Since this is a GUI application using tkinter, tkinter must be installed
-separately.
-
-* Debian, Ubuntu, and derivatives
-
-    ```bash
-    sudo apt install python3-tk
-    ```
-
-* Fedora and derivatives
-
-    ```bash
-    sudo dnf install python3-tkinter
-    ```
-
-* MacOS
+Make sure the Python interface to Tcl/Tk (tkinter) is installed.
 
-    ```bash
-    brew install python-tk
-    ```
+[tkinter Installation Instructions](https://github.com/staceybellerose/sysmon-pytk/blob/main/docs/PRE-INSTALLATION.md)
 
 ## Install Using pip
 
-Download the wheel file from the latest release, then install it. Once a PyPI
-account can be set up, the program will be downloadable from there.
-
 ```bash
-pip install ./sysmon_pytk-0.4.1-py3-none-any.whl
+pip install sysmon-pytk
 ```
 
 Two versions of the program will be installed, a GUI program and a command line
 program.
 
-To run the GUI program:
+## Run the GUI program
 
 ```bash
 sysmon
 ```
 
-To run the command line program:
-
-```bash
-cli_sysmon
-```
-
-## Install Manually, for local development
-
-Note when cloning this repo that it has a submodule
-[Azure ttk theme](https://github.com/rdbende/Azure-ttk-theme)
-which must be copied over:
+or
 
 ```bash
-git clone --recurse-submodules https://github.com/staceybellerose/sysmon-pytk.git
+gui_sysmon
 ```
 
-If you didn't clone the submodule when cloning this repo, run this to update:
+## Run the command line program
 
 ```bash
-git submodule update --init --recursive
-```
-
-### Install the required python packages
-
-```bash
-make venv
-```
-
-### Generate translation files
-
-Translations are available in English, Spanish, German, and Norwegian Bokmål.
-To build the translation files, run the following bash commands:
-
-```bash
-make translations
+cli_sysmon
 ```
 
-| Run the GUI program | |
-|-|-|
-| While the venv is activated | `python -m sysmon_pytk.gui_monitor &` |
-| Explicitly using the venv | `venv/bin/python -m sysmon_pytk.gui_monitor &` |
-| Let make handle everything automatically | `make run` |
-
-| Run the command line program | |
-|-|-|
-| While the venv is activated | `python -m sysmon_pytk.cli_monitor &` |
-| Explicitly using the venv | `venv/bin/python -m sysmon_pytk.cli_monitor &` |
-| Let make handle everything automatically | `make cli` |
+To get available options for the command line program, use `cli_sysmon -h`.
 
 ## Translations
 
 Special thanks to our translators!
 
 | Language         | Code  | Translator |
 |------------------|-------|------------|
-| German           | de    | Alisyn Arness |
-| Spanish          | es    | Stacey Adams (author) |
+| German           | de    | Alisyn Arness, [Rainer Schwarzbach](https://github.com/blackstream-x) |
+| Spanish          | es    | Stacey Adams (author), [Félix Medrano](https://github.com/robertxgray) |
 | Norwegian Bokmål | nb_NO | [Allan Nordhøy](https://github.com/comradekingu) |
+
+## Contributing
+
+Translations are always welcome! The strings to be translated are located in
+[app.pot](https://github.com/staceybellerose/sysmon-pytk/blob/main/sysmon_pytk/locale/app.pot)
+and
+[argparse.pot](https://github.com/staceybellerose/sysmon-pytk/blob/main/sysmon_pytk/locale/argparse.pot).
+
+`argparse.pot` contains standard strings from the Python Standard Library file
+`argparse.py` (Python versions 3.9–3.12).
+
+If you want to work on the code, read the
+[Development Guide](https://github.com/staceybellerose/sysmon-pytk/blob/main/docs/DEVELOPING.md).
+Also, check out the [API Documentation](https://staceybellerose.github.io/sysmon-pytk/).
+
+Contributers are expected to follow our
+[Code of Conduct](https://github.com/staceybellerose/sysmon-pytk/blob/main/CODE_OF_CONDUCT.md).
```

### Comparing `sysmon_pytk-0.5.0/azure/LICENSE` & `sysmon_pytk-0.5.1/azure/LICENSE`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/azure.tcl` & `sysmon_pytk-0.5.1/azure/azure.tcl`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/off-basic.png` & `sysmon_pytk-0.5.1/azure/theme/dark/off-basic.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/on-accent.png` & `sysmon_pytk-0.5.1/azure/theme/dark/on-accent.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/on-basic.png` & `sysmon_pytk-0.5.1/azure/theme/dark/on-basic.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/outline-basic.png` & `sysmon_pytk-0.5.1/azure/theme/dark/outline-basic.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/outline-hover.png` & `sysmon_pytk-0.5.1/azure/theme/dark/outline-hover.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/radio-accent.png` & `sysmon_pytk-0.5.1/azure/theme/dark/radio-accent.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/radio-basic.png` & `sysmon_pytk-0.5.1/azure/theme/dark/radio-basic.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/radio-hover.png` & `sysmon_pytk-0.5.1/azure/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark/radio-tri-accent.png` & `sysmon_pytk-0.5.1/azure/theme/dark/radio-tri-accent.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/dark.tcl` & `sysmon_pytk-0.5.1/azure/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/off-basic.png` & `sysmon_pytk-0.5.1/azure/theme/light/off-basic.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/off-hover.png` & `sysmon_pytk-0.5.1/azure/theme/light/off-hover.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/on-accent.png` & `sysmon_pytk-0.5.1/azure/theme/light/on-accent.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/on-basic.png` & `sysmon_pytk-0.5.1/azure/theme/light/on-basic.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/on-hover.png` & `sysmon_pytk-0.5.1/azure/theme/light/on-hover.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/outline-hover.png` & `sysmon_pytk-0.5.1/azure/theme/light/outline-hover.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/radio-accent.png` & `sysmon_pytk-0.5.1/azure/theme/light/radio-accent.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light/radio-hover.png` & `sysmon_pytk-0.5.1/azure/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/azure/theme/light.tcl` & `sysmon_pytk-0.5.1/azure/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/pyproject.toml` & `sysmon_pytk-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -22,26 +22,31 @@
     "Intended Audience :: System Administrators",
     "Environment :: Console",
     "Environment :: X11 Applications",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 keywords = ["system monitor"]
 
 [project.scripts]
-cli_sysmon = "sysmon_pytk.cli_monitor:cli_monitor"
+cli_sysmon = "sysmon_pytk.cli_sysmon:monitor"
 
 [project.gui-scripts]
-sysmon = "sysmon_pytk.gui_monitor:gui_monitor"
+gui_sysmon = "sysmon_pytk.gui_sysmon:monitor"
+sysmon = "sysmon_pytk.gui_sysmon:monitor"
 
 [project.urls]
 Homepage = "https://github.com/staceybellerose/sysmon-pytk"
+Documentation = "https://staceybellerose.github.io/sysmon-pytk/"
 Repository = "https://github.com/staceybellerose/sysmon-pytk"
 Issues = "https://github.com/staceybellerose/sysmon-pytk/issues"
 
 [tool.setuptools.packages.find]
 include = ["sysmon_pytk*", "azure*"]
 
 [tool.setuptools.package-data]
@@ -51,15 +56,14 @@
 
 [tool.setuptools.exclude-package-data]
 "sysmon_pytk.azure" = ["*screenshot.png"]
 
 [tool.setuptools.dynamic]
 version = {attr = "sysmon_pytk.about.__version__"}
 dependencies = {file = ["requirements.txt"]}
-optional-dependencies = {dev = {file = ["requirements-dev.txt"]}}
 
 [tool.ruff]
 line-length = 99
 
 [tool.ruff.lint]
 select = ["ALL"]
 extend-select = ["ANN401"]
```

### Comparing `sysmon_pytk-0.5.0/setup.cfg` & `sysmon_pytk-0.5.1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 
 [isort]
 line_length = 99
 wrap_length = 99
 multi_line_output = 3
 ensure_newline_before_comments = True
 atomic = True
+include_trailing_comma = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/_common.py` & `sysmon_pytk-0.5.1/sysmon_pytk/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,24 @@
 import subprocess  # nosec B404
 import time
 from socket import AF_INET
 
 import psutil
 
 DISK_ALERT_LEVEL = 80
+"""Percent of disk usage at which the meter shows red."""
+
 DISK_WARN_LEVEL = 60
-REFRESH_INTERVAL = 750  # milliseconds
+"""Percent of disk usage at which the meter shows yellow."""
+
+REFRESH_INTERVAL = 750
+"""Number of milliseconds between widget refreshes."""
+
 INTERNAL_PAD = 12
+"""Standard widget padding, in pixels."""
 
 BYTE_SYMBOLS = ("B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB", "YiB")
 
 # SPDX-SnippetBegin
 # SPDX-SnippetName bytes2human function
 # http://code.google.com/p/pyftpdlib/source/browse/trunk/test/bench.py
 # SPDX-FileCopyrightText: © 2007-2013 Giampaolo Rodola' <g.rodola@gmail.com>
@@ -113,15 +120,15 @@
     [13, 22, 585, 588, 1996]
     """
     return [int(s) for s in re.findall(r"\d+", numstr)]
 
 
 def cpu_temp() -> float:
     """
-    Return the CPU temperature, as a float.
+    Return the CPU temperature in degrees Celsius.
 
     Returns
     -------
     float
         The current CPU temperature.
 
     Examples
@@ -132,15 +139,15 @@
     temps = psutil.sensors_temperatures()
     key = "coretemp" if "coretemp" in temps else next(iter(temps))
     return temps[key][0].current
 
 
 def net_addr() -> str:
     """
-    Get the first non-loopback network address.
+    Get the first non-loopback network address (IPv4).
 
     Returns
     -------
     str
         The discovered network address.
     """
     addresses = psutil.net_if_addrs()
@@ -212,15 +219,15 @@
     if digits(total_fmt)[0] < 10:  # noqa: PLR2004
         total_fmt = bytes2human(diskinfo.total)
     return f"{used_fmt}/{total_fmt} {round(diskinfo.percent)}%"
 
 
 def get_processor_name() -> str:
     """
-    Get the full processor name of the computer running.
+    Get the full processor name of the computer.
     """
     if platform.system() == "Windows":
         return _get_processor_name_windows()
     if platform.system() == "Darwin":
         return _get_processor_name_darwin()
     if platform.system() == "Linux":
         return _get_processor_name_linux()
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/about.py` & `sysmon_pytk-0.5.1/sysmon_pytk/about.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 
 """
-Metadata about the application.
+Metadata about the application (name, version, author, license, etc.).
 """
 
 from .app_locale import get_translator
 
 _ = get_translator()
 
 __app_name__ = "sysmon-pytk"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 __license__ = _("MIT License")
-__author__ = "Stacey Adams"
+__author_name__ = "Stacey Adams"
 __author_email__ = "stacey.belle.rose@gmail.com"
 __url__ = "https://github.com/staceybellerose/sysmon-pytk"
 __summary__ = _("""\
 sysmon-pytk is a system monitor. It monitors CPU usage and temperature, \
 RAM usage, and disk usage of the primary disk (containing the root \
 partition). It also displays the system's hostname, IP address, uptime, \
 and current process count.""")
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/app_locale.py` & `sysmon_pytk-0.5.1/sysmon_pytk/app_locale.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,25 +21,45 @@
 
 LANGUAGES = {
     "English": "en",
     "Español": "es",
     "Deutsch": "de",
     "Norsk Bokmål": "nb_NO"
 }
+"""The list of language translations available."""
 
 __i18n_domain__ = "app"
 
 TRANSLATED_MODULES: list = []
+"""
+List of modules which have requested translated strings.
+
+When the translation is changed, these modules will be reloaded.
+"""
 
 
 def get_translator(
     *, forced_lang: str | None = None, domain: str = __i18n_domain__
 ) -> GettextCallable:
     """
     Load the selected translation.
+
+    Parameters
+    ----------
+    forced_lang : str, optional
+        The language to force-load. If not set, read the language from Settings
+        and load that one.
+    domain : str, optional
+        The gettext domain to use. Default is set by `__i18n_domain__`. Useful
+        for loading translation files for other modules, such as `argparse.py`.
+
+    Returns
+    -------
+    GettextCallable
+        a Callable with the signature: func(message: str) -> str:
     """
     current_lang = forced_lang if forced_lang else _get_lang_from_config()
     frm = inspect.stack()[1]  # get caller
     mod = inspect.getmodule(frm.frame)
     if mod not in TRANSLATED_MODULES:
         TRANSLATED_MODULES.append(mod)
         TRANSLATED_MODULES.sort(key=lambda x: x.__name__)
@@ -49,14 +69,16 @@
     )
     return translation.gettext
 
 
 def reload_translated_modules() -> None:
     """
     Reload any modules that have requested translations.
+
+    This should be called when the user selects a new translation.
     """
     for mod in TRANSLATED_MODULES:
         importlib.reload(mod)
 
 
 def _get_lang_from_config() -> str:
     current_lang = "en"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/application.py` & `sysmon_pytk-0.5.1/sysmon_pytk/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 
 """
-System monitor.
+System monitor application.
 """
 
 from __future__ import annotations
 
 import sys
 import tkinter as tk
 from socket import gethostname
@@ -14,33 +14,35 @@
 from typing import TYPE_CHECKING
 
 import psutil
 
 from . import _common, about
 from .app_locale import get_translator, reload_translated_modules
 from .file_utils import get_full_path, settings_path
-from .modals import SettingsDialog
-from .modals.about_modal import AboutDialog, AboutMetadata, LicenseMetadata
+from .modals import AboutDialog, AboutMetadata, LicenseMetadata, SettingsDialog
 from .settings import Settings
 from .style_manager import StyleManager
 from .widgets import TempToolTip, ToolTip
 from .widgets.meters import CpuMeter, DiskMeter, RamMeter, TempMeter
 
 if TYPE_CHECKING:
-    from tkinter import Variable
+    from tkinter import Event, Variable
 
 _ = get_translator()
 
 APP_TITLE = _("System Monitor")
+"""Application title, which appears in window title bars."""
 
 
 class Application(tk.Tk):
     """
     System monitor application.
 
+    Toplevel widget of Tk which represents the main window of the application.
+
     Attributes
     ----------
     _name : StringVar
         The hostname of the system.
     _ip_addr : StringVar
         The IP Address of the system.
     _uptime : StringVar
@@ -50,14 +52,15 @@
     _update_job : str
         The ID of the scheduled job to update the screen.
     _menu_icons : dict[str, PhotoImage]
         The icons used in the menu.
     """
 
     def __init__(self) -> None:
+        """Return a new Toplevel Tk widget."""
         super().__init__()
         self.title(APP_TITLE)
         self.iconphoto(False, tk.PhotoImage(file=get_full_path("images/icon.png")))
         self.read_settings()
         self._name = tk.StringVar()
         self._ip_addr = tk.StringVar()
         self._uptime = tk.StringVar()
@@ -70,15 +73,18 @@
         self.bind_events()
         self.update()
         self.minsize(self.winfo_width(), self.winfo_height())
         self.update_screen()
 
     def read_settings(self, *_args) -> None:
         """
-        Read application settings from configuration file.
+        Read and process application settings from configuration file.
+
+        This method is triggered on a `<<SettingsChanged>>` event, and is part
+        of the application startup program flow.
         """
         self.settings = Settings(settings_path())
         self.call("wm", "attributes", ".", "-topmost", f"{self.settings.always_on_top}")
 
     def create_widgets(self) -> None:
         """
         Create the widgets to be displayed in the main application window.
@@ -88,15 +94,15 @@
         for row in [1, 2]:
             frame.rowconfigure(row, weight=1)
         for column in [1, 2, 3, 4]:
             frame.columnconfigure(column, weight=1)
         self._add_variable_label(frame, self._name, 1, 1)
         ip_label = self._add_variable_label(frame, self._ip_addr, 1, 2)
         ToolTip(ip_label, _("Click to copy IP Address to clipboard"))
-        ip_label.bind("<Button-1>", self._on_click_ip_address)
+        ip_label.bind("<Button-1>", self.on_click_ip_address)
         self._add_variable_label(frame, self._processes, 1, 3)
         self._add_variable_label(frame, self._uptime, 1, 4)
         self._add_meters(frame)
         self._add_sizegrip(frame)
 
     @classmethod
     def _add_variable_label(
@@ -138,15 +144,15 @@
             "preferences": tk.PhotoImage(file=get_full_path("images/preferences-system.png")),
             "restart": tk.PhotoImage(file=get_full_path("images/view-refresh.png")),
             "quit": tk.PhotoImage(file=get_full_path("images/blank.png"))
         }
 
     def build_menu(self) -> None:
         """
-        Build the application menu.
+        Build the application menu and bind associated keypress events to functions.
         """
         top = self.winfo_toplevel()
         top.rowconfigure(0, weight=1)
         top.columnconfigure(0, weight=1)
         menu_bar = tk.Menu(
             top, relief=tk.FLAT, activeborderwidth=0,
             font=font.nametofont("TkMenuFont"),
@@ -160,90 +166,104 @@
             foreground=StyleManager.get_menu_foreground()
         )
 
         menu_bar.add_cascade(
             label=_("File"), menu=file_menu,
         )
         file_menu.add_command(
-            label=_("About"), accelerator=_("Ctrl+A"), command=self._on_about,
+            label=_("About"), accelerator=_("Ctrl+A"), command=self.on_about,
             compound=tk.LEFT, image=self._menu_icons["about"]
         )
         file_menu.add_command(
-            label=_("Preferences"), accelerator=_("Ctrl+Shift+P"), command=self._on_settings,
+            label=_("Preferences"), accelerator=_("Ctrl+Shift+P"), command=self.on_settings,
             compound=tk.LEFT, image=self._menu_icons["preferences"]
         )
         file_menu.add_command(
-            label=_("Restart"), accelerator=_("Ctrl+R"), command=self._on_restart,
+            label=_("Restart"), accelerator=_("Ctrl+R"), command=self.on_restart,
             compound=tk.LEFT, image=self._menu_icons["restart"]
         )
         file_menu.add_separator()
         file_menu.add_command(
             label=_("Quit"), accelerator=_("Ctrl+Q"), command=lambda: sys.exit(0),
             compound=tk.LEFT, image=self._menu_icons["quit"]
         )
         top["menu"] = menu_bar
         # bind keypress events for menu here
-        self.bind("<Control-KeyPress-a>", self._on_about)
-        self.bind("<Control-Shift-KeyPress-P>", self._on_settings)
-        self.bind("<Control-KeyPress-r>", self._on_restart)
+        self.bind("<Control-KeyPress-a>", self.on_about)
+        self.bind("<Control-Shift-KeyPress-P>", self.on_settings)
+        self.bind("<Control-KeyPress-r>", self.on_restart)
         self.bind("<Control-KeyPress-q>", lambda _x: sys.exit(0))
 
     def bind_events(self) -> None:
         """
-        Set up bindings for app events.
+        Set up bindings for custom application events.
         """
         self.bind("<<SettingsChanged>>", self.read_settings)
-        self.bind("<<LanguageChanged>>", self._on_language)
-        self.bind("<<FontChanged>>", self._on_restart)
+        self.bind("<<LanguageChanged>>", self.on_language)
+        self.bind("<<FontChanged>>", self.on_restart)
 
-    def _on_click_ip_address(self, event: tk.Event) -> None:
+    def on_click_ip_address(self, event: Event) -> None:
+        """
+        Copy the IP address to the clipboard.
+        """
         self.clipboard_clear()
         self.clipboard_append(_common.net_addr())
         TempToolTip(self, _("Copied!"), (event.x_root, event.y_root), 5000)
 
-    def _on_language(self, *_args) -> None:
+    def on_language(self, *_args) -> None:
         """
-        Update the selected language.
+        Update the selected translation after the user selects a new language.
+
+        This method is triggered on a `<<LanguageChanged>>` event.
         """
         reload_translated_modules()
-        self._on_restart()
+        self.on_restart()
 
-    def _on_about(self, *_args) -> None:
+    def on_about(self, *_args) -> None:
         """
-        Open About box.
+        Open the About modal dialog box.
         """
         metadata = AboutMetadata(
-            about.__app_name__, about.__version__, about.__author__,
+            about.__app_name__, about.__version__, about.__author_name__,
             about.__copyright_year__, about.__summary__, about.__url__,
             LicenseMetadata(
                 about.__full_license__, about.__license__, about.__license_url__
             )
         )
         AboutDialog(self, metadata, iconpath=get_full_path("images/icon.png"))
 
-    def _on_restart(self, *_args) -> None:
+    def on_restart(self, *_args) -> None:
+        """
+        Restart the application.
+
+        This method is triggered on a `<<FontChanged>>` event, and is part of
+        the program flow for `<<LanguageChanged>>` event processing.
+        """
         if self._update_job is not None:
             self.after_cancel(self._update_job)
             self._update_job = None
         self.destroy()
         self.__init__()  # type: ignore[misc] # pylint: disable=unnecessary-dunder-call
 
-    def _on_settings(self, *_args) -> None:
+    def on_settings(self, *_args) -> None:
         """
-        Open Settings and process any changes afterward.
+        Open the Settings modal dialog and process any changes afterward.
         """
         SettingsDialog(
             self.settings, self, _("{} Preferences").format(APP_TITLE),
             iconpath=get_full_path("images/icon.png")
         )
         StyleManager.update_by_dark_mode(self, self.settings)
 
     def update_screen(self) -> None:
         """
-        Update the screen.
+        Periodically update the screen to refresh the displayed data.
+
+        This method reschedules itself after `sysmon_pytk._common.REFRESH_INTERVAL`
+        milliseconds.
         """
         self._name.set(_("Hostname: {}").format(gethostname()))
         self._ip_addr.set(_("IP Address: {}").format(_common.net_addr()))
         self._processes.set(_("Processes: {}").format(len(psutil.pids())))
         self._uptime.set(_("Uptime: {}").format(_common.system_uptime()))
         self._update_job = self.after(
             _common.REFRESH_INTERVAL, self.update_screen
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/cli_monitor.py` & `sysmon_pytk-0.5.1/sysmon_pytk/cli_sysmon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 
 """
 Command line system monitor.
+
+.. include:: ../docs/CLI_USAGE.md
 """
 
 import gettext
 import sys
 import time
 from socket import gethostname
 from typing import NoReturn
@@ -143,15 +145,15 @@
                 current=entry.current, high=entry.high, critical=entry.critical
             )
             print(term.move(line, 0) + " "*10 + tag + display + term.el)
             line += 1
     print(term.clear_eos)
 
 
-def blank_below_line(line: int, start_col: int, width: int) -> None:
+def _blank_below_line(line: int, start_col: int, width: int) -> None:
     """
     Blank a rectangular section of the screen with spaces.
     """
     for row in range(line, term.height-1):
         print(term.move(row, start_col) + " "*width)
 
 
@@ -165,15 +167,15 @@
     for idx, part in enumerate(partitions):
         line = 2*idx + starting_line + 1
         if line + 1 > term.height:
             break
         mountpoint = part.mountpoint
         print(term.move(line, 1) + mountpoint.ljust(allowed_width))
         print(term.move(line + 1, 1) + _disk_usage_rjust(mountpoint, allowed_width))
-    blank_below_line(2*len(partitions) + starting_line + 1, 1, allowed_width)
+    _blank_below_line(2*len(partitions) + starting_line + 1, 1, allowed_width)
 
 
 def _temp_details_half(*, starting_line: int) -> None:
     start_col = term.width//2 + 1
     print(
         term.move(starting_line, start_col) + term.black_on_bright_white
         + _("Temperature Sensors").upper() + term.normal
@@ -189,18 +191,18 @@
             label_width = term.width//2 - 7
             print(
                 term.move(line, start_col) + " "*5
                 + (entry.label or name).ljust(label_width)[:label_width]
             )
             print(term.move(line, term.width-11) + f"{entry.current}°C".rjust(10))
             line += 1
-    blank_below_line(line, start_col, term.width-start_col)
+    _blank_below_line(line, start_col, term.width-start_col)
 
 
-def monitor_system(args: argparse.Namespace) -> NoReturn:
+def _monitor_system(args: argparse.Namespace) -> NoReturn:
     """
     Monitor the system usage.
     """
     app_title = _("System Monitor").upper()
     while True:
         print(term.move(0, 1) + term.black_on_bright_white + app_title + term.normal)
         print(term.move(1, 1) + _("Hostname: {}").format(gethostname()) + term.el)
@@ -275,24 +277,24 @@
         "-x", "--no-details", action="store_const", dest="details", const="",
         help=_("show no details, only the header")
     )
     parser.set_defaults(details="d")
     return parser.parse_args()
 
 
-def cli_monitor() -> NoReturn:
+def monitor() -> NoReturn:
     """
     Entry point for CLI monitor.
     """
     args = _get_parser()
     global _  # noqa: PLW0603 # pylint: disable=global-statement
     _ = get_translator(forced_lang=args.language)
     print(term.enter_fullscreen() + term.clear + term.civis)
     try:
-        monitor_system(args)
+        _monitor_system(args)
     except KeyboardInterrupt:
         print(term.cnorm + term.clear + term.exit_fullscreen())
         sys.exit(0)
 
 
 if __name__ == "__main__":
-    cli_monitor()
+    monitor()
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/desktop_menu.py` & `sysmon_pytk-0.5.1/sysmon_pytk/desktop_menu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-FileCopyrightText: © 2017-2024 Akuli
 # SPDX-FileCopyrightText: © 2024 Stacey Adams
 # SPDX-License-Identifier: MIT
 
 """
 Installs an entry in the desktop menu system.
 
-You can enable it in Settings.
-This plugin doesn't do anything on Windows or MacOS.
+You can enable it in Settings. This only works in Linux/X11.
 
 Originally from https://github.com/Akuli/porcupine/blob/main/porcupine/plugins/desktop_menu.py
 """
 
 from __future__ import annotations
 
 import os
@@ -27,25 +26,35 @@
 from .modals import messagebox
 
 if TYPE_CHECKING:
     from tkinter import Tk, Toplevel
 
 _ = get_translator()
 
-setup_after = ["filetypes"]  # To group the checkbutton on the bottom
-
 XDG_DESKTOP_MENU = "xdg-desktop-menu"
+"""Program to execute to create/remove the desktop menu entry."""
+
 DESKTOP_FILE_NAME = "sysmon.desktop"
+"""Filename of the desktop menu entry to create."""
+
 EXECUTABLE = "sysmon"
+"""Executable to run fro the desktop menu entry."""
 
 
 def install_desktop_file(parent: Tk | Toplevel) -> bool:
     """
-    Install a desktop menu file.
+    Install a desktop menu entry on Linux/X11.
+
+    Parameters
+    ----------
+    parent : Tk | Toplevel
+        The parent window that is calling this function. Needed for error reporting.
     """
+    if parent.tk.call("tk", "windowingsystem") != "x11":
+        return False
     location = shutil.which(EXECUTABLE)
     if location is None:
         messagebox.show_error(
             parent, _("Error creating desktop menu item"),
             _("System Monitor (sysmon) must be installed in a virtual "
                 "environment in order to create a desktop menu entry.")
         )
@@ -82,12 +91,12 @@
     )  # nosec B603
     launcher_path.unlink()
     return True
 
 
 def uninstall_desktop_file() -> None:
     """
-    Uninstall the desktop menu file.
+    Uninstall the desktop menu entry that was previously installed.
     """
     subprocess.call(
         [XDG_DESKTOP_MENU, "uninstall", "--mode", "user", DESKTOP_FILE_NAME]
     )  # nosec B603
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/file_utils.py` & `sysmon_pytk-0.5.1/sysmon_pytk/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 """
 File utility functions.
 """
 
 import inspect
 import sys
-from distutils.sysconfig import get_python_lib
+from distutils.sysconfig import get_python_lib  # pylint: disable=W4901
 from pathlib import Path
 
 import platformdirs
 
 SETTINGS_FILE = "sysmon.ini"
+"""The settings file used by the application."""
 
 
 def get_full_path(relative_path: str) -> str:
     """
     Get the full path of a file, based on its relative path to this project.
     """
     std_lib = Path(get_python_lib())
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-error.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-error.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-information.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-information.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-question.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-question.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/custom/dialog-warning.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/custom/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/edit-copy.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/edit-copy.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/edit-cut.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/edit-cut.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/edit-paste.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/edit-paste.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/edit-select-all.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/edit-select-all.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/icon-lg.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/icon-lg.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/icon.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/icon.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/preferences-system.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/preferences-system.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/images/view-refresh.png` & `sysmon_pytk-0.5.1/sysmon_pytk/images/view-refresh.png`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/app.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/app.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: sysmon-pytk 0.4.1\n"
+"Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-30 19:01-0500\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
 "Last-Translator: Alisyn Arness\n"
 "Language-Team: German <https://hosted.weblate.org/projects/sysmon-pytk/"
 "sysmon-pytk/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -51,36 +51,26 @@
 
 msgid "Cancel"
 msgstr "Abbrechen"
 
 msgid "Choose Font"
 msgstr "Schriftart wählen"
 
-msgid "Click for detailed memory statistics"
-msgstr "Klicken Sie hier, um detaillierte RAM-Statistiken anzuzeigen"
-
-msgid "Click for detailed temperature readings"
-msgstr "Klicken Sie hier, um detaillierte Temperaturmessungen anzuzeigen"
-
-msgid "Click for per-CPU usage"
-msgstr "Klicken Sie hier, um die Nutzung pro CPU anzuzeigen"
-
-msgid "Click for usage details of each mount point"
-msgstr ""
-"Klicken Sie hier, um Nutzungsinformationen für jeden Mountpunkt anzuzeigen"
-
 msgid "Click to copy IP Address to clipboard"
 msgstr "Klicken Sie hier, um die IP-Adresse in die Zwischenablage zu kopieren"
 
 msgid "Close"
 msgstr "Schließen"
 
 msgid "Copied!"
 msgstr "Kopiert!"
 
+msgid "Copy"
+msgstr "Kopieren"
+
 msgid "Ctrl+A"
 msgstr "Strg+A"
 
 msgid "Ctrl+C"
 msgstr "Strg+C"
 
 msgid "Ctrl+Q"
@@ -94,23 +84,23 @@
 
 msgid "Ctrl+V"
 msgstr "Strg+V"
 
 msgid "Ctrl+X"
 msgstr "Strg+X"
 
+msgid "Cut"
+msgstr "Ausschneiden"
+
 msgid "Dark"
 msgstr "Dunkel"
 
 msgid "Disk Usage"
 msgstr "Plattenauslastung"
 
-msgid "Disk Usage: /"
-msgstr "Plattenauslastung: /"
-
 msgid "Display Details"
 msgstr "Anzeigedetails"
 
 msgid "Effects"
 msgstr "Effekte"
 
 msgid "Error creating desktop menu item"
@@ -148,26 +138,26 @@
 
 msgid "Memory Statistics"
 msgstr "Speicherstatistik"
 
 msgid "Monospace Font"
 msgstr "Dicktengleiche Schrift"
 
-msgid "No"
-msgstr "Nein"
-
 msgid "OK"
 msgstr "Verstanden"
 
 msgid "Options"
 msgstr "Optionen"
 
 msgid "Overstrike"
 msgstr "Durchgestrichen"
 
+msgid "Paste"
+msgstr "Einfügen"
+
 msgid "Preferences"
 msgstr "Einstellungen"
 
 msgid "Preview"
 msgstr "Vorschau"
 
 msgid "Processes: {}"
@@ -184,20 +174,20 @@
 
 msgid "Regular Font"
 msgstr "Normal Schriftart"
 
 msgid "Restart"
 msgstr "Neustart"
 
-msgid "Retry"
-msgstr "Wiederholen"
-
 msgid "Same as System"
 msgstr "Gleiches wie System"
 
+msgid "Select All"
+msgstr "Alles auswählen"
+
 msgid "Select a font"
 msgstr "Schriftart auswählen"
 
 msgid "Size"
 msgstr "Größe"
 
 msgid "Source Code"
@@ -244,17 +234,14 @@
 
 msgid "Version {}"
 msgstr "Version {}"
 
 msgid "Virtual Memory"
 msgstr "Virtueller Speicher"
 
-msgid "Yes"
-msgstr "Ja"
-
 msgid "per-core CPU Frequency (in MHz)"
 msgstr "CPU-Frequenz pro Kern (in MHz)"
 
 msgid "per-core CPU Usage"
 msgstr "CPU-Auslastung pro Kern"
 
 msgid "show both disk and temperature details"
@@ -293,21 +280,9 @@
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
 msgstr ""
 "Zeit zwischen Bildschirmaktualisierungen (in Sekunden, Standard=%(default)s)"
 
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
 msgstr "{current}°C (höchste = {high}°C, kritischer = {critical}°C)"
 
-msgid "{} :: CPU Details"
-msgstr "{} :: CPU-Details"
-
-msgid "{} :: Disk Usage"
-msgstr "{} :: Plattenauslastung"
-
-msgid "{} :: Memory Usage"
-msgstr "{} :: RAM-Auslastung"
-
-msgid "{} :: Temperature Details"
-msgstr "{} :: Temperaturdetails"
-
 msgid "{} Preferences"
 msgstr "{} Einstellungen"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/app.po` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/app.po`

 * *Files 17% similar despite different names*

```diff
@@ -2,424 +2,416 @@
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"POT-Creation-Date: 2024-03-31 04:00-0500\n"
-"PO-Revision-Date: 2024-03-31 04:00-0500\n"
-"Last-Translator: Alisyn Arness\n"
-"Language-Team: German <https://hosted.weblate.org/projects/sysmon-pytk/"
-"sysmon-pytk/de/>\n"
-"Language: de\n"
+"POT-Creation-Date: 2024-04-11 15:23+0000\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
+"Last-Translator: Stacey Adams <stacey.belle.rose@gmail.com>\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/sysmon-pytk/"
+"sysmon-pytk/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5-dev\n"
 
 #: ../about.py:14
 msgid "MIT License"
-msgstr "MIT Lizenz"
+msgstr "Licencia MIT"
 
 #: ../about.py:18
 msgid ""
 "sysmon-pytk is a system monitor. It monitors CPU usage and temperature, RAM "
 "usage, and disk usage of the primary disk (containing the root partition). "
 "It also displays the system's hostname, IP address, uptime, and current "
 "process count."
 msgstr ""
-"sysmon-pytk ist ein Systemmonitor. Es überwacht die CPU-Nutzung und -"
-"Temperatur, die RAM-Nutzung und die Festplattennutzung der primären "
-"Festplatte (die die Root-Partition enthält). Außerdem werden der Hostname, "
-"die IP-Adresse, die Betriebszeit und die aktuelle Prozessanzahl des Systems "
-"angezeigt."
+"sysmon-pytk es un monitor del sistema. Monitorea el uso y la temperatura de "
+"la CPU, el uso de RAM y el uso del disco primario (que contiene la partición "
+"raíz). También muestra el nombre de host del sistema, la dirección IP, el "
+"tiempo de actividad y el recuento de procesos actuales."
 
-#: ../application.py:33 ../cli_monitor.py:203 ../desktop_menu.py:72
+#: ../application.py:32 ../cli_sysmon.py:205 ../desktop_menu.py:81
 msgid "System Monitor"
-msgstr "Systemmonitor"
+msgstr "Monitoreo del sistema"
 
-#: ../application.py:94
+#: ../application.py:100
 msgid "Click to copy IP Address to clipboard"
-msgstr "Klicken Sie hier, um die IP-Adresse in die Zwischenablage zu kopieren"
+msgstr "Clic para copiar la dirección IP al portapapeles"
 
-#: ../application.py:164
+#: ../application.py:170
 msgid "File"
-msgstr "Datei"
+msgstr "Archivo"
 
-#: ../application.py:167
+#: ../application.py:173
 msgid "About"
-msgstr "Über"
+msgstr "Acerca de"
 
-#: ../application.py:167 ../widgets/edit_menu.py:65
+#: ../application.py:173 ../widgets/edit_menu.py:79
 msgid "Ctrl+A"
-msgstr "Strg+A"
+msgstr "Ctrl+A"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Preferences"
-msgstr "Einstellungen"
+msgstr "Preferencias"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Ctrl+Shift+P"
-msgstr "Strg+Umschalt+P"
+msgstr "Ctrl+Mayús+P"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Restart"
-msgstr "Neustart"
+msgstr "Reiniciar"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Ctrl+R"
-msgstr "Strg+R"
+msgstr "Ctrl+R"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Quit"
-msgstr "Beenden"
+msgstr "Salir"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Ctrl+Q"
-msgstr "Strg-Q"
+msgstr "Ctrl+Q"
 
-#: ../application.py:201
+#: ../application.py:210
 msgid "Copied!"
-msgstr "Kopiert!"
+msgstr "¡Copiado!"
 
-#: ../application.py:235
+#: ../application.py:252
 msgid "{} Preferences"
-msgstr "{} Einstellungen"
+msgstr "{} Preferencias"
 
-#: ../application.py:244 ../cli_monitor.py:206
+#: ../application.py:264 ../cli_sysmon.py:208
 msgid "Hostname: {}"
-msgstr "Hostname : {}"
+msgstr "Nombre del host: {}"
 
-#: ../application.py:245 ../cli_monitor.py:207
+#: ../application.py:265 ../cli_sysmon.py:209
 msgid "IP Address: {}"
-msgstr "IP-Adresse: {}"
+msgstr "Dirección IP: {}"
 
-#: ../application.py:246 ../cli_monitor.py:208
+#: ../application.py:266 ../cli_sysmon.py:210
 msgid "Processes: {}"
-msgstr "Prozesse: {}"
+msgstr "Recuento de procesos: {}"
 
-#: ../application.py:247 ../cli_monitor.py:209
+#: ../application.py:267 ../cli_sysmon.py:211
 msgid "Uptime: {}"
-msgstr "Betriebszeit: {}"
+msgstr "Tiempo de actividad: {}"
 
-#: ../cli_monitor.py:50 ../widgets/meters.py:116
+#: ../cli_sysmon.py:52
 msgid "CPU Usage"
-msgstr "CPU-Auslastung"
+msgstr "Uso de CPU"
 
-#: ../cli_monitor.py:58 ../widgets/meters.py:154
+#: ../cli_sysmon.py:60
 msgid "Temperature"
-msgstr "Temperatur"
+msgstr "Temperatura"
 
-#: ../cli_monitor.py:68 ../widgets/meters.py:187
+#: ../cli_sysmon.py:70
 msgid "RAM Usage"
-msgstr "RAM-Auslastung"
+msgstr "Uso de RAM"
 
-#: ../cli_monitor.py:78 ../modals/mem_usage_modal.py:63
+#: ../cli_sysmon.py:80 ../modals/mem_usage_modal.py:63
 msgid "Swap Memory"
-msgstr "Speicher Austauschen"
+msgstr "memoria de intercambio"
 
-#: ../cli_monitor.py:114 ../cli_monitor.py:162 ../modals/disk_usage_modal.py:59
+#: ../cli_sysmon.py:116 ../cli_sysmon.py:164 ../modals/disk_usage_modal.py:71
 msgid "Disk Usage"
-msgstr "Plattenauslastung"
+msgstr "Uso del disco"
 
-#: ../cli_monitor.py:131 ../cli_monitor.py:179
-#: ../modals/temperature_modal.py:45
+#: ../cli_sysmon.py:133 ../cli_sysmon.py:181 ../modals/temperature_modal.py:45
 msgid "Temperature Sensors"
-msgstr "Wärmesensoren"
+msgstr "Sensores de temperatura"
 
-#: ../cli_monitor.py:142 ../modals/temperature_modal.py:103
+#: ../cli_sysmon.py:144 ../modals/temperature_modal.py:103
 #, python-brace-format
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
-msgstr "{current}°C (höchste = {high}°C, kritischer = {critical}°C)"
+msgstr "{current}°C (alta = {high}°C, critica = {critical}°C)"
 
-#: ../cli_monitor.py:222
+#: ../cli_sysmon.py:224
 msgid "<Ctrl-C> to quit"
-msgstr "<Strg-C> zum Beenden"
+msgstr "<Ctrl-C> para salir"
 
-#: ../cli_monitor.py:232
+#: ../cli_sysmon.py:234
 msgid "System monitor: display CPU usage/temperature, memory usage, disk usage"
 msgstr ""
-"Systemmonitor: Zeigt CPU-Auslastung/-Temperatur, Speichernutzung und "
-"Festplattennutzung an"
+"Monitor del sistema: muestra el uso/temperatura de la CPU, el uso de la "
+"memoria, el uso del disco"
 
-#: ../cli_monitor.py:235
+#: ../cli_sysmon.py:237
 msgid ""
 "By default, this program will use the same language as that selected for the "
 "GUI application. To override it, use the '-l' option. To quit, press <Ctrl-"
 "C>."
 msgstr ""
-"Standardmäßig verwendet dieses Programm dieselbe Sprache wie die für die GUI-"
-"Anwendung ausgewählte Sprache. Um es zu überschreiben, verwenden Sie die "
-"Option „-l“. Zum Beenden drücken Sie <Strg-C>."
+"De forma predeterminada, este programa utilizará el mismo idioma que el "
+"seleccionado para la aplicación GUI. Para anularlo, utilice la opción '-l'. "
+"Para salir, presione <Ctrl-C>."
 
-#: ../cli_monitor.py:242
+#: ../cli_sysmon.py:244
 msgid "Options"
-msgstr "Optionen"
+msgstr "Opciones"
 
-#: ../cli_monitor.py:245
+#: ../cli_sysmon.py:247
 msgid "show this help message and exit"
-msgstr "diese Meldung anzeigen und beenden"
+msgstr "muestra este mensaje de ayuda y termina"
 
-#: ../cli_monitor.py:250
+#: ../cli_sysmon.py:252
 msgid "show program's version number and exit"
-msgstr "Versionsnummer der Anwendung anzeigen und beenden"
+msgstr "mostrar el número de versión del programa y salir"
 
-#: ../cli_monitor.py:254
+#: ../cli_sysmon.py:256
 #, python-format
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
 msgstr ""
-"Zeit zwischen Bildschirmaktualisierungen (in Sekunden, Standard=%(default)s)"
+"tiempo entre actualizaciones de pantalla (en segundos, "
+"predeterminado=%(default)s)"
 
-#: ../cli_monitor.py:258
+#: ../cli_sysmon.py:260
 msgid "the language to use for display"
-msgstr "die Sprache, die für die Anzeige verwendet werden soll"
+msgstr "el idioma a utilizar para la visualización"
 
-#: ../cli_monitor.py:260
+#: ../cli_sysmon.py:262
 msgid "Display Details"
-msgstr "Anzeigedetails"
+msgstr "detalles de la pantalla"
 
-#: ../cli_monitor.py:264
+#: ../cli_sysmon.py:266
 msgid "show disk details (default)"
-msgstr "Festplattendetails anzeigen (Standard)"
+msgstr "mostrar detalles del disco (predeterminado)"
 
-#: ../cli_monitor.py:268
+#: ../cli_sysmon.py:270
 msgid "show temperature details"
-msgstr "Temperaturdetails anzeigen"
+msgstr "mostrar detalles de temperatura"
 
-#: ../cli_monitor.py:272
+#: ../cli_sysmon.py:274
 msgid "show both disk and temperature details"
-msgstr "Zeigt sowohl Festplattendetails als auch Temperaturdetails an"
+msgstr "mostrar detalles del disco y de la temperatura"
 
-#: ../cli_monitor.py:276
+#: ../cli_sysmon.py:278
 msgid "show no details, only the header"
-msgstr "Keine Details anzeigen, nur die Kopfzeile"
+msgstr "no mostrar detalles, solo el encabezado"
 
-#: ../desktop_menu.py:48
+#: ../desktop_menu.py:57
 msgid "Error creating desktop menu item"
-msgstr "Fehler beim Erstellen des Desktop-Menüeinträg"
+msgstr "Error al crear el elemento del menú del escritorio"
 
-#: ../desktop_menu.py:49
+#: ../desktop_menu.py:58
 msgid ""
 "System Monitor (sysmon) must be installed in a virtual environment in order "
 "to create a desktop menu entry."
 msgstr ""
-"System Monitor (sysmon) muss in einer virtuellen Umgebung installiert "
-"werden, um einen Desktop-Menüeintrag zu erstellen."
+"System Monitor (sysmon) debe instalarse en un entorno virtual para poder "
+"crear una entrada de menú en el escritorio."
 
-#: ../font_utils.py:74 ../modals/font_modal.py:171
+#: ../font_utils.py:153 ../modals/font_modal.py:171
 msgid "Bold"
-msgstr "Fett"
+msgstr "Negrita"
 
-#: ../font_utils.py:76 ../modals/font_modal.py:175
+#: ../font_utils.py:155 ../modals/font_modal.py:175
 msgid "Italic"
-msgstr "Kursiv"
+msgstr "Cursiva"
 
-#: ../font_utils.py:78 ../modals/font_modal.py:179
+#: ../font_utils.py:157 ../modals/font_modal.py:179
 msgid "Bold Italic"
-msgstr "Fett Kursiv"
+msgstr "Cursiva negrita"
 
-#: ../modals/about_modal.py:93
+#: ../font_utils.py:171 ../modals/font_modal.py:193
+msgid "Underline"
+msgstr "Subrayada"
+
+#: ../font_utils.py:172 ../modals/font_modal.py:197
+msgid "Overstrike"
+msgstr "Tachado"
+
+#: ../modals/_base_modal.py:158
+msgid "Close"
+msgstr "Cerrar"
+
+#: ../modals/_base_modal.py:168
+msgid "Cancel"
+msgstr "Cancelar"
+
+#: ../modals/_base_modal.py:169
+msgid "OK"
+msgstr "Aceptar"
+
+#: ../modals/about_modal.py:115
 msgid "About {}"
-msgstr "Über {}"
+msgstr "Acerca del {}"
 
-#: ../modals/about_modal.py:125
+#: ../modals/about_modal.py:147
 msgid "Translators"
-msgstr "Übersetzer"
+msgstr "Traductores"
 
-#: ../modals/about_modal.py:131
+#: ../modals/about_modal.py:153
 msgid "License"
-msgstr "Lizenz"
+msgstr "Licencia"
 
-#: ../modals/about_modal.py:149
+#: ../modals/about_modal.py:171
 msgid "Version {}"
-msgstr "Version {}"
+msgstr "Versión {}"
 
-#: ../modals/about_modal.py:155
+#: ../modals/about_modal.py:177
 msgid "Source Code"
-msgstr "Quellcode"
+msgstr "Código fuente"
 
-#: ../modals/about_modal.py:220
+#: ../modals/about_modal.py:242
 msgid "Full license text available here"
-msgstr "Den vollständigen Lizenztext finden Sie hier"
-
-#: ../modals/_base_modal.py:158 ../widgets/button_mixin.py:113
-msgid "Close"
-msgstr "Schließen"
-
-#: ../modals/_base_modal.py:168 ../widgets/button_mixin.py:110
-msgid "Cancel"
-msgstr "Abbrechen"
-
-#: ../modals/_base_modal.py:169 ../widgets/button_mixin.py:107
-msgid "OK"
-msgstr "Verstanden"
+msgstr "Texto completo de la licencia disponible aquí"
 
-#: ../modals/cpu_modal.py:70
+#: ../modals/cpu_modal.py:82
 msgid "per-core CPU Usage"
-msgstr "CPU-Auslastung pro Kern"
+msgstr "uso del CPU por núcleo"
 
-#: ../modals/cpu_modal.py:76
+#: ../modals/cpu_modal.py:88
 msgid "per-core CPU Frequency (in MHz)"
-msgstr "CPU-Frequenz pro Kern (in MHz)"
+msgstr "frecuencia de CPU pro núcleo (en MHz)"
 
-#: ../modals/cpu_modal.py:91 ../modals/cpu_modal.py:111
+#: ../modals/cpu_modal.py:103 ../modals/cpu_modal.py:123
 msgid "CPU #{}"
 msgstr "CPU #{}"
 
 #: ../modals/font_modal.py:74
 msgid "Choose Font"
-msgstr "Schriftart wählen"
+msgstr "Elege fuente"
 
 #: ../modals/font_modal.py:132
 msgid "Font"
-msgstr "Schriftart"
+msgstr "Fuente"
 
 #: ../modals/font_modal.py:159
 msgid "Style"
-msgstr "Stil"
+msgstr "Estilo"
 
 #: ../modals/font_modal.py:167
 msgid "Regular"
 msgstr "Normal"
 
 #: ../modals/font_modal.py:186
 msgid "Effects"
-msgstr "Effekte"
-
-#: ../modals/font_modal.py:193
-msgid "Underline"
-msgstr "Unterstrichen"
-
-#: ../modals/font_modal.py:197
-msgid "Overstrike"
-msgstr "Durchgestrichen"
+msgstr "Efectos"
 
 #: ../modals/font_modal.py:203
 msgid "Size"
-msgstr "Größe"
+msgstr "Tamaño"
 
 #: ../modals/font_modal.py:214
 msgid "Preview"
-msgstr "Vorschau"
+msgstr "Previsualización"
 
 #: ../modals/mem_usage_modal.py:54
 msgid "Memory Statistics"
-msgstr "Speicherstatistik"
+msgstr "Estadísticas de memoria"
 
 #: ../modals/mem_usage_modal.py:58
 msgid "Virtual Memory"
-msgstr "Virtueller Speicher"
+msgstr "memoria virtual"
 
 #: ../modals/settings_modal.py:31
 msgid "Light"
-msgstr "Licht"
+msgstr "Claro"
 
 #: ../modals/settings_modal.py:32
 msgid "Dark"
-msgstr "Dunkel"
+msgstr "Oscuro"
 
 #: ../modals/settings_modal.py:33
 msgid "Same as System"
-msgstr "Gleiches wie System"
+msgstr "Igual que en el sistema"
 
-#: ../modals/settings_modal.py:106
+#: ../modals/settings_modal.py:107
 msgid "Language"
-msgstr "Sprache"
+msgstr "Idioma"
 
-#: ../modals/settings_modal.py:121
+#: ../modals/settings_modal.py:122
 msgid "Theme"
-msgstr "Thema"
+msgstr "Tema"
 
-#: ../modals/settings_modal.py:139
+#: ../modals/settings_modal.py:140
 msgid "Always on top"
-msgstr "Immer im Vordergrund"
+msgstr "Siempre encima"
 
-#: ../modals/settings_modal.py:146
+#: ../modals/settings_modal.py:147
 msgid "Regular Font"
-msgstr "Normal Schriftart"
+msgstr "Fuente normal"
 
-#: ../modals/settings_modal.py:156
+#: ../modals/settings_modal.py:157
 msgid "Monospace Font"
-msgstr "Dicktengleiche Schrift"
+msgstr "Fuente monoespaciada"
 
-#: ../modals/settings_modal.py:166
+#: ../modals/settings_modal.py:167
 msgid "Add to desktop menu system"
-msgstr "Zum Desktop-Menüsystem hinzufügen"
+msgstr "Agregar al sistema de menú del escritorio"
 
-#: ../modals/settings_modal.py:191 ../modals/settings_modal.py:210
+#: ../modals/settings_modal.py:192 ../modals/settings_modal.py:211
 msgid "Select a font"
-msgstr "Schriftart auswählen"
+msgstr "Seleccione una fuente"
 
-#: ../widgets/button_mixin.py:116
-msgid "Yes"
-msgstr "Ja"
+#: ../widgets/edit_menu.py:65 ../widgets/edit_menu.py:94
+#: ../widgets/edit_menu.py:97
+msgid "Cut"
+msgstr "Cortar"
 
-#: ../widgets/button_mixin.py:119
-msgid "No"
-msgstr "Nein"
-
-#: ../widgets/button_mixin.py:122
-msgid "Retry"
-msgstr "Wiederholen"
-
-#: ../widgets/edit_menu.py:51
+#: ../widgets/edit_menu.py:65
 msgid "Ctrl+X"
-msgstr "Strg+X"
+msgstr "Ctrl+X"
 
-#: ../widgets/edit_menu.py:55
+#: ../widgets/edit_menu.py:69
+msgid "Copy"
+msgstr "Copiar"
+
+#: ../widgets/edit_menu.py:69
 msgid "Ctrl+C"
-msgstr "Strg+C"
+msgstr "Ctrl+C"
+
+#: ../widgets/edit_menu.py:73 ../widgets/edit_menu.py:95
+#: ../widgets/edit_menu.py:98
+msgid "Paste"
+msgstr "Pegar"
 
-#: ../widgets/edit_menu.py:59
+#: ../widgets/edit_menu.py:73
 msgid "Ctrl+V"
-msgstr "Strg+V"
+msgstr "Ctrl+V"
 
-#: ../widgets/meters.py:119
-msgid "Click for per-CPU usage"
-msgstr "Klicken Sie hier, um die Nutzung pro CPU anzuzeigen"
-
-#: ../widgets/meters.py:139
-msgid "{} :: CPU Details"
-msgstr "{} :: CPU-Details"
-
-#: ../widgets/meters.py:157
-msgid "Click for detailed temperature readings"
-msgstr "Klicken Sie hier, um detaillierte Temperaturmessungen anzuzeigen"
-
-#: ../widgets/meters.py:172
-msgid "{} :: Temperature Details"
-msgstr "{} :: Temperaturdetails"
-
-#: ../widgets/meters.py:190
-msgid "Click for detailed memory statistics"
-msgstr "Klicken Sie hier, um detaillierte RAM-Statistiken anzuzeigen"
-
-#: ../widgets/meters.py:204
-msgid "{} :: Memory Usage"
-msgstr "{} :: RAM-Auslastung"
-
-#: ../widgets/meters.py:219
-msgid "Disk Usage: /"
-msgstr "Plattenauslastung: /"
+#: ../widgets/edit_menu.py:78
+msgid "Select All"
+msgstr "Seleccionar todo"
 
-#: ../widgets/meters.py:222
-msgid "Click for usage details of each mount point"
-msgstr ""
-"Klicken Sie hier, um Nutzungsinformationen für jeden Mountpunkt anzuzeigen"
+#~ msgid "Yes"
+#~ msgstr "Sí"
+
+#~ msgid "No"
+#~ msgstr "No"
+
+#~ msgid "Retry"
+#~ msgstr "Reintentar"
+
+#~ msgid "Click for per-CPU usage"
+#~ msgstr "Clic para ver el uso por CPU"
+
+#~ msgid "{} :: CPU Details"
+#~ msgstr "{} :: Detalles de la CPU"
+
+#~ msgid "Click for detailed temperature readings"
+#~ msgstr "Clic para ver todos los sensores de temperatura"
+
+#~ msgid "{} :: Temperature Details"
+#~ msgstr "{} :: Detalles de temperatura"
 
-#: ../widgets/meters.py:236
-msgid "{} :: Disk Usage"
-msgstr "{} :: Plattenauslastung"
+#~ msgid "Click for detailed memory statistics"
+#~ msgstr "Clic para obtener estadísticas detalladas de la memoria"
 
-#~ msgid "Cut"
-#~ msgstr "Ausschneiden"
+#~ msgid "{} :: Memory Usage"
+#~ msgstr "{} :: Uso de memoria"
 
-#~ msgid "Copy"
-#~ msgstr "Kopieren"
+#~ msgid "Disk Usage: /"
+#~ msgstr "Uso del disco: /"
 
-#~ msgid "Paste"
-#~ msgstr "Einfügen"
+#~ msgid "Click for usage details of each mount point"
+#~ msgstr "Clic para obtener detalles de uso de cada punto de montaje"
 
-#~ msgid "Select All"
-#~ msgstr "Alles auswählen"
+#~ msgid "{} :: Disk Usage"
+#~ msgstr "{} :: Uso del disco"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/de/LC_MESSAGES/argparse.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/argparse.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: i18nparse\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-21 15:13-0500\n"
+"PO-Revision-Date: 2024-04-03 08:01-0500\n"
 "Last-Translator: blackstream-x <rz498sc@gmx.net>\n"
 "Language-Team: German\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -15,25 +15,28 @@
 msgid "%(prog)s: error: %(message)s\n"
 msgstr "%(prog)s: Fehler: %(message)s\n"
 
 msgid "%r is not callable"
 msgstr "%r ist nicht aufrufbar"
 
 msgid "'required' is an invalid argument for positionals"
-msgstr "'required' ist in Verbindung mit Positionsparametern ungültig"
+msgstr "'required' darf nicht mit Positionsparametern verwendet werden"
 
 msgid ".__call__() not defined"
 msgstr ".__call__() ist undefiniert"
 
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "Option nicht eindeutig: %(option)s passt auf %(matches)s"
 
 msgid "argument \"-\" with mode %r"
 msgstr "Parameter \"-\" mit Zugriffsart %r"
 
+msgid "argument %(argument_name)s: %(message)s"
+msgstr "Parameter %(argument_name)s: %(message)s"
+
 msgid "can't open '%(filename)s': %(error)s"
 msgstr "kann '%(filename)s' nicht öffnen: %(error)s"
 
 msgid "cannot have multiple subparser arguments"
 msgstr "mehrfache Subparser werden nicht unterstützt"
 
 msgid "cannot merge actions - two groups are named %r"
@@ -41,14 +44,20 @@
 "kann Aktionen nicht zusammenführen - zwei Gruppen haben den gleichen Namen %r"
 
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "Option steht im Konflikt: %s"
 msgstr[1] "Optionen stehen im Konflikt: %s"
 
+msgid "conflicting subparser alias: %s"
+msgstr "Subparser-Alias im Konflikt: %s"
+
+msgid "conflicting subparser: %s"
+msgstr "Subparser im Konflikt: %s"
+
 msgid "dest= is required for options like %r"
 msgstr "dest= wird bei Optionen wie %r benötigt"
 
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "%s Parameter wird erwartet"
 msgstr[1] "%s Parameter werden erwartet"
@@ -65,15 +74,15 @@
 msgid "ignored explicit argument %r"
 msgstr "expliziten Parameter %r ignoriert"
 
 msgid "invalid %(type)s value: %(value)r"
 msgstr "ungültiger Wert für %(type)s: %(value)r"
 
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
-msgstr "ungültige Wahl: %(value)r (Auswahl aus %(choices)s)"
+msgstr "ungültiger Wert: %(value)r (Auswahl aus %(choices)s)"
 
 msgid "invalid conflict_resolution value: %r"
 msgstr "ungültiger Wert für conflict_resolution: %r"
 
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
@@ -86,15 +95,18 @@
 msgid "not allowed with argument %s"
 msgstr "in Verbindung mit Parameter %s nicht erlaubt"
 
 msgid "one of the arguments %s is required"
 msgstr "einer der Parameter %s wird benötigt"
 
 msgid "optional arguments"
-msgstr "optionale Argumente"
+msgstr "Optionen"
+
+msgid "options"
+msgstr "Optionen"
 
 msgid "positional arguments"
 msgstr "Positionsparameter"
 
 msgid "show this help message and exit"
 msgstr "diese Meldung anzeigen und beenden"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/app.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/app.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: sysmon-pytk 0.4.1\n"
+"Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-30 19:01-0500\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
 "Last-Translator: Stacey Adams <stacey.belle.rose@gmail.com>\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "<Ctrl-C> to quit"
@@ -47,35 +47,26 @@
 
 msgid "Cancel"
 msgstr "Cancel"
 
 msgid "Choose Font"
 msgstr "Choose Font"
 
-msgid "Click for detailed memory statistics"
-msgstr "Click for detailed memory statistics"
-
-msgid "Click for detailed temperature readings"
-msgstr "Click for detailed temperature readings"
-
-msgid "Click for per-CPU usage"
-msgstr "Click for per-CPU usage"
-
-msgid "Click for usage details of each mount point"
-msgstr "Click for usage details of each mount point"
-
 msgid "Click to copy IP Address to clipboard"
 msgstr "Click to copy IP Address to clipboard"
 
 msgid "Close"
 msgstr "Close"
 
 msgid "Copied!"
 msgstr "Copied!"
 
+msgid "Copy"
+msgstr "Copy"
+
 msgid "Ctrl+A"
 msgstr "Ctrl+A"
 
 msgid "Ctrl+C"
 msgstr "Ctrl+C"
 
 msgid "Ctrl+Q"
@@ -89,23 +80,23 @@
 
 msgid "Ctrl+V"
 msgstr "Ctrl+V"
 
 msgid "Ctrl+X"
 msgstr "Ctrl+X"
 
+msgid "Cut"
+msgstr "Cut"
+
 msgid "Dark"
 msgstr "Dark"
 
 msgid "Disk Usage"
 msgstr "Disk Usage"
 
-msgid "Disk Usage: /"
-msgstr "Disk Usage: /"
-
 msgid "Display Details"
 msgstr "Display Details"
 
 msgid "Effects"
 msgstr "Effects"
 
 msgid "Error creating desktop menu item"
@@ -143,26 +134,26 @@
 
 msgid "Memory Statistics"
 msgstr "Memory Statistics"
 
 msgid "Monospace Font"
 msgstr "Monospace Font"
 
-msgid "No"
-msgstr "No"
-
 msgid "OK"
 msgstr "OK"
 
 msgid "Options"
 msgstr "Options"
 
 msgid "Overstrike"
 msgstr "Strikethrough"
 
+msgid "Paste"
+msgstr "Paste"
+
 msgid "Preferences"
 msgstr "Preferences"
 
 msgid "Preview"
 msgstr "Preview"
 
 msgid "Processes: {}"
@@ -179,20 +170,20 @@
 
 msgid "Regular Font"
 msgstr "Regular Font"
 
 msgid "Restart"
 msgstr "Restart"
 
-msgid "Retry"
-msgstr "Retry"
-
 msgid "Same as System"
 msgstr "Same as System"
 
+msgid "Select All"
+msgstr "Select All"
+
 msgid "Select a font"
 msgstr "Select a font"
 
 msgid "Size"
 msgstr "Size"
 
 msgid "Source Code"
@@ -238,17 +229,14 @@
 
 msgid "Version {}"
 msgstr "Version {}"
 
 msgid "Virtual Memory"
 msgstr "Virtual Memory"
 
-msgid "Yes"
-msgstr "Yes"
-
 msgid "per-core CPU Frequency (in MHz)"
 msgstr "per-core CPU Frequency (in MHz)"
 
 msgid "per-core CPU Usage"
 msgstr "per-core CPU Usage"
 
 msgid "show both disk and temperature details"
@@ -285,21 +273,9 @@
 
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
 msgstr "time between screen refreshes (in seconds, default=%(default)s)"
 
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
 msgstr "{current}°C (high = {high}°C, critical = {critical}°C)"
 
-msgid "{} :: CPU Details"
-msgstr "{} :: CPU Details"
-
-msgid "{} :: Disk Usage"
-msgstr "{} :: Disk Usage"
-
-msgid "{} :: Memory Usage"
-msgstr "{} :: Memory Usage"
-
-msgid "{} :: Temperature Details"
-msgstr "{} :: Temperature Details"
-
 msgid "{} Preferences"
 msgstr "{} Preferences"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/app.po` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/app.po`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"POT-Creation-Date: 2024-03-31 04:00-0500\n"
-"PO-Revision-Date: 2024-03-31 04:00-0500\n"
+"POT-Creation-Date: 2024-04-11 15:23+0000\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
 "Last-Translator: Stacey Adams <stacey.belle.rose@gmail.com>\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: ../about.py:14
@@ -26,241 +26,248 @@
 "process count."
 msgstr ""
 "sysmon-pytk is a system monitor. It monitors CPU usage and temperature, RAM "
 "usage, and disk usage of the primary disk (containing the root partition). "
 "It also displays the system's hostname, IP address, uptime, and current "
 "process count."
 
-#: ../application.py:33 ../cli_monitor.py:203 ../desktop_menu.py:72
+#: ../application.py:32 ../cli_sysmon.py:205 ../desktop_menu.py:81
 msgid "System Monitor"
 msgstr "System Monitor"
 
-#: ../application.py:94
+#: ../application.py:100
 msgid "Click to copy IP Address to clipboard"
 msgstr "Click to copy IP Address to clipboard"
 
-#: ../application.py:164
+#: ../application.py:170
 msgid "File"
 msgstr "File"
 
-#: ../application.py:167
+#: ../application.py:173
 msgid "About"
 msgstr "About"
 
-#: ../application.py:167 ../widgets/edit_menu.py:65
+#: ../application.py:173 ../widgets/edit_menu.py:79
 msgid "Ctrl+A"
 msgstr "Ctrl+A"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Preferences"
 msgstr "Preferences"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Ctrl+Shift+P"
 msgstr "Ctrl+Shift+P"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Restart"
 msgstr "Restart"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Ctrl+R"
 msgstr "Ctrl+R"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Quit"
 msgstr "Quit"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Ctrl+Q"
 msgstr "Ctrl+Q"
 
-#: ../application.py:201
+#: ../application.py:210
 msgid "Copied!"
 msgstr "Copied!"
 
-#: ../application.py:235
+#: ../application.py:252
 msgid "{} Preferences"
 msgstr "{} Preferences"
 
-#: ../application.py:244 ../cli_monitor.py:206
+#: ../application.py:264 ../cli_sysmon.py:208
 msgid "Hostname: {}"
 msgstr "Hostname: {}"
 
-#: ../application.py:245 ../cli_monitor.py:207
+#: ../application.py:265 ../cli_sysmon.py:209
 msgid "IP Address: {}"
 msgstr "IP Address: {}"
 
-#: ../application.py:246 ../cli_monitor.py:208
+#: ../application.py:266 ../cli_sysmon.py:210
 msgid "Processes: {}"
 msgstr "Processes: {}"
 
-#: ../application.py:247 ../cli_monitor.py:209
+#: ../application.py:267 ../cli_sysmon.py:211
 msgid "Uptime: {}"
 msgstr "Uptime: {}"
 
-#: ../cli_monitor.py:50 ../widgets/meters.py:116
+#: ../cli_sysmon.py:52
 msgid "CPU Usage"
 msgstr "CPU Usage"
 
-#: ../cli_monitor.py:58 ../widgets/meters.py:154
+#: ../cli_sysmon.py:60
 msgid "Temperature"
 msgstr "Temperature"
 
-#: ../cli_monitor.py:68 ../widgets/meters.py:187
+#: ../cli_sysmon.py:70
 msgid "RAM Usage"
 msgstr "RAM Usage"
 
-#: ../cli_monitor.py:78 ../modals/mem_usage_modal.py:63
+#: ../cli_sysmon.py:80 ../modals/mem_usage_modal.py:63
 msgid "Swap Memory"
 msgstr "Swap Memory"
 
-#: ../cli_monitor.py:114 ../cli_monitor.py:162 ../modals/disk_usage_modal.py:59
+#: ../cli_sysmon.py:116 ../cli_sysmon.py:164 ../modals/disk_usage_modal.py:71
 msgid "Disk Usage"
 msgstr "Disk Usage"
 
-#: ../cli_monitor.py:131 ../cli_monitor.py:179
-#: ../modals/temperature_modal.py:45
+#: ../cli_sysmon.py:133 ../cli_sysmon.py:181 ../modals/temperature_modal.py:45
 msgid "Temperature Sensors"
 msgstr "Temperature Sensors"
 
-#: ../cli_monitor.py:142 ../modals/temperature_modal.py:103
+#: ../cli_sysmon.py:144 ../modals/temperature_modal.py:103
 #, python-brace-format
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
 msgstr "{current}°C (high = {high}°C, critical = {critical}°C)"
 
-#: ../cli_monitor.py:222
+#: ../cli_sysmon.py:224
 msgid "<Ctrl-C> to quit"
 msgstr "<Ctrl-C> to quit"
 
-#: ../cli_monitor.py:232
+#: ../cli_sysmon.py:234
 msgid "System monitor: display CPU usage/temperature, memory usage, disk usage"
 msgstr ""
 "System monitor: display CPU usage/temperature, memory usage, disk usage"
 
-#: ../cli_monitor.py:235
+#: ../cli_sysmon.py:237
 msgid ""
 "By default, this program will use the same language as that selected for the "
 "GUI application. To override it, use the '-l' option. To quit, press <Ctrl-"
 "C>."
 msgstr ""
 "By default, this program will use the same language as that selected for the "
 "GUI application. To override it, use the '-l' option. To quit, press <Ctrl-"
 "C>."
 
-#: ../cli_monitor.py:242
+#: ../cli_sysmon.py:244
 msgid "Options"
 msgstr "Options"
 
-#: ../cli_monitor.py:245
+#: ../cli_sysmon.py:247
 msgid "show this help message and exit"
 msgstr "show this help message and exit"
 
-#: ../cli_monitor.py:250
+#: ../cli_sysmon.py:252
 msgid "show program's version number and exit"
 msgstr "show program's version number and exit"
 
-#: ../cli_monitor.py:254
+#: ../cli_sysmon.py:256
 #, python-format
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
 msgstr "time between screen refreshes (in seconds, default=%(default)s)"
 
-#: ../cli_monitor.py:258
+#: ../cli_sysmon.py:260
 msgid "the language to use for display"
 msgstr "the language to use for display"
 
-#: ../cli_monitor.py:260
+#: ../cli_sysmon.py:262
 msgid "Display Details"
 msgstr "Display Details"
 
-#: ../cli_monitor.py:264
+#: ../cli_sysmon.py:266
 msgid "show disk details (default)"
 msgstr "show disk details (default)"
 
-#: ../cli_monitor.py:268
+#: ../cli_sysmon.py:270
 msgid "show temperature details"
 msgstr "show temperature details"
 
-#: ../cli_monitor.py:272
+#: ../cli_sysmon.py:274
 msgid "show both disk and temperature details"
 msgstr "show both disk and temperature details"
 
-#: ../cli_monitor.py:276
+#: ../cli_sysmon.py:278
 msgid "show no details, only the header"
 msgstr "show no details, only the header"
 
-#: ../desktop_menu.py:48
+#: ../desktop_menu.py:57
 msgid "Error creating desktop menu item"
 msgstr "Error creating desktop menu item"
 
-#: ../desktop_menu.py:49
+#: ../desktop_menu.py:58
 msgid ""
 "System Monitor (sysmon) must be installed in a virtual environment in order "
 "to create a desktop menu entry."
 msgstr ""
 "System Monitor (sysmon) must be installed in a virtual environment in order "
 "to create a desktop menu entry."
 
-#: ../font_utils.py:74 ../modals/font_modal.py:171
+#: ../font_utils.py:153 ../modals/font_modal.py:171
 msgid "Bold"
 msgstr "Bold"
 
-#: ../font_utils.py:76 ../modals/font_modal.py:175
+#: ../font_utils.py:155 ../modals/font_modal.py:175
 msgid "Italic"
 msgstr "Italic"
 
-#: ../font_utils.py:78 ../modals/font_modal.py:179
+#: ../font_utils.py:157 ../modals/font_modal.py:179
 msgid "Bold Italic"
 msgstr "Bold Italic"
 
-#: ../modals/about_modal.py:93
+#: ../font_utils.py:171 ../modals/font_modal.py:193
+msgid "Underline"
+msgstr "Underline"
+
+#: ../font_utils.py:172 ../modals/font_modal.py:197
+msgid "Overstrike"
+msgstr "Strikethrough"
+
+#: ../modals/_base_modal.py:158
+msgid "Close"
+msgstr "Close"
+
+#: ../modals/_base_modal.py:168
+msgid "Cancel"
+msgstr "Cancel"
+
+#: ../modals/_base_modal.py:169
+msgid "OK"
+msgstr "OK"
+
+#: ../modals/about_modal.py:115
 msgid "About {}"
 msgstr "About {}"
 
-#: ../modals/about_modal.py:125
+#: ../modals/about_modal.py:147
 msgid "Translators"
 msgstr "Translators"
 
-#: ../modals/about_modal.py:131
+#: ../modals/about_modal.py:153
 msgid "License"
 msgstr "License"
 
-#: ../modals/about_modal.py:149
+#: ../modals/about_modal.py:171
 msgid "Version {}"
 msgstr "Version {}"
 
-#: ../modals/about_modal.py:155
+#: ../modals/about_modal.py:177
 msgid "Source Code"
 msgstr "Source Code"
 
-#: ../modals/about_modal.py:220
+#: ../modals/about_modal.py:242
 msgid "Full license text available here"
 msgstr "Full license text available here"
 
-#: ../modals/_base_modal.py:158 ../widgets/button_mixin.py:113
-msgid "Close"
-msgstr "Close"
-
-#: ../modals/_base_modal.py:168 ../widgets/button_mixin.py:110
-msgid "Cancel"
-msgstr "Cancel"
-
-#: ../modals/_base_modal.py:169 ../widgets/button_mixin.py:107
-msgid "OK"
-msgstr "OK"
-
-#: ../modals/cpu_modal.py:70
+#: ../modals/cpu_modal.py:82
 msgid "per-core CPU Usage"
 msgstr "per-core CPU Usage"
 
-#: ../modals/cpu_modal.py:76
+#: ../modals/cpu_modal.py:88
 msgid "per-core CPU Frequency (in MHz)"
 msgstr "per-core CPU Frequency (in MHz)"
 
-#: ../modals/cpu_modal.py:91 ../modals/cpu_modal.py:111
+#: ../modals/cpu_modal.py:103 ../modals/cpu_modal.py:123
 msgid "CPU #{}"
 msgstr "CPU #{}"
 
 #: ../modals/font_modal.py:74
 msgid "Choose Font"
 msgstr "Choose Font"
 
@@ -276,22 +283,14 @@
 msgid "Regular"
 msgstr "Regular"
 
 #: ../modals/font_modal.py:186
 msgid "Effects"
 msgstr "Effects"
 
-#: ../modals/font_modal.py:193
-msgid "Underline"
-msgstr "Underline"
-
-#: ../modals/font_modal.py:197
-msgid "Overstrike"
-msgstr "Strikethrough"
-
 #: ../modals/font_modal.py:203
 msgid "Size"
 msgstr "Size"
 
 #: ../modals/font_modal.py:214
 msgid "Preview"
 msgstr "Preview"
@@ -312,109 +311,103 @@
 msgid "Dark"
 msgstr "Dark"
 
 #: ../modals/settings_modal.py:33
 msgid "Same as System"
 msgstr "Same as System"
 
-#: ../modals/settings_modal.py:106
+#: ../modals/settings_modal.py:107
 msgid "Language"
 msgstr "Language"
 
-#: ../modals/settings_modal.py:121
+#: ../modals/settings_modal.py:122
 msgid "Theme"
 msgstr "Theme"
 
-#: ../modals/settings_modal.py:139
+#: ../modals/settings_modal.py:140
 msgid "Always on top"
 msgstr "Always on top"
 
-#: ../modals/settings_modal.py:146
+#: ../modals/settings_modal.py:147
 msgid "Regular Font"
 msgstr "Regular Font"
 
-#: ../modals/settings_modal.py:156
+#: ../modals/settings_modal.py:157
 msgid "Monospace Font"
 msgstr "Monospace Font"
 
-#: ../modals/settings_modal.py:166
+#: ../modals/settings_modal.py:167
 msgid "Add to desktop menu system"
 msgstr "Add to desktop menu system"
 
-#: ../modals/settings_modal.py:191 ../modals/settings_modal.py:210
+#: ../modals/settings_modal.py:192 ../modals/settings_modal.py:211
 msgid "Select a font"
 msgstr "Select a font"
 
-#: ../widgets/button_mixin.py:116
-msgid "Yes"
-msgstr "Yes"
-
-#: ../widgets/button_mixin.py:119
-msgid "No"
-msgstr "No"
-
-#: ../widgets/button_mixin.py:122
-msgid "Retry"
-msgstr "Retry"
+#: ../widgets/edit_menu.py:65 ../widgets/edit_menu.py:94
+#: ../widgets/edit_menu.py:97
+msgid "Cut"
+msgstr "Cut"
 
-#: ../widgets/edit_menu.py:51
+#: ../widgets/edit_menu.py:65
 msgid "Ctrl+X"
 msgstr "Ctrl+X"
 
-#: ../widgets/edit_menu.py:55
+#: ../widgets/edit_menu.py:69
+msgid "Copy"
+msgstr "Copy"
+
+#: ../widgets/edit_menu.py:69
 msgid "Ctrl+C"
 msgstr "Ctrl+C"
 
-#: ../widgets/edit_menu.py:59
+#: ../widgets/edit_menu.py:73 ../widgets/edit_menu.py:95
+#: ../widgets/edit_menu.py:98
+msgid "Paste"
+msgstr "Paste"
+
+#: ../widgets/edit_menu.py:73
 msgid "Ctrl+V"
 msgstr "Ctrl+V"
 
-#: ../widgets/meters.py:119
-msgid "Click for per-CPU usage"
-msgstr "Click for per-CPU usage"
-
-#: ../widgets/meters.py:139
-msgid "{} :: CPU Details"
-msgstr "{} :: CPU Details"
-
-#: ../widgets/meters.py:157
-msgid "Click for detailed temperature readings"
-msgstr "Click for detailed temperature readings"
-
-#: ../widgets/meters.py:172
-msgid "{} :: Temperature Details"
-msgstr "{} :: Temperature Details"
-
-#: ../widgets/meters.py:190
-msgid "Click for detailed memory statistics"
-msgstr "Click for detailed memory statistics"
-
-#: ../widgets/meters.py:204
-msgid "{} :: Memory Usage"
-msgstr "{} :: Memory Usage"
-
-#: ../widgets/meters.py:219
-msgid "Disk Usage: /"
-msgstr "Disk Usage: /"
-
-#: ../widgets/meters.py:222
-msgid "Click for usage details of each mount point"
-msgstr "Click for usage details of each mount point"
-
-#: ../widgets/meters.py:236
-msgid "{} :: Disk Usage"
-msgstr "{} :: Disk Usage"
+#: ../widgets/edit_menu.py:78
+msgid "Select All"
+msgstr "Select All"
 
-#~ msgid "Creating menu entry failed"
-#~ msgstr "Creating menu entry failed"
+#~ msgid "Yes"
+#~ msgstr "Yes"
+
+#~ msgid "No"
+#~ msgstr "No"
+
+#~ msgid "Retry"
+#~ msgstr "Retry"
+
+#~ msgid "Click for per-CPU usage"
+#~ msgstr "Click for per-CPU usage"
+
+#~ msgid "{} :: CPU Details"
+#~ msgstr "{} :: CPU Details"
+
+#~ msgid "Click for detailed temperature readings"
+#~ msgstr "Click for detailed temperature readings"
 
-#~ msgid "Cut"
-#~ msgstr "Cut"
+#~ msgid "{} :: Temperature Details"
+#~ msgstr "{} :: Temperature Details"
 
-#~ msgid "Copy"
-#~ msgstr "Copy"
+#~ msgid "Click for detailed memory statistics"
+#~ msgstr "Click for detailed memory statistics"
 
-#~ msgid "Paste"
-#~ msgstr "Paste"
+#~ msgid "{} :: Memory Usage"
+#~ msgstr "{} :: Memory Usage"
 
-#~ msgid "Select All"
-#~ msgstr "Select All"
+#~ msgid "Disk Usage: /"
+#~ msgstr "Disk Usage: /"
+
+#~ msgid "Click for usage details of each mount point"
+#~ msgstr "Click for usage details of each mount point"
+
+#~ msgid "{} :: Disk Usage"
+#~ msgstr "{} :: Disk Usage"
+
+#~ msgid "Creating menu entry failed"
+#~ msgstr "Creating menu entry failed"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/en/LC_MESSAGES/argparse.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/en/LC_MESSAGES/argparse.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: i18nparse\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-21 15:13-0500\n"
+"PO-Revision-Date: 2024-04-03 08:01-0500\n"
 "Last-Translator: Stacey Adams <stacey.belle.rose@gmail.com>\n"
 "Language-Team: English\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -25,28 +25,37 @@
 
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "ambiguous option: %(option)s could match %(matches)s"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" with mode %r"
 
+msgid "argument %(argument_name)s: %(message)s"
+msgstr "argument %(argument_name)s: %(message)s"
+
 msgid "can't open '%(filename)s': %(error)s"
 msgstr "can't open '%(filename)s': %(error)s"
 
 msgid "cannot have multiple subparser arguments"
 msgstr "cannot have multiple subparser arguments"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "cannot merge actions - two groups are named %r"
 
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "conflicting option string: %s"
 msgstr[1] "conflicting option strings: %s"
 
+msgid "conflicting subparser alias: %s"
+msgstr "conflicting subparser alias: %s"
+
+msgid "conflicting subparser: %s"
+msgstr "conflicting subparser: %s"
+
 msgid "dest= is required for options like %r"
 msgstr "dest= is required for options like %r"
 
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "expected %s argument"
 msgstr[1] "expected %s arguments"
@@ -87,14 +96,17 @@
 
 msgid "one of the arguments %s is required"
 msgstr "one of the arguments %s is required"
 
 msgid "optional arguments"
 msgstr "optional arguments"
 
+msgid "options"
+msgstr "options"
+
 msgid "positional arguments"
 msgstr "positional arguments"
 
 msgid "show this help message and exit"
 msgstr "show this help message and exit"
 
 msgid "the following arguments are required: %s"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/app.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/app.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: sysmon-pytk 0.4.1\n"
+"Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-30 19:01-0500\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
 "Last-Translator: Stacey Adams <stacey.belle.rose@gmail.com>\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/sysmon-pytk/"
 "sysmon-pytk/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -51,35 +51,26 @@
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Choose Font"
 msgstr "Elege fuente"
 
-msgid "Click for detailed memory statistics"
-msgstr "Clic para obtener estadísticas detalladas de la memoria"
-
-msgid "Click for detailed temperature readings"
-msgstr "Clic para ver todos los sensores de temperatura"
-
-msgid "Click for per-CPU usage"
-msgstr "Clic para ver el uso por CPU"
-
-msgid "Click for usage details of each mount point"
-msgstr "Clic para obtener detalles de uso de cada punto de montaje"
-
 msgid "Click to copy IP Address to clipboard"
 msgstr "Clic para copiar la dirección IP al portapapeles"
 
 msgid "Close"
 msgstr "Cerrar"
 
 msgid "Copied!"
 msgstr "¡Copiado!"
 
+msgid "Copy"
+msgstr "Copiar"
+
 msgid "Ctrl+A"
 msgstr "Ctrl+A"
 
 msgid "Ctrl+C"
 msgstr "Ctrl+C"
 
 msgid "Ctrl+Q"
@@ -93,23 +84,23 @@
 
 msgid "Ctrl+V"
 msgstr "Ctrl+V"
 
 msgid "Ctrl+X"
 msgstr "Ctrl+X"
 
+msgid "Cut"
+msgstr "Cortar"
+
 msgid "Dark"
 msgstr "Oscuro"
 
 msgid "Disk Usage"
 msgstr "Uso del disco"
 
-msgid "Disk Usage: /"
-msgstr "Uso del disco: /"
-
 msgid "Display Details"
 msgstr "detalles de la pantalla"
 
 msgid "Effects"
 msgstr "Efectos"
 
 msgid "Error creating desktop menu item"
@@ -147,26 +138,26 @@
 
 msgid "Memory Statistics"
 msgstr "Estadísticas de memoria"
 
 msgid "Monospace Font"
 msgstr "Fuente monoespaciada"
 
-msgid "No"
-msgstr "No"
-
 msgid "OK"
 msgstr "Aceptar"
 
 msgid "Options"
 msgstr "Opciones"
 
 msgid "Overstrike"
 msgstr "Tachado"
 
+msgid "Paste"
+msgstr "Pegar"
+
 msgid "Preferences"
 msgstr "Preferencias"
 
 msgid "Preview"
 msgstr "Previsualización"
 
 msgid "Processes: {}"
@@ -183,20 +174,20 @@
 
 msgid "Regular Font"
 msgstr "Fuente normal"
 
 msgid "Restart"
 msgstr "Reiniciar"
 
-msgid "Retry"
-msgstr "Reintentar"
-
 msgid "Same as System"
 msgstr "Igual que en el sistema"
 
+msgid "Select All"
+msgstr "Seleccionar todo"
+
 msgid "Select a font"
 msgstr "Seleccione una fuente"
 
 msgid "Size"
 msgstr "Tamaño"
 
 msgid "Source Code"
@@ -243,17 +234,14 @@
 
 msgid "Version {}"
 msgstr "Versión {}"
 
 msgid "Virtual Memory"
 msgstr "memoria virtual"
 
-msgid "Yes"
-msgstr "Sí"
-
 msgid "per-core CPU Frequency (in MHz)"
 msgstr "frecuencia de CPU pro núcleo (en MHz)"
 
 msgid "per-core CPU Usage"
 msgstr "uso del CPU por núcleo"
 
 msgid "show both disk and temperature details"
@@ -292,21 +280,9 @@
 msgstr ""
 "tiempo entre actualizaciones de pantalla (en segundos, "
 "predeterminado=%(default)s)"
 
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
 msgstr "{current}°C (alta = {high}°C, critica = {critical}°C)"
 
-msgid "{} :: CPU Details"
-msgstr "{} :: Detalles de la CPU"
-
-msgid "{} :: Disk Usage"
-msgstr "{} :: Uso del disco"
-
-msgid "{} :: Memory Usage"
-msgstr "{} :: Uso de memoria"
-
-msgid "{} :: Temperature Details"
-msgstr "{} :: Detalles de temperatura"
-
 msgid "{} Preferences"
 msgstr "{} Preferencias"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/app.po` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,424 +1,413 @@
 # System monitor written in Python using Tk.
-# SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
+# SPDX-FileCopyrightText: © 2024 Allan Nordhøy <epost@anotheragency.no>
 # SPDX-License-Identifier: MIT
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"POT-Creation-Date: 2024-03-31 04:00-0500\n"
-"PO-Revision-Date: 2024-03-31 04:00-0500\n"
-"Last-Translator: Stacey Adams <stacey.belle.rose@gmail.com>\n"
-"Language-Team: Spanish <https://hosted.weblate.org/projects/sysmon-pytk/"
-"sysmon-pytk/es/>\n"
-"Language: es\n"
+"POT-Creation-Date: 2024-04-11 15:23+0000\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
+"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
+"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/sysmon-"
+"pytk/sysmon-pytk/nb_NO/>\n"
+"Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5-dev\n"
 
 #: ../about.py:14
 msgid "MIT License"
-msgstr "Licencia MIT"
+msgstr "MIT-lisens"
 
 #: ../about.py:18
 msgid ""
 "sysmon-pytk is a system monitor. It monitors CPU usage and temperature, RAM "
 "usage, and disk usage of the primary disk (containing the root partition). "
 "It also displays the system's hostname, IP address, uptime, and current "
 "process count."
 msgstr ""
-"sysmon-pytk es un monitor del sistema. Monitorea el uso y la temperatura de "
-"la CPU, el uso de RAM y el uso del disco primario (que contiene la partición "
-"raíz). También muestra el nombre de host del sistema, la dirección IP, el "
-"tiempo de actividad y el recuento de procesos actuales."
+"sysmon-pytk er en systemmonitor. Den holder øye med prosessor-, disk-, minne-"
+"bruk og temperatur, samt bruk av hovedpartisjon (som inneholder rot-"
+"partisjonen). Verktøyet viser også systemets vertsnavn, IP-adresse, oppetid, "
+"og nåværende prosessantall."
 
-#: ../application.py:33 ../cli_monitor.py:203 ../desktop_menu.py:72
+#: ../application.py:32 ../cli_sysmon.py:205 ../desktop_menu.py:81
 msgid "System Monitor"
-msgstr "Monitoreo del sistema"
+msgstr "Systemmonitor"
 
-#: ../application.py:94
+#: ../application.py:100
 msgid "Click to copy IP Address to clipboard"
-msgstr "Clic para copiar la dirección IP al portapapeles"
+msgstr "Klikk for å kopiere IP-adressen til utklippstavlen"
 
-#: ../application.py:164
+#: ../application.py:170
 msgid "File"
-msgstr "Archivo"
+msgstr "Fil"
 
-#: ../application.py:167
+#: ../application.py:173
 msgid "About"
-msgstr "Acerca de"
+msgstr "Om"
 
-#: ../application.py:167 ../widgets/edit_menu.py:65
+#: ../application.py:173 ../widgets/edit_menu.py:79
 msgid "Ctrl+A"
 msgstr "Ctrl+A"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Preferences"
-msgstr "Preferencias"
+msgstr "Innstillinger"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Ctrl+Shift+P"
-msgstr "Ctrl+Mayús+P"
+msgstr "Ctrl+Shift+P"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Restart"
-msgstr "Reiniciar"
+msgstr "Omstart"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Ctrl+R"
 msgstr "Ctrl+R"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Quit"
-msgstr "Salir"
+msgstr "Avslutt"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Ctrl+Q"
 msgstr "Ctrl+Q"
 
-#: ../application.py:201
+#: ../application.py:210
 msgid "Copied!"
-msgstr "¡Copiado!"
+msgstr "Kopiert!"
 
-#: ../application.py:235
+#: ../application.py:252
 msgid "{} Preferences"
-msgstr "{} Preferencias"
+msgstr "{} Innstillinger"
 
-#: ../application.py:244 ../cli_monitor.py:206
+#: ../application.py:264 ../cli_sysmon.py:208
 msgid "Hostname: {}"
-msgstr "Nombre del host: {}"
+msgstr "Vertsnavn: {}"
 
-#: ../application.py:245 ../cli_monitor.py:207
+#: ../application.py:265 ../cli_sysmon.py:209
 msgid "IP Address: {}"
-msgstr "Dirección IP: {}"
+msgstr "IP-adresse: {}"
 
-#: ../application.py:246 ../cli_monitor.py:208
+#: ../application.py:266 ../cli_sysmon.py:210
 msgid "Processes: {}"
-msgstr "Recuento de procesos: {}"
+msgstr "Prosesser: {}"
 
-#: ../application.py:247 ../cli_monitor.py:209
+#: ../application.py:267 ../cli_sysmon.py:211
 msgid "Uptime: {}"
-msgstr "Tiempo de actividad: {}"
+msgstr "Oppetid: {}"
 
-#: ../cli_monitor.py:50 ../widgets/meters.py:116
+#: ../cli_sysmon.py:52
 msgid "CPU Usage"
-msgstr "Uso de CPU"
+msgstr "Prosessorbruk"
 
-#: ../cli_monitor.py:58 ../widgets/meters.py:154
+#: ../cli_sysmon.py:60
 msgid "Temperature"
-msgstr "Temperatura"
+msgstr "Temperatur"
 
-#: ../cli_monitor.py:68 ../widgets/meters.py:187
+#: ../cli_sysmon.py:70
 msgid "RAM Usage"
-msgstr "Uso de RAM"
+msgstr "Minnebruk"
 
-#: ../cli_monitor.py:78 ../modals/mem_usage_modal.py:63
+#: ../cli_sysmon.py:80 ../modals/mem_usage_modal.py:63
 msgid "Swap Memory"
-msgstr "memoria de intercambio"
+msgstr "Sidevekslingsfil"
 
-#: ../cli_monitor.py:114 ../cli_monitor.py:162 ../modals/disk_usage_modal.py:59
+#: ../cli_sysmon.py:116 ../cli_sysmon.py:164 ../modals/disk_usage_modal.py:71
 msgid "Disk Usage"
-msgstr "Uso del disco"
+msgstr "Diskbruk"
 
-#: ../cli_monitor.py:131 ../cli_monitor.py:179
-#: ../modals/temperature_modal.py:45
+#: ../cli_sysmon.py:133 ../cli_sysmon.py:181 ../modals/temperature_modal.py:45
 msgid "Temperature Sensors"
-msgstr "Sensores de temperatura"
+msgstr "Temperatursensorer"
 
-#: ../cli_monitor.py:142 ../modals/temperature_modal.py:103
+#: ../cli_sysmon.py:144 ../modals/temperature_modal.py:103
 #, python-brace-format
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
-msgstr "{current}°C (alta = {high}°C, critica = {critical}°C)"
+msgstr "{current}°C (høy = {high}°C, kritisk = {critical}°C)"
 
-#: ../cli_monitor.py:222
+#: ../cli_sysmon.py:224
 msgid "<Ctrl-C> to quit"
-msgstr "<Ctrl-C> para salir"
+msgstr "<Ctrl-C> for å avslutte"
 
-#: ../cli_monitor.py:232
+#: ../cli_sysmon.py:234
 msgid "System monitor: display CPU usage/temperature, memory usage, disk usage"
-msgstr ""
-"Monitor del sistema: muestra el uso/temperatura de la CPU, el uso de la "
-"memoria, el uso del disco"
+msgstr "Systemmonitor: Vis CPU-bruk/temperatur, minnebruk, diskbruk"
 
-#: ../cli_monitor.py:235
+#: ../cli_sysmon.py:237
 msgid ""
 "By default, this program will use the same language as that selected for the "
 "GUI application. To override it, use the '-l' option. To quit, press <Ctrl-"
 "C>."
 msgstr ""
-"De forma predeterminada, este programa utilizará el mismo idioma que el "
-"seleccionado para la aplicación GUI. Para anularlo, utilice la opción '-l'. "
-"Para salir, presione <Ctrl-C>."
+"Som standard vil dette programmet bruke samme språk som det som er valgt for "
+"GUI-applikasjonen. For å overstyre det, bruk alternativet '-l'. For å "
+"avslutte, trykk <Ctrl-C>."
 
-#: ../cli_monitor.py:242
+#: ../cli_sysmon.py:244
 msgid "Options"
-msgstr "Opciones"
+msgstr "Valg"
 
-#: ../cli_monitor.py:245
+#: ../cli_sysmon.py:247
 msgid "show this help message and exit"
-msgstr "muestra este mensaje de ayuda y termina"
+msgstr "vis denne hjelpemeldingen og avslutt"
 
-#: ../cli_monitor.py:250
+#: ../cli_sysmon.py:252
 msgid "show program's version number and exit"
-msgstr "mostrar el número de versión del programa y salir"
+msgstr "vis programmets versjonsnummer og avslutt"
 
-#: ../cli_monitor.py:254
+#: ../cli_sysmon.py:256
 #, python-format
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
-msgstr ""
-"tiempo entre actualizaciones de pantalla (en segundos, predeterminado="
-"%(default)s)"
+msgstr "tid mellom skjermoppdateringer (i sekunder, standard=%(default)s)"
 
-#: ../cli_monitor.py:258
+#: ../cli_sysmon.py:260
 msgid "the language to use for display"
-msgstr "el idioma a utilizar para la visualización"
+msgstr "språket som skal brukes for visning"
 
-#: ../cli_monitor.py:260
+#: ../cli_sysmon.py:262
 msgid "Display Details"
-msgstr "detalles de la pantalla"
+msgstr "Skjermdetaljene"
 
-#: ../cli_monitor.py:264
+#: ../cli_sysmon.py:266
 msgid "show disk details (default)"
-msgstr "mostrar detalles del disco (predeterminado)"
+msgstr "vis diskdetaljer (standard)"
 
-#: ../cli_monitor.py:268
+#: ../cli_sysmon.py:270
 msgid "show temperature details"
-msgstr "mostrar detalles de temperatura"
+msgstr "vis temperaturdetaljer"
 
-#: ../cli_monitor.py:272
+#: ../cli_sysmon.py:274
 msgid "show both disk and temperature details"
-msgstr "mostrar detalles del disco y de la temperatura"
+msgstr "vis både disk- og temperaturdetaljer"
 
-#: ../cli_monitor.py:276
+#: ../cli_sysmon.py:278
 msgid "show no details, only the header"
-msgstr "no mostrar detalles, solo el encabezado"
+msgstr "vis ingen detaljer, bare overskriften"
 
-#: ../desktop_menu.py:48
+#: ../desktop_menu.py:57
 msgid "Error creating desktop menu item"
-msgstr "Error al crear el elemento del menú del escritorio"
+msgstr "Feil under oppretting av skrivebordsmenyelement"
 
-#: ../desktop_menu.py:49
+#: ../desktop_menu.py:58
 msgid ""
 "System Monitor (sysmon) must be installed in a virtual environment in order "
 "to create a desktop menu entry."
 msgstr ""
-"System Monitor (sysmon) debe instalarse en un entorno virtual para poder "
-"crear una entrada de menú en el escritorio."
+"Systemmonitor (sysmon) må installeres i et virtuelt miljø for å opprette en "
+"skrivebordsmenyoppføring."
 
-#: ../font_utils.py:74 ../modals/font_modal.py:171
+#: ../font_utils.py:153 ../modals/font_modal.py:171
 msgid "Bold"
-msgstr "Negrita"
+msgstr "Fet"
 
-#: ../font_utils.py:76 ../modals/font_modal.py:175
+#: ../font_utils.py:155 ../modals/font_modal.py:175
 msgid "Italic"
-msgstr "Cursiva"
+msgstr "Kursiv"
 
-#: ../font_utils.py:78 ../modals/font_modal.py:179
+#: ../font_utils.py:157 ../modals/font_modal.py:179
 msgid "Bold Italic"
-msgstr "Cursiva negrita"
+msgstr "Fet kursiv"
+
+#: ../font_utils.py:171 ../modals/font_modal.py:193
+msgid "Underline"
+msgstr "Understrek"
 
-#: ../modals/about_modal.py:93
+#: ../font_utils.py:172 ../modals/font_modal.py:197
+msgid "Overstrike"
+msgstr "Gjennomstrek"
+
+#: ../modals/_base_modal.py:158
+msgid "Close"
+msgstr "Lukk"
+
+#: ../modals/_base_modal.py:168
+msgid "Cancel"
+msgstr "Avbryt"
+
+#: ../modals/_base_modal.py:169
+msgid "OK"
+msgstr "OK"
+
+#: ../modals/about_modal.py:115
 msgid "About {}"
-msgstr "Acerca del {}"
+msgstr "Om {}"
 
-#: ../modals/about_modal.py:125
+#: ../modals/about_modal.py:147
 msgid "Translators"
-msgstr "Traductores"
+msgstr "Oversettere"
 
-#: ../modals/about_modal.py:131
+#: ../modals/about_modal.py:153
 msgid "License"
-msgstr "Licencia"
+msgstr "Lisens"
 
-#: ../modals/about_modal.py:149
+#: ../modals/about_modal.py:171
 msgid "Version {}"
-msgstr "Versión {}"
+msgstr "Versjon {}"
 
-#: ../modals/about_modal.py:155
+#: ../modals/about_modal.py:177
 msgid "Source Code"
-msgstr "Código fuente"
+msgstr "Kildekode"
 
-#: ../modals/about_modal.py:220
+#: ../modals/about_modal.py:242
 msgid "Full license text available here"
-msgstr "Texto completo de la licencia disponible aquí"
-
-#: ../modals/_base_modal.py:158 ../widgets/button_mixin.py:113
-msgid "Close"
-msgstr "Cerrar"
-
-#: ../modals/_base_modal.py:168 ../widgets/button_mixin.py:110
-msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Full lisenstekst tilgjengelig her"
 
-#: ../modals/_base_modal.py:169 ../widgets/button_mixin.py:107
-msgid "OK"
-msgstr "Aceptar"
-
-#: ../modals/cpu_modal.py:70
+#: ../modals/cpu_modal.py:82
 msgid "per-core CPU Usage"
-msgstr "uso del CPU por núcleo"
+msgstr "prosessorbruk per kjerne"
 
-#: ../modals/cpu_modal.py:76
+#: ../modals/cpu_modal.py:88
 msgid "per-core CPU Frequency (in MHz)"
-msgstr "frecuencia de CPU pro núcleo (en MHz)"
+msgstr "prosessorfrekvens per kjerne (i MHz)"
 
-#: ../modals/cpu_modal.py:91 ../modals/cpu_modal.py:111
+#: ../modals/cpu_modal.py:103 ../modals/cpu_modal.py:123
 msgid "CPU #{}"
-msgstr "CPU #{}"
+msgstr "Prosessor #{}"
 
 #: ../modals/font_modal.py:74
 msgid "Choose Font"
-msgstr "Elege fuente"
+msgstr "Velg skrift"
 
 #: ../modals/font_modal.py:132
 msgid "Font"
-msgstr "Fuente"
+msgstr "Skrift"
 
 #: ../modals/font_modal.py:159
 msgid "Style"
-msgstr "Estilo"
+msgstr "Stil"
 
 #: ../modals/font_modal.py:167
 msgid "Regular"
-msgstr "Normal"
+msgstr "Vanlig"
 
 #: ../modals/font_modal.py:186
 msgid "Effects"
-msgstr "Efectos"
-
-#: ../modals/font_modal.py:193
-msgid "Underline"
-msgstr "Subrayada"
-
-#: ../modals/font_modal.py:197
-msgid "Overstrike"
-msgstr "Tachado"
+msgstr "Effekter"
 
 #: ../modals/font_modal.py:203
 msgid "Size"
-msgstr "Tamaño"
+msgstr "Størrelse"
 
 #: ../modals/font_modal.py:214
 msgid "Preview"
-msgstr "Previsualización"
+msgstr "Forhåndsvis"
 
 #: ../modals/mem_usage_modal.py:54
 msgid "Memory Statistics"
-msgstr "Estadísticas de memoria"
+msgstr "Minnestatistikk"
 
 #: ../modals/mem_usage_modal.py:58
 msgid "Virtual Memory"
-msgstr "memoria virtual"
+msgstr "Virtuelt minne"
 
 #: ../modals/settings_modal.py:31
 msgid "Light"
-msgstr "Claro"
+msgstr "Lys"
 
 #: ../modals/settings_modal.py:32
 msgid "Dark"
-msgstr "Oscuro"
+msgstr "Mørk"
 
 #: ../modals/settings_modal.py:33
 msgid "Same as System"
-msgstr "Igual que en el sistema"
+msgstr "Samme som systemet"
 
-#: ../modals/settings_modal.py:106
+#: ../modals/settings_modal.py:107
 msgid "Language"
-msgstr "Idioma"
+msgstr "Språk"
 
-#: ../modals/settings_modal.py:121
+#: ../modals/settings_modal.py:122
 msgid "Theme"
-msgstr "Tema"
+msgstr "Drakt"
 
-#: ../modals/settings_modal.py:139
+#: ../modals/settings_modal.py:140
 msgid "Always on top"
-msgstr "Siempre encima"
+msgstr "Alltid på topp"
 
-#: ../modals/settings_modal.py:146
+#: ../modals/settings_modal.py:147
 msgid "Regular Font"
-msgstr "Fuente normal"
+msgstr "Vanlig skrift"
 
-#: ../modals/settings_modal.py:156
+#: ../modals/settings_modal.py:157
 msgid "Monospace Font"
-msgstr "Fuente monoespaciada"
+msgstr "Fastbreddeskrift"
 
-#: ../modals/settings_modal.py:166
+#: ../modals/settings_modal.py:167
 msgid "Add to desktop menu system"
-msgstr "Agregar al sistema de menú del escritorio"
+msgstr "Legg til skrivebordets menysystem"
 
-#: ../modals/settings_modal.py:191 ../modals/settings_modal.py:210
+#: ../modals/settings_modal.py:192 ../modals/settings_modal.py:211
 msgid "Select a font"
-msgstr "Seleccione una fuente"
-
-#: ../widgets/button_mixin.py:116
-msgid "Yes"
-msgstr "Sí"
+msgstr "Velg en skrift"
 
-#: ../widgets/button_mixin.py:119
-msgid "No"
-msgstr "No"
+#: ../widgets/edit_menu.py:65 ../widgets/edit_menu.py:94
+#: ../widgets/edit_menu.py:97
+msgid "Cut"
+msgstr "Klipp ut"
 
-#: ../widgets/button_mixin.py:122
-msgid "Retry"
-msgstr "Reintentar"
-
-#: ../widgets/edit_menu.py:51
+#: ../widgets/edit_menu.py:65
 msgid "Ctrl+X"
 msgstr "Ctrl+X"
 
-#: ../widgets/edit_menu.py:55
+#: ../widgets/edit_menu.py:69
+msgid "Copy"
+msgstr "Kopier"
+
+#: ../widgets/edit_menu.py:69
 msgid "Ctrl+C"
 msgstr "Ctrl+C"
 
-#: ../widgets/edit_menu.py:59
+#: ../widgets/edit_menu.py:73 ../widgets/edit_menu.py:95
+#: ../widgets/edit_menu.py:98
+msgid "Paste"
+msgstr "Lim inn"
+
+#: ../widgets/edit_menu.py:73
 msgid "Ctrl+V"
 msgstr "Ctrl+V"
 
-#: ../widgets/meters.py:119
-msgid "Click for per-CPU usage"
-msgstr "Clic para ver el uso por CPU"
+#: ../widgets/edit_menu.py:78
+msgid "Select All"
+msgstr "Velg alt"
 
-#: ../widgets/meters.py:139
-msgid "{} :: CPU Details"
-msgstr "{} :: Detalles de la CPU"
+#~ msgid "Yes"
+#~ msgstr "Ja"
 
-#: ../widgets/meters.py:157
-msgid "Click for detailed temperature readings"
-msgstr "Clic para ver todos los sensores de temperatura"
+#~ msgid "No"
+#~ msgstr "Nei"
 
-#: ../widgets/meters.py:172
-msgid "{} :: Temperature Details"
-msgstr "{} :: Detalles de temperatura"
+#~ msgid "Retry"
+#~ msgstr "Prøv igjen"
 
-#: ../widgets/meters.py:190
-msgid "Click for detailed memory statistics"
-msgstr "Clic para obtener estadísticas detalladas de la memoria"
+#~ msgid "Click for per-CPU usage"
+#~ msgstr "Klikk for bruk per prosessor"
 
-#: ../widgets/meters.py:204
-msgid "{} :: Memory Usage"
-msgstr "{} :: Uso de memoria"
+#~ msgid "{} :: CPU Details"
+#~ msgstr "{} :: Prosessordetaljer"
 
-#: ../widgets/meters.py:219
-msgid "Disk Usage: /"
-msgstr "Uso del disco: /"
+#~ msgid "Click for detailed temperature readings"
+#~ msgstr "Klikk for detaljerte temperaturavlesninger"
 
-#: ../widgets/meters.py:222
-msgid "Click for usage details of each mount point"
-msgstr "Clic para obtener detalles de uso de cada punto de montaje"
+#~ msgid "{} :: Temperature Details"
+#~ msgstr "{} :: Temperaturdetaljer"
 
-#: ../widgets/meters.py:236
-msgid "{} :: Disk Usage"
-msgstr "{} :: Uso del disco"
+#~ msgid "Click for detailed memory statistics"
+#~ msgstr "Klikk for detaljert minnestatistikk"
 
-#~ msgid "Cut"
-#~ msgstr "Cortar"
+#~ msgid "{} :: Memory Usage"
+#~ msgstr "{} :: Minnebruk"
 
-#~ msgid "Copy"
-#~ msgstr "Copiar"
+#~ msgid "Disk Usage: /"
+#~ msgstr "Diskbruk: /"
 
-#~ msgid "Paste"
-#~ msgstr "Pegar"
+#~ msgid "Click for usage details of each mount point"
+#~ msgstr "Klikk for detaljert for hvert monteringspunkt"
 
-#~ msgid "Select All"
-#~ msgstr "Seleccionar todo"
+#~ msgid "{} :: Disk Usage"
+#~ msgstr "{} :: Diskbruk"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/es/LC_MESSAGES/argparse.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/es/LC_MESSAGES/argparse.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: i18nparse\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-21 15:13-0500\n"
+"PO-Revision-Date: 2024-04-03 08:01-0500\n"
 "Last-Translator: Félix Medrano\n"
 "Language-Team: Spanish\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
+"1 : 2;\n"
 
 msgid "%(prog)s: error: %(message)s\n"
 msgstr "%(prog)s: error: %(message)s\n"
 
 msgid "%r is not callable"
 msgstr "%r no es invocable"
 
@@ -25,35 +26,46 @@
 
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "opción ambigua: %(option)s podría corresponder con %(matches)s"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argumento \"-\" con modo %r"
 
+msgid "argument %(argument_name)s: %(message)s"
+msgstr "argumento %(argument_name)s: %(message)s"
+
 msgid "can't open '%(filename)s': %(error)s"
 msgstr "no se puede abrir '%(filename)s': %(error)s"
 
 msgid "cannot have multiple subparser arguments"
 msgstr "no puede haber múltiples argumentos de subanalizador"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "no se pueden unir las acciones - dos grupos se llaman %r"
 
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "literal de opción en conflicto: %s"
 msgstr[1] "literales de opción en conflicto: %s"
+msgstr[2] "literales de opción en conflicto: %s"
+
+msgid "conflicting subparser alias: %s"
+msgstr "alias de subanalizador en conflicto: %s"
+
+msgid "conflicting subparser: %s"
+msgstr "subanalizador en conflicto: %s"
 
 msgid "dest= is required for options like %r"
 msgstr "dest= es necesario en opciones como %r"
 
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "se espera el argumento %s"
 msgstr[1] "se esperan los argumentos %s"
+msgstr[2] "se esperan los argumentos %s"
 
 msgid "expected at least one argument"
 msgstr "se espera al menos un argumento"
 
 msgid "expected at most one argument"
 msgstr "se espera a lo sumo un argumento"
 
@@ -87,14 +99,17 @@
 
 msgid "one of the arguments %s is required"
 msgstr "uno de los argumentos %s es necesario"
 
 msgid "optional arguments"
 msgstr "argumentos opcionales"
 
+msgid "options"
+msgstr "opciones"
+
 msgid "positional arguments"
 msgstr "argumentos posicionales"
 
 msgid "show this help message and exit"
 msgstr "muestra este mensaje de ayuda y termina"
 
 msgid "the following arguments are required: %s"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: sysmon-pytk 0.4.1\n"
+"Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-30 19:01-0500\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/sysmon-"
 "pytk/sysmon-pytk/nb_NO/>\n"
 "Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -51,35 +51,26 @@
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid "Choose Font"
 msgstr "Velg skrift"
 
-msgid "Click for detailed memory statistics"
-msgstr "Klikk for detaljert minnestatistikk"
-
-msgid "Click for detailed temperature readings"
-msgstr "Klikk for detaljerte temperaturavlesninger"
-
-msgid "Click for per-CPU usage"
-msgstr "Klikk for bruk per prosessor"
-
-msgid "Click for usage details of each mount point"
-msgstr "Klikk for detaljert for hvert monteringspunkt"
-
 msgid "Click to copy IP Address to clipboard"
 msgstr "Klikk for å kopiere IP-adressen til utklippstavlen"
 
 msgid "Close"
 msgstr "Lukk"
 
 msgid "Copied!"
 msgstr "Kopiert!"
 
+msgid "Copy"
+msgstr "Kopier"
+
 msgid "Ctrl+A"
 msgstr "Ctrl+A"
 
 msgid "Ctrl+C"
 msgstr "Ctrl+C"
 
 msgid "Ctrl+Q"
@@ -93,23 +84,23 @@
 
 msgid "Ctrl+V"
 msgstr "Ctrl+V"
 
 msgid "Ctrl+X"
 msgstr "Ctrl+X"
 
+msgid "Cut"
+msgstr "Klipp ut"
+
 msgid "Dark"
 msgstr "Mørk"
 
 msgid "Disk Usage"
 msgstr "Diskbruk"
 
-msgid "Disk Usage: /"
-msgstr "Diskbruk: /"
-
 msgid "Display Details"
 msgstr "Skjermdetaljene"
 
 msgid "Effects"
 msgstr "Effekter"
 
 msgid "Error creating desktop menu item"
@@ -147,26 +138,26 @@
 
 msgid "Memory Statistics"
 msgstr "Minnestatistikk"
 
 msgid "Monospace Font"
 msgstr "Fastbreddeskrift"
 
-msgid "No"
-msgstr "Nei"
-
 msgid "OK"
 msgstr "OK"
 
 msgid "Options"
 msgstr "Valg"
 
 msgid "Overstrike"
 msgstr "Gjennomstrek"
 
+msgid "Paste"
+msgstr "Lim inn"
+
 msgid "Preferences"
 msgstr "Innstillinger"
 
 msgid "Preview"
 msgstr "Forhåndsvis"
 
 msgid "Processes: {}"
@@ -183,20 +174,20 @@
 
 msgid "Regular Font"
 msgstr "Vanlig skrift"
 
 msgid "Restart"
 msgstr "Omstart"
 
-msgid "Retry"
-msgstr "Prøv igjen"
-
 msgid "Same as System"
 msgstr "Samme som systemet"
 
+msgid "Select All"
+msgstr "Velg alt"
+
 msgid "Select a font"
 msgstr "Velg en skrift"
 
 msgid "Size"
 msgstr "Størrelse"
 
 msgid "Source Code"
@@ -241,17 +232,14 @@
 
 msgid "Version {}"
 msgstr "Versjon {}"
 
 msgid "Virtual Memory"
 msgstr "Virtuelt minne"
 
-msgid "Yes"
-msgstr "Ja"
-
 msgid "per-core CPU Frequency (in MHz)"
 msgstr "prosessorfrekvens per kjerne (i MHz)"
 
 msgid "per-core CPU Usage"
 msgstr "prosessorbruk per kjerne"
 
 msgid "show both disk and temperature details"
@@ -288,21 +276,9 @@
 
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
 msgstr "tid mellom skjermoppdateringer (i sekunder, standard=%(default)s)"
 
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
 msgstr "{current}°C (høy = {high}°C, kritisk = {critical}°C)"
 
-msgid "{} :: CPU Details"
-msgstr "{} :: Prosessordetaljer"
-
-msgid "{} :: Disk Usage"
-msgstr "{} :: Diskbruk"
-
-msgid "{} :: Memory Usage"
-msgstr "{} :: Minnebruk"
-
-msgid "{} :: Temperature Details"
-msgstr "{} :: Temperaturdetaljer"
-
 msgid "{} Preferences"
 msgstr "{} Innstillinger"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/app.po` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/de/LC_MESSAGES/app.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,420 +1,418 @@
 # System monitor written in Python using Tk.
-# SPDX-FileCopyrightText: © 2024 Allan Nordhøy <epost@anotheragency.no>
+# SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: sysmon-pytk 0.5.0\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"POT-Creation-Date: 2024-03-31 04:00-0500\n"
-"PO-Revision-Date: 2024-03-31 04:00-0500\n"
-"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
-"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/sysmon-"
-"pytk/sysmon-pytk/nb_NO/>\n"
-"Language: nb_NO\n"
+"POT-Creation-Date: 2024-04-11 15:23+0000\n"
+"PO-Revision-Date: 2024-04-08 03:09-0500\n"
+"Last-Translator: Alisyn Arness\n"
+"Language-Team: German <https://hosted.weblate.org/projects/sysmon-pytk/"
+"sysmon-pytk/de/>\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5-dev\n"
 
 #: ../about.py:14
 msgid "MIT License"
-msgstr "MIT-lisens"
+msgstr "MIT Lizenz"
 
 #: ../about.py:18
 msgid ""
 "sysmon-pytk is a system monitor. It monitors CPU usage and temperature, RAM "
 "usage, and disk usage of the primary disk (containing the root partition). "
 "It also displays the system's hostname, IP address, uptime, and current "
 "process count."
 msgstr ""
-"sysmon-pytk er en systemmonitor. Den holder øye med prosessor-, disk-, minne-"
-"bruk og temperatur, samt bruk av hovedpartisjon (som inneholder rot-"
-"partisjonen). Verktøyet viser også systemets vertsnavn, IP-adresse, oppetid, "
-"og nåværende prosessantall."
+"sysmon-pytk ist ein Systemmonitor. Es überwacht die CPU-Nutzung und -"
+"Temperatur, die RAM-Nutzung und die Festplattennutzung der primären "
+"Festplatte (die die Root-Partition enthält). Außerdem werden der Hostname, "
+"die IP-Adresse, die Betriebszeit und die aktuelle Prozessanzahl des Systems "
+"angezeigt."
 
-#: ../application.py:33 ../cli_monitor.py:203 ../desktop_menu.py:72
+#: ../application.py:32 ../cli_sysmon.py:205 ../desktop_menu.py:81
 msgid "System Monitor"
 msgstr "Systemmonitor"
 
-#: ../application.py:94
+#: ../application.py:100
 msgid "Click to copy IP Address to clipboard"
-msgstr "Klikk for å kopiere IP-adressen til utklippstavlen"
+msgstr "Klicken Sie hier, um die IP-Adresse in die Zwischenablage zu kopieren"
 
-#: ../application.py:164
+#: ../application.py:170
 msgid "File"
-msgstr "Fil"
+msgstr "Datei"
 
-#: ../application.py:167
+#: ../application.py:173
 msgid "About"
-msgstr "Om"
+msgstr "Über"
 
-#: ../application.py:167 ../widgets/edit_menu.py:65
+#: ../application.py:173 ../widgets/edit_menu.py:79
 msgid "Ctrl+A"
-msgstr "Ctrl+A"
+msgstr "Strg+A"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Preferences"
-msgstr "Innstillinger"
+msgstr "Einstellungen"
 
-#: ../application.py:171
+#: ../application.py:177
 msgid "Ctrl+Shift+P"
-msgstr "Ctrl+Shift+P"
+msgstr "Strg+Umschalt+P"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Restart"
-msgstr "Omstart"
+msgstr "Neustart"
 
-#: ../application.py:175
+#: ../application.py:181
 msgid "Ctrl+R"
-msgstr "Ctrl+R"
+msgstr "Strg+R"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Quit"
-msgstr "Avslutt"
+msgstr "Beenden"
 
-#: ../application.py:180
+#: ../application.py:186
 msgid "Ctrl+Q"
-msgstr "Ctrl+Q"
+msgstr "Strg-Q"
 
-#: ../application.py:201
+#: ../application.py:210
 msgid "Copied!"
 msgstr "Kopiert!"
 
-#: ../application.py:235
+#: ../application.py:252
 msgid "{} Preferences"
-msgstr "{} Innstillinger"
+msgstr "{} Einstellungen"
 
-#: ../application.py:244 ../cli_monitor.py:206
+#: ../application.py:264 ../cli_sysmon.py:208
 msgid "Hostname: {}"
-msgstr "Vertsnavn: {}"
+msgstr "Hostname : {}"
 
-#: ../application.py:245 ../cli_monitor.py:207
+#: ../application.py:265 ../cli_sysmon.py:209
 msgid "IP Address: {}"
-msgstr "IP-adresse: {}"
+msgstr "IP-Adresse: {}"
 
-#: ../application.py:246 ../cli_monitor.py:208
+#: ../application.py:266 ../cli_sysmon.py:210
 msgid "Processes: {}"
-msgstr "Prosesser: {}"
+msgstr "Prozesse: {}"
 
-#: ../application.py:247 ../cli_monitor.py:209
+#: ../application.py:267 ../cli_sysmon.py:211
 msgid "Uptime: {}"
-msgstr "Oppetid: {}"
+msgstr "Betriebszeit: {}"
 
-#: ../cli_monitor.py:50 ../widgets/meters.py:116
+#: ../cli_sysmon.py:52
 msgid "CPU Usage"
-msgstr "Prosessorbruk"
+msgstr "CPU-Auslastung"
 
-#: ../cli_monitor.py:58 ../widgets/meters.py:154
+#: ../cli_sysmon.py:60
 msgid "Temperature"
 msgstr "Temperatur"
 
-#: ../cli_monitor.py:68 ../widgets/meters.py:187
+#: ../cli_sysmon.py:70
 msgid "RAM Usage"
-msgstr "Minnebruk"
+msgstr "RAM-Auslastung"
 
-#: ../cli_monitor.py:78 ../modals/mem_usage_modal.py:63
+#: ../cli_sysmon.py:80 ../modals/mem_usage_modal.py:63
 msgid "Swap Memory"
-msgstr "Sidevekslingsfil"
+msgstr "Speicher Austauschen"
 
-#: ../cli_monitor.py:114 ../cli_monitor.py:162 ../modals/disk_usage_modal.py:59
+#: ../cli_sysmon.py:116 ../cli_sysmon.py:164 ../modals/disk_usage_modal.py:71
 msgid "Disk Usage"
-msgstr "Diskbruk"
+msgstr "Plattenauslastung"
 
-#: ../cli_monitor.py:131 ../cli_monitor.py:179
-#: ../modals/temperature_modal.py:45
+#: ../cli_sysmon.py:133 ../cli_sysmon.py:181 ../modals/temperature_modal.py:45
 msgid "Temperature Sensors"
-msgstr "Temperatursensorer"
+msgstr "Wärmesensoren"
 
-#: ../cli_monitor.py:142 ../modals/temperature_modal.py:103
+#: ../cli_sysmon.py:144 ../modals/temperature_modal.py:103
 #, python-brace-format
 msgid "{current}°C (high = {high}°C, critical = {critical}°C)"
-msgstr "{current}°C (høy = {high}°C, kritisk = {critical}°C)"
+msgstr "{current}°C (höchste = {high}°C, kritischer = {critical}°C)"
 
-#: ../cli_monitor.py:222
+#: ../cli_sysmon.py:224
 msgid "<Ctrl-C> to quit"
-msgstr "<Ctrl-C> for å avslutte"
+msgstr "<Strg-C> zum Beenden"
 
-#: ../cli_monitor.py:232
+#: ../cli_sysmon.py:234
 msgid "System monitor: display CPU usage/temperature, memory usage, disk usage"
-msgstr "Systemmonitor: Vis CPU-bruk/temperatur, minnebruk, diskbruk"
+msgstr ""
+"Systemmonitor: Zeigt CPU-Auslastung/-Temperatur, Speichernutzung und "
+"Festplattennutzung an"
 
-#: ../cli_monitor.py:235
+#: ../cli_sysmon.py:237
 msgid ""
 "By default, this program will use the same language as that selected for the "
 "GUI application. To override it, use the '-l' option. To quit, press <Ctrl-"
 "C>."
 msgstr ""
-"Som standard vil dette programmet bruke samme språk som det som er valgt for "
-"GUI-applikasjonen. For å overstyre det, bruk alternativet '-l'. For å "
-"avslutte, trykk <Ctrl-C>."
+"Standardmäßig verwendet dieses Programm dieselbe Sprache wie die für die GUI-"
+"Anwendung ausgewählte Sprache. Um es zu überschreiben, verwenden Sie die "
+"Option „-l“. Zum Beenden drücken Sie <Strg-C>."
 
-#: ../cli_monitor.py:242
+#: ../cli_sysmon.py:244
 msgid "Options"
-msgstr "Valg"
+msgstr "Optionen"
 
-#: ../cli_monitor.py:245
+#: ../cli_sysmon.py:247
 msgid "show this help message and exit"
-msgstr "vis denne hjelpemeldingen og avslutt"
+msgstr "diese Meldung anzeigen und beenden"
 
-#: ../cli_monitor.py:250
+#: ../cli_sysmon.py:252
 msgid "show program's version number and exit"
-msgstr "vis programmets versjonsnummer og avslutt"
+msgstr "Versionsnummer der Anwendung anzeigen und beenden"
 
-#: ../cli_monitor.py:254
+#: ../cli_sysmon.py:256
 #, python-format
 msgid "time between screen refreshes (in seconds, default=%(default)s)"
-msgstr "tid mellom skjermoppdateringer (i sekunder, standard=%(default)s)"
+msgstr ""
+"Zeit zwischen Bildschirmaktualisierungen (in Sekunden, Standard=%(default)s)"
 
-#: ../cli_monitor.py:258
+#: ../cli_sysmon.py:260
 msgid "the language to use for display"
-msgstr "språket som skal brukes for visning"
+msgstr "die Sprache, die für die Anzeige verwendet werden soll"
 
-#: ../cli_monitor.py:260
+#: ../cli_sysmon.py:262
 msgid "Display Details"
-msgstr "Skjermdetaljene"
+msgstr "Anzeigedetails"
 
-#: ../cli_monitor.py:264
+#: ../cli_sysmon.py:266
 msgid "show disk details (default)"
-msgstr "vis diskdetaljer (standard)"
+msgstr "Festplattendetails anzeigen (Standard)"
 
-#: ../cli_monitor.py:268
+#: ../cli_sysmon.py:270
 msgid "show temperature details"
-msgstr "vis temperaturdetaljer"
+msgstr "Temperaturdetails anzeigen"
 
-#: ../cli_monitor.py:272
+#: ../cli_sysmon.py:274
 msgid "show both disk and temperature details"
-msgstr "vis både disk- og temperaturdetaljer"
+msgstr "Zeigt sowohl Festplattendetails als auch Temperaturdetails an"
 
-#: ../cli_monitor.py:276
+#: ../cli_sysmon.py:278
 msgid "show no details, only the header"
-msgstr "vis ingen detaljer, bare overskriften"
+msgstr "Keine Details anzeigen, nur die Kopfzeile"
 
-#: ../desktop_menu.py:48
+#: ../desktop_menu.py:57
 msgid "Error creating desktop menu item"
-msgstr "Feil under oppretting av skrivebordsmenyelement"
+msgstr "Fehler beim Erstellen des Desktop-Menüeinträg"
 
-#: ../desktop_menu.py:49
+#: ../desktop_menu.py:58
 msgid ""
 "System Monitor (sysmon) must be installed in a virtual environment in order "
 "to create a desktop menu entry."
 msgstr ""
-"Systemmonitor (sysmon) må installeres i et virtuelt miljø for å opprette en "
-"skrivebordsmenyoppføring."
+"System Monitor (sysmon) muss in einer virtuellen Umgebung installiert "
+"werden, um einen Desktop-Menüeintrag zu erstellen."
 
-#: ../font_utils.py:74 ../modals/font_modal.py:171
+#: ../font_utils.py:153 ../modals/font_modal.py:171
 msgid "Bold"
-msgstr "Fet"
+msgstr "Fett"
 
-#: ../font_utils.py:76 ../modals/font_modal.py:175
+#: ../font_utils.py:155 ../modals/font_modal.py:175
 msgid "Italic"
 msgstr "Kursiv"
 
-#: ../font_utils.py:78 ../modals/font_modal.py:179
+#: ../font_utils.py:157 ../modals/font_modal.py:179
 msgid "Bold Italic"
-msgstr "Fet kursiv"
+msgstr "Fett Kursiv"
+
+#: ../font_utils.py:171 ../modals/font_modal.py:193
+msgid "Underline"
+msgstr "Unterstrichen"
 
-#: ../modals/about_modal.py:93
+#: ../font_utils.py:172 ../modals/font_modal.py:197
+msgid "Overstrike"
+msgstr "Durchgestrichen"
+
+#: ../modals/_base_modal.py:158
+msgid "Close"
+msgstr "Schließen"
+
+#: ../modals/_base_modal.py:168
+msgid "Cancel"
+msgstr "Abbrechen"
+
+#: ../modals/_base_modal.py:169
+msgid "OK"
+msgstr "Verstanden"
+
+#: ../modals/about_modal.py:115
 msgid "About {}"
-msgstr "Om {}"
+msgstr "Über {}"
 
-#: ../modals/about_modal.py:125
+#: ../modals/about_modal.py:147
 msgid "Translators"
-msgstr "Oversettere"
+msgstr "Übersetzer"
 
-#: ../modals/about_modal.py:131
+#: ../modals/about_modal.py:153
 msgid "License"
-msgstr "Lisens"
+msgstr "Lizenz"
 
-#: ../modals/about_modal.py:149
+#: ../modals/about_modal.py:171
 msgid "Version {}"
-msgstr "Versjon {}"
+msgstr "Version {}"
 
-#: ../modals/about_modal.py:155
+#: ../modals/about_modal.py:177
 msgid "Source Code"
-msgstr "Kildekode"
+msgstr "Quellcode"
 
-#: ../modals/about_modal.py:220
+#: ../modals/about_modal.py:242
 msgid "Full license text available here"
-msgstr "Full lisenstekst tilgjengelig her"
-
-#: ../modals/_base_modal.py:158 ../widgets/button_mixin.py:113
-msgid "Close"
-msgstr "Lukk"
-
-#: ../modals/_base_modal.py:168 ../widgets/button_mixin.py:110
-msgid "Cancel"
-msgstr "Avbryt"
+msgstr "Den vollständigen Lizenztext finden Sie hier"
 
-#: ../modals/_base_modal.py:169 ../widgets/button_mixin.py:107
-msgid "OK"
-msgstr "OK"
-
-#: ../modals/cpu_modal.py:70
+#: ../modals/cpu_modal.py:82
 msgid "per-core CPU Usage"
-msgstr "prosessorbruk per kjerne"
+msgstr "CPU-Auslastung pro Kern"
 
-#: ../modals/cpu_modal.py:76
+#: ../modals/cpu_modal.py:88
 msgid "per-core CPU Frequency (in MHz)"
-msgstr "prosessorfrekvens per kjerne (i MHz)"
+msgstr "CPU-Frequenz pro Kern (in MHz)"
 
-#: ../modals/cpu_modal.py:91 ../modals/cpu_modal.py:111
+#: ../modals/cpu_modal.py:103 ../modals/cpu_modal.py:123
 msgid "CPU #{}"
-msgstr "Prosessor #{}"
+msgstr "CPU #{}"
 
 #: ../modals/font_modal.py:74
 msgid "Choose Font"
-msgstr "Velg skrift"
+msgstr "Schriftart wählen"
 
 #: ../modals/font_modal.py:132
 msgid "Font"
-msgstr "Skrift"
+msgstr "Schriftart"
 
 #: ../modals/font_modal.py:159
 msgid "Style"
 msgstr "Stil"
 
 #: ../modals/font_modal.py:167
 msgid "Regular"
-msgstr "Vanlig"
+msgstr "Normal"
 
 #: ../modals/font_modal.py:186
 msgid "Effects"
-msgstr "Effekter"
-
-#: ../modals/font_modal.py:193
-msgid "Underline"
-msgstr "Understrek"
-
-#: ../modals/font_modal.py:197
-msgid "Overstrike"
-msgstr "Gjennomstrek"
+msgstr "Effekte"
 
 #: ../modals/font_modal.py:203
 msgid "Size"
-msgstr "Størrelse"
+msgstr "Größe"
 
 #: ../modals/font_modal.py:214
 msgid "Preview"
-msgstr "Forhåndsvis"
+msgstr "Vorschau"
 
 #: ../modals/mem_usage_modal.py:54
 msgid "Memory Statistics"
-msgstr "Minnestatistikk"
+msgstr "Speicherstatistik"
 
 #: ../modals/mem_usage_modal.py:58
 msgid "Virtual Memory"
-msgstr "Virtuelt minne"
+msgstr "Virtueller Speicher"
 
 #: ../modals/settings_modal.py:31
 msgid "Light"
-msgstr "Lys"
+msgstr "Licht"
 
 #: ../modals/settings_modal.py:32
 msgid "Dark"
-msgstr "Mørk"
+msgstr "Dunkel"
 
 #: ../modals/settings_modal.py:33
 msgid "Same as System"
-msgstr "Samme som systemet"
+msgstr "Gleiches wie System"
 
-#: ../modals/settings_modal.py:106
+#: ../modals/settings_modal.py:107
 msgid "Language"
-msgstr "Språk"
+msgstr "Sprache"
 
-#: ../modals/settings_modal.py:121
+#: ../modals/settings_modal.py:122
 msgid "Theme"
-msgstr "Drakt"
+msgstr "Thema"
 
-#: ../modals/settings_modal.py:139
+#: ../modals/settings_modal.py:140
 msgid "Always on top"
-msgstr "Alltid på topp"
+msgstr "Immer im Vordergrund"
 
-#: ../modals/settings_modal.py:146
+#: ../modals/settings_modal.py:147
 msgid "Regular Font"
-msgstr "Vanlig skrift"
+msgstr "Normal Schriftart"
 
-#: ../modals/settings_modal.py:156
+#: ../modals/settings_modal.py:157
 msgid "Monospace Font"
-msgstr "Fastbreddeskrift"
+msgstr "Dicktengleiche Schrift"
 
-#: ../modals/settings_modal.py:166
+#: ../modals/settings_modal.py:167
 msgid "Add to desktop menu system"
-msgstr "Legg til skrivebordets menysystem"
+msgstr "Zum Desktop-Menüsystem hinzufügen"
 
-#: ../modals/settings_modal.py:191 ../modals/settings_modal.py:210
+#: ../modals/settings_modal.py:192 ../modals/settings_modal.py:211
 msgid "Select a font"
-msgstr "Velg en skrift"
-
-#: ../widgets/button_mixin.py:116
-msgid "Yes"
-msgstr "Ja"
+msgstr "Schriftart auswählen"
 
-#: ../widgets/button_mixin.py:119
-msgid "No"
-msgstr "Nei"
+#: ../widgets/edit_menu.py:65 ../widgets/edit_menu.py:94
+#: ../widgets/edit_menu.py:97
+msgid "Cut"
+msgstr "Ausschneiden"
 
-#: ../widgets/button_mixin.py:122
-msgid "Retry"
-msgstr "Prøv igjen"
-
-#: ../widgets/edit_menu.py:51
+#: ../widgets/edit_menu.py:65
 msgid "Ctrl+X"
-msgstr "Ctrl+X"
+msgstr "Strg+X"
+
+#: ../widgets/edit_menu.py:69
+msgid "Copy"
+msgstr "Kopieren"
 
-#: ../widgets/edit_menu.py:55
+#: ../widgets/edit_menu.py:69
 msgid "Ctrl+C"
-msgstr "Ctrl+C"
+msgstr "Strg+C"
+
+#: ../widgets/edit_menu.py:73 ../widgets/edit_menu.py:95
+#: ../widgets/edit_menu.py:98
+msgid "Paste"
+msgstr "Einfügen"
 
-#: ../widgets/edit_menu.py:59
+#: ../widgets/edit_menu.py:73
 msgid "Ctrl+V"
-msgstr "Ctrl+V"
+msgstr "Strg+V"
 
-#: ../widgets/meters.py:119
-msgid "Click for per-CPU usage"
-msgstr "Klikk for bruk per prosessor"
+#: ../widgets/edit_menu.py:78
+msgid "Select All"
+msgstr "Alles auswählen"
 
-#: ../widgets/meters.py:139
-msgid "{} :: CPU Details"
-msgstr "{} :: Prosessordetaljer"
+#~ msgid "Yes"
+#~ msgstr "Ja"
 
-#: ../widgets/meters.py:157
-msgid "Click for detailed temperature readings"
-msgstr "Klikk for detaljerte temperaturavlesninger"
+#~ msgid "No"
+#~ msgstr "Nein"
 
-#: ../widgets/meters.py:172
-msgid "{} :: Temperature Details"
-msgstr "{} :: Temperaturdetaljer"
+#~ msgid "Retry"
+#~ msgstr "Wiederholen"
 
-#: ../widgets/meters.py:190
-msgid "Click for detailed memory statistics"
-msgstr "Klikk for detaljert minnestatistikk"
+#~ msgid "Click for per-CPU usage"
+#~ msgstr "Klicken Sie hier, um die Nutzung pro CPU anzuzeigen"
 
-#: ../widgets/meters.py:204
-msgid "{} :: Memory Usage"
-msgstr "{} :: Minnebruk"
+#~ msgid "{} :: CPU Details"
+#~ msgstr "{} :: CPU-Details"
 
-#: ../widgets/meters.py:219
-msgid "Disk Usage: /"
-msgstr "Diskbruk: /"
+#~ msgid "Click for detailed temperature readings"
+#~ msgstr "Klicken Sie hier, um detaillierte Temperaturmessungen anzuzeigen"
 
-#: ../widgets/meters.py:222
-msgid "Click for usage details of each mount point"
-msgstr "Klikk for detaljert for hvert monteringspunkt"
+#~ msgid "{} :: Temperature Details"
+#~ msgstr "{} :: Temperaturdetails"
 
-#: ../widgets/meters.py:236
-msgid "{} :: Disk Usage"
-msgstr "{} :: Diskbruk"
+#~ msgid "Click for detailed memory statistics"
+#~ msgstr "Klicken Sie hier, um detaillierte RAM-Statistiken anzuzeigen"
 
-#~ msgid "Cut"
-#~ msgstr "Klipp ut"
+#~ msgid "{} :: Memory Usage"
+#~ msgstr "{} :: RAM-Auslastung"
 
-#~ msgid "Copy"
-#~ msgstr "Kopier"
+#~ msgid "Disk Usage: /"
+#~ msgstr "Plattenauslastung: /"
 
-#~ msgid "Paste"
-#~ msgstr "Lim inn"
+#~ msgid "Click for usage details of each mount point"
+#~ msgstr ""
+#~ "Klicken Sie hier, um Nutzungsinformationen für jeden Mountpunkt anzuzeigen"
 
-#~ msgid "Select All"
-#~ msgstr "Velg alt"
+#~ msgid "{} :: Disk Usage"
+#~ msgstr "{} :: Plattenauslastung"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/locale/nb_NO/LC_MESSAGES/argparse.mo` & `sysmon_pytk-0.5.1/sysmon_pytk/locale/nb_NO/LC_MESSAGES/argparse.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: i18nparse\n"
 "Report-Msgid-Bugs-To: stacey.belle.rose@gmail.com\n"
-"PO-Revision-Date: 2024-03-21 15:13-0500\n"
+"PO-Revision-Date: 2024-04-03 08:01-0500\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language-Team: Norwegian Bokmål\n"
 "Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -25,28 +25,37 @@
 
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "tvetydig valg: %(option)s kan matche %(matches)s"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" med modus %r"
 
+msgid "argument %(argument_name)s: %(message)s"
+msgstr "argumenter %(argument_name)s: %(message)s"
+
 msgid "can't open '%(filename)s': %(error)s"
 msgstr "kan ikke åpne '%(filename)s': %(error)s"
 
 msgid "cannot have multiple subparser arguments"
 msgstr "kan ikke ha flere underfortolkningsargumenter"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "kan ikke flette handlinger - to grupper heter %r"
 
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "konflikterende valgstreng: %s"
 msgstr[1] "konflikterende valgstrenger: %s"
 
+msgid "conflicting subparser alias: %s"
+msgstr "konflikterende underfortolkeralias: %s"
+
+msgid "conflicting subparser: %s"
+msgstr "konflikterende underfortolker: %s"
+
 msgid "dest= is required for options like %r"
 msgstr "dest= er påkrevd for valg som %r"
 
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "forventet %s argument"
 msgstr[1] "forventet %s argumenter"
@@ -85,14 +94,17 @@
 
 msgid "one of the arguments %s is required"
 msgstr "ett av argumentene %s kreves"
 
 msgid "optional arguments"
 msgstr "valgfrie argumenter"
 
+msgid "options"
+msgstr "valg"
+
 msgid "positional arguments"
 msgstr "posisjonelle argumenter"
 
 msgid "show this help message and exit"
 msgstr "vis denne hjelpemeldingen og avslutt"
 
 msgid "the following arguments are required: %s"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/__init__.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 
 """
 Modal dialogs.
 """
 
-from .about_modal import AboutDialog
+from . import messagebox
+from ._base_modal import ModalDialog
+from .about_modal import AboutDialog, AboutMetadata, LicenseMetadata
 from .cpu_modal import CpuDialog
 from .disk_usage_modal import DiskUsageDialog
 from .font_modal import FontChooser
 from .mem_usage_modal import MemUsageDialog
 from .settings_modal import SettingsDialog
 from .temperature_modal import TempDetailsDialog
 
 __all__ = [
+    "ModalDialog",
     "AboutDialog",
+    "AboutMetadata",
+    "LicenseMetadata",
     "CpuDialog",
     "DiskUsageDialog",
     "FontChooser",
     "MemUsageDialog",
     "SettingsDialog",
-    "TempDetailsDialog"
+    "TempDetailsDialog",
+    "messagebox"
 ]
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/_base_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/_base_modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from abc import ABCMeta, abstractmethod
 from tkinter import ttk
 from typing import TYPE_CHECKING, final
 
 from .._common import INTERNAL_PAD
 from ..app_locale import get_translator
 from ..style_manager import StyleManager
-from ..widgets.button_mixin import ButtonDefinition, ButtonMixin
+from ..widgets.buttons import ButtonDefinition, ButtonMixin
 
 if TYPE_CHECKING:
     from tkinter import Misc
 
 _ = get_translator()
 
 # These lint errors don't make sense for GUI widgets, so are disabled here.
@@ -61,15 +61,15 @@
         ----------
         parent : Misc, optional
             The parent widget.
         title : str, optional
             The title to display in the window title bar.
         iconpath : str, optional
             The path to the icon to display in the window title bar.
-        class_ : str, default: "ModalDialog"
+        class_ : str, default = "ModalDialog"
             The class name of this modal dialog, used with the option database
             for styling.
         """
         super().__init__(parent, class_=class_)
         self.parent = parent
         self.iconpath = iconpath
         self._events: list[str] = []
@@ -87,15 +87,15 @@
         top.columnconfigure(0, weight=1)
         self.make_modal()
         self.wait_window()
 
     @final
     def load_fonts(self) -> None:
         """
-        Load the standard fonts from the StyleManager.
+        Load the standard fonts from the `sysmon_pytk.style_manager.StyleManager`.
         """
         self.base_font = StyleManager.get_base_font()
         self.large_font = StyleManager.get_large_font()
         self.bold_font = StyleManager.get_bold_font()
         self.fixed_font = StyleManager.get_fixed_font()
 
     @final
@@ -169,15 +169,15 @@
             ButtonDefinition(text=_("OK"), command=self.save_and_dismiss),
         ]
         self.add_buttons(self.internal_frame, buttons=buttons, default=1)
 
     @final
     def add_sizegrip(self) -> None:
         """
-        Add a Sizegrip widget to the bottom row of the modal dialog.
+        Add a ttk.Sizegrip widget to the bottom row of the modal dialog.
         """
         max_columns, max_rows = self.internal_frame.grid_size()
         ttk.Sizegrip(self.internal_frame).grid(
             row=max_rows, column=max_columns-1, sticky=tk.SE, padx=INTERNAL_PAD/2,
             pady=INTERNAL_PAD/2
         )
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/about_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/about_modal.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,31 +29,41 @@
 @dataclasses.dataclass
 class LicenseMetadata:
     """
     Metadata about the license used by the application.
     """
 
     full_license: str
+    """The full license text for the application. Can be an empty string."""
     license_name: str
+    """The name of the license used by the application."""
     license_url: str
+    """A URL pointing to an online copy of the license text."""
 
 
 @dataclasses.dataclass
 class AboutMetadata:
     """
     Metadata about the application.
     """
 
     app_name: str
+    """The application name."""
     version: str
+    """The current version of the application."""
     author: str
+    """The author of the application."""
     copyright_year: str
+    """The copyright year of the application."""
     description: str
+    """A description of the application."""
     url: str
+    """A URL that points to the source code repository for the application."""
     license: LicenseMetadata | None = None
+    """License metadata about the application."""
 
     def get_copyright_text(self) -> str:
         """
         Build the copyright text based on year and author.
         """
         if self.author:
             if self.copyright_year:
@@ -85,14 +95,26 @@
     logo : PhotoImage
         A logo to be displayed.
     """
 
     def __init__(
         self, parent: Misc | None, about: AboutMetadata, iconpath: str | None = None
     ) -> None:
+        """
+        Construct a modal dialog containing metadata about the application.
+
+        Parameters
+        ----------
+        parent : Misc, optional
+            The parent widget.
+        about : AboutMetadata
+            The metadata about the application.
+        iconpath : str, optional
+            The path to the icon to display in the window title bar.
+        """
         self.about = about
         title = _("About {}").format(about.app_name).strip()
         self.logo = tk.PhotoImage(file=get_full_path("images/icon-lg.png"))
         super().__init__(parent, title=title, iconpath=iconpath, class_="AboutBox")
 
     def update_screen(self) -> None:
         """
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/cpu_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/cpu_modal.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,30 @@
         The number of logical CPUs in the system.
     """
 
     MAX_COLUMNS = 4
 
     def __init__(
         self, parent: Misc | None = None, *, title: str | None = None,
-        iconpath: str | None = None, class_: str = "ModalDialog"
+        iconpath: str | None = None
     ) -> None:
+        """
+        Construct a modal dialog containing information about CPU usage.
+
+        Parameters
+        ----------
+        parent : Misc, optional
+            The parent widget.
+        title : str, optional
+            The title to display in the window title bar.
+        iconpath : str, optional
+            The path to the icon to display in the window title bar.
+        """
         self._max_used_column = 0
-        super().__init__(parent, title=title, iconpath=iconpath, class_=class_)
+        super().__init__(parent, title=title, iconpath=iconpath)
 
     def on_save(self) -> None:
         """
         Save what was entered in the modal dialog.
 
         This dialog does not need a save feature.
         """
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/disk_usage_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/disk_usage_modal.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,18 +26,30 @@
 class DiskUsageDialog(ModalDialog):
     """
     Display disk usage in a modal dialog.
     """
 
     def __init__(
         self, parent: Misc | None = None, *, title: str | None = None,
-        iconpath: str | None = None, class_: str = "ModalDialog"
+        iconpath: str | None = None
     ) -> None:
+        """
+        Construct a modal dialog containing information about disk usage.
+
+        Parameters
+        ----------
+        parent : Misc, optional
+            The parent widget.
+        title : str, optional
+            The title to display in the window title bar.
+        iconpath : str, optional
+            The path to the icon to display in the window title bar.
+        """
         self._update_job: str | None = None
-        super().__init__(parent, title=title, iconpath=iconpath, class_=class_)
+        super().__init__(parent, title=title, iconpath=iconpath)
 
     def on_save(self) -> None:
         """
         Save what was entered in the modal dialog.
 
         This dialog does not need a save feature.
         """
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/font_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/font_modal.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 Application font settings modal dialog.
 """
 
 from __future__ import annotations
 
 import tkinter as tk
 from tkinter import font, ttk
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING
 
 from .. import _common
 from ..app_locale import get_translator
-from ..settings import FontDescription
+from ..font_utils import FontDescription, FontSlant, FontStyle, FontWeight
 from ..style_manager import StyleManager
 from ..widgets import ScaleSpinner
 from ._base_modal import ModalDialog
 
 if TYPE_CHECKING:
     from tkinter import Event, Listbox, Misc
 
@@ -77,23 +77,23 @@
         self.fontchoices.sort()
         self.fontsize = tk.IntVar()
         self.fontstyle = tk.StringVar()
         self.underline = tk.BooleanVar()
         self.overstrike = tk.BooleanVar()
         if self.current_font is not None:
             self.fontname: str | None = self.current_font.family
-            self.fontstyle.set(self.current_font.get_style())
+            self.fontstyle.set(str(self.current_font.get_style()))
             self.fontsize.set(self.current_font.size)
             self.underline.set(self.current_font.underline)
             self.overstrike.set(self.current_font.overstrike)
             self.preview_font = self.current_font.get_font()
         else:
             # default selections
             self.fontname = None
-            self.fontstyle.set(FontDescription.REGULAR)
+            self.fontstyle.set(str(FontStyle.REGULAR))
             self.fontsize.set(12)
             self.underline.set(False)
             self.overstrike.set(False)
             self.preview_font = self.base_font
         self.fontsize.trace_add("write", self._update_preview)
         self.fontstyle.trace_add("write", self._update_preview)
         self.underline.trace_add("write", self._update_preview)
@@ -160,27 +160,27 @@
             )
         )
         styleframe.grid(
             row=0, column=1, sticky=tk.NSEW,
             padx=_common.INTERNAL_PAD, pady=_common.INTERNAL_PAD
         )
         ttk.Radiobutton(
-            styleframe, text=_("Regular"), value=FontDescription.REGULAR,
+            styleframe, text=_("Regular"), value=FontStyle.REGULAR.value,
             variable=self.fontstyle
         ).grid(row=1, padx=_common.INTERNAL_PAD, sticky=tk.NSEW)
         ttk.Radiobutton(
-            styleframe, text=_("Bold"), value=FontDescription.BOLD,
+            styleframe, text=_("Bold"), value=FontStyle.BOLD.value,
             variable=self.fontstyle
         ).grid(row=2, padx=_common.INTERNAL_PAD, sticky=tk.NSEW)
         ttk.Radiobutton(
-            styleframe, text=_("Italic"), value=FontDescription.ITALIC,
+            styleframe, text=_("Italic"), value=FontStyle.ITALIC.value,
             variable=self.fontstyle
         ).grid(row=3, padx=_common.INTERNAL_PAD, sticky=tk.NSEW)
         ttk.Radiobutton(
-            styleframe, text=_("Bold Italic"), value=FontDescription.BOLD_ITALIC,
+            styleframe, text=_("Bold Italic"), value=FontStyle.BOLD_ITALIC.value,
             variable=self.fontstyle
         ).grid(row=4, padx=_common.INTERNAL_PAD, sticky=tk.NSEW)
 
         effectsframe = ttk.LabelFrame(
             self.internal_frame,
             labelwidget=ttk.Label(
                 self.internal_frame, text=_("Effects"), font=self.base_font
@@ -223,40 +223,44 @@
         previewframe.grid_propagate(False)
         ttk.Label(
             previewframe, text=self.PREVIEW_TEXT, font=self.preview_font,
             anchor=tk.CENTER
         ).grid(sticky=tk.NSEW)
 
     def _update_preview(self, *_args) -> None:
+        try:
+            fontstyle = FontStyle(self.fontstyle.get())
+        except ValueError:
+            fontstyle = FontStyle.REGULAR
         if self.fontname:
             self.preview_font.configure(
                 family=self.fontname,
                 size=self.fontsize.get(),
-                weight="bold" if self.fontstyle.get() in {"b", "bi"} else "normal",
-                slant="italic" if self.fontstyle.get() in {"i", "bi"} else "roman",
+                weight=fontstyle.get_weight(),
+                slant=fontstyle.get_slant(),
                 underline=self.underline.get(),
                 overstrike=self.overstrike.get()
             )
 
     def _on_select(self, event: Event[Listbox]) -> None:
         value = event.widget.get(event.widget.curselection()[0])
         self.fontname = value
         self._update_preview()
 
     def on_save(self) -> None:
         """
-        Update `current_font` based on currently selected options.
+        Update `self.current_font` based on currently selected options.
         """
-        weight: Literal["bold", "normal"] = "normal"
-        slant: Literal["italic", "roman"] = "roman"
-        if self.fontstyle.get() == FontDescription.BOLD:
+        weight: FontWeight = "normal"
+        slant: FontSlant = "roman"
+        if self.fontstyle.get() == FontStyle.BOLD:
             weight = "bold"
-        elif self.fontstyle.get() == FontDescription.ITALIC:
+        elif self.fontstyle.get() == FontStyle.ITALIC:
             slant = "italic"
-        elif self.fontstyle.get() == FontDescription.BOLD_ITALIC:
+        elif self.fontstyle.get() == FontStyle.BOLD_ITALIC:
             weight = "bold"
             slant = "italic"
         self.current_font = FontDescription(
             family=self.fontname,
             size=self.fontsize.get(),
             weight=weight,
             slant=slant,
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/mem_usage_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/mem_usage_modal.py`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/messagebox.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/messagebox/mb_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 Themed message boxes.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from .messagebox_base import MessageBox, MessageBoxButtonSet, MessageBoxIcon
+from .base import MessageBox, MessageBoxButtonSet, MessageBoxIcon
 
 if TYPE_CHECKING:
     from tkinter import Misc
 
-    from ..widgets.button_mixin import ButtonName
+    from ...widgets.buttons import ButtonName
 
 
 def show_message(parent: Misc | None, title: str, message: str) -> ButtonName:
     """
     Display a message box to show a message.
     """
     return MessageBox(
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/messagebox_base.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/messagebox/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,44 +12,54 @@
 
 import tkinter as tk
 from contextlib import suppress
 from enum import IntEnum
 from tkinter import ttk
 from typing import Callable
 
-from .._common import INTERNAL_PAD
-from ..app_locale import get_translator
-from ..file_utils import get_full_path
-from ..widgets.button_mixin import ButtonMixin, ButtonName
+from ..._common import INTERNAL_PAD
+from ...app_locale import get_translator
+from ...file_utils import get_full_path
+from ...widgets.buttons import ButtonMixin, ButtonName
 
 _ = get_translator()
 
 
 class MessageBoxIcon(IntEnum):
     """
     Standard message box icons.
     """
 
     INFO = 1
+    """Message box displays the INFO icon."""
     QUESTION = 2
+    """Message box displays the QUESTION icon."""
     WARNING = 3
+    """Message box displays the WARNING icon."""
     ERROR = 4
+    """Message box displays the ERROR icon."""
 
 
 class MessageBoxButtonSet(IntEnum):
     """
     Standard sets of buttons to use in a message box.
     """
 
     OK = 1
+    """Message box contains OK button."""
     OKCANCEL = 2
+    """Message box contains OK and Cancel buttons."""
     CLOSE = 3
+    """Message box contains Close button."""
     YESNO = 4
+    """Message box contains Yes and No buttons."""
     YESNOCANCEL = 5
+    """Message box contains Yes, No, and Cancel buttons."""
     RETRYCANCEL = 6
+    """Message box contains Retry and Cancel buttons."""
 
 
 MESSAGE_BOX_ICON_PATHS = {
     MessageBoxIcon.INFO: "images/custom/dialog-information.png",
     MessageBoxIcon.QUESTION: "images/custom/dialog-question.png",
     MessageBoxIcon.WARNING: "images/custom/dialog-warning.png",
     MessageBoxIcon.ERROR: "images/custom/dialog-error.png"
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/settings_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/settings_modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # pragma pylint: disable=too-many-instance-attributes
 
 THEMES = {
     _("Light"): "Light",
     _("Dark"): "Dark",
     _("Same as System"): "Same as System"
 }
+"""The translated names of the application themes."""
 
 
 class SettingsDialog(ModalDialog):
     """
     Manage application settings in a modal dialog.
 
     Attributes
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/modals/temperature_modal.py` & `sysmon_pytk-0.5.1/sysmon_pytk/modals/temperature_modal.py`

 * *Files identical despite different names*

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/settings.py` & `sysmon_pytk-0.5.1/sysmon_pytk/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 Application settings.
 """
 
 from __future__ import annotations
 
 from configparser import ConfigParser
 from pathlib import Path
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING
 
-from .font_utils import MAIN_FONT_FAMILY, FontDescription
+from .font_utils import MAIN_FONT_FAMILY, FontDescription, FontSlant, FontWeight
 
 if TYPE_CHECKING:
     from tkinter.font import Font
 
 
 class FontSettings:  # pylint: disable=too-many-instance-attributes
     """
@@ -26,14 +26,24 @@
     config : ConfigParser
         A configuration file parser.
     section : str
         Which section of the configuration file to use.
     """
 
     def __init__(self, config: ConfigParser, section: str) -> None:
+        """
+        Construct a Font Settings manager.
+
+        Parameters
+        ----------
+        config : ConfigParser
+            A configuration file parser.
+        section : str
+            Which section of the configuration file to use.
+        """
         self.config = config
         self.section = section
 
     @property
     def name(self) -> str:
         """
         The font name to use in the application.
@@ -52,29 +62,29 @@
         return self.config[self.section].getint("size", fallback=12)
 
     @size.setter
     def size(self, fontsize: int) -> None:
         self.config[self.section]["size"] = f"{fontsize}"
 
     @property
-    def weight(self) -> Literal["bold", "normal"]:
+    def weight(self) -> FontWeight:
         """
         The font weight to use in the application.
         """
         weight = self.config[self.section].get("weight", fallback="normal")
         if weight == "bold":
             return "bold"
         return "normal"
 
     @weight.setter
     def weight(self, weight: str) -> None:
         self.config[self.section]["weight"] = weight
 
     @property
-    def slant(self) -> Literal["italic", "roman"]:
+    def slant(self) -> FontSlant:
         """
         The font slant to use in the application.
         """
         slant = self.config[self.section].get("slant", fallback="roman")
         if slant == "italic":
             return "italic"
         return "roman"
@@ -155,16 +165,24 @@
         A configuration file parser.
     regular_font : FontSettings
         Font settings for the regular font.
     fixed_font : FontSettings
         Font settings for the monospace font.
     """
 
-    def __init__(self, settings_file: str) -> None:
-        self.filename = settings_file
+    def __init__(self, filename: str) -> None:
+        """
+        Construct a Settings manager.
+
+        Parameters
+        ----------
+        filename : str
+            The full path to the configuration file.
+        """
+        self.filename = filename
         self.config = ConfigParser()
         self.read_settings()
         self.regular_font = FontSettings(self.config, "font")
         self.fixed_font = FontSettings(self.config, "fixedfont")
 
     def read_settings(self) -> None:
         """
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/style_manager.py` & `sysmon_pytk-0.5.1/sysmon_pytk/style_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 import re
 import tkinter as tk
 from tkinter import font, ttk
 from typing import TYPE_CHECKING, TypeVar
 
 import darkdetect
 
+import azure
+
 from . import font_utils
-from .file_utils import get_full_path
 
 if TYPE_CHECKING:
     from tkinter.font import Font
 
     from .settings import Settings
 
 T = TypeVar("T")
@@ -84,25 +85,34 @@
         return darkdetect.isDark()
 
     @classmethod
     def init_theme(cls, root: tk.Tk, settings: Settings) -> None:
         """
         Initialize theme and styles for the application.
         """
-        root.tk.call("source", get_full_path("../azure/azure.tcl"))
+        azure.init_theme(root)  # pylint: disable=W0212
         cls.update_by_dark_mode(root, settings)
         cls.init_fonts(settings)
         root.option_add("*TCombobox*Listbox.font", "TkDefaultFont")
         root.option_add("*tearOff", False)  # Fix menus
         root.bind_class("Menu", "<<ThemeChanged>>", cls.update_menu)
 
     @classmethod
     def init_fonts(cls, settings: Settings) -> None:
         """
         Initialize the fonts to be used.
+
+        The following tk named fonts are updated based on Settings:
+
+        * TkDefaultFont - set to Regular Font from Settings
+        * TkTextFont - set to Regular Font from Settings
+        * TkMenuFont - set to Regular Font from Settings
+        * TkFixedFont - set to Fixed Font from Settings
+
+        In addition, widgets are configured to use TkDefaultFont.
         """
         base_font = font.nametofont("TkDefaultFont")
         text_font = font.nametofont("TkTextFont")
         menu_font = font.nametofont("TkMenuFont")
         fixed_font = font.nametofont("TkFixedFont")
         if settings.regular_font.name:
             settings.regular_font.configure_font(base_font)
@@ -126,35 +136,43 @@
         style.configure("System.TLabel", font="TkDefaultFont")
         style.configure("URL.TLabel", foreground="#0066cc")
 
     @classmethod
     def update_by_dark_mode(cls, root: tk.Tk, settings: Settings) -> None:
         """
         Update styles based on dark mode.
+
+        Colors are updated for various styles and widgets:
+
+        * Safe.TLabel style (green)
+        * Warn.TLabel style (yellow)
+        * Alert.TLabel style (red)
+        * Combobox Listbox background (grey)
         """
         dark_mode = cls.get_dark_mode(settings)
-        root.tk.call("set_theme", "dark" if dark_mode else "light")
+        azure.set_theme("dark" if dark_mode else "light", root)
         root.event_generate("<<ThemeChanged>>")
         style = ttk.Style()
         if dark_mode:
             style.configure("Safe.TLabel", foreground="#00aa00")
             style.configure("Warn.TLabel", foreground="#ffff22")
             style.configure("Alert.TLabel", foreground="#ff2222")
             root.option_add("*TCombobox*Listbox.background", "#444444")
         else:
             style.configure("Safe.TLabel", foreground="#009900")
             style.configure("Warn.TLabel", foreground="#aaaa00")
             style.configure("Alert.TLabel", foreground="#cc0000")
             root.option_add("*TCombobox*Listbox.background", "#dddddd")
+        # ComboboxPopdownFrame must be reset every time the theme changes
         style.configure("ComboboxPopdownFrame", relief=tk.FLAT)
 
     @classmethod
     def test_dark_mode(cls, trueval: T, falseval: T) -> T:
         """
-        If currently in dark mode, return trueval; otherwise return falseval.
+        If currently in dark mode, return `trueval`; otherwise return `falseval`.
         """
         style = ttk.Style()
         background = style.lookup("TLabel", "background")
         if is_dark(f"{background}"):
             return trueval
         return falseval
 
@@ -182,42 +200,48 @@
         Get the foreground color for menus, based on dark mode.
         """
         return cls.test_dark_mode("#ffffff", "#000000")
 
     @classmethod
     def get_base_font(cls) -> Font:
         """
-        Get the base font for use in the application.
+        Get the base font for use in the application. Returns `TkDefaultFont`.
         """
         return font.nametofont("TkDefaultFont")
 
     @classmethod
     def get_large_font(cls) -> Font:
         """
         Get the large font for use in the application.
+
+        Returns a modified `TkDefaultFont` with font size increased by 4.
         """
         return font_utils.modify_named_font(
             "TkDefaultFont", size=cls.get_base_font().actual()["size"]+4
         )
 
     @classmethod
     def get_small_font(cls) -> Font:
         """
         Get the small font for use in the application.
+
+        Returns a modified `TkDefaultFont` with font size decreased by 2.
         """
         return font_utils.modify_named_font(
             "TkDefaultFont", size=cls.get_base_font().actual()["size"]-2
         )
 
     @classmethod
     def get_bold_font(cls) -> Font:
         """
         Get the bold font for use in the application.
+
+        Returns a modified `TkDefaultFont` with font weight set to bold.
         """
         return font_utils.modify_named_font("TkDefaultFont", weight="bold")
 
     @classmethod
     def get_fixed_font(cls) -> Font:
         """
-        Get the monospace font for use in the application.
+        Get the monospace font for use in the application. Returns `TkFixedFont`.
         """
         return font.nametofont("TkFixedFont")
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/translator.py` & `sysmon_pytk-0.5.1/sysmon_pytk/translator.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,29 +13,34 @@
 @dataclasses.dataclass
 class Translator:
     """
     App translator data.
     """
 
     name: str
+    """The translator's name (or pseudonym)."""
     github_username: str = ""
+    """The translator's GitHub username, if available. Can be an empty string."""
 
     def github_url(self) -> str:
         """
         Build the translator's github link from their username, if available.
         """
         if self.github_username is not None:
             return f"https://github.com/{self.github_username}"
         return None
 
 
 TRANSLATORS: dict[str, list[Translator]] = {
     "Español": [
-        Translator("Stacey Adams (author)")
+        Translator("Stacey Adams (author)"),
+        Translator("Félix Medrano", "robertxgray")
     ],
     "Deutsch": [
-        Translator("Alisyn Arness")
+        Translator("Alisyn Arness"),
+        Translator("Rainer Schwarzbach", "blackstream-x")
     ],
     "Norsk Bokmål": [
         Translator("Allan Nordhøy", "comradekingu")
     ]
 }
+"""The translator team, for use in credits."""
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/__init__.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 # SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 # SPDX-License-Identifier: MIT
 
 """
 Various Tk widgets.
 """
 
+from . import buttons, meters
 from .autoscrollbar import AutoScrollbar
 from .dropdown import DropDown
-from .edit_menu import EditMenu
+from .edit_menu import EditMenu, EditMenuImages
 from .meter import Meter
 from .scalespinner import ScaleSpinner
 from .scrolling_text import ScrollingText
 from .tooltip import TempToolTip, TextToolTip, ToolTip
 from .url_label import UrlLabel
 
 __all__ = [
-    "AutoScrollbar", "DropDown", "EditMenu", "Meter", "ScaleSpinner",
-    "ScrollingText", "TempToolTip", "TextToolTip", "ToolTip", "UrlLabel"
+    "AutoScrollbar",
+    "DropDown",
+    "EditMenuImages",
+    "EditMenu",
+    "Meter",
+    "ScaleSpinner",
+    "ScrollingText",
+    "ToolTip",
+    "TempToolTip",
+    "TextToolTip",
+    "UrlLabel",
+    "buttons",
+    "meters",
 ]
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/autoscrollbar.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/autoscrollbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,39 @@
 AutoScrollbar widget.
 """
 
 from __future__ import annotations
 
 import tkinter as tk
 from tkinter import TclError, ttk
-from typing import Any, Literal, TypeVar
+from typing import Any, Literal, TypeVar, Union
 
 from typing_extensions import Self
 
+# Tk widgets that allow scrollbars
 ScrollableWidget = TypeVar(
-    "ScrollableWidget", tk.Canvas, tk.Listbox, tk.Text, ttk.Treeview
+    "ScrollableWidget", bound=Union[tk.Canvas, tk.Listbox, tk.Text, ttk.Treeview]
 )
 
 
 class AutoScrollbar(ttk.Scrollbar):  # pylint: disable=too-many-ancestors
     """
     A scrollbar that automatically removes itself when not needed.
     """
 
     def set(self, first: Any, last: Any) -> None:  # noqa: ANN401
         """
         Set the fractional values of the slider position.
 
-        Upper and lower ends are values between 0 and 1.
+        Parameters
+        ----------
+        first : Any
+            A string representation of a float, between 0 and 1.
+        last : Any
+            A string representation of a float, between 0 and 1.
         """
         if float(first) <= 0 and float(last) >= 1:
             self.grid_remove()
         else:
             self.grid()
         super().set(first, last)
 
@@ -52,14 +58,23 @@
     @classmethod
     def add_to_widget(
         cls, widget: ScrollableWidget, orient: Literal["horizontal", "vertical"],
         **kwargs
     ) -> Self:
         """
         Add a scrollbar to a scrollable widget.
+
+        Parameters
+        ----------
+        widget : ScrollableWidget
+            The parent widget that will be linked to this scrollbar.
+        orient : Literal["horizontal", "vertical"]
+            The scrollbar orientation: horizontal or vertical.
+        **kwargs : dict, optional
+            Arguments to pass to parent `Scrollbar` class.
         """
         scroller = cls(widget.master, orient=orient, **kwargs)
         if orient == "horizontal":
             scroller.config(command=widget.xview)
             widget.config(xscrollcommand=scroller.set)
         else:
             scroller.config(command=widget.yview)
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/button_mixin.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/buttons/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,44 +9,55 @@
 
 import dataclasses
 import tkinter as tk
 from enum import IntEnum
 from tkinter import ttk
 from typing import Any, Callable, TypeVar, Union
 
-from .._common import INTERNAL_PAD
-from ..app_locale import get_translator
+from ..._common import INTERNAL_PAD
+from ...app_locale import get_translator
 
 _ = get_translator()
 
+__all__ = ["ButtonName", "ButtonDefinition", "ButtonMixin"]
+
 WidgetFrame = TypeVar("WidgetFrame", bound=Union[ttk.Frame, tk.Frame])
 
 
 class ButtonName(IntEnum):
     """
     Standard button names.
     """
 
     NONE = 0
+    """None."""
     OK = 1
+    """OK button."""
     CANCEL = 2
+    """Cancel button."""
     CLOSE = 3
+    """Close button."""
     YES = 4
+    """Yes button."""
     NO = 5
+    """No button."""
     RETRY = 6
+    """Retry button."""
 
 
 @dataclasses.dataclass
 class ButtonDefinition:
     """
     Necessary metadata for creating a button.
     """
 
     text: str
+    """The text to appear on the button."""
     command: Callable[[], Any]
+    """The command to call when the button is pressed."""
 
 
 class ButtonMixin:  # pylint: disable=too-few-public-methods
     """
     Mixin class for standard button sets in dialogs.
 
     Attributes
@@ -70,15 +81,15 @@
         """
         Add buttons to the provided frame at the bottom, justified right.
 
         Parameters
         ----------
         frame : WidgetFrame (tk.Frame or ttk.Frame)
             The frame to which the buttons will be added
-        buttons : list[ButtonDefinition]
+        buttons : list[`ButtonDefinition`]
             The list of buttons to add
         default : int
             The default button, displayed with style="Accent.TButton"
         """
         self.toplevel = frame.winfo_toplevel()
         max_columns, max_rows = frame.grid_size()
         buttonframe = ttk.Frame(frame)
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/dropdown.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/dropdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,27 +36,25 @@
 
         Parameters
         ----------
         parent : BaseWidget
             The parent widget.
         dictionary : dict
             The dictionary to use in the dropdown.
-        *args : tuple, optional
-            Additional arguments for initializing a `Combobox`.
         **kwargs : dict, optional
             Additional keyword arguments for a `Combobox`.
         """
         super().__init__(
             parent, values=sorted(dictionary.keys()), **kwargs
         )
         self.dictionary = dictionary
 
     def get(self) -> str:
         """
-        Get the selected value.
+        Get the selected value of the dropdown.
         """
         key = super().get()
         return self.dictionary[key] if key else ""
 
     def set(self, value: str) -> None:
         """
         Set the value of the dropdown, if value is found in the dictionary.
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/edit_menu.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/edit_menu.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,53 +19,67 @@
 @dataclasses.dataclass
 class EditMenuImages:
     """
     Images used for the Edit Menu.
     """
 
     cut: tk.PhotoImage
+    """Image for Cut."""
     copy: tk.PhotoImage
+    """Image for Copy."""
     paste: tk.PhotoImage
+    """Image for Paste."""
     select_all: tk.PhotoImage
+    """Image for Select All."""
 
 
 class EditMenu(tk.Menu):
     """
     Standard Edit Menu with Cut/Copy/Paste/Select All items.
 
     Attributes
     ----------
-    images : EditMenuImages
+    images : `EditMenuImages`
         A collection of images needed for the menu.
     """
 
     def __init__(self, master: tk.Text, **kwarg) -> None:
+        """
+        Construct an edit menu for a Text widget.
+
+        Parameters
+        ----------
+        master : tk.Text
+            The parent Text widget.
+        **kwarg : dict, optional
+            Additional keyword arguments for a `Menu`.
+        """
         self.master: tk.Text = master
         super().__init__(master, **kwarg)
         self.images = EditMenuImages(
             cut=tk.PhotoImage(file=get_full_path("images/edit-cut.png")),
             copy=tk.PhotoImage(file=get_full_path("images/edit-copy.png")),
             paste=tk.PhotoImage(file=get_full_path("images/edit-paste.png")),
             select_all=tk.PhotoImage(file=get_full_path("images/edit-select-all.png"))
         )
         self.add_command(
-            label=("Cut"), command=self.cut, accelerator=_("Ctrl+X"),
+            label=_("Cut"), command=self.cut, accelerator=_("Ctrl+X"),
             compound=tk.LEFT, image=self.images.cut
         )
         self.add_command(
-            label=("Copy"), command=self.copy, accelerator=_("Ctrl+C"),
+            label=_("Copy"), command=self.copy, accelerator=_("Ctrl+C"),
             compound=tk.LEFT, image=self.images.copy
         )
         self.add_command(
-            label=("Paste"), command=self.paste, accelerator=_("Ctrl+V"),
+            label=_("Paste"), command=self.paste, accelerator=_("Ctrl+V"),
             compound=tk.LEFT, image=self.images.paste
         )
         self.add_separator()
         self.add_command(
-            label=("Select All"), command=self.select_all,
+            label=_("Select All"), command=self.select_all,
             accelerator=_("Ctrl+A"), compound=tk.LEFT, image=self.images.select_all
         )
         self.master.bind("<Button-3>", self.show_popup)
         self.master.bind("<Control-X>", self.cut)
         self.master.bind("<Control-C>", self.copy)
         self.master.bind("<Control-V>", self.paste)
         self.master.bind("<Control-A>", self.select_all)
@@ -73,19 +87,19 @@
     def show_popup(self, event: tk.Event) -> None:
         """
         Show the edit menu.
         """
         if self.focus_get() != self:
             self.focus_set()
         if self.master.cget("state") == tk.DISABLED:
-            self.entryconfigure(("Cut"), state=tk.DISABLED)
-            self.entryconfigure(("Paste"), state=tk.DISABLED)
+            self.entryconfigure(_("Cut"), state=tk.DISABLED)
+            self.entryconfigure(_("Paste"), state=tk.DISABLED)
         else:
-            self.entryconfigure(("Cut"), state=tk.NORMAL)
-            self.entryconfigure(("Paste"), state=tk.NORMAL)
+            self.entryconfigure(_("Cut"), state=tk.NORMAL)
+            self.entryconfigure(_("Paste"), state=tk.NORMAL)
         self.tk_popup(event.x_root, event.y_root, 0)
 
     def cut(self, *_args) -> None:
         """
         Generate a Cut Text event.
         """
         if self.master.cget("state") == tk.NORMAL:
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/meter.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/meter.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 from tkinter import ttk
 from typing import TYPE_CHECKING
 
 from ..font_utils import modify_named_font
 from ..style_manager import StyleManager
 
 if TYPE_CHECKING:
-    from tkinter import BaseWidget
+    from tkinter import Misc
 
 
 @dataclasses.dataclass
 class CanvasObjects:
     """
-    Various canvas objects that need to be tracked.
+    Various canvas objects that need to be tracked within a `Meter` widget.
     """
 
     label1: int = 0
     min_value: int = 0
     max_value: int = 0
     current: int = 0
     meter: int = 0
@@ -48,27 +48,51 @@
     RED = "#d00"
     BLUE = "#00a"
 
     START_ANGLE = 36
     EXTENT_ANGLE = 180 - 2*START_ANGLE
 
     def __init__(
-            self,
-            parent: BaseWidget, *,
-            width: int = 300,
-            height: int = 225,
-            min_value: float = 0.0,
-            max_value: float = 100.0,
-            label: str = "",
-            unit: str = "",
-            divisions: int = 10,
-            yellow: float = 15,
-            red: float = 15,
-            blue: float = 0, **kw
+            self, parent: Misc, *,
+            width: int = 300, height: int = 225,
+            min_value: float = 0.0, max_value: float = 100.0,
+            label: str = "", unit: str = "",
+            divisions: int = 10, yellow: float = 15,
+            red: float = 15, blue: float = 0, **kw
     ) -> None:
+        """
+        Construct a meter widget.
+
+        Parameters
+        ----------
+        parent : Misc
+            The parent widget.
+        width : int, default = 300
+            The width of the meter widget.
+        height : int, default = 225
+            The height of the meter widget.
+        min_value : float, default = 0.0
+            The minimum value to display on the meter.
+        max_value : float, default = 100.0
+            The maximum value to display on the meter.
+        label : str, default = ""
+            The label to display above the meter.
+        unit : str, default = ""
+            The units, used when displaying numbers on the meter.
+        divisions : int, default = 10
+            The number of divisions between the start and end of the meter.
+        yellow : float, default = 15
+            The percent of the meter to show in yellow. Appears just before red.
+        red : float, default = 15
+            The percent of the meter to show in red. Appears at the max values.
+        blue : float, default = 0
+            The percent of the meter to show in blue. Appears at the min values.
+        **kw : dict, optional
+            Arguments to pass to parent `Frame` class.
+        """
         self._unit = unit
         self._min_value = min_value
         self._max_value = max_value
         self._width = width
         self._height = height
         self._divisions = divisions
         self.range = {"blue": blue, "yellow": yellow, "red": red}
@@ -128,68 +152,60 @@
             self._width / 30, self._height / 4,
             self._width * 29 / 30, self._height * 1.5
         )
         # Add the divisions
         self.canvas_objects.wedges = []
         for i in range(self._divisions):
             self.canvas_objects.wedges.append(self.canvas.create_arc(
-                coord,
+                coord, width=1, outline=self._text_color,
                 start=(i * (Meter.EXTENT_ANGLE / self._divisions) + Meter.START_ANGLE),
-                extent=(Meter.EXTENT_ANGLE / self._divisions),
-                width=1, outline=self._text_color
+                extent=(Meter.EXTENT_ANGLE / self._divisions)
             ))
 
         # Add the color scale arcs
         self.canvas.create_arc(
-            coord,
-            extent=Meter.EXTENT_ANGLE, start=Meter.START_ANGLE,
+            coord, extent=Meter.EXTENT_ANGLE, start=Meter.START_ANGLE,
             style="arc", outline=self.GREEN, width=self._width / 12
         )
         if red > 0:
             self.canvas.create_arc(
-                coord,
-                extent=self._percent_to_degrees(red), start=Meter.START_ANGLE,
+                coord, extent=self._percent_to_degrees(red), start=Meter.START_ANGLE,
                 style="arc", outline=self.RED, width=self._width / 12
             )
         if yellow > 0:
             self.canvas.create_arc(
-                coord,
-                extent=self._percent_to_degrees(yellow),
+                coord, extent=self._percent_to_degrees(yellow),
                 start=self._percent_to_degrees(red) + Meter.START_ANGLE,
                 style="arc", outline=self.YELLOW, width=self._width / 12
             )
         if blue > 0:
             self.canvas.create_arc(
-                coord,
-                start=Meter.EXTENT_ANGLE + Meter.START_ANGLE,
+                coord, start=Meter.EXTENT_ANGLE + Meter.START_ANGLE,
                 extent=-self._percent_to_degrees(blue),
                 style="arc", outline=self.BLUE, width=self._width / 12
             )
 
         # Add the moving indicator line
         self.canvas_objects.meter = self.canvas.create_arc(
-            coord,
-            start=Meter.EXTENT_ANGLE + Meter.START_ANGLE, extent=1,
+            coord, start=Meter.EXTENT_ANGLE + Meter.START_ANGLE, extent=1,
             fill=self._meter_color, outline=self._meter_color, width=3
         )
 
     def _add_inset(self) -> None:
         # Add the inset
         inset_coord = (
             self._width * 23 / 60, self._height * 23 / 32,
             self._width * 37 / 60, self._height * 33 / 32
         )
         self.canvas_objects.inset = self.canvas.create_arc(
-            inset_coord,
-            start=Meter.START_ANGLE, extent=Meter.EXTENT_ANGLE,
+            inset_coord, start=Meter.START_ANGLE, extent=Meter.EXTENT_ANGLE,
             fill=self._text_color, outline=self._text_color, width=2
         )
         self.canvas_objects.inset_border = self.canvas.create_arc(
-            inset_coord,
-            start=Meter.START_ANGLE, extent=Meter.EXTENT_ANGLE,
+            inset_coord, start=Meter.START_ANGLE, extent=Meter.EXTENT_ANGLE,
             outline=self._meter_color, style="arc", width=1
         )
 
     def check_dark_mode(self) -> None:
         """
         Detect whether using dark mode and adjust base colors.
         """
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/scalespinner.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/scalespinner.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,22 +48,24 @@
         ----------
         parent : BaseWidget
             The parent widget.
         variable : Variable
             The control variable which maintains the selected value.
         text : str, optional
             The text to display as a `Label`.
-        length : int, default: 100
+        length : int, default = 100
             The length of the `Scale` widget.
-        from_ : float, default: 0.0
+        from_ : float, default = 0.0
             The smallest value allowed for the `Scale` and `Spinbox`.
-        to : float, default: 100.0
+        to : float, default = 100.0
             The largest value allowed for the `Scale` and `Spinbox`.
-        as_int : bool, default: False
+        as_int : bool, default = False
             A flag indicating whether to round the values from the `Scale`.
+        **kwargs : dict, optional
+            Arguments to pass to parent `Frame` class.
         """
         super().__init__(parent, **kwargs)
         self.variable = variable
         self.as_int = as_int
         self.rowconfigure(0, weight=1)
         self.columnconfigure(1, weight=1)
         base_font = StyleManager.get_base_font()
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/scrolling_text.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/scrolling_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,39 +29,50 @@
     Attributes
     ----------
     frame : Frame
         The frame which holds this widget and its accompanying AutoScrollbar.
 
     Notes
     -----
-    This Text widget is configured with several standard tags.
-        center : Center the tagged text.
-        left : Left justify the tagged text.
-        right : Right justify the tagged text.
-        large : apply the large font to the tagged text.
-        bold : apply the bold font to the tagged text.
-        fixed : apply the fixed font to the tagged text.
-        link : treat the tagged text as a clickable link.
-        linkurl : follows a link tag, and contains the url to open - hidden text.
+    This Text widget is configured with several standard tags:
+
+    * `center` : Center the tagged text.
+    * `left` : Left justify the tagged text.
+    * `right` : Right justify the tagged text.
+    * `large` : apply the large font to the tagged text.
+    * `bold` : apply the bold font to the tagged text.
+    * `fixed` : apply the fixed font to the tagged text.
+    * `link` : treat the tagged text as a clickable link.
+    * `linkurl` : follows a link tag, and contains the url to open - hidden text.
 
     To use links, insert a `link` tag with the clickable link text, and then
     insert a `linkurl` tag containing the url to open for the previous link
     text. The `linkurl` text will be hidden, but accessible when the user
     clicks on the link. When the user clicks, the text position of the click
     will be determined, from that position, the text will be searched for the
     next occurrence of a `linkurl` tag, and that url will be opened.
     """
 
     def __init__(self, master: tk.Misc | None = None, **kwargs) -> None:
+        """
+        Construct a scrolling text widget.
+
+        Parameters
+        ----------
+        master : Misc, optional
+            The parent widget.
+        **kwargs : dict, optional
+            Arguments to pass to parent `Text` class.
+        """
         self.frame = ttk.Frame(master)
         self.frame.rowconfigure(0, weight=1)
         self.frame.columnconfigure(0, weight=1)
         super().__init__(self.frame, **kwargs)
         self.grid(row=0, column=0, sticky=tk.NSEW)
-        self._configure_tags()
+        self.configure_tags()
         AutoScrollbar.add_to_widget(self, orient=tk.VERTICAL).grid(
             row=0, column=1, sticky=tk.NS
         )
         EditMenu(
             self, activeborderwidth=0,  # relief=tk.FLAT,
             background=StyleManager.test_dark_mode("#444444", "#dddddd"),
             foreground=StyleManager.test_dark_mode("#ffffff", "#000000"),
@@ -70,15 +81,15 @@
 
     def get_frame(self) -> ttk.Frame:
         """
         Get the containing frame.
         """
         return self.frame
 
-    def _configure_tags(self) -> None:
+    def configure_tags(self) -> None:
         """
         Configure the standard tags for the Text widget.
         """
         self.tag_configure("center", justify="center")
         self.tag_configure("left", justify="left")
         self.tag_configure("right", justify="right")
         self.tag_configure("large", font=StyleManager.get_large_font())
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/tooltip.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/tooltip.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,26 @@
     Attributes
     ----------
     tag : str
         A tag used in the Text widget with which to link this tooltip.
     """
 
     def __init__(self, parent: Text, text: str = "", tag: str = "") -> None:
+        """
+        Construct a tooltip.
+
+        Parameters
+        ----------
+        parent : Text
+            The parent widget, which will host the tooltip.
+        text : str
+            The text to display in the tooltip.
+        tag : str
+            A tag from the parent Text widget that will be bound for the tooltip.
+        """
         self.tag = tag
         super().__init__(parent, text)
 
     def bind_events(self) -> None:
         """
         Bind the Enter, Leave, Motion events to the tag on the parent Text widget.
         """
@@ -114,15 +126,15 @@
     """
 
     def __init__(
         self, parent: Misc, text: str = "",
         position: tuple[int, int] = (0, 0), timer_ms: int = 2000
     ) -> None:
         """
-        Construct a tooltip.
+        Construct a temporary tooltip.
 
         Parameters
         ----------
         parent : Misc
             The parent widget, which will host the tooltip.
         text : str
             The text to display in the tooltip.
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk/widgets/url_label.py` & `sysmon_pytk-0.5.1/sysmon_pytk/widgets/url_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             The text to display in the label.
         url : str
             The URL to use when opening a web browser.
         style : str
             A Tcl/Tk style to use for display.
         show_tooltip : bool
             A flag to indicate whether to show a tooltip containing the URL.
-        **kw : dict, optional
+        **kwargs : dict, optional
             Additional keyword arguments for a `Label`.
         """
         self.url = url
         cursor = "hand2" if self._has_web_protocol() else "arrow"
         super().__init__(parent, cursor=cursor, style=style, text=text, **kwargs)
         if show_tooltip and url:
             ToolTip(self, url)
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk.egg-info/PKG-INFO` & `sysmon_pytk-0.5.1/sysmon_pytk.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysmon_pytk
-Version: 0.5.0
+Version: 0.5.1
 Summary: System monitor app using Tkinter
 Author-email: Stacey Adams <stacey.belle.rose@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Stacey Adams
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,172 +22,123 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/staceybellerose/sysmon-pytk
+Project-URL: Documentation, https://staceybellerose.github.io/sysmon-pytk/
 Project-URL: Repository, https://github.com/staceybellerose/sysmon-pytk
 Project-URL: Issues, https://github.com/staceybellerose/sysmon-pytk/issues
 Keywords: system monitor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: blessings>=1.7
 Requires-Dist: darkdetect==0.8.0
 Requires-Dist: platformdirs>=4.2
 Requires-Dist: psutil<6.0,>=5.8.0
 Requires-Dist: typing-extensions>=4.10
-Provides-Extra: dev
-Requires-Dist: bandit>=1.7.7; extra == "dev"
-Requires-Dist: build>=1.1.1; extra == "dev"
-Requires-Dist: coloredlogs>=15; extra == "dev"
-Requires-Dist: liccheck>=0.9.2; extra == "dev"
-Requires-Dist: mypy>=1.5; extra == "dev"
-Requires-Dist: pycodestyle>=2.11; extra == "dev"
-Requires-Dist: pydocstyle>=6.2; extra == "dev"
-Requires-Dist: pyflakes>=3.1; extra == "dev"
-Requires-Dist: pylint>=3.0; extra == "dev"
-Requires-Dist: pyroma>=4.2; extra == "dev"
-Requires-Dist: radon>=6.0; extra == "dev"
-Requires-Dist: redbaron>=0.9.2; extra == "dev"
-Requires-Dist: reuse>=3.0; extra == "dev"
-Requires-Dist: ruff>=0.3; extra == "dev"
-Requires-Dist: setuptools>=64; extra == "dev"
-Requires-Dist: twine>=5.0; extra == "dev"
-Requires-Dist: types-docutils>=0.20; extra == "dev"
-Requires-Dist: types-psutil<6.0,>=5.8.0; extra == "dev"
-Requires-Dist: types-setuptools>=64; extra == "dev"
 
 # System Monitor for Python/Tk
 
 <!--
 SPDX-FileCopyrightText: © 2024 Stacey Adams <stacey.belle.rose@gmail.com>
 
 SPDX-License-Identifier: MIT
 -->
+<!-- markdownlint-disable MD033 -->
+
+[![GitHub License](https://img.shields.io/github/license/staceybellerose/sysmon-pytk?color=7C4DFF)](https://github.com/staceybellerose/sysmon-pytk)
+[![GitHub Release](https://img.shields.io/github/v/release/staceybellerose/sysmon-pytk)](https://github.com/staceybellerose/sysmon-pytk/releases)
+[![AppVeyor Build](https://img.shields.io/appveyor/build/staceybellerose/sysmon-pytk/main)](https://ci.appveyor.com/project/staceybellerose/sysmon-pytk/)
+
+[![PyPI - Status](https://img.shields.io/pypi/status/sysmon-pytk)](https://pypi.org/project/sysmon-pytk/)
+[![PyPI - Version](https://img.shields.io/pypi/v/sysmon-pytk)](https://pypi.org/project/sysmon-pytk/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sysmon-pytk)](https://pypi.org/project/sysmon-pytk/)
 
-![GitHub License](https://img.shields.io/github/license/staceybellerose/sysmon-pytk?color=7C4DFF)
-![GitHub Release](https://img.shields.io/github/v/release/staceybellerose/sysmon-pytk)
 [![REUSE status](https://api.reuse.software/badge/github.com/staceybellerose/sysmon-pytk)](https://api.reuse.software/info/github.com/staceybellerose/sysmon-pytk)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/staceybellerose/sysmon-pytk?logo=codefactor)](https://www.codefactor.io/repository/github/staceybellerose/sysmon-pytk)
 [![Maintainability](https://api.codeclimate.com/v1/badges/556c93bf800d0d58e7e4/maintainability)](https://codeclimate.com/github/staceybellerose/sysmon-pytk/maintainability)
 
 System monitor written in Python using Tk. It monitors CPU usage and
 temperature, RAM usage, and disk usage of the primary disk (containing the
 root partition). It also displays the system's hostname, IP address, uptime,
 and current process count.
 
 ![Main Window](images/main_window.png)
 
 ## Pre-installation
 
-### Make sure the Python interface to Tcl/Tk (tkinter) is installed
-
-Since this is a GUI application using tkinter, tkinter must be installed
-separately.
-
-* Debian, Ubuntu, and derivatives
-
-    ```bash
-    sudo apt install python3-tk
-    ```
-
-* Fedora and derivatives
-
-    ```bash
-    sudo dnf install python3-tkinter
-    ```
-
-* MacOS
+Make sure the Python interface to Tcl/Tk (tkinter) is installed.
 
-    ```bash
-    brew install python-tk
-    ```
+[tkinter Installation Instructions](https://github.com/staceybellerose/sysmon-pytk/blob/main/docs/PRE-INSTALLATION.md)
 
 ## Install Using pip
 
-Download the wheel file from the latest release, then install it. Once a PyPI
-account can be set up, the program will be downloadable from there.
-
 ```bash
-pip install ./sysmon_pytk-0.4.1-py3-none-any.whl
+pip install sysmon-pytk
 ```
 
 Two versions of the program will be installed, a GUI program and a command line
 program.
 
-To run the GUI program:
+## Run the GUI program
 
 ```bash
 sysmon
 ```
 
-To run the command line program:
-
-```bash
-cli_sysmon
-```
-
-## Install Manually, for local development
-
-Note when cloning this repo that it has a submodule
-[Azure ttk theme](https://github.com/rdbende/Azure-ttk-theme)
-which must be copied over:
+or
 
 ```bash
-git clone --recurse-submodules https://github.com/staceybellerose/sysmon-pytk.git
+gui_sysmon
 ```
 
-If you didn't clone the submodule when cloning this repo, run this to update:
+## Run the command line program
 
 ```bash
-git submodule update --init --recursive
-```
-
-### Install the required python packages
-
-```bash
-make venv
-```
-
-### Generate translation files
-
-Translations are available in English, Spanish, German, and Norwegian Bokmål.
-To build the translation files, run the following bash commands:
-
-```bash
-make translations
+cli_sysmon
 ```
 
-| Run the GUI program | |
-|-|-|
-| While the venv is activated | `python -m sysmon_pytk.gui_monitor &` |
-| Explicitly using the venv | `venv/bin/python -m sysmon_pytk.gui_monitor &` |
-| Let make handle everything automatically | `make run` |
-
-| Run the command line program | |
-|-|-|
-| While the venv is activated | `python -m sysmon_pytk.cli_monitor &` |
-| Explicitly using the venv | `venv/bin/python -m sysmon_pytk.cli_monitor &` |
-| Let make handle everything automatically | `make cli` |
+To get available options for the command line program, use `cli_sysmon -h`.
 
 ## Translations
 
 Special thanks to our translators!
 
 | Language         | Code  | Translator |
 |------------------|-------|------------|
-| German           | de    | Alisyn Arness |
-| Spanish          | es    | Stacey Adams (author) |
+| German           | de    | Alisyn Arness, [Rainer Schwarzbach](https://github.com/blackstream-x) |
+| Spanish          | es    | Stacey Adams (author), [Félix Medrano](https://github.com/robertxgray) |
 | Norwegian Bokmål | nb_NO | [Allan Nordhøy](https://github.com/comradekingu) |
+
+## Contributing
+
+Translations are always welcome! The strings to be translated are located in
+[app.pot](https://github.com/staceybellerose/sysmon-pytk/blob/main/sysmon_pytk/locale/app.pot)
+and
+[argparse.pot](https://github.com/staceybellerose/sysmon-pytk/blob/main/sysmon_pytk/locale/argparse.pot).
+
+`argparse.pot` contains standard strings from the Python Standard Library file
+`argparse.py` (Python versions 3.9–3.12).
+
+If you want to work on the code, read the
+[Development Guide](https://github.com/staceybellerose/sysmon-pytk/blob/main/docs/DEVELOPING.md).
+Also, check out the [API Documentation](https://staceybellerose.github.io/sysmon-pytk/).
+
+Contributers are expected to follow our
+[Code of Conduct](https://github.com/staceybellerose/sysmon-pytk/blob/main/CODE_OF_CONDUCT.md).
```

### Comparing `sysmon_pytk-0.5.0/sysmon_pytk.egg-info/SOURCES.txt` & `sysmon_pytk-0.5.1/sysmon_pytk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 azure/LICENSE
 azure/azure.tcl
+azure/icon.png
 azure/theme/dark.tcl
 azure/theme/light.tcl
 azure/theme/dark/box-accent.png
 azure/theme/dark/box-basic.png
 azure/theme/dark/box-hover.png
 azure/theme/dark/box-invalid.png
 azure/theme/dark/button-hover.png
@@ -136,19 +136,20 @@
 azure/theme/light/vert-hover.png
 sysmon_pytk/__init__.py
 sysmon_pytk/_common.py
 sysmon_pytk/about.py
 sysmon_pytk/app_locale.py
 sysmon_pytk/application.py
 sysmon_pytk/callables.pyi
-sysmon_pytk/cli_monitor.py
+sysmon_pytk/cli_sysmon.py
 sysmon_pytk/desktop_menu.py
 sysmon_pytk/file_utils.py
 sysmon_pytk/font_utils.py
-sysmon_pytk/gui_monitor.py
+sysmon_pytk/gui_sysmon.py
+sysmon_pytk/py.typed
 sysmon_pytk/settings.py
 sysmon_pytk/style_manager.py
 sysmon_pytk/translator.py
 sysmon_pytk.egg-info/PKG-INFO
 sysmon_pytk.egg-info/SOURCES.txt
 sysmon_pytk.egg-info/dependency_links.txt
 sysmon_pytk.egg-info/entry_points.txt
@@ -187,22 +188,28 @@
 sysmon_pytk/modals/__init__.py
 sysmon_pytk/modals/_base_modal.py
 sysmon_pytk/modals/about_modal.py
 sysmon_pytk/modals/cpu_modal.py
 sysmon_pytk/modals/disk_usage_modal.py
 sysmon_pytk/modals/font_modal.py
 sysmon_pytk/modals/mem_usage_modal.py
-sysmon_pytk/modals/messagebox.py
-sysmon_pytk/modals/messagebox_base.py
 sysmon_pytk/modals/settings_modal.py
 sysmon_pytk/modals/temperature_modal.py
+sysmon_pytk/modals/messagebox/__init__.py
+sysmon_pytk/modals/messagebox/base.py
+sysmon_pytk/modals/messagebox/mb_functions.py
 sysmon_pytk/widgets/__init__.py
 sysmon_pytk/widgets/autoscrollbar.py
-sysmon_pytk/widgets/button_mixin.py
 sysmon_pytk/widgets/dropdown.py
 sysmon_pytk/widgets/edit_menu.py
 sysmon_pytk/widgets/meter.py
-sysmon_pytk/widgets/meters.py
 sysmon_pytk/widgets/scalespinner.py
 sysmon_pytk/widgets/scrolling_text.py
 sysmon_pytk/widgets/tooltip.py
-sysmon_pytk/widgets/url_label.py
+sysmon_pytk/widgets/url_label.py
+sysmon_pytk/widgets/buttons/__init__.py
+sysmon_pytk/widgets/meters/__init__.py
+sysmon_pytk/widgets/meters/cpu_meter.py
+sysmon_pytk/widgets/meters/disk_meter.py
+sysmon_pytk/widgets/meters/ram_meter.py
+sysmon_pytk/widgets/meters/temp_meter.py
+sysmon_pytk/widgets/meters/updating_meter.py
```

