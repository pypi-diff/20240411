# Comparing `tmp/qimview-1.0.9.tar.gz` & `tmp/qimview-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qimview-1.0.9.tar", last modified: Wed Dec  6 08:58:03 2023, max compression
+gzip compressed data, was "qimview-1.1.0.tar", last modified: Thu Apr 11 21:09:10 2024, max compression
```

## Comparing `qimview-1.0.9.tar` & `qimview-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.535145 qimview-1.0.9/
--rw-rw-r--   0 karl      (1000) karl      (1000)    11323 2023-10-21 21:07:24.000000 qimview-1.0.9/LICENSE.txt
--rw-r--r--   0 karl      (1000) karl      (1000)     1976 2023-12-06 08:58:03.531145 qimview-1.0.9/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      876 2023-10-22 19:06:06.000000 qimview-1.0.9/README.md
--rw-rw-r--   0 karl      (1000) karl      (1000)     1341 2023-11-12 18:05:33.000000 qimview-1.0.9/pyproject.toml
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.483153 qimview-1.0.9/qimview/
--rw-rw-r--   0 karl      (1000) karl      (1000)       88 2023-12-06 08:54:07.000000 qimview-1.0.9/qimview/__init__.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.499150 qimview-1.0.9/qimview/cache/
--rw-rw-r--   0 karl      (1000) karl      (1000)      108 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/cache/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     4481 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/cache/basecache.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     5223 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/cache/filecache.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     4939 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/cache/imagecache.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.503150 qimview-1.0.9/qimview/cpp_bind/
--rw-rw-r--   0 karl      (1000) karl      (1000)     3789 2023-12-06 08:53:10.000000 qimview-1.0.9/qimview/cpp_bind/image_histogram.hpp
--rw-rw-r--   0 karl      (1000) karl      (1000)     8374 2023-12-06 08:53:10.000000 qimview-1.0.9/qimview/cpp_bind/image_resize.hpp
--rw-rw-r--   0 karl      (1000) karl      (1000)    21749 2023-12-06 08:53:10.000000 qimview-1.0.9/qimview/cpp_bind/image_to_rgb.hpp
--rw-rw-r--   0 karl      (1000) karl      (1000)     3891 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/cpp_bind/qimview_cpp.cpp
--rw-rw-r--   0 karl      (1000) karl      (1000)      733 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/cpp_bind/test_speed.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      505 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/cpp_bind/test_speed_resize.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.511149 qimview-1.0.9/qimview/image_readers/
--rw-rw-r--   0 karl      (1000) karl      (1000)       74 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/image_readers/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     4844 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_readers/image_reader.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1524 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/image_readers/libraw_reader.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2483 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/image_readers/opencv_reader.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1433 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/image_readers/simplejpeg_reader.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2375 2023-11-20 08:25:08.000000 qimview-1.0.9/qimview/image_readers/turbojpeg_reader.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.519147 qimview-1.0.9/qimview/image_viewers/
--rw-rw-r--   0 karl      (1000) karl      (1000)      607 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/image_viewers/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2997 2023-11-20 08:25:08.000000 qimview-1.0.9/qimview/image_viewers/fullscreen_helper.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     4187 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/image_viewers/gl_image_viewer.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    16159 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/gl_image_viewer_base.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    14808 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/gl_image_viewer_shaders.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1632 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/image_viewers/image_filter_parameters.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2538 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/image_viewers/image_filter_parameters_gui.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    24699 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/image_viewer.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     8773 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/image_viewer_key_events.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     6983 2023-12-06 08:53:10.000000 qimview-1.0.9/qimview/image_viewers/image_viewer_mouse_events.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     8310 2023-12-06 08:53:10.000000 qimview-1.0.9/qimview/image_viewers/mouse_events.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    30438 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/multi_view.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     8343 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/multi_view_key_events.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2124 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/image_viewers/multi_view_mouse_events.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    37409 2023-12-06 08:53:10.000000 qimview-1.0.9/qimview/image_viewers/qt_image_viewer.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     6241 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/imview.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3119 2023-11-20 08:25:08.000000 qimview-1.0.9/qimview/mview.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.519147 qimview-1.0.9/qimview/parameters/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/parameters/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1009 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/parameters/numeric_parameter.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2167 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/parameters/numeric_parameter_gui.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.475154 qimview-1.0.9/qimview/pytests/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.523147 qimview-1.0.9/qimview/pytests/tutorial/
--rw-rw-r--   0 karl      (1000) karl      (1000)      238 2023-10-22 15:41:33.000000 qimview-1.0.9/qimview/pytests/tutorial/test_div_by_3_6.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      192 2023-10-22 15:41:33.000000 qimview-1.0.9/qimview/pytests/tutorial/test_square.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.523147 qimview-1.0.9/qimview/tests_utils/
--rw-rw-r--   0 karl      (1000) karl      (1000)     2386 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/tests_utils/event_player.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1978 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/tests_utils/event_recorder.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     5837 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/tests_utils/qtdump.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.531145 qimview-1.0.9/qimview/utils/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/utils/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      470 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/utils/import_tools.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1819 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/utils/menu_selection.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      791 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/utils/mvlabel.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      276 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/utils/qt_imports.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1734 2023-10-21 21:07:24.000000 qimview-1.0.9/qimview/utils/suffix_auto.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2311 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/utils/tab_dialog.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3204 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/utils/thread_pool.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     2232 2023-11-02 00:13:31.000000 qimview-1.0.9/qimview/utils/utils.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     4161 2023-12-02 17:41:45.000000 qimview-1.0.9/qimview/utils/viewer_image.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.531145 qimview-1.0.9/qimview/video_player/
--rw-rw-r--   0 karl      (1000) karl      (1000)      247 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/video_player/test_videoplayer.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     8799 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/video_player/video_player.py
--rw-rw-r--   0 karl      (1000) karl      (1000)    12376 2023-11-12 17:56:54.000000 qimview-1.0.9/qimview/video_player/vlc_player.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2023-12-06 08:58:03.531145 qimview-1.0.9/qimview.egg-info/
--rw-r--r--   0 karl      (1000) karl      (1000)     1976 2023-12-06 08:58:03.000000 qimview-1.0.9/qimview.egg-info/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)     2198 2023-12-06 08:58:03.000000 qimview-1.0.9/qimview.egg-info/SOURCES.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2023-12-06 08:58:03.000000 qimview-1.0.9/qimview.egg-info/dependency_links.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       74 2023-12-06 08:58:03.000000 qimview-1.0.9/qimview.egg-info/entry_points.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)      212 2023-12-06 08:58:03.000000 qimview-1.0.9/qimview.egg-info/requires.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       20 2023-12-06 08:58:03.000000 qimview-1.0.9/qimview.egg-info/top_level.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       38 2023-12-06 08:58:03.535145 qimview-1.0.9/setup.cfg
--rw-rw-r--   0 karl      (1000) karl      (1000)     1973 2023-12-06 08:53:10.000000 qimview-1.0.9/setup.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.882859 qimview-1.1.0/
+-rw-rw-r--   0 karl      (1000) karl      (1000)    11323 2023-10-21 21:07:24.000000 qimview-1.1.0/LICENSE.txt
+-rw-r--r--   0 karl      (1000) karl      (1000)     2068 2024-04-11 21:09:10.882859 qimview-1.1.0/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      876 2023-10-22 19:06:06.000000 qimview-1.1.0/README.md
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1441 2024-04-11 21:07:46.000000 qimview-1.1.0/pyproject.toml
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.846859 qimview-1.1.0/qimview/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       88 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/__init__.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.850859 qimview-1.1.0/qimview/cache/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      108 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/cache/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     4519 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/cache/basecache.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     5229 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/cache/filecache.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     4945 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/cache/imagecache.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.862859 qimview-1.1.0/qimview/cpp_bind/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3789 2023-12-06 08:53:10.000000 qimview-1.1.0/qimview/cpp_bind/image_histogram.hpp
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8374 2023-12-06 08:53:10.000000 qimview-1.1.0/qimview/cpp_bind/image_resize.hpp
+-rw-rw-r--   0 karl      (1000) karl      (1000)    21749 2023-12-06 08:53:10.000000 qimview-1.1.0/qimview/cpp_bind/image_to_rgb.hpp
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3891 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/cpp_bind/qimview_cpp.cpp
+-rw-rw-r--   0 karl      (1000) karl      (1000)      733 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/cpp_bind/test_speed.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      505 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/cpp_bind/test_speed_resize.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.862859 qimview-1.1.0/qimview/image_readers/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       74 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/image_readers/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     4844 2023-12-02 17:41:45.000000 qimview-1.1.0/qimview/image_readers/image_reader.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1524 2023-11-12 17:56:54.000000 qimview-1.1.0/qimview/image_readers/libraw_reader.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2483 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/image_readers/opencv_reader.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1433 2023-11-12 17:56:54.000000 qimview-1.1.0/qimview/image_readers/simplejpeg_reader.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2375 2023-11-20 08:25:08.000000 qimview-1.1.0/qimview/image_readers/turbojpeg_reader.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.870859 qimview-1.1.0/qimview/image_viewers/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      607 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/image_viewers/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2997 2023-11-20 08:25:08.000000 qimview-1.1.0/qimview/image_viewers/fullscreen_helper.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     4269 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/gl_image_viewer.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    14327 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/gl_image_viewer_base.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    26395 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/gl_image_viewer_shaders.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1632 2023-11-02 00:13:31.000000 qimview-1.1.0/qimview/image_viewers/image_filter_parameters.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2900 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/image_filter_parameters_gui.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    25838 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/image_viewer.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     9340 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/image_viewer_key_events.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     7077 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/image_viewer_mouse_events.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8310 2023-12-06 08:53:10.000000 qimview-1.1.0/qimview/image_viewers/mouse_events.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    30555 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/multi_view.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8343 2023-12-02 17:41:45.000000 qimview-1.1.0/qimview/image_viewers/multi_view_key_events.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2722 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/multi_view_mouse_events.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    38293 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/image_viewers/qt_image_viewer.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     6262 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/imview.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3190 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/mview.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     5311 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/npViewer.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.870859 qimview-1.1.0/qimview/parameters/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/parameters/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1009 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/parameters/numeric_parameter.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3808 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/parameters/numeric_parameter_gui.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.838859 qimview-1.1.0/qimview/pytests/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.870859 qimview-1.1.0/qimview/pytests/tutorial/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      238 2023-10-22 15:41:33.000000 qimview-1.1.0/qimview/pytests/tutorial/test_div_by_3_6.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      192 2023-10-22 15:41:33.000000 qimview-1.1.0/qimview/pytests/tutorial/test_square.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.874859 qimview-1.1.0/qimview/tests_utils/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2386 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/tests_utils/event_player.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1978 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/tests_utils/event_recorder.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     5837 2023-12-02 17:41:45.000000 qimview-1.1.0/qimview/tests_utils/qtdump.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.878859 qimview-1.1.0/qimview/utils/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/utils/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      470 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/utils/import_tools.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1819 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/utils/menu_selection.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      791 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/utils/mvlabel.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      303 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/utils/qt_imports.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1734 2023-10-21 21:07:24.000000 qimview-1.1.0/qimview/utils/suffix_auto.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2311 2023-12-02 17:41:45.000000 qimview-1.1.0/qimview/utils/tab_dialog.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3670 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/utils/thread_pool.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2084 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/utils/utils.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     5093 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/utils/viewer_image.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.878859 qimview-1.1.0/qimview/video_player/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      247 2023-11-12 17:56:54.000000 qimview-1.1.0/qimview/video_player/test_videoplayer.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8817 2024-04-11 21:07:46.000000 qimview-1.1.0/qimview/video_player/video_player.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)    12376 2023-11-12 17:56:54.000000 qimview-1.1.0/qimview/video_player/vlc_player.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-11 21:09:10.878859 qimview-1.1.0/qimview.egg-info/
+-rw-r--r--   0 karl      (1000) karl      (1000)     2068 2024-04-11 21:09:10.000000 qimview-1.1.0/qimview.egg-info/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)     2218 2024-04-11 21:09:10.000000 qimview-1.1.0/qimview.egg-info/SOURCES.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-11 21:09:10.000000 qimview-1.1.0/qimview.egg-info/dependency_links.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       74 2024-04-11 21:09:10.000000 qimview-1.1.0/qimview.egg-info/entry_points.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)      237 2024-04-11 21:09:10.000000 qimview-1.1.0/qimview.egg-info/requires.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       31 2024-04-11 21:09:10.000000 qimview-1.1.0/qimview.egg-info/top_level.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-11 21:09:10.882859 qimview-1.1.0/setup.cfg
+-rw-rw-r--   0 karl      (1000) karl      (1000)     8014 2024-04-11 21:07:46.000000 qimview-1.1.0/setup.py
```

### Comparing `qimview-1.0.9/LICENSE.txt` & `qimview-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/PKG-INFO` & `qimview-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: qimview
-Version: 1.0.9
+Version: 1.1.0
 Summary: Library for multiple image visualization and comparison
 Author-email: Karl Krissian <karl.krissian@gmail.com>
 Project-URL: Homepage, https://github.com/qimview/qimview
 Project-URL: Wiki, https://github.com/qimview/qimview/wiki
 Project-URL: Bug Tracker, https://github.com/qimview/qimview/issues
 Project-URL: API, https://qimview.github.io/qimview/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: opencv_python>=4.2
 Requires-Dist: psutil>=5.8.0
 Requires-Dist: PyOpenGL>=3.1.5
 Requires-Dist: PySide6>=6.5.2
 Requires-Dist: PySide6_Addons>=6.5.1.1
 Requires-Dist: PySide6_Essentials>=6.5.1.1
 Requires-Dist: simplejpeg>=1.4.0
 Provides-Extra: extra
 Requires-Dist: rawpy>=0.16.0; extra == "extra"
 Requires-Dist: python_vlc>=3.0.11115; extra == "extra"
 Requires-Dist: PyTurboJPEG>=1.4.1; extra == "extra"
+Requires-Dist: PyOpenGL_accelerate; extra == "extra"
+Requires-Dist: PyAV; extra == "extra"
 
 # Description
 _qimview_ (qt-based image view) is a set of classes that are designed to visualize and compare images. 
 It uses Python as the main language, and include some code in C++ or OpenGL shading language.
 Main features are:
 * **image reader**: read type image format (like jpeg and png) and also raw image format (bayer images)
 * **image cache**: save image reading/uncompressing time by loading previously read image into a buffer
```

### Comparing `qimview-1.0.9/README.md` & `qimview-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/pyproject.toml` & `qimview-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = [
   "setuptools", 
   "pybind11>=2.10.0",
+  "cmake>=3.21",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 dynamic = ["version"]
 name = "qimview"
 authors = [
   { name="Karl Krissian", email="karl.krissian@gmail.com" },
 ]
 description = "Library for multiple image visualization and comparison"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
@@ -33,27 +34,32 @@
 ]
 
 [project.optional-dependencies]
 extra = [
     "rawpy>=0.16.0",
     "python_vlc>=3.0.11115",
     "PyTurboJPEG>=1.4.1",
+    "PyOpenGL_accelerate", 
+    "PyAV",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/qimview/qimview"
 "Wiki" = "https://github.com/qimview/qimview/wiki"
 "Bug Tracker" = "https://github.com/qimview/qimview/issues"
 "API" = "https://qimview.github.io/qimview/"
 
 [tool.pytest.ini_options]
 testpaths = [
     "qimview/pytests",
 ]
 
+[tool.setuptools]
+packages = ["qimview"]
+
 [tool.setuptools.dynamic]
 version = {attr = "qimview.__version__"}
 
 [project.scripts]
 # Single image viewer
 imview = "qimview.imview:main"
 # Mutiple image viewer
```

### Comparing `qimview-1.0.9/qimview/cache/basecache.py` & `qimview-1.1.0/qimview/cache/basecache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from collections import deque
+from typing import List, TypeVar, Optional, Generic, Any, Tuple
+
 from qimview.utils.utils      import deep_getsizeof
 from qimview.utils.thread_pool import ThreadPool
 from qimview.utils.qt_imports import QtWidgets
 
-from collections import deque
-from typing import List, TypeVar, Optional, Generic, Any, Tuple
-
 TId    = TypeVar("TId")
 TValue = TypeVar("TValue")
 TExtra = TypeVar("TExtra")
 
 class BaseCache(Generic[TId, TValue, TExtra]):
+    """ Base class for Image and File caches """
     # --- Private methods
     def __init__(self, name : str =""):
         # Python list and deque are thread-safe
-        self.cache      : deque[Tuple[TId, TValue, TExtra]] = deque()
-        self.cache_list : List[TId]                                   = []
-        self.cache_size : int                                         = 0
+        self.cache      : deque[Tuple[TId, TValue, TExtra]]    = deque()
+        self.cache_list : List[TId]                            = []
+        self.cache_size : int                                  = 0
         # Max size in Mb
         self.max_cache_size : int                              = 2000
         self.verbose        : bool                             = False
         self.cache_unit     : int                              = 1024*1024 # Megabyte
         self.thread_pool    : ThreadPool                       = ThreadPool()
         self.memory_bar     : Optional[QtWidgets.QProgressBar] = None
         self._name          : str                              = name
```

### Comparing `qimview-1.0.9/qimview/cache/filecache.py` & `qimview-1.1.0/qimview/cache/filecache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
-from qimview.utils.utils import get_time
-# from qimview.utils.qt_imports import *
-from .basecache import BaseCache
 import os
 from os import path as osp
 import psutil
 from typing import Optional, Tuple
+from qimview.utils.utils import get_time
+# from qimview.utils.qt_imports import *
+from .basecache import BaseCache
 
 class FileCache(BaseCache[str,bytes,float]):
     """
         Save output bytes from read() function into a cache indexed by the filename
         inherits from BaseCache, with
             id as string: input filename
             bytes: output from binary read()
@@ -124,9 +124,9 @@
         # This part may be causing issues
         use_threads = True
         if use_threads:
             self.thread_pool.set_worker(self.thread_add_files, filenames)
             self.thread_pool.set_worker_callbacks(finished_cb=self.on_finished)
             self.thread_pool.start_worker()
         else:
-            self.thread_add_files(filenames, progress_cb=self.show_progress)
+            self.thread_add_files(filenames, progress_callback=self.show_progress)
         self._print_log(f" FileCache.add_files() {self.add_results} took {int((get_time()-start)*1000+0.5)} ms;")
```

### Comparing `qimview-1.0.9/qimview/cache/imagecache.py` & `qimview-1.1.0/qimview/cache/imagecache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 
 from qimview.utils.utils import get_time
 from qimview.image_readers import gb_image_reader
 from .basecache import BaseCache
 import os
 import psutil
-from typing import TYPE_CHECKING
 from qimview.utils.viewer_image import ViewerImage
 
-class ImageCache(BaseCache[str, ViewerImage, float]): 
+class ImageCache(BaseCache[str, ViewerImage, float]):
     """
         Save output bytes from read() function into a cache indexed by the filename
         inherits from BaseCache, with
             id as string: input filename
             ViewerImage: image object
             mtime: modification time as float from osp.getmtime(filename)
         If a file is in the cache but its modification time on disk is more recent,
         we can enable an automatic reload
 
     Args:
         BaseCache (_type_): _description_
-    """    
+    """
     def __init__(self):
         BaseCache.__init__(self, "ImageCache")
         # let use 25% of total memory
         total_memory = psutil.virtual_memory().total / self.cache_unit
         self.max_cache_size = int(total_memory * 0.25)
-        self.verbose : bool = False
+        self.verbose : bool = True
 
     def has_image(self, filename):
         # is it too slow
         filename = os.path.abspath(filename)
         return filename in self.cache_list
 
-    def get_image(self, filename, read_size='full', verbose=False, use_RGB=True, image_transform=None,
+    def get_image(self, filename, read_size='full', verbose=False,
+                  use_RGB=True, image_transform=None,
                   check_size=True):
         """
         :param filename:
         :param show_timing:
         :return: pair image_data, boolean (True is coming from cache)
         """
         start = get_time()
@@ -49,29 +49,30 @@
         if image_data is not None:
             if image_data[2] >= mtime:
                 return image_data[1], True
             else:
                 # Remove outdated cache element
                 self.cache.remove(image_data)
                 self.cache_list.remove(filename)
-        
+
         image = gb_image_reader.read(filename, None, read_size, use_RGB=use_RGB, verbose=verbose,
                                             check_filecache_size=check_size)
         if image is not None:
             if image_transform is not None:
                 image = image_transform(image)
             self.append(filename, image, extra=mtime, check_size=check_size)
             self._print_log(" get_image after read_image took {0:0.3f} sec.".format(get_time() - start))
         else:
             print(f"Failed to load image {filename}")
             return None, False
         return image, False
 
-    def add_image(self, filename, read_size='full', verbose=False, use_RGB=True, image_transform=None,
-                    progress_callback = None):
+    def add_image(self, filename, read_size='full', verbose=False,
+                  use_RGB=True, image_transform=None,
+                  progress_callback = None):
         """
         :param filename:
         :param show_timing:
         :return: pair image_data, boolean (True is coming from cache)
         """
         data, flag = self.get_image(filename, read_size, verbose, use_RGB, image_transform, check_size=False)
         return data is not None
@@ -80,15 +81,16 @@
         pass
         # print(f" *** Added image {os.path.basename(filename)} to cache finished")
 
     def add_result(self, r):
         # print(f"adding {r} to results ")
         self.add_results.append(r)
 
-    def add_images(self, filenames, read_size='full', verbose=False, use_RGB=True, image_transform=None):
+    def add_images(self, filenames, read_size='full', verbose=False,
+                   use_RGB=True, image_transform=None):
         start = get_time()
         self.add_results = []
         num_workers = 0
         for f in filenames:
             if f is not None and not self.has_image(f):
                 # print(f" start worker with image {f}")
                 self.thread_pool.set_worker(self.add_image, f, read_size, verbose, use_RGB, image_transform)
```

### Comparing `qimview-1.0.9/qimview/cpp_bind/image_histogram.hpp` & `qimview-1.1.0/qimview/cpp_bind/image_histogram.hpp`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/cpp_bind/image_resize.hpp` & `qimview-1.1.0/qimview/cpp_bind/image_resize.hpp`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/cpp_bind/image_to_rgb.hpp` & `qimview-1.1.0/qimview/cpp_bind/image_to_rgb.hpp`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/cpp_bind/qimview_cpp.cpp` & `qimview-1.1.0/qimview/cpp_bind/qimview_cpp.cpp`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/cpp_bind/test_speed.py` & `qimview-1.1.0/qimview/cpp_bind/test_speed.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_readers/image_reader.py` & `qimview-1.1.0/qimview/image_readers/image_reader.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_readers/libraw_reader.py` & `qimview-1.1.0/qimview/image_readers/libraw_reader.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_readers/opencv_reader.py` & `qimview-1.1.0/qimview/image_readers/opencv_reader.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_readers/simplejpeg_reader.py` & `qimview-1.1.0/qimview/image_readers/simplejpeg_reader.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_readers/turbojpeg_reader.py` & `qimview-1.1.0/qimview/image_readers/turbojpeg_reader.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_viewers/__init__.py` & `qimview-1.1.0/qimview/image_viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_viewers/fullscreen_helper.py` & `qimview-1.1.0/qimview/image_viewers/fullscreen_helper.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_viewers/gl_image_viewer.py` & `qimview-1.1.0/qimview/image_viewers/gl_image_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
 class GLImageViewer(GLImageViewerBase):
 
     def __init__(self, parent=None, event_recorder=None):
         self.event_recorder = event_recorder
         super().__init__(parent)
         self.setAutoFillBackground(False)
-        self.textureID  = None
-        self.tex_width, self.tex_height = 0, 0
         self.opengl_debug = True
         self.trace_calls  = False
 
     def initializeGL(self):
         """Initialize OpenGL, VBOs, upload data on the GPU, etc.
         """
         # self.setTexture()
@@ -42,20 +40,22 @@
 
     def myPaintGL(self):
         """Paint the scene.
         """
         if self.trace_calls:
             t = trace_method(self.tab)
         self.start_timing()
-        if self.textureID is None:
-            print("GLImageViewer paintGL not textureID")
+        if self.texture is None:
+            print("GLImageViewer paintGL texture not set")
             return
         gl.glClear(gl.GL_COLOR_BUFFER_BIT)
         gl.glTexEnvi(gl.GL_TEXTURE_ENV, gl.GL_TEXTURE_ENV_MODE, gl.GL_DECAL)
-        gl.glBindTexture(gl.GL_TEXTURE_2D, self.textureID)
+        # TODO: fix textureID will only work for RGB textures, not YUV
+        assert self.texture.textureID is not None, "RGB texture not initialized"
+        gl.glBindTexture(gl.GL_TEXTURE_2D, self.texture.textureID)
         # gl.glGenerateMipmap (gl.GL_TEXTURE_2D)
         gl.glEnable(gl.GL_TEXTURE_2D)
         gl.glBegin(gl.GL_QUADS)
 
         x0, x1, y0, y1 = self.image_centered_position()
         x0 = int(x0)
         x1 = int(x1)
```

### Comparing `qimview-1.0.9/qimview/image_viewers/gl_image_viewer_base.py` & `qimview-1.1.0/qimview/image_viewers/gl_image_viewer_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 #
 #
 # started from https://cyrille.rossant.net/2d-graphics-rendering-tutorial-with-pyopengl/
 #
 # check also https://doc.qt.io/archives/4.6/opengl-overpainting.html
 #
 
-from qimview.utils.qt_imports   import QtWidgets, QOpenGLWidget, QtCore, QtGui
-
+import traceback
+from typing import Optional, Tuple
+import numpy as np
 import OpenGL
 OpenGL.ERROR_ON_COPY = True
 import OpenGL.GL as gl
 import OpenGL.GLU as glu
-import traceback
-import numpy as np
-from typing import Optional, Tuple
 
+from .gltexture import GLTexture
+from qimview.utils.qt_imports   import QtWidgets, QOpenGLWidget, QtCore, QtGui
 from qimview.utils.viewer_image import ImageFormat, ViewerImage
 from qimview.image_viewers.image_viewer import ImageViewer, trace_method
 
 
 class GLImageViewerBase(ImageViewer, QOpenGLWidget, ):
 
     def __init__(self, parent : Optional[QtWidgets.QWidget] = None):
         ImageViewer.__init__(self, self)
         QOpenGLWidget.__init__(self, parent)
         self.setAutoFillBackground(False)
 
         _format = QtGui.QSurfaceFormat()
-        print('profile is {}'.format(_format.profile()))
-        print('version is {}'.format(_format.version()))
+        print(f'profile is {_format.profile()}')
+        print(f'version is {_format.version()}')
         # _format.setDepthBufferSize(24)
         # _format.setVersion(4,0)
         # _format.setProfile(PySide2.QtGui.QSurfaceFormat.CoreProfile)
-        _format.setProfile(QtGui.QSurfaceFormat.CompatibilityProfile)
+        _format.setProfile(QtGui.QSurfaceFormat.OpenGLContextProfile.CompatibilityProfile)
         self.setFormat(_format)
 
-        # self.setFormat()
-        self.textureID  = None
-        self.tex_width, self.tex_height = 0, 0
+        self.texture     : GLTexture | None = None
+        # YUV texture of reference image
+        self.texture_ref : GLTexture | None = None
         self.opengl_debug = True
         self.current_text = None
         self.cursor_imx_ratio = 0.5
         self.cursor_imy_ratio = 0.5
         self.trace_calls = False
         self.setMouseTracking(True)
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.ClickFocus)
-
-    # def __del__(self):
-    #     if self.textureID is not None:
-    #         gl.glDeleteTextures(np.array([self.textureID]))
+        # default type
+        self._gl_types = {
+            'int8'   : gl.GL_BYTE,
+            'uint8'  : gl.GL_UNSIGNED_BYTE,
+            'int16'  : gl.GL_SHORT,
+            'uint16' : gl.GL_UNSIGNED_SHORT,
+            'int32'  : gl.GL_INT,
+            'uint32' : gl.GL_UNSIGNED_INT,
+            'float32': gl.GL_FLOAT,
+            'float64': gl.GL_DOUBLE
+        }
 
     def set_image(self, image):
         if self.trace_calls:
             t = trace_method(self.tab)
         changed = super(GLImageViewerBase, self).set_image(image)
 
         if self._image is None:
@@ -62,22 +69,30 @@
             print("Image is resized to a multiple of 4 dimension in X")
             img_width = ((img_width >> 4) << 4)
             im = np.ascontiguousarray(self._image.data[:,:img_width, :])
             self._image = ViewerImage(im, precision = self._image.precision, downscale = 1,
                                         channels = self._image.channels)
             print(self._image.data.shape)
 
-        if changed:  # and self.textureID is not None:
-            print(f"self.textureID {self.textureID}")
+        if changed:
             if self.setTexture():
-                self.show()
-                self.update()
+                # self.show()
+                # self.update()
+                pass
             else:
                 print("setTexture() return False")
 
+    def set_image_fast(self, image, image_ref=None):
+        self._image     = image
+        self._image_ref = image_ref
+        self.image_id += 1
+        res = self.setTexture()
+        if not res: print("setTexture() returned False")
+
+
     def synchronize_data(self, other_viewer):
         super(GLImageViewerBase, self).synchronize_data(other_viewer)
         other_viewer.cursor_imx_ratio = self.cursor_imx_ratio
         other_viewer.cursor_imy_ratio = self.cursor_imy_ratio
 
     def opengl_error(self, force=False):
         if self.opengl_debug or force:
@@ -85,214 +100,153 @@
             if status != gl.GL_NO_ERROR:
                 print(self.tab[0]+'gl error %s' % status)
 
     def setTexture(self) -> bool:
         """
         :return: set opengl texture based on input numpy array image
         """
+
         # gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_GENERATE_MIPMAP_SGIS, gl.GL_TRUE)
 
         if self.trace_calls:
             t = trace_method(self.tab)
         self.start_timing()
         self.makeCurrent()
+        # _gl = QtGui.QOpenGLContext.currentContext().functions()
+        _gl = gl
 
         # Replace texture only if required
         if self._image is None:
             print("self._image is None")
             return False
 
-        img_height, img_width = self._image.data.shape[:2]
-
-        # default type
-        gl_types = {
-            'int8'   : gl.GL_BYTE,
-            'uint8'  : gl.GL_UNSIGNED_BYTE,
-            'int16'  : gl.GL_SHORT,
-            'uint16' : gl.GL_UNSIGNED_SHORT,
-            'int32'  : gl.GL_INT,
-            'uint32' : gl.GL_UNSIGNED_INT,
-            'float32': gl.GL_FLOAT,
-            'float64': gl.GL_DOUBLE
-        }
-        gl_type = gl_types[self._image.data.dtype.name]
-
-        # It seems that the dimension in X should be even
-
-        # Not sure what is the right parameter for internal format of 2D texture based
-        # on the input data type uint8, uint16, ...
-        # need to test with different DXR images
-        internal_format = gl.GL_RGB
-        if self._image.data.shape[2] == 3:
-            if self._image.precision == 8:
-                internal_format = gl.GL_RGB
-            if self._image.precision == 10:
-                internal_format = gl.GL_RGB10
-            if self._image.precision == 12:
-                internal_format = gl.GL_RGB12
-        if self._image.data.shape[2] == 4:
-            if self._image.precision == 8:
-                internal_format = gl.GL_RGBA
-            else:
-                if self._image.precision <= 12:
-                    internal_format = gl.GL_RGBA12
-                else:
-                    if self._image.precision <= 16:
-                        internal_format = gl.GL_RGBA16
-                    else:
-                        internal_format = gl.GL_RGBA32F
-
-        channels2format = {
-            ImageFormat.CH_RGB  : gl.GL_RGB,
-            ImageFormat.CH_BGR  : gl.GL_BGR,
-            ImageFormat.CH_Y    : gl.GL_RED, # not sure about this one
-            ImageFormat.CH_RGGB : gl.GL_RGBA, # we save 4 component data
-            ImageFormat.CH_GRBG : gl.GL_RGBA,
-            ImageFormat.CH_GBRG : gl.GL_RGBA,
-            ImageFormat.CH_BGGR : gl.GL_RGBA
-        }
-        texture_pixel_format = channels2format[self._image.channels]
-
-        if (self.tex_width,self.tex_height) != (img_width,img_height):
-            try:
-                if self.textureID is not None:
-                    gl.glDeleteTextures(np.array([self.textureID]))
-                self.textureID = gl.glGenTextures(1)
-                gl.glPixelStorei(gl.GL_UNPACK_ALIGNMENT, 4)
-                gl.glBindTexture(gl.GL_TEXTURE_2D, self.textureID)
-                gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_BASE_LEVEL, 0)
-                gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_MAX_LEVEL, 0)
-                # gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_MAX_LEVEL, 10)
-                # gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_MIN_FILTER, gl.GL_NEAREST)
-                # gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_MIN_FILTER, gl.GL_NEAREST_MIPMAP_NEAREST)
-                gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_MIN_FILTER, gl.GL_NEAREST)
-                gl.glTexParameteri(gl.GL_TEXTURE_2D, gl.GL_TEXTURE_MAG_FILTER, gl.GL_NEAREST)
-                gl.glTexImage2D(gl.GL_TEXTURE_2D, 0,
-                                internal_format,
-                                img_width, img_height,
-                            0, texture_pixel_format, gl_type, self._image.data)
-                # gl.glGenerateMipmap(gl.GL_TEXTURE_2D)
-                self.tex_width, self.tex_height = img_width, img_height
-            except Exception as e:
-                print("setTexture failed shape={}: {}".format(self._image.data.shape, e))
-                return False
-        else:
-            try:
-                gl.glTexSubImage2D(gl.GL_TEXTURE_2D, 0, 0, 0, img_width, img_height,
-                             texture_pixel_format, gl_type, self._image.data)
-                # gl.glGenerateMipmap(gl.GL_TEXTURE_2D)
-            except Exception as e:
-                print("setTexture failed shape={}: {}".format(self._image.data.shape, e))
-                return False
+        # Set Y, U and V
+        if self.texture is None:
+            self.texture = GLTexture(_gl)
+        self.texture.create_texture_gl(self._image)
+        # Set image_ref if available and compatible
+        if self._image_ref and self._image_ref.channels == self._image.channels:
+            if self.texture_ref is None:
+                self.texture_ref = GLTexture(_gl)
+            self.texture_ref.create_texture_gl(self._image_ref)
 
         self.print_timing(add_total=True)
         self.opengl_error()
+        # self.doneCurrent()
         return True
 
     # @abstract_method
     def viewer_update(self):
         self.update()
 
     # To be defined in children
-    def myPaintGL(self):  pass 
+    def myPaintGL(self):  pass
 
     def paintAll(self):
+        """ Should be called from PaintGL() exclusively """
+        # print("GLIVB paintAll")
         if self.trace_calls:
             t = trace_method(self.tab)
-        if self.textureID is None or not self.isValid() or not self.isVisible():
-            print("paintGL()** not ready {} {}".format(self.textureID, self.isValid()))
+        if self._image is None:
+            return
+        if self.texture is None or not self.isValid() or not self.isVisible():
+            print(f"paintGL()** not ready {self.texture} isValid = {self.isValid()} isVisible {self.isVisible()}")
             return
-        # No need for makeCurrent() since it is called from PaintGL() only
+        # No need for makeCurrent() since it is called from PaintGL() only ?
         # self.makeCurrent()
         painter = QtGui.QPainter()
         painter.begin(self)
         painter.beginNativePainting()
         im_pos = None
-        scale  = None
+        scale  = 1
         try:
             self.updateViewPort()
-            scale = self.updateTransforms()
+            scale = self.updateTransforms(make_current=False)
             self.myPaintGL()
             if self.show_cursor:
                 im_pos = self.gl_draw_cursor()
         except Exception as e:
             self.print_log(" failed paintGL {}".format(e))
             traceback.print_exc()
         painter.endNativePainting()
-        # status = gl.glGetError()
+        # status = _gl.glGetError()
 
-        draw_text = True
-        if draw_text:
-            # adapt scale depending on the ratio image / viewport
+        # adapt scale depending on the ratio image / viewport
+        if self._show_text:
             scale *= self._width/self._image.data.shape[1]
             self.display_text(painter, self.display_message(im_pos, scale))
 
         # draw histogram
         if self.show_histogram:
             current_image = self._image.data
             rect = QtCore.QRect(0, 0, self.width(), self.height())
             histograms = self.compute_histogram_Cpp(current_image, show_timings=self.display_timing)
             self.display_histogram(histograms, 1,  painter, rect, show_timings=self.display_timing)
 
         painter.end()
+        # self.context().swapBuffers(self.context().surface())
         # Seems required here, at least on linux
         # self.update()
+        # self.doneCurrent()
 
     def set_cursor_image_position(self, cursor_x, cursor_y):
         """
         Sets the image position from the cursor in proportion of the image dimension
         :return:
         """
-        self.updateTransforms()
+        self.updateTransforms(make_current=True, force=True)
         ratio = self.screen().devicePixelRatio()
         self.print_log("ratio {}".format(ratio))
         pos_x = cursor_x * ratio
         pos_y = (self.height() - cursor_y) * ratio
         self.print_log("pos {} {}".format(pos_x, pos_y))
         x0, x1, y0, y1 = self.image_centered_position()
 
         gl_posX, gl_posY = self.get_mouse_gl_coordinates(pos_x, pos_y)
         self.cursor_imx_ratio = (gl_posX - x0) / (x1 - x0)
         self.cursor_imy_ratio = 1 - (gl_posY - y0) / (y1 - y0)
         self.print_log("cursor ratio {} {}".format(self.cursor_imx_ratio, self.cursor_imy_ratio))
 
 
     def gl_draw_cursor(self) -> Optional[Tuple[int, int]]:
+        # _gl = QtGui.QOpenGLContext.currentContext().functions()
+        _gl = gl
+
         x0, x1, y0, y1 = self.image_centered_position()
 
-        im_x = int(self.cursor_imx_ratio*self.tex_width)
-        im_y = int(self.cursor_imy_ratio*self.tex_height)
+        im_x = int(self.cursor_imx_ratio*self.texture.width)
+        im_y = int(self.cursor_imy_ratio*self.texture.height)
 
-        glpos_from_im_x = (im_x+0.5)*(x1-x0)/self.tex_width + x0
-        glpos_from_im_y = (self.tex_height - (im_y+0.5))*(y1-y0)/self.tex_height+y0
+        glpos_from_im_x = (im_x+0.5)*(x1-x0)/self.texture.width + x0
+        glpos_from_im_y = (self.texture.height - (im_y+0.5))*(y1-y0)/self.texture.height+y0
 
         # get image coordinates
         length = 20 # /self.current_scale
         width = 4
-        gl.glLineWidth(width)
+        _gl.glLineWidth(width)
         gl.glColor3f(0.0, 1.0, 1.0)
         gl.glBegin(gl.GL_LINES)
         gl.glVertex3f(glpos_from_im_x-length, glpos_from_im_y, -0.001)
         gl.glVertex3f(glpos_from_im_x+length, glpos_from_im_y, -0.001)
         gl.glVertex3f(glpos_from_im_x, glpos_from_im_y-length, -0.001)
         gl.glVertex3f(glpos_from_im_x, glpos_from_im_y+length, -0.001)
         gl.glEnd()
-        if im_x>=0 and im_x<self.tex_width and im_y>=0 and im_y<=self.tex_height:
-            return (im_x, im_y) 
+        if im_x>=0 and im_x<self.texture.width and im_y>=0 and im_y<=self.texture.height:
+            return (im_x, im_y)
         return None
 
 
     def image_centered_position(self):
         w = self._width
         h = self._height
-        self.print_log(f'self width height {self._width} {self._height} tex {self.tex_width} {self.tex_height}')
-        if self.tex_width == 0 or self.tex_height == 0:
+        self.print_log(f'self width height {self._width} {self._height} tex {self.texture.width} {self.texture.height}')
+        if self.texture.width == 0 or self.texture.height == 0:
             return 0, w, 0, h
         # self.print_log(' {}x{}'.format(w, h))
-        image_ratio = float(self.tex_width)/float(self.tex_height)
+        image_ratio = float(self.texture.width)/float(self.texture.height)
         if h*image_ratio < w:
             view_width  = int(h*image_ratio+0.5)
             view_height = h
             start_x = int((w - view_width) / 2 + 0.5)
             start_y = 0
         else:
             view_width  = w
@@ -316,23 +270,26 @@
         # print(f" w, h {w, h}")
         try:
             gl.glViewport(0,0,w,h) # keep everything in viewport
         except Exception as e:
             self.print_log(" failed glViewport {}".format(e))
         self.print_timing(add_total=True)
 
-    def updateTransforms(self) -> float:
+    def updateTransforms(self, make_current=True, force=True) -> float:
         if self.trace_calls:
             t = trace_method(self.tab)
         self.start_timing()
-        self.makeCurrent()
+        if make_current:
+            self.makeCurrent()
+        # _gl = QtGui.QOpenGLContext.currentContext().functions()
+        _gl = gl
         w = self._width
         h = self._height
         dx, dy = self.new_translation()
-        scale = self.new_scale(-self.mouse_zoom_displ.y(), self.tex_height)
+        scale = self.new_scale(-self.mouse_zoom_displ.y(), self.texture.height)
         print(f"updateTransforms scale {scale}")
         try:
             # print("current context ", QtOpenGL.QGLContext.currentContext())
             # gl = QtOpenGL.QGLContext.currentContext().functions()
             # update the window size
             gl.glMatrixMode(gl.GL_PROJECTION)
             gl.glLoadIdentity()
@@ -359,26 +316,42 @@
         # size give for opengl are in pixels, qt uses device independent size otherwise
         print(f"self.devicePixelRatio() {self.devicePixelRatio()}")
         self._width = width*self.devicePixelRatio()
         self._height = height*self.devicePixelRatio()
         # print("width height ratios {} {}".format(self._width/self.width(), self._height/self.height()))
         self.viewer_update()
 
+    # def event(self, evt):
+    #     print(f"event {evt.type()}")
+    #     return super().event(evt)
+
     def get_mouse_gl_coordinates(self, x, y):
         modelview = gl.glGetDoublev(gl.GL_MODELVIEW_MATRIX)
+        # print(f"modelview {modelview}")
         projection = gl.glGetDoublev(gl.GL_PROJECTION_MATRIX)
+        # print(f"projection {projection}")
         viewport = gl.glGetIntegerv(gl.GL_VIEWPORT)
+        # print(f"viewport {viewport}")
         posX, posY, posZ = glu.gluUnProject(x, y, 0, modelview, projection, viewport)
+        # print(f"get_mouse_gl_coordinates({x},{y}) -> {posX} {posY}")
         return posX, posY
 
+    # def paintEvent(self, event):
+    #     # print("GLIVB paintEvent")
+    #     if self._image is not None:
+    #         self.paintAll()
+
+    # def paintGL(self):
+    #     self.paintAll()
+
     def mousePressEvent(self, event):
         self._mouse_events.mouse_press_event(event)
 
     def mouseMoveEvent(self, event):
-        if self.show_cursor:
+        if self.show_cursor or self._show_overlay:
             self.set_cursor_image_position(event.x(), event.y())
         self._mouse_events.mouse_move_event(event)
 
     def mouseReleaseEvent(self, event):
         self._mouse_events.mouse_release_event(event)
 
     def mouseDoubleClickEvent(self, event):
```

### Comparing `qimview-1.0.9/qimview/image_viewers/image_filter_parameters.py` & `qimview-1.1.0/qimview/image_viewers/image_filter_parameters.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_viewers/image_filter_parameters_gui.py` & `qimview-1.1.0/qimview/image_viewers/image_filter_parameters_gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,24 +38,33 @@
         self.g_r_gui.set_event_recorder(self.event_recorder)
 
     def add_g_b(self, layout, callback):
         self.g_b_gui = NumericParameterGui("G/B", self.params.g_b, callback, layout, self.name)
         self.g_b_gui.set_event_recorder(self.event_recorder)
 
     def add_saturation(self, layout, callback):
-        self.saturation_gui = NumericParameterGui("Saturation", self.params.saturation, callback, layout, self.name)
+        self.saturation_gui = NumericParameterGui("Sat", self.params.saturation, callback, layout, self.name)
+        self.saturation_gui.set_tooltip("Image Saturation")
         self.saturation_gui.set_event_recorder(self.event_recorder)
 
     def add_imdiff_factor(self, layout, callback):
-        self.imdiff_factor_gui = NumericParameterGui("Image diff factor", self.params.imdiff_factor, callback, layout, self.name)
+        self.imdiff_factor_gui = NumericParameterGui("Imdiff x", self.params.imdiff_factor, callback, layout, self.name)
+        self.imdiff_factor_gui.set_tooltip("Image differences display factor")
         self.imdiff_factor_gui.set_event_recorder(self.event_recorder)
 
     def register_event_player(self, event_player):
         for v in vars(self):
             if 'gui' in v and self.__dict__[v]:
                 self.__dict__[v].register_event_player(event_player)
 
     def reset_all(self):
         for v in vars(self):
             if 'gui' in v:
                 self.__dict__[v].reset()
 
+    def updateGui(self):
+        # Call updateGui for all members that contain this method
+        for v in vars(self):
+          if ug := getattr(self.__dict__[v],'updateGui',False):
+              if callable(ug):
+                  ug()
+
```

### Comparing `qimview-1.0.9/qimview/image_viewers/image_viewer.py` & `qimview-1.1.0/qimview/image_viewers/image_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,14 +149,22 @@
         # Key event class
         self._key_events   : ImageViewerKeyEvents   = ImageViewerKeyEvents(self)
         # Mouse event class
         self._mouse_events : ImageViewerMouseEvents = ImageViewerMouseEvents(self)
         # Add Mouse help tab
         self._key_events.add_help_tab("ImageViewer Mouse", self._mouse_events.markdown_help())
 
+        self._show_overlay          : bool = False
+        self._show_overlay_possible : bool = False
+        self._show_text             : bool = True
+
+        self._show_image_differences          : bool  = False
+        self._show_image_differences_possible : bool  = False
+        self._mean_absolute_difference        : float = 0
+
         # Current mouse information: position, displacement
         self.mouse_displ      : QtCore.QPoint = QtCore.QPoint(0,0)
         self.mouse_pos        : QtCore.QPoint = QtCore.QPoint(0,0)
         self.mouse_zoom_displ : QtCore.QPoint = QtCore.QPoint(0,0)
 
         # --- Public members
         self.data = None
@@ -168,17 +176,15 @@
 
         self.start_time = dict()
         self.timings = dict()
         self.replacing_widget = None
         self.before_max_parent = None
         self.show_histogram         : bool = True
         self.show_cursor            : bool = False
-        self.show_overlay           : bool = False
         self.show_stats             : bool = False
-        self.show_image_differences : bool = False
         self.show_intensity_line    : bool = False
         self.antialiasing           : bool = True
         # We track an image counter, changed by set_image, to help reducing same calculations
         self.image_id       = -1
         self.image_ref_id   = -1
         # Widget dimensions to be defined in child resize event
         self.evt_width : int
@@ -196,14 +202,23 @@
     def display_timing(self):
         return self._display_timing
 
     @display_timing.setter
     def display_timing(self, v):
         self._display_timing = v
 
+    # --- show_text
+    @property
+    def show_text(self):
+        return self._show_text
+
+    @show_text.setter
+    def show_text(self, v):
+        self._show_text = v
+
     # --- verbose
     @property
     def verbose(self):
         return self._verbose
 
     @verbose.setter
     def verbose(self, v):
@@ -275,14 +290,19 @@
         if image is not None:
             self.print_log(f'set_image({image.data.shape}): is_different = {is_different}')
         if is_different:
             self._image = image
             self.image_id += 1
         return is_different
 
+    def set_image_fast(self, image : Optional[ViewerImage]) -> None:
+        """ Set the viewer image """
+        self._image = image
+        self.image_id += 1
+
     def set_image_ref(self, image_ref : Optional[ViewerImage] = None):
         """ Set the reference image """
         is_different = (self._image_ref is None) or (self._image_ref is not image_ref)
         if is_different:
             self._image_ref = image_ref
             self.image_ref_id += 1
 
@@ -391,21 +411,31 @@
                 text += f"\n x{scale:0.2f}"
             im_x, im_y = im_pos
             values = self._image.data[im_y, im_x]
             text += f"\n pos {im_x:4}, {im_y:4} \n {self._image.channels.name[3:]}:{str(values).strip('[]')}"
 
         # ref_txt = self.image_ref_name if self.image_ref_name else 'ref'
         ref_txt = 'ref'
-        if self.show_overlay:
-            text += f"\n {ref_txt} | im"
-        if self.show_image_differences:
-            text += f"\n im - {ref_txt}"
+        if self._show_overlay:
+            text += f"\n {ref_txt} | im" if self._show_overlay_possible else "\noverlay not available"
+        if self._show_image_differences:
+            if self._show_image_differences_possible:
+                np.set_printoptions(precision=2)
+                if self._mean_absolute_difference>0:
+                    text += f"\n im - {ref_txt}, MAD = {self._mean_absolute_difference:0.5f} "
+                else:
+                    text += f"\n im - {ref_txt}, SAME IMAGES"
+            else:
+                text += "\nimage differences not available"
         return text
 
     def display_text(self, painter: QtGui.QPainter, text: str, font_size=-1) -> None:
+        """ Display the text inside the image widget, with transparent background """
+        if not self._show_text:
+            return
         self.start_timing()
         color = QtGui.QColor(255, 50, 50, 255) if self.is_active else QtGui.QColor(50, 50, 255, 255)
         painter.setPen(color)
         # Compute font size base on widget size
         if font_size == -1:
             # from 4 tp 14
             # for now very ad-hoc formula
```

### Comparing `qimview-1.0.9/qimview/image_viewers/image_viewer_key_events.py` & `qimview-1.1.0/qimview/image_viewers/image_viewer_key_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,24 @@
                 'A'     : self.toggleAntialiasing,
                 'C'     : self.toggleCursor,
                 'D'     : self.toggleDifferences,
                 'H'     : self.toggleHistogram,
                 'I'     : self.toggleIntensityLine,
                 'O'     : self.toggleOverlay,
                 'S'     : self.toggleStats,
+                'T'     : self.toggleText,
                 'F1'    : self.helpDialog,
                 'F11'   : self.toggleFullScreen,
                 'Esc'   : self.exitFullScreen,
                 'Alt+A' : self.zoomUpperLeft,
                 'Alt+B' : self.zoomUpperRight,
                 'Alt+C' : self.zoomLowerLeft,
                 'Alt+D' : self.zoomLowerRight,
                 'Alt+F' : self.unZoom,
+                'Ctrl+P': self.ImagePath2Clipboard,
                 'Ctrl+B': self.copy2Clipboard,
                 'Ctrl+S': self.saveImage,
         }
 
         self._help_tabs  : List[Tuple[str,str]] = []
         self._help_links : str = ''
 
@@ -155,37 +157,51 @@
     def toggleHistogram(self) ->bool:
         """ Toggle histogram display """
         self._viewer.show_histogram = not self._viewer.show_histogram
         return self.updateAndAccept()
     
     def toggleOverlay(self) ->bool:
         """ Toggle overlay display """
-        self._viewer.show_overlay   = not self._viewer.show_overlay
+        self._viewer._show_overlay = not self._viewer._show_overlay
         return self.updateAndAccept()
     
     def toggleCursor(self) ->bool:
         """ Toggle cursor display """
-        self._viewer.show_cursor    = not self._viewer.show_cursor
+        self._viewer.show_cursor = not self._viewer.show_cursor
         return self.updateAndAccept()
     
     def toggleStats(self) ->bool:
         """ Toggle stats display """
-        self._viewer.show_stats     = not self._viewer.show_stats
+        self._viewer.show_stats = not self._viewer.show_stats
+        return self.updateAndAccept()
+
+    def toggleText(self) ->bool:
+        """ Toggle text/info display """
+        self._viewer.show_text = not self._viewer.show_text
         return self.updateAndAccept()
 
     def toggleDifferences(self) ->bool: 
         """ Toggle image difference with reference """
-        self._viewer.show_image_differences = not self._viewer.show_image_differences
+        self._viewer._show_image_differences = not self._viewer._show_image_differences
         return self.updateAndAccept()
     
     def toggleIntensityLine(self) ->bool: 
         """ Toggle horizontal intensity line display """
         self._viewer.show_intensity_line = not self._viewer.show_intensity_line
         return self.updateAndAccept()
     
+    def ImagePath2Clipboard(self)->bool:
+        """ Copy image full path to clipboard """
+        clipboard = QtWidgets.QApplication.clipboard()
+        im = self._viewer.get_image()
+        if im and im.filename:
+            clipboard.setText(im.filename)
+            return True
+        return False
+
     def copy2Clipboard(self)->bool:
         """ Copy current image to clipboard """
         clipboard = QtWidgets.QApplication.clipboard()
         self._viewer.set_clipboard(clipboard, True)
         self._viewer.widget.repaint()
         self._viewer.set_clipboard(None, False)
         print("Image saved to clipboard")
```

### Comparing `qimview-1.0.9/qimview/image_viewers/image_viewer_mouse_events.py` & `qimview-1.1.0/qimview/image_viewers/image_viewer_mouse_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         self._regions.update({
             'histogram'  : in_histo,
             'text'       : in_text,
         })
 
     def mouse_move_unpressed(self, event: QtGui.QMoveEvent)->None:
         """ Actions while moving the mouse without pressing any button """
-        if self._widget.show_overlay:
+        if self._widget._show_overlay:
             self._widget.mouse_pos = event.pos()
             self._widget.viewer_update()
             event.accept()
         elif self._widget.show_cursor:
             self._widget.mouse_pos = event.pos()
             self._widget.viewer_update()
             self._widget.synchronize()
@@ -111,15 +111,15 @@
     def toogle_histo_size(self, _)->bool:
         """ Switch histogram scale from 1 to 3 """
         self._widget._histo_scale = (self._widget._histo_scale % 3) + 1 
         self._widget.viewer_update()
         return True
 
     def wheel_zoom(self, event: QtGui.QWheelEvent) -> bool:
-        """ Zoom in/out based on wheel angle """
+        """ Zoom in/out based on wheel angle, works with touchpad 2 fingers """
         # Zoom by applying a factor to the distances to the sides
         # print(f"{event.angleDelta(), event.deviceType(), event.source()}")
         delta = event.angleDelta().y()
         # print("delta = {}".format(delta))
         coeff = delta/5
         # coeff = 20 if delta > 0 else -20
         if im := self._widget.get_image():
@@ -131,38 +131,39 @@
 
     def wheel_pan(self, event: QtGui.QWheelEvent) -> bool:
         """ Pan (image translation) based on wheel angle, mainly for touchpad """
         # Zoom by applying a factor to the distances to the sides
         # print(f"{event.angleDelta(), event.deviceType(), event.source()}")
         delta = event.angleDelta()
         if im := self._widget.get_image():
-            self._widget.mouse_displ = delta
-            self._widget.viewer_update()
-            self._widget.synchronize()
+            # Reduce wheel delta for smaller translations
+            self._widget.mouse_displ = delta/3
             # Update current displacement
             self._widget.current_dx = int(self._widget.check_translation()[0])
             self._widget.current_dy = int(self._widget.check_translation()[1])
+            self._widget.viewer_update()
+            self._widget.synchronize()
             return True
         return False
 
     def wheel_pan_horizontal(self, event: QtGui.QWheelEvent) -> bool:
         """ Pan horizontal (image horizontal translation) based on wheel angle """
         # Zoom by applying a factor to the distances to the sides
         # print(f"{event.angleDelta(), event.deviceType(), event.source()}")
         delta = event.angleDelta()
         # To translation horizontally using wheel mouse
-        delta.setX(delta.y())
+        delta.setX(delta.y()/3)
         delta.setY(0)
         if im := self._widget.get_image():
             self._widget.mouse_displ = delta
-            self._widget.viewer_update()
-            self._widget.synchronize()
             # Update current displacement
             self._widget.current_dx = int(self._widget.check_translation()[0])
             self._widget.current_dy = int(self._widget.check_translation()[1])
+            self._widget.viewer_update()
+            self._widget.synchronize()
             return True
         return False
 
     def tooltip_image_filename(self, event: QtGui.QMoveEvent) -> bool:
         """ Display image filename as tooltip """
         global_pos = self._widget.mapToGlobal(event.pos())
         QtWidgets.QToolTip.showText(global_pos, f"{self._widget._image.filename}",
```

### Comparing `qimview-1.0.9/qimview/image_viewers/mouse_events.py` & `qimview-1.1.0/qimview/image_viewers/mouse_events.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_viewers/multi_view.py` & `qimview-1.1.0/qimview/image_viewers/multi_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -257,17 +257,21 @@
         '''
         Uses the variable self.output_label_current_image
         :return:
         '''
         self.print_log('update_image_parameters')
         update_start = get_time()
 
-        for n in range(self.nb_viewers_used):
-            self.image_viewers[n].filter_params.copy_from(self.filter_params)
-            self.image_viewers[n].widget.update()
+        if self.sync_filters.isChecked():
+            for n in range(self.nb_viewers_used):
+                self.image_viewers[n].filter_params.copy_from(self.filter_params)
+                self.image_viewers[n].widget.update()
+        else:
+            self._active_viewer.filter_params.copy_from(self.filter_params)
+            self._active_viewer.widget.update()
 
         if self.show_timing():
             time_spent = get_time() - update_start
             self.print_log(" Update image took {0:0.3f} sec.".format(time_spent))
 
     def set_images(self, images, set_viewers=False):
         self.print_log(f"MultiView.set_images() {images}")
@@ -372,25 +376,24 @@
         vertical_layout.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetMinimumSize)
         # vertical_layout.setSizeConstraint(QtWidgets.QLayout.SetNoConstraint)
         self.button_widget.setSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
         self.button_widget.setLayout(self.button_layout)
         vertical_layout.addWidget(self.button_widget, 0, QtCore.Qt.AlignmentFlag.AlignTop)
 
     def layout_parameters(self, parameters_layout):
-        # Add Profiles and keep zoom options
-        self.display_profiles = QtWidgets.QCheckBox("Profiles")
-        self.display_profiles.stateChanged.connect(self.toggle_display_profiles)
-        self.display_profiles.setChecked(False)
-        parameters_layout.addWidget(self.display_profiles)
-        self.keep_zoom = QtWidgets.QCheckBox("Keep zoom")
-        self.keep_zoom.setChecked(False)
-        parameters_layout.addWidget(self.keep_zoom)
+        # Sync filter and keep zoom options
+        self.sync_filters = QtWidgets.QCheckBox("Sync")
+        self.sync_filters.setToolTip("Synchronize image filters on all images")
+        self.sync_filters.setChecked(True)
+        parameters_layout.addWidget(self.sync_filters)
 
         # Reset button
-        self.reset_button = QtWidgets.QPushButton("reset")
+        self.reset_button = QtWidgets.QPushButton()
+        self.reset_button.setIcon(self.style().standardIcon(QtWidgets.QStyle.SP_BrowserReload))
+        self.reset_button.setToolTip("Reset filters to default values")
         parameters_layout.addWidget(self.reset_button)
         self.reset_button.clicked.connect(self.reset_intensities)
 
         # Add color difference slider
         self.filter_params_gui.add_imdiff_factor(parameters_layout, self.update_image_intensity_event)
 
         # --- Saturation adjustment
@@ -425,52 +428,50 @@
 
         self.viewer_grid_layout = QtWidgets.QGridLayout()
         self.viewer_grid_layout.setHorizontalSpacing(1)
         self.viewer_grid_layout.setVerticalSpacing(1)
         self.set_number_of_viewers(1)
         vertical_layout.addLayout(self.viewer_grid_layout, 1)
 
-        self.figures_widget = QtWidgets.QWidget()
-        self.figures_layout = QtWidgets.QHBoxLayout()
-        self.figures_layout.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetMinimumSize)
-        # for the moment ignore this
-        # self.figures_layout.addWidget(self.value_in_range_canvas)
-        # self.figures_widget.setLayout(self.figures_layout)
-
-        vertical_layout.addWidget(self.figures_widget)
-        self.toggle_display_profiles()
         self.setLayout(vertical_layout)
         print("update_layout done")
 
-    def toggle_display_profiles(self):
-        self.figures_widget.setVisible(self.display_profiles.isChecked())
-        self.update_image()
-
     def get_output_image(self, im_string_id : str):
         """
         Search for the image with given label in the current row
         if not in cache reads it and add it to the cache
         :param im_string_id: string that identifies the image to display
         :return:
         """
         # print(f"get_output_image({im_string_id}) ")
         start = get_time()
 
-        image_filename = self.image_dict[im_string_id]
-        image_transform = None
-        self.print_log(f"MultiView.get_output_image() image_filename:{image_filename}")
-
-        image_data, _ = self.cache.get_image(image_filename, self.read_size, verbose=self.show_timing_detailed(),
-                                             use_RGB=not self.use_opengl, image_transform=image_transform)
+        #
+        image_data = None
+        img = self.image_dict[im_string_id]
+        # if osp.isfile(img):
+        if True:
+            image_filename = img
+            # Allow to pass a string or a numpy array
+            image_transform = None
+            self.print_log(f"MultiView.get_output_image() image_filename:{image_filename}")
+
+            image_data, _ = self.cache.get_image(image_filename, self.read_size, verbose=self.show_timing_detailed(),
+                                                use_RGB=not self.use_opengl, image_transform=image_transform)
+        # elif isinstance(img, np.ndarray):
+        #     if len(img.shape) == 3 and img.shape[2]==3:
+        #         image_data = ViewerImage(img)
+        #     elif len(img.shape) == 2:
+        #         image_data = ViewerImage(img, channels=CH_Y)
 
         if image_data is not None:
             self.output_image_label[im_string_id] = image_filename
             output_image = image_data
         else:
-            print(f"failed to get image {im_string_id}: {image_filename}")
+            print(f"failed to get image {im_string_id}")
             return None
 
         if self.show_timing_detailed():
             print(f" get_output_image took {int((get_time() - start)*1000+0.5)} ms".format)
 
         # force image bayer information if selected from menu
         res = output_image
@@ -518,14 +519,17 @@
                 self.label[im_name].setFont(self.bold_font)
                 self.label[im_name].setWordWrap(True)
             # self.label[im_name].setMaximumWidth(160)
     
     def on_active(self, viewer : ImageViewerClass) -> None:
         # Activation requested for a given viewer
         self._active_viewer = viewer
+        # Update filters
+        self.filter_params.copy_from(viewer.filter_params)
+        self.filter_params_gui.updateGui()
         self.update_image(viewer.image_name)
  
     def on_synchronize(self, viewer : ImageViewerClass) -> None:
         # Synchronize other viewer to calling viewer
         for v in self.image_viewers:
             if v != viewer:
                 viewer.synchronize_data(v)
```

### Comparing `qimview-1.0.9/qimview/image_viewers/multi_view_key_events.py` & `qimview-1.1.0/qimview/image_viewers/multi_view_key_events.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/image_viewers/multi_view_mouse_events.py` & `qimview-1.1.0/qimview/image_viewers/multi_view_mouse_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,41 @@
 class MultiViewMouseEvents(MouseEvents['MultiView']):
     """ Implement mouse events for MultiView """
 
     def __init__(self, multiview: 'MultiView'):
         super().__init__(multiview)
 
         self._mouse_callback.update({
-            'Left Pressed'  : self.action_activate,
-            'Left+DblClick' : self.toggle_show_single_viewer,
+            'Left Pressed'      : self.action_activate,
+            'Ctrl+Left Pressed' : self.action_setreference,
+            'Left+DblClick'     : self.toggle_show_single_viewer,
         })
 
 
     def action_activate(self,  event: QtGui.QMouseEvent) -> bool:
         """ Set viewer active """
         for v in self._widget.image_viewers:
             if v.geometry().contains(event.pos()):
                 # Set the current viewer active before processing the double click event
                 self._widget.on_active(v)
                 self._widget.update_image()
                 return True
         return False
 
+    def action_setreference(self,  event: QtGui.QMouseEvent) -> bool:
+        """ Set viewer active """
+        for v in self._widget.image_viewers:
+            if v.geometry().contains(event.pos()):
+                # Set the current viewer image as the reference
+                if self._widget.output_label_current_image != v.image_name:
+                    self._widget.set_reference_label(v.image_name, update_viewers=True)
+                    self._widget.update_image()
+                    return True
+        return False
+
     def toggle_show_single_viewer(self, event: QtGui.QMouseEvent)->bool:
         """ Show only the selected viewer or all viewers """
         # Need to find the viewer that has been double clicked
         for v in self._widget.image_viewers:
             if v.geometry().contains(event.pos()):
                 # Set the current viewer active before processing the double click event
                 self._widget.on_active(v)
```

### Comparing `qimview-1.0.9/qimview/image_viewers/qt_image_viewer.py` & `qimview-1.1.0/qimview/image_viewers/qt_image_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         self.setMouseTracking(True)
         self.anti_aliasing = True
         size_policy = QtWidgets.QSizePolicy()
         size_policy.setHorizontalPolicy(QtWidgets.QSizePolicy.Policy.Ignored)
         size_policy.setVerticalPolicy  (QtWidgets.QSizePolicy.Policy.Ignored)
         self.setSizePolicy(size_policy)
         # self.setAlignment(QtCore.Qt.AlignCenter )
+        # output crop [ width min, height min, width max, height max]
         self.output_crop = np.array([0., 0., 1., 1.], dtype=np.float32)
         self.zoom_center = np.array([0.5, 0.5, 0.5, 0.5])
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.ClickFocus)
 
         self.paint_cache      = None
         self.paint_diff_cache = None
         self.diff_image       = None
@@ -374,15 +375,15 @@
             im_y += crop_ymin
             im_pos = (im_x, im_y)
         else:
             im_pos = None
         if self.display_timing: self.print_timing()
         return im_pos
 
-    def get_difference_image(self, verbose=True) -> Optional[ViewerImage]:
+    def get_difference_image(self, verbose=False) -> Optional[ViewerImage]:
 
         factor = self.filter_params.imdiff_factor.float
         if self.paint_diff_cache is not None:
             use_cache = self.paint_diff_cache['imid'] == self.image_id and \
                         self.paint_diff_cache['imrefid'] == self.image_ref_id and \
                         self.paint_diff_cache['factor'] == factor
         else:
@@ -390,24 +391,26 @@
 
         if self._image is None or self._image_ref is None: return None
         if not use_cache:
             im1 = self._image.data
             im2 = self._image_ref.data
             # TODO: get factor from parameters ...
             # factor = int(self.diff_color_slider.value())
-            print(f'factor = {factor}')
-            print(f' im1.dtype {im1.dtype} im2.dtype {im2.dtype}')
+            # print(f'factor = {factor}')
+            # print(f' im1.dtype {im1.dtype} im2.dtype {im2.dtype}')
             # Fast OpenCV code
             start = get_time()
             # positive diffs in unsigned 8 bits, OpenCV puts negative values to 0
             try:
                 if im1.dtype.name == 'uint8' and im2.dtype.name == 'uint8':
                     diff_plus = cv2.subtract(im1, im2)
                     diff_minus = cv2.subtract(im2, im1)
                     res = cv2.addWeighted(diff_plus, factor, diff_minus, -factor, 127)
+                    # Will slow down the display
+                    self._mean_absolute_difference = np.mean(np.absolute(im1.astype(np.int16)-im2.astype(np.int16)))
                     if verbose:
                         print(f" qtImageViewer.difference_image()  took {int((get_time() - start)*1000)} ms")
                         vmin = np.min(res)
                         vmax = np.max(res)
                         print(f"min-max diff = {vmin} - {vmax}")
                         histo,_ = np.histogram(res, bins=int(vmax-vmin+0.5), range=(vmin, vmax))
                         sum = 0
@@ -423,60 +426,66 @@
                                             downscale=self._image.downscale,
                                             channels=self._image.channels)
                     self.paint_diff_cache = {  'imid': self.image_id, 'imrefid': self.image_ref_id, 
                         'factor': self.filter_params.imdiff_factor.float
                     }
                     self.diff_image = res
                 else:
-                    d = (im1.astype(np.float32)-im2.astype(np.float32))*factor
+                    d = (im1.astype(np.float32)-im2.astype(np.float32))
+                    # Will slow down the display
+                    self._mean_absolute_difference = np.mean(np.absolute(d))
+                    d = d*factor
                     d[d<-127] = -127
                     d[d>128] = 128
                     d = (d+127).astype(np.uint8)*255
                     res = ViewerImage(d,  precision=8, 
                                             downscale=self._image.downscale,
                                             channels=self._image.channels)
                     self.paint_diff_cache = {  'imid': self.image_id, 'imrefid': self.image_ref_id, 
                         'factor': self.filter_params.imdiff_factor.float
                     }
                     self.diff_image = res
             except Exception as e:
                 print(f"Error {e}")
                 res = (im1!=im2).astype(np.uint8)*255
+                self._mean_absolute_difference = np.mean(np.absolute(self.diff_image.data))
                 res = ViewerImage(res,  precision=8, 
                                         downscale=self._image.downscale,
                                         channels=ImageFormat.CH_Y)
                 self.diff_image = res
 
+
         return self.diff_image
 
     def paint_image(self):
         # print(f"paint_image display_timing {self.display_timing}")
         if self.trace_calls: t = trace_method(self.tab)
         self.start_timing()
         time0 = time1 = get_time()
 
         label_width = self.size().width()
         label_height = self.size().height()
 
-        show_diff = self.show_image_differences and self._image is not self._image_ref and \
+        show_diff = self._show_image_differences and self._image is not self._image_ref and \
                     self._image is not None and \
                     self._image_ref is not None and self._image.data.shape == self._image_ref.data.shape
+        self._show_image_differences_possible = show_diff
 
         c = self.update_crop()
         # check paint_cache
         if self.paint_cache is not None:
             use_cache = self.paint_cache['imid'] == self.image_id and \
                         np.array_equal(self.paint_cache['crop'],c) and \
                         self.paint_cache['labelw'] == label_width and \
                         self.paint_cache['labelh'] == label_height and \
                         self.paint_cache['filterp'].is_equal(self.filter_params) and \
                         (self.paint_cache['showhist'] == self.show_histogram or not self.show_histogram) and \
                         self.paint_cache['show_diff'] == show_diff and \
                         self.paint_cache['antialiasing'] == self.antialiasing and \
-                        not self.show_overlay
+                        not self._show_overlay
         else:
             use_cache = False
 
         # if show_diff, compute the image difference (put it in cache??)
         if show_diff:
             # Cache does not work well with differences
             use_cache = False
@@ -518,16 +527,22 @@
         image_height, image_width  = image_data.shape[:2]
         ratio_width = float(label_width) / image_width
         ratio_height = float(label_height) / image_height
         ratio = min(ratio_width, ratio_height)
         display_width = int(round(image_width * ratio))
         display_height = int(round(image_height * ratio))
 
-        if self.show_overlay and self._image_ref is not self._image and self._image_ref and self._image and \
-            self._image.data.shape == self._image_ref.data.shape:
+        self._show_overlay_possible = self._show_overlay and \
+                self._image_ref is not self._image and \
+                self._image_ref is not None and self._image is not None and \
+                self._image.data.shape == self._image_ref.data.shape
+                
+        # TODO: show overlay with different filters applied on each image?
+        if self._show_overlay_possible:
+            self._show_overlay_possible = True
             # to create the overlay rapidly, we will mix the two images based on the current cursor position
             # 1. convert cursor position to image position
             (height, width) = cropped_image_shape[:2]
             # compute rect
             rect = QtCore.QRect(0, 0, display_width, display_height)
             devRect = QtCore.QRect(0, 0, self.evt_width, self.evt_height)
             rect.moveCenter(devRect.center())
@@ -649,15 +664,15 @@
                 current_image = self.paint_cache['current_image']
                 histograms = self.paint_cache['histograms']
             # histograms2 = self.paint_cache['histograms2']
 
         # if could_use_cache:
         #     print(f" ======= current_image equal ? {np.array_equal(self.paint_cache['current_image'],current_image)}")
 
-        if not use_cache and not self.show_overlay:
+        if not use_cache and not (self._show_overlay and self._show_overlay_possible):
             # cache_time = get_time()
             fp = ImageFilterParameters()
             fp.copy_from(self.filter_params)
             self.paint_cache = {
                 'imid': self.image_id,
                 'imrefid': self.image_ref_id,
                 'crop': c, 'labelw': label_width, 'labelh': label_height,
@@ -699,15 +714,15 @@
         time1 = get_time()
         if BaseWidget is QOpenGLWidget:
             painter.drawImage(rect, qimage)
         else:
             painter.drawImage(rect.topLeft(), qimage)
         self.add_time('painter.drawImage',time1)
 
-        if self.show_overlay:
+        if self._show_overlay and self._show_overlay_possible:
             self.draw_overlay_separation(cropped_image_shape, rect, painter)
 
         # Draw cursor
         im_pos = None
         if self.show_cursor:
             im_pos = self.draw_cursor(cropped_image_shape, 
                                       crop_xmin,
```

### Comparing `qimview-1.0.9/qimview/imview.py` & `qimview-1.1.0/qimview/imview.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     parser.add_argument('--gl', action='store_true', help='use opengl viewer')
     args = parser.parse_args()
     _params = vars(args)
     print(f"record {_params['record']}")
 
 
     # create the Qt App and window
-    QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_ShareOpenGLContexts)
+    QtCore.QCoreApplication.setAttribute(QtCore.Qt.ApplicationAttribute.AA_ShareOpenGLContexts)
     app = QtWidgets.QApplication(sys.argv)
     app.setApplicationDisplayName('imview ' + ' '.join(sys.argv[1:]))
     if _params['play'] is not None:
         with open(_params['play']) as json_file:
             events = json.load(json_file)
     else:
         events = None
```

### Comparing `qimview-1.0.9/qimview/mview.py` & `qimview-1.1.0/qimview/mview.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,33 @@
 
 from qimview.utils.qt_imports import QtWidgets, QtCore
 from qimview.image_viewers    import MultiView, ViewerType
 
 def get_filenames():
     filenames = []
     # Ask for input file
-    selected_files =  QtWidgets.QFileDialog.getOpenFileNames(caption="miview: Select  one or various input images")
+    selected_files =  QtWidgets.QFileDialog.getOpenFileNames(caption="mview: Select one or various input images")
     filenames.extend(selected_files[0])
     return filenames
 
 
 def main():
     parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('images', nargs='*', help='input images')
     parser.add_argument('-v', '--viewer', type=str, choices={'gl', 'qt', 'shader'}, default='qt',
                         help="Viewer mode, qt: standard qt display, gl: use opengl,  shader: enable opengl with "
                              "shaders")
-    parser.add_argument('-l', '--layout', type=str, default='0', help='Set the layout (number of images in comparison on the window), if 0 try to use the number of input images')
+    parser.add_argument('-l', '--layout', type=str, default='0', 
+                        help='Set the layout (number of images in comparison on the window),'
+                        ' if 0 try to use the number of input images')
 
     args = parser.parse_args()
     _params = vars(args)
 
-    QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_ShareOpenGLContexts)
+    QtCore.QCoreApplication.setAttribute(QtCore.Qt.ApplicationAttribute.AA_ShareOpenGLContexts)
     app = QtWidgets.QApplication(sys.argv)
     app.setApplicationDisplayName('mview ' + ' '.join(sys.argv[1:]))
 
     filenames = []
     for im in _params['images']:
         filenames.extend(glob.glob(im,recursive=False))
     checked_filenames = []
```

### Comparing `qimview-1.0.9/qimview/parameters/numeric_parameter.py` & `qimview-1.1.0/qimview/parameters/numeric_parameter.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/parameters/numeric_parameter_gui.py` & `qimview-1.1.0/qimview/parameters/numeric_parameter_gui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,110 @@
-from ..utils.qt_imports import QtWidgets, QtCore
+"""
+    GUI for NumericParameter instances
+"""
+
+from typing import Callable
+from qimview.utils.qt_imports import QtWidgets, QtCore
+
 
 class NumericParameterGui(QtWidgets.QSlider):
     """
     For the moment, it can only be a slider with associated text
     """
-    def __init__(self, name, param, callback, layout=None, parent_name=""):
+    def __init__(self, name, param, callback = None, layout=None, parent_name=""):
         QtWidgets.QSlider.__init__(self, QtCore.Qt.Horizontal)
         self.name = name
         self.param = param
-        self.callback = callback
+        self._valuechanged_callback : Callable | None = callback
+        self._pressed_callback      : Callable | None = None
+        self._moved_callback        : Callable | None = None
+        self._released_callback     : Callable | None = None
         self.event_recorder = None
         self.parent_name = parent_name
         self.widget_name = f"slider_{self.parent_name}_{self.name}"
         self.created = False
         self.decimals = 2
+        self._text_format : Callable | None = None
         if layout is not None:
             self.create()
+            self.updateText()
             self.add_to_layout(layout)
 
     def set_event_recorder(self, evtrec):
         self.event_recorder = evtrec
         if self.event_recorder is not None:
             self.event_recorder.register_widget(id(self), self.widget_name)
 
     def register_event_player(self, event_player):
         event_player.register_widget(self.widget_name, self)
 
-    def create(self, moved_callback=False):
-        self.label = QtWidgets.QLabel("")
+    def set_valuechanged_callback(self,cb:Callable):
+        self._valuechanged_callback = cb
+
+    def set_pressed_callback(self,cb:Callable):
+        self._pressed_callback = cb
+
+    def set_moved_callback(self,cb:Callable):
+        self._moved_callback = cb
+
+    def set_released_callback(self,cb:Callable):
+        self._released_callback = cb
+
+    def create(self):
+        self.label = QtWidgets.QLabel(f"{self.name}")
         self.setRange(self.param.range[0], self.param.range[1])
         self.setValue(self.param.value)
         self.changed()
-        if moved_callback:
-            self.sliderMoved.connect(lambda: self.changed(self.callback))
-        else:
-            self.valueChanged.connect(lambda: self.changed(self.callback))
+        if self._moved_callback:
+            # Move callback is used only if tracking is off, so set it to off here
+            self.setTracking(False)
+            self.sliderMoved.connect(self._moved_callback)
+        if self._valuechanged_callback:
+            self.valueChanged.connect(lambda: self.changed(self._valuechanged_callback))
+        if self._pressed_callback:
+            self.sliderPressed.connect(self._pressed_callback)
+        if self._released_callback:
+            self.sliderReleased.connect(self._released_callback)
         self.created = True
 
-    def add_to_layout(self, layout):
+    def set_tooltip(self, mess):
+        self.label.setToolTip(mess)
+
+    def add_to_layout(self, layout, stretch=0):
         if not self.created:
             self.create()
         layout.addWidget(self.label)
-        layout.addWidget(self)
+        if stretch!=0:
+            layout.addWidget(self, stretch)
+        else:
+            layout.addWidget(self)
 
     def reset(self):
         self.setValue(self.param.default_value)
 
+    def updateSlider(self):
+        self.setValue(self.param.int)
+
+    def setTextFormat(self, _format: Callable):
+        self._text_format = _format
+
+    def updateText(self):
+        if self._text_format:
+            text = self._text_format(self.param)
+        else:
+            text = f"{self.param.float:0.{self.decimals}f}"
+        self.label.setText(f"{self.name} {text}")
+
+    def updateGui(self):
+        self.updateSlider()
+        self.updateText()
+
     def changed(self, callback=None):
-        self.param.int = int(self.value())
-        self.label.setText(f"{self.name} {self.param.float:0.{self.decimals}f}")
+        self.param.int = self.value()
+        self.updateText()
         if callback is not None:
             callback()
 
     def mouseDoubleClickEvent(self, evt):
         self.reset()
 
     def event(self, evt):
```

### Comparing `qimview-1.0.9/qimview/tests_utils/event_player.py` & `qimview-1.1.0/qimview/tests_utils/event_player.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/tests_utils/event_recorder.py` & `qimview-1.1.0/qimview/tests_utils/event_recorder.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/tests_utils/qtdump.py` & `qimview-1.1.0/qimview/tests_utils/qtdump.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/utils/menu_selection.py` & `qimview-1.1.0/qimview/utils/menu_selection.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/utils/mvlabel.py` & `qimview-1.1.0/qimview/utils/mvlabel.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/utils/suffix_auto.py` & `qimview-1.1.0/qimview/utils/suffix_auto.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/utils/tab_dialog.py` & `qimview-1.1.0/qimview/utils/tab_dialog.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview/utils/thread_pool.py` & `qimview-1.1.0/qimview/utils/thread_pool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # example from https://www.learnpyqt.com/tutorials/multithreading-pyqt-applications-qthreadpool/
 
 from .qt_imports import *
 
-import traceback, sys
 
 class WorkerSignals(QtCore.QObject):
     '''
     Defines the signals available from a running worker thread.
     Supported signals are:
     finished
         No data
@@ -14,16 +13,16 @@
         tuple (exctype, value, traceback.format_exc() )
     result
         object data returned from processing, anything
     progress
         int indicating % progress
     '''
     finished = Signal()
-    error = Signal(tuple)
-    result = Signal(object)
+    error    = Signal(tuple)
+    result   = Signal(object)
     progress = Signal(int)
 
 
 class Worker(QtCore.QRunnable):
     '''
     Worker thread
     Inherits from QRunnable to handler worker thread setup, signals and wrap-up.
@@ -64,36 +63,48 @@
     @Slot()
     def run(self):
         """
         Initialise the runner function with passed args, kwargs.
         """
         # Retrieve args/kwargs here; and fire processing using them
         try:
+            # print("run")
             result = self.fn(*self.args, **self.kwargs)
-        except:
+        except Exception as e:
+            print(f"Exception catched while processing Worker task: {e}")
+            import sys
+            import traceback
             traceback.print_exc()
             exctype, value = sys.exc_info()[:2]
             self.signals.error.emit((exctype, value, traceback.format_exc()))
         else:
             # print(" ***** emit result signal ")
             if self.result_cb is not None:
                 self.result_cb(result)  # Return the result of the processing
         finally:
             self.signals.finished.emit()  # Done
 
 
 class ThreadPool(QtCore.QThreadPool):
-    def __init(self):
-        super(ThreadPool, self).__init__()
-        print("Multithreading with maximum %d threads" % self.threadpool.maxThreadCount())
+    """ Can start several runnables in threads """
+    def __init__(self):
+        super().__init__()
+        # print(f"Multithreading with maximum {self.maxThreadCount()} threads" )
+        self._worker : Worker
 
     def set_worker(self, work_function, *args, **kwargs):
-        self.worker = Worker(work_function,  *args, **kwargs)  # Any other args, kwargs are passed to the run function
+        """ Define a new worker to process work_function and its arguments """
+        self._worker = Worker(work_function,  *args, **kwargs)  # Any other args, kwargs are passed to the run function
+
+    def set_autodelete(self, d: bool):
+        self._worker.setAutoDelete(d)
 
     def set_worker_callbacks(self, progress_cb=None, finished_cb=None, result_cb=None):
-        self.worker.set_progress_callback(progress_cb)
-        self.worker.set_finished_callback(finished_cb)
-        self.worker.set_result_callback(result_cb)
+        """ Define several possible callbacks """
+        self._worker.set_progress_callback(progress_cb)
+        self._worker.set_finished_callback(finished_cb)
+        self._worker.set_result_callback(result_cb)
 
     def start_worker(self):
-        self.start(self.worker)
+        """ Starts the worker in a thread """
+        self.start(self._worker)
```

### Comparing `qimview-1.0.9/qimview/utils/utils.py` & `qimview-1.1.0/qimview/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,15 @@
 import time
 import numpy as np
 from collections import deque
 import os
 
 
 def get_time():
-	is_windows = sys.platform.startswith('win')
-	if is_windows:
-		if hasattr(time, 'clock'):
-			return time.clock()
-		else:
-			return time.perf_counter()
-	else:
-		return time.time()
+    return time.perf_counter()
 
 def clip_value(value, lower, upper):
     return lower if value < lower else upper if value > upper else value
 
 def get_size(obj, seen=None):
 	"""
 	Recursively finds size of objects
```

### Comparing `qimview-1.0.9/qimview/video_player/video_player.py` & `qimview-1.1.0/qimview/video_player/video_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # required to install codecs to work well on windows, I installed K-Lite standard codecs
 
-from ..utils.qt_imports import QtGui, QtCore, QtWidgets, QtMultimedia, QtMultimediaWidgets
-from ..parameters.numeric_parameter import  NumericParameter
-from ..parameters.numeric_parameter_gui import NumericParameterGui
+from qimview.utils.qt_imports import QtGui, QtCore, QtWidgets, QtMultimedia, QtMultimediaWidgets
+from qimview.parameters.numeric_parameter import  NumericParameter
+from qimview.parameters.numeric_parameter_gui import NumericParameterGui
 
 import sys
 
 class myVideoWidget(QtMultimediaWidgets.QVideoWidget):
     def __init__(self, parent=None):
         super().__init__(parent)
         self.current_scale = 1
```

### Comparing `qimview-1.0.9/qimview/video_player/vlc_player.py` & `qimview-1.1.0/qimview/video_player/vlc_player.py`

 * *Files identical despite different names*

### Comparing `qimview-1.0.9/qimview.egg-info/PKG-INFO` & `qimview-1.1.0/qimview.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: qimview
-Version: 1.0.9
+Version: 1.1.0
 Summary: Library for multiple image visualization and comparison
 Author-email: Karl Krissian <karl.krissian@gmail.com>
 Project-URL: Homepage, https://github.com/qimview/qimview
 Project-URL: Wiki, https://github.com/qimview/qimview/wiki
 Project-URL: Bug Tracker, https://github.com/qimview/qimview/issues
 Project-URL: API, https://qimview.github.io/qimview/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: opencv_python>=4.2
 Requires-Dist: psutil>=5.8.0
 Requires-Dist: PyOpenGL>=3.1.5
 Requires-Dist: PySide6>=6.5.2
 Requires-Dist: PySide6_Addons>=6.5.1.1
 Requires-Dist: PySide6_Essentials>=6.5.1.1
 Requires-Dist: simplejpeg>=1.4.0
 Provides-Extra: extra
 Requires-Dist: rawpy>=0.16.0; extra == "extra"
 Requires-Dist: python_vlc>=3.0.11115; extra == "extra"
 Requires-Dist: PyTurboJPEG>=1.4.1; extra == "extra"
+Requires-Dist: PyOpenGL_accelerate; extra == "extra"
+Requires-Dist: PyAV; extra == "extra"
 
 # Description
 _qimview_ (qt-based image view) is a set of classes that are designed to visualize and compare images. 
 It uses Python as the main language, and include some code in C++ or OpenGL shading language.
 Main features are:
 * **image reader**: read type image format (like jpeg and png) and also raw image format (bayer images)
 * **image cache**: save image reading/uncompressing time by loading previously read image into a buffer
```

### Comparing `qimview-1.0.9/qimview.egg-info/SOURCES.txt` & `qimview-1.1.0/qimview.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 qimview/__init__.py
 qimview/imview.py
 qimview/mview.py
+qimview/npViewer.py
 qimview.egg-info/PKG-INFO
 qimview.egg-info/SOURCES.txt
 qimview.egg-info/dependency_links.txt
 qimview.egg-info/entry_points.txt
 qimview.egg-info/requires.txt
 qimview.egg-info/top_level.txt
 qimview/cache/__init__.py
```

