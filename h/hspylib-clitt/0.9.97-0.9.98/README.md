# Comparing `tmp/hspylib-clitt-0.9.97.tar.gz` & `tmp/hspylib-clitt-0.9.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-clitt-0.9.97.tar", last modified: Thu Sep 21 22:10:02 2023, max compression
+gzip compressed data, was "hspylib-clitt-0.9.98.tar", last modified: Tue Oct  3 22:20:28 2023, max compression
```

## Comparing `hspylib-clitt-0.9.97.tar` & `hspylib-clitt-0.9.98.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.748916 hspylib-clitt-0.9.97/clitt/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/.version
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/__classpath__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5327 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.748916 hspylib-clitt-0.9.97/clitt/addons/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.748916 hspylib-clitt-0.9.97/clitt/addons/appman/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/addons/appman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/appman.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/appman_enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.748916 hspylib-clitt-0.9.97/clitt/addons/appman/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/build.gradle.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/classpath.py.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/dependencies.hspd.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/gitignore.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/main.py.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/main_qt.py.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/main_qt_view.py.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/main_qt_view.ui.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/run.sh.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/test_main.py.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/usage.txt.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/appman/templates/widget.py.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.748916 hspylib-clitt-0.9.97/clitt/addons/widman/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/addons/widman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widget_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/addons/widman/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_free.py
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_punch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_send_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_time_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/addons/widman/widman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/core/exception/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/exception/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/core/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/icons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/core/icons/emojis/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/icons/emojis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/emojis/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/emojis/face_smiling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/app_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/awesome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/dashboard_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/form_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/game_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/nav_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/trickplay_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/widget_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.752916 hspylib-clitt-0.9.97/clitt/core/term/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/term/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/term/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/term/screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/term/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.756917 hspylib-clitt-0.9.97/clitt/core/tui/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.756917 hspylib-clitt-0.9.97/clitt/core/tui/mchoose/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/mchoose/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mchoose/mchoose.py
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mchoose/menu_choose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.756917 hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/dashboard_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/dashboard_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      890 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/mdashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/menu_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.756917 hspylib-clitt-0.9.97/clitt/core/tui/menu/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.756917 hspylib-clitt-0.9.97/clitt/core/tui/minput/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/access_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/field_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/form_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/form_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/input_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/input_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/menu_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1607 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/minput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/minput/minput_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/clitt/core/tui/mselect/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/mselect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mselect/menu_select.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/mselect/mselect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/clitt/core/tui/table/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/core/tui/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/table/table_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/table/table_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/tui_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/tui_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/core/tui/tui_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/clitt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-21 22:09:56.000000 hspylib-clitt-0.9.97/clitt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/utils/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/clitt/welcome.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/hspylib_clitt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-09-21 22:10:02.000000 hspylib-clitt-0.9.97/hspylib_clitt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-09-21 22:10:02.000000 hspylib-clitt-0.9.97/hspylib_clitt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 22:10:02.000000 hspylib-clitt-0.9.97/hspylib_clitt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 22:10:02.000000 hspylib-clitt-0.9.97/hspylib_clitt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-21 22:10:02.000000 hspylib-clitt-0.9.97/hspylib_clitt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 22:10:02.760917 hspylib-clitt-0.9.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2023-09-21 22:09:07.000000 hspylib-clitt-0.9.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.207773 hspylib-clitt-0.9.98/clitt/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/.version
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/__classpath__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5327 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.207773 hspylib-clitt-0.9.98/clitt/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.207773 hspylib-clitt-0.9.98/clitt/addons/appman/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/addons/appman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/appman.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/appman_enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.207773 hspylib-clitt-0.9.98/clitt/addons/appman/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/build.gradle.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/classpath.py.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/dependencies.hspd.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/gitignore.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/main.py.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/main_qt.py.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/main_qt_view.py.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/main_qt_view.ui.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/run.sh.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/test_main.py.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/usage.txt.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/appman/templates/widget.py.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.211773 hspylib-clitt-0.9.98/clitt/addons/widman/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/addons/widman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widget_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.211773 hspylib-clitt-0.9.98/clitt/addons/widman/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_punch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_send_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_time_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/addons/widman/widman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.211773 hspylib-clitt-0.9.98/clitt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.211773 hspylib-clitt-0.9.98/clitt/core/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/exception/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.211773 hspylib-clitt-0.9.98/clitt/core/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/icons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.211773 hspylib-clitt-0.9.98/clitt/core/icons/emojis/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/icons/emojis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/emojis/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/emojis/face_smiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.215773 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/app_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/awesome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/dashboard_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/form_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/game_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/nav_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/trickplay_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/widget_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.215773 hspylib-clitt-0.9.98/clitt/core/term/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/term/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/term/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/term/screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/term/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.215773 hspylib-clitt-0.9.98/clitt/core/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.215773 hspylib-clitt-0.9.98/clitt/core/tui/mchoose/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/mchoose/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mchoose/mchoose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mchoose/menu_choose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.219773 hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/dashboard_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/dashboard_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      890 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/mdashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/menu_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.219773 hspylib-clitt-0.9.98/clitt/core/tui/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/clitt/core/tui/minput/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/access_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/field_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/form_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/form_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/input_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/menu_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1607 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/minput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/minput/minput_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/clitt/core/tui/mselect/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/mselect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mselect/menu_select.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/mselect/mselect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/clitt/core/tui/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/core/tui/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/table/table_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/table/table_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/tui_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/tui_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/core/tui/tui_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/clitt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-10-03 22:20:22.000000 hspylib-clitt-0.9.98/clitt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/utils/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/clitt/welcome.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/hspylib_clitt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-03 22:20:28.000000 hspylib-clitt-0.9.98/hspylib_clitt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-10-03 22:20:28.000000 hspylib-clitt-0.9.98/hspylib_clitt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-03 22:20:28.000000 hspylib-clitt-0.9.98/hspylib_clitt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-03 22:20:28.000000 hspylib-clitt-0.9.98/hspylib_clitt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-03 22:20:28.000000 hspylib-clitt-0.9.98/hspylib_clitt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-03 22:20:28.223773 hspylib-clitt-0.9.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2023-10-03 22:19:44.000000 hspylib-clitt-0.9.98/setup.py
```

### Comparing `hspylib-clitt-0.9.97/PKG-INFO` & `hspylib-clitt-0.9.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-clitt
-Version: 0.9.97
+Version: 0.9.98
 Summary: HsPyLib - CLI Terminal Tools
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-clitt/
@@ -31,12 +31,12 @@
 Requires-Dist: urllib3<2.0.0
 
 # HsPyLib - CLI Terminal Tools
 
 ## Create professional CLI applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-clitt)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-clitt-0.9.97/README.md` & `hspylib-clitt-0.9.98/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - CLI Terminal Tools
 
 ## Create professional CLI applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-clitt)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-clitt-0.9.97/clitt/__classpath__.py` & `hspylib-clitt-0.9.98/clitt/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/__main__.py` & `hspylib-clitt-0.9.98/clitt/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/appman.py` & `hspylib-clitt-0.9.98/clitt/addons/appman/appman.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/appman_enums.py` & `hspylib-clitt-0.9.98/clitt/addons/appman/appman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/build.gradle.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/build.gradle.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/dependencies.hspd.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/dependencies.hspd.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/gitignore.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/gitignore.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/main.py.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/main.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/main_qt.py.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/main_qt.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/main_qt_view.py.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/main_qt_view.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/main_qt_view.ui.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/main_qt_view.ui.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/test_main.py.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/test_main.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/appman/templates/widget.py.tpl` & `hspylib-clitt-0.9.98/clitt/addons/appman/templates/widget.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widget.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widget.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widget_entry.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widget_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_free.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_free.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_punch.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_punch.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_send_msg.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_send_msg.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widgets/widget_time_calc.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widgets/widget_time_calc.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/addons/widman/widman.py` & `hspylib-clitt-0.9.98/clitt/addons/widman/widman.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/emojis/emojis.py` & `hspylib-clitt-0.9.98/clitt/core/icons/emojis/emojis.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/emojis/face_smiling.py` & `hspylib-clitt-0.9.98/clitt/core/icons/emojis/face_smiling.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/app_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/app_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/awesome.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/awesome.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/dashboard_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/dashboard_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/form_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/form_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/game_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/game_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/nav_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/nav_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/trickplay_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/trickplay_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/icons/font_awesome/widget_icons.py` & `hspylib-clitt-0.9.98/clitt/core/icons/font_awesome/widget_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/preferences.py` & `hspylib-clitt-0.9.98/clitt/core/preferences.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/term/commons.py` & `hspylib-clitt-0.9.98/clitt/core/term/commons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/term/cursor.py` & `hspylib-clitt-0.9.98/clitt/core/term/cursor.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/term/screen.py` & `hspylib-clitt-0.9.98/clitt/core/term/screen.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/term/terminal.py` & `hspylib-clitt-0.9.98/clitt/core/term/terminal.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mchoose/mchoose.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mchoose/mchoose.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mchoose/menu_choose.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mchoose/menu_choose.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/dashboard_builder.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/dashboard_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/dashboard_item.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/mdashboard.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/mdashboard.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mdashboard/menu_dashboard.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mdashboard/menu_dashboard.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu.py` & `hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_action.py` & `hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_action.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_factory.py` & `hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_item.py` & `hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_item.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_ui.py` & `hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_ui.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/menu/tui_menu_view.py` & `hspylib-clitt-0.9.98/clitt/core/tui/menu/tui_menu_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/access_type.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/access_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/field_builder.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/field_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/form_builder.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/form_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/form_field.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/form_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/input_type.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/input_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/input_validator.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/input_validator.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/menu_input.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/menu_input.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/minput.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/minput.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/minput/minput_utils.py` & `hspylib-clitt-0.9.98/clitt/core/tui/minput/minput_utils.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mselect/menu_select.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mselect/menu_select.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/mselect/mselect.py` & `hspylib-clitt-0.9.98/clitt/core/tui/mselect/mselect.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/table/table_enums.py` & `hspylib-clitt-0.9.98/clitt/core/tui/table/table_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/table/table_renderer.py` & `hspylib-clitt-0.9.98/clitt/core/tui/table/table_renderer.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/tui_application.py` & `hspylib-clitt-0.9.98/clitt/core/tui/tui_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/tui_component.py` & `hspylib-clitt-0.9.98/clitt/core/tui/tui_component.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/core/tui/tui_preferences.py` & `hspylib-clitt-0.9.98/clitt/core/tui/tui_preferences.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/clitt/utils/git_utils.py` & `hspylib-clitt-0.9.98/clitt/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/hspylib_clitt.egg-info/PKG-INFO` & `hspylib-clitt-0.9.98/hspylib_clitt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-clitt
-Version: 0.9.97
+Version: 0.9.98
 Summary: HsPyLib - CLI Terminal Tools
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-clitt/
@@ -31,12 +31,12 @@
 Requires-Dist: urllib3<2.0.0
 
 # HsPyLib - CLI Terminal Tools
 
 ## Create professional CLI applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-clitt)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-clitt-0.9.97/hspylib_clitt.egg-info/SOURCES.txt` & `hspylib-clitt-0.9.98/hspylib_clitt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.97/setup.py` & `hspylib-clitt-0.9.98/setup.py`

 * *Files identical despite different names*

