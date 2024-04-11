# Comparing `tmp/conan-explorer-2.3.0a2.tar.gz` & `tmp/conan-explorer-2.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conan-explorer-2.3.0a2.tar", last modified: Thu Mar 28 18:52:01 2024, max compression
+gzip compressed data, was "conan-explorer-2.3.0a3.tar", last modified: Thu Apr 11 20:47:40 2024, max compression
```

## Comparing `conan-explorer-2.3.0a2.tar` & `conan-explorer-2.3.0a3.tar`

### file list

```diff
@@ -1,279 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.833261 conan-explorer-2.3.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-03-28 18:52:01.833261 conan-explorer-2.3.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.785261 conan-explorer-2.3.0a2/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.793261 conan-explorer-2.3.0a2/doc/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/doc/example_plugin/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.793261 conan-explorer-2.3.0a2/doc/example_plugin/cal_example_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/doc/example_plugin/cal_example_plugin/example.ui
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:52:01.833261 conan-explorer-2.3.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.785261 conan-explorer-2.3.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.793261 conan-explorer-2.3.0a2/src/conan_explorer/
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.793261 conan-explorer-2.3.0a2/src/conan_explorer/app/
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.793261 conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/crash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/theming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/app/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.793261 conan-explorer-2.3.0a2/src/conan_explorer/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/config_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.797261 conan-explorer-2.3.0a2/src/conan_explorer/assets/font/
--rw-r--r--   0 runner    (1001) docker     (127)   556216 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/font/NotoSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)  1593904 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/font/NotoSansMono.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.797261 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/conan.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.801261 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/android.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/conan_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/conan_settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/grid.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/linux.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/mac_os.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/package.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/package_explorer.svg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/package_orig.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/search_packages.svg
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/windows.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.809261 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/about.svg
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/add_link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/app.svg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/bar_chart.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/cleanup.svg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/close_lgr.svg
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/close_white_lgr.svg
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/cmd.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/copy.svg
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/copy_link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/copy_to_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/cut.svg
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/dark_mode.svg
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/decrease_font.svg
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/default_pkg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/difference.svg
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/download.svg
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/download_pkg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/download_update.svg
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/edit.svg
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/edit_file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/edit_with_line.svg
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/expand.svg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/expand_b.svg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/expand_less.svg
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/expand_w.svg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/export_notes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/file_explorer.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/file_open_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/file_preview.svg
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/forward.svg
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/forward_b.svg
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/forward_w.svg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/hide.svg
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/increase_font.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/lock_open_FILL0_wght400_GRAD0_opsz48.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/login.svg
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/maximize.svg
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/menu_stripes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/minus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/move_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/no-access.svg
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/opened_folder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/package.svg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/paste.svg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/plugin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/plus_rounded.svg
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/rearrange.svg
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/remove-lock.svg
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/remove-lock2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/rename.svg
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/restore.svg
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/save.svg
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/search.svg
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/search_packages.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/show.svg
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/view.svg
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/launch.bat.in
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/assets/launch.sh.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.809261 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conanV1.py
--rw-r--r--   0 runner    (1001) docker     (127)    21706 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conanV2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conan_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conan_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conan_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    27613 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/unified_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.813261 conan-explorer-2.3.0a2/src/conan_explorer/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/settings/ini_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.813261 conan-explorer-2.3.0a2/src/conan_explorer/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.813261 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/syntax_highlighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/common/theming.py
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dark_style.qss.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.813261 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.813261 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/conan_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/conan_install.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/conan_install_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.813261 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/crash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/crash.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/crash_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.817261 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.817261 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/diff.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/diff_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.817261 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.817261 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23123 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/fluent_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    47941 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/fluent_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)    32368 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/fluent_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/side_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/side_menu.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/side_menu_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/light_style.qss.in
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.817261 conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/plugins.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.817261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.821261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about_text.html
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.821261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/app_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/app_link.ui
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/app_link_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.821261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/json_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.821261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19487 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/tab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.825261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/conan_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    27495 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/conan_conf.ui
--rw-r--r--   0 runner    (1001) docker     (127)    27296 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/conan_conf_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.825261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/editable_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/editable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/profiles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/remotes_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/remotes_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.825261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/conan_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/conan_search.ui
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/conan_search_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.829261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/file_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/package_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/package_explorer.ui
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/package_explorer_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    14822 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/sel_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/sel_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.829261 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/plugins.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/plugins_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.829261 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/clickable_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/conan_line_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/password_line_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/text_broswer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/toggle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.833261 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-03-28 18:52:01.000000 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-03-28 18:52:01.000000 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:52:01.000000 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 18:52:01.000000 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-28 18:52:01.000000 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 18:52:01.000000 conan-explorer-2.3.0a2/src/conan_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.789261 conan-explorer-2.3.0a2/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.789261 conan-explorer-2.3.0a2/test/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.829261 conan-explorer-2.3.0a2/test/testdata/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_empty_section.ini
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_iconpath_invalid.ini
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_importpath_invalid.ini
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_minimal_valid.ini
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_no_class.ini
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_no_icon.ini
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_no_importpath.ini
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/plugin/plugins_no_name.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.789261 conan-explorer-2.3.0a2/test/testdata/settings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.829261 conan-explorer-2.3.0a2/test/testdata/settings/read/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/settings/read/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:52:01.833261 conan-explorer-2.3.0a2/test/testdata/settings/write/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 18:51:52.000000 conan-explorer-2.3.0a2/test/testdata/settings/write/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.982886 conan-explorer-2.3.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-11 20:47:40.982886 conan-explorer-2.3.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.934886 conan-explorer-2.3.0a3/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.938886 conan-explorer-2.3.0a3/doc/example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/doc/example_plugin/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.938886 conan-explorer-2.3.0a3/doc/example_plugin/cal_example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/doc/example_plugin/cal_example_plugin/example.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:47:40.982886 conan-explorer-2.3.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.934886 conan-explorer-2.3.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.938886 conan-explorer-2.3.0a3/src/conan_explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.942886 conan-explorer-2.3.0a3/src/conan_explorer/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.942886 conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/theming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/app/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.942886 conan-explorer-2.3.0a3/src/conan_explorer/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/config_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.942886 conan-explorer-2.3.0a3/src/conan_explorer/assets/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   556216 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/font/NotoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)  1593904 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/font/NotoSansMono.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.946886 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/conan.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.946886 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/android.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/conan_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/conan_settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/grid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/linux.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/mac_os.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/package.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/package_explorer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/package_orig.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/search_packages.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/windows.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.958886 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/about.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/add_link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/app.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/bar_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/cleanup.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/close_lgr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/close_white_lgr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/cmd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/copy_link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/copy_to_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/dark_mode.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/decrease_font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/default_pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/difference.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/download_pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/download_update.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/edit_file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/edit_with_line.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/expand_b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/expand_less.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/expand_w.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/export_notes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/file_explorer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/file_open_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/file_preview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/forward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/forward_b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/forward_w.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/hide.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/increase_font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/lock_open_FILL0_wght400_GRAD0_opsz48.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/login.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/maximize.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/menu_stripes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/move_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/no-access.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/opened_folder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/package.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/plugin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/plus_rounded.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/rearrange.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/remove-lock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/remove-lock2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/rename.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/restore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/save.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/search.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/search_packages.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/show.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/view.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/launch.bat.in
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/assets/launch.sh.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.958886 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conanV1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21706 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conanV2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conan_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conan_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conan_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27613 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/unified_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.958886 conan-explorer-2.3.0a3/src/conan_explorer/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/settings/ini_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.962886 conan-explorer-2.3.0a3/src/conan_explorer/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.962886 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/syntax_highlighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/common/theming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dark_style.qss.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.962886 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.962886 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/conan_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/conan_install.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/conan_install_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.962886 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/crash.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/crash_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.962886 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.966886 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/diff.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/diff_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.966886 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.966886 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23123 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/fluent_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47941 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/fluent_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    32368 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/fluent_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/side_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/side_menu.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/side_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/light_style.qss.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18661 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/notifier_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.966886 conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/plugins.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.966886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.966886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about_text.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.970886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/app_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/app_link.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/app_link_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.970886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/json_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.970886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19487 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/tab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.970886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/conan_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27495 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/conan_conf.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    27296 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/conan_conf_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.974886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/editable_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/editable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/profiles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/remotes_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/remotes_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.974886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/conan_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/conan_search.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/conan_search_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.974886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/file_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/package_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/package_explorer.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/package_explorer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14822 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/sel_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/sel_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.974886 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/plugins.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/plugins_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.978886 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/clickable_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/conan_line_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/password_line_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/text_broswer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.978886 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-11 20:47:40.000000 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12004 2024-04-11 20:47:40.000000 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:47:40.000000 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 20:47:40.000000 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-11 20:47:40.000000 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 20:47:40.000000 conan-explorer-2.3.0a3/src/conan_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.938886 conan-explorer-2.3.0a3/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.938886 conan-explorer-2.3.0a3/test/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.978886 conan-explorer-2.3.0a3/test/testdata/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_empty_section.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_iconpath_invalid.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_importpath_invalid.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_minimal_valid.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_no_class.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_no_icon.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_no_importpath.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/plugin/plugins_no_name.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.938886 conan-explorer-2.3.0a3/test/testdata/settings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.978886 conan-explorer-2.3.0a3/test/testdata/settings/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/settings/read/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:47:40.978886 conan-explorer-2.3.0a3/test/testdata/settings/write/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 20:47:32.000000 conan-explorer-2.3.0a3/test/testdata/settings/write/config.ini
```

### Comparing `conan-explorer-2.3.0a2/LICENSE` & `conan-explorer-2.3.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/PKG-INFO` & `conan-explorer-2.3.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-explorer
-Version: 2.3.0a2
+Version: 2.3.0a3
 Summary: Package Explorer and App Launcher for Conan
 Home-page: https://github.com/goszpeti/conan_explorer
 Author: Péter Gosztolya and Contributors
 License: LGPL v3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,15 @@
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: conan<2.2,>=1.48
 Requires-Dist: PySide6-Essentials>=6.4.0
+Requires-Dist: pyqt-toast-notification==1.1.0
 Requires-Dist: jsonschema<5,>=3.2.0
 Requires-Dist: dictdiffer==0.9.0
 Requires-Dist: contextlib-chdir==1.0.2; python_version < "3.11"
 Requires-Dist: typing-extensions<5,>=3.10.0.2
 Requires-Dist: packaging
 Requires-Dist: Jinja2<4,>=2.3
 Provides-Extra: dev
```

### Comparing `conan-explorer-2.3.0a2/README.md` & `conan-explorer-2.3.0a3/README.md`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/doc/example_plugin/cal_example_plugin/example.ui` & `conan-explorer-2.3.0a3/doc/example_plugin/cal_example_plugin/example.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/setup.py` & `conan-explorer-2.3.0a3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pkg_resources import Requirement
 
 # Package meta-data.
 NAME = "conan-explorer"
-VERSION = "2.3.0a2"
+VERSION = "2.3.0a3"
 DESCRIPTION = "Package Explorer and App Launcher for Conan"
 URL = "https://github.com/goszpeti/conan_explorer"
 AUTHOR = "Péter Gosztolya and Contributors"
 PYTHON_REQUIRES = ">=3.8.0"
 
 
 # Force Conan version from envvar CONAN_VERSION
@@ -35,15 +35,16 @@
 conan_req_spec = "conan>=1.48, <2.2"
 if conan_major_version == "1":
     conan_req_spec = "conan>=1.48, <2.0"
 if conan_major_version == "2":
     conan_req_spec = "conan>=2.0, <2.2"
 REQUIRES = [
     conan_req_spec,  # MIT License
-    "PySide6-Essentials>=6.4.0", # LGPLv3
+    "PySide6-Essentials>=6.4.0", # LGPLv3,
+    "pyqt-toast-notification==1.1.0", # MIT License, not finalized yet
     "jsonschema>=3.2.0, <5", # MIT License
     "dictdiffer==0.9.0",  # MIT License
     # compatibility
     'contextlib-chdir==1.0.2; python_version<"3.11"',  # BSD License (BSD-3-Clause)
     'typing-extensions>=3.10.0.2, <5',  # Python Software Foundation License(PSF)
     "packaging",  # use the built-in, or get latest if there is some issue with pip
     # transitive compatibility
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     """ Start the Qt application and load the main window """
     init_platform()
     # Change cwd to temp, so temporary files become writable, 
     # even if the current folder is not - Fixes #168
     os.chdir(gettempdir())
 
     qt_app = load_qapp()
-
     # Loading dialog until Conan is available
     loader = AsyncLoader(None)
     loader.async_loading(None, load_conan, (loader, ), cancel_button=False,
                             loading_text="Starting Conan Explorer")
     loader.wait_for_finished()
 
     # inline imports to optimize load times
@@ -92,14 +91,18 @@
 
     if check_for_wayland(): # enable native Wayland support
         os.environ["QT_QPA_PLATFORM"] = "wayland"
 
     # to use icons in qss file
     QtCore.QDir.addSearchPath('icons', os.path.join(asset_path, 'icons'))
 
+    # disable reacting on light and dark themed mode automatically, otherwise
+    # we can get get dark mode window bar in light mode
+    QtWidgets.QApplication.setDesktopSettingsAware(False)
+
     qt_app = QtWidgets.QApplication([])
     qt_app.setApplicationName(APP_NAME)
     qt_app.setApplicationDisplayName(APP_NAME + " " + __version__)
 
     # Overwrite the excepthook with our own -
     # this will provide a method to report bugs for the user
     sys.excepthook = bug_dialog_exc_hook  # dialog needs qt_app
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/crash.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/crash.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/loading.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/loading.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/base_ui/theming.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/base_ui/theming.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/logger.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/logger.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/system.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/system.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/app/typing.py` & `conan-explorer-2.3.0a3/src/conan_explorer/app/typing.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/config_schema.json` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/config_schema.json`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/font/NotoSans-Regular.ttf` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/font/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/font/NotoSansMono.ttf` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/font/NotoSansMono.ttf`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/conan.png` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/conan.png`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/android.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/android.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/conan_logo.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/conan_logo.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/grid.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/grid.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/linux.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/linux.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/mac_os.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/mac_os.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/package.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/package.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/package_explorer.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/package_explorer.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/search_packages.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/search_packages.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/global/windows.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/global/windows.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/icon.ico` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/about.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/about.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/cleanup.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/cleanup.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/cut.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/cut.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/export_notes.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/export_notes.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/file_preview.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/file_preview.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/hide.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/hide.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/no-access.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/no-access.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/plugin.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/plugin.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/plus_rounded.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/plus_rounded.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/remove-lock.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/remove-lock.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/remove-lock2.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/remove-lock2.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/search_packages.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/search_packages.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/settings.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/settings.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/show.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/show.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/assets/icons/material/view.svg` & `conan-explorer-2.3.0a3/src/conan_explorer/assets/icons/material/view.svg`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conanV1.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conanV1.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conanV2.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conanV2.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conan_cache.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conan_cache.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conan_cleanup.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conan_cleanup.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/conan_worker.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/conan_worker.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/types.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/types.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/conan_wrapper/unified_api.py` & `conan-explorer-2.3.0a3/src/conan_explorer/conan_wrapper/unified_api.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/settings/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/settings/ini_file.py` & `conan-explorer-2.3.0a3/src/conan_explorer/settings/ini_file.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/common/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/common/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/common/icon.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/common/icon.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/common/logger.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/common/logger.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/common/model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/common/model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/common/syntax_highlighting.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/common/syntax_highlighting.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/common/theming.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/common/theming.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dark_style.qss.in` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dark_style.qss.in`

 * *Files 0% similar despite different names*

```diff
@@ -557,7 +557,11 @@
 QTreeView::branch:hover:closed:has-children {
     image: url(icons:material/forward_b.svg);
 }
 QTreeView::branch:hover:open:has-children:hover {
     image: url(icons:material/expand_b.svg);
 }
 
+Toast .QLabel{
+    font-size: 10pt;
+    color: #5c5c5c;
+}
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/conan_install.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/conan_install.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/conan_install.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/conan_install.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_install/conan_install_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_install/conan_install_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/conan_remove.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/conan_remove.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/crash.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/crash.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/crash.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/crash.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/crash/crash_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/crash/crash_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selection.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selection.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/file_editor_selection/file_editor_selector_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/diff.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/diff.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/diff.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/diff.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/pkg_diff/diff_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/pkg_diff/diff_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/dialogs/reorder_dialog/reorder_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/fluent_window.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/fluent_window.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/fluent_window.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/fluent_window_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/fluent_window_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/side_menu.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/side_menu.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/side_menu.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/side_menu.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/fluent_window/side_menu_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/fluent_window/side_menu_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/light_style.qss.in` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/light_style.qss.in`

 * *Files 0% similar despite different names*

```diff
@@ -493,7 +493,11 @@
 }
 QTreeView::branch:hover:closed:has-children {
     image: url(icons:material/forward_b.svg);
 }
 QTreeView::branch:hover:open:has-children:hover {
     image: url(icons:material/expand_b.svg);
 }
+
+Toast .QLabel{
+    font-size: 10pt;
+}
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/main_window.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/main_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from conan_explorer.app.system import delete_path
 from conan_explorer.settings import (AUTO_OPEN_LAST_VIEW, CONSOLE_SPLIT_SIZES, FILE_EDITOR_EXECUTABLE,
     FONT_SIZE, GUI_MODE, GUI_MODE_DARK, GUI_MODE_LIGHT, GUI_STYLE, GUI_STYLE_FLUENT,
     GUI_STYLE_MATERIAL, LAST_CONFIG_FILE, LAST_VIEW, WINDOW_SIZE)
 from conan_explorer.ui.common.theming import (get_gui_dark_mode, get_gui_style, 
                                                   get_themed_asset_icon)
 from conan_explorer.ui.dialogs import FileEditorSelDialog
+from conan_explorer.ui.notifier_service import NotifierService
 from conan_explorer.ui.plugin import PluginHandler
 from conan_explorer.ui.widgets import AnimatedToggle, WideMessageBox
 
 from .common import init_qt_logger, remove_qt_logger
 from .fluent_window import FluentWindow, SideSubMenu
 from .views.app_grid.config.model import UiApplicationModel
 from .plugin import PluginInterfaceV1
@@ -206,15 +207,15 @@
         if app.active_settings.get_bool(AUTO_OPEN_LAST_VIEW):
             try:
                 last_view = app.active_settings.get_string(LAST_VIEW)
                 page = self.page_widgets.get_page_by_name(last_view)
                 self.page_widgets.get_button_by_type(type(page)).click()
             except Exception as e:
                 Logger().debug("Can't switch to page for auto open: " + str(e))
-        
+        self.notifier = NotifierService(self)
         self.loaded = True
 
     def _load_plugins(self):
         self._plugin_handler.load_all_plugins()
 
     def _load_job(self, config_source: str):
         self._plugin_handler.post_load_plugins()
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/file.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/file.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/handler.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/handler.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/plugin/types.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/plugin/types.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/plugins.ini` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/plugins.ini`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about_page.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about_page.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about_text.html` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about_text.html`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/about/about_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/about/about_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/app_link.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/app_link.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/app_link.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/app_link.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/app_link_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/app_link_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/json_file.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/json_file.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/config/model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/config/model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/dialogs/app_edit_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/app_grid/tab.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/app_grid/tab.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/conan_conf.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/conan_conf.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/conan_conf.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/conan_conf.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/conan_conf_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/conan_conf_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/editable_edit_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_edit_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/dialogs/remote_login_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/editable_controller.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/editable_controller.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/editable_model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/editable_model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/profiles_model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/profiles_model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/remotes_controller.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/remotes_controller.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_conf/remotes_model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_conf/remotes_model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/conan_search.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/conan_search.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/conan_search.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/conan_search.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/conan_search_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/conan_search_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/controller.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/controller.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/conan_search/model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/conan_search/model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/file_controller.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/file_controller.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/file_model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/file_model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/package_explorer.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/package_explorer.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/package_explorer.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/package_explorer.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/package_explorer_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/package_explorer_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/sel_controller.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/sel_controller.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/package_explorer/sel_model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/package_explorer/sel_model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/controller.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/controller.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/model.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/model.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/plugins.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/plugins.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/plugins.ui` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/plugins.ui`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/views/plugins_manager/plugins_ui.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/views/plugins_manager/plugins_ui.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/__init__.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/clickable_icon.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/clickable_icon.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/conan_line_edit.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/conan_line_edit.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/password_line_edit.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/password_line_edit.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer/ui/widgets/toggle.py` & `conan-explorer-2.3.0a3/src/conan_explorer/ui/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer.egg-info/PKG-INFO` & `conan-explorer-2.3.0a3/src/conan_explorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-explorer
-Version: 2.3.0a2
+Version: 2.3.0a3
 Summary: Package Explorer and App Launcher for Conan
 Home-page: https://github.com/goszpeti/conan_explorer
 Author: Péter Gosztolya and Contributors
 License: LGPL v3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,15 @@
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: conan<2.2,>=1.48
 Requires-Dist: PySide6-Essentials>=6.4.0
+Requires-Dist: pyqt-toast-notification==1.1.0
 Requires-Dist: jsonschema<5,>=3.2.0
 Requires-Dist: dictdiffer==0.9.0
 Requires-Dist: contextlib-chdir==1.0.2; python_version < "3.11"
 Requires-Dist: typing-extensions<5,>=3.10.0.2
 Requires-Dist: packaging
 Requires-Dist: Jinja2<4,>=2.3
 Provides-Extra: dev
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer.egg-info/SOURCES.txt` & `conan-explorer-2.3.0a3/src/conan_explorer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 src/conan_explorer/conan_wrapper/unified_api.py
 src/conan_explorer/settings/__init__.py
 src/conan_explorer/settings/ini_file.py
 src/conan_explorer/ui/__init__.py
 src/conan_explorer/ui/dark_style.qss.in
 src/conan_explorer/ui/light_style.qss.in
 src/conan_explorer/ui/main_window.py
+src/conan_explorer/ui/notifier_service.py
 src/conan_explorer/ui/plugins.ini
 src/conan_explorer/ui/common/__init__.py
 src/conan_explorer/ui/common/icon.py
 src/conan_explorer/ui/common/logger.py
 src/conan_explorer/ui/common/model.py
 src/conan_explorer/ui/common/syntax_highlighting.py
 src/conan_explorer/ui/common/theming.py
```

### Comparing `conan-explorer-2.3.0a2/src/conan_explorer.egg-info/requires.txt` & `conan-explorer-2.3.0a3/src/conan_explorer.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 conan<2.2,>=1.48
 PySide6-Essentials>=6.4.0
+pyqt-toast-notification==1.1.0
 jsonschema<5,>=3.2.0
 dictdiffer==0.9.0
 typing-extensions<5,>=3.10.0.2
 packaging
 Jinja2<4,>=2.3
 
 [:python_version < "3.11"]
```

### Comparing `conan-explorer-2.3.0a2/test/testdata/settings/read/config.ini` & `conan-explorer-2.3.0a3/test/testdata/settings/read/config.ini`

 * *Files identical despite different names*

